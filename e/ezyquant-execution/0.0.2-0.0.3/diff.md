# Comparing `tmp/ezyquant-execution-0.0.2.tar.gz` & `tmp/ezyquant-execution-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyquant-execution-0.0.2.tar", last modified: Tue Apr 18 07:50:37 2023, max compression
+gzip compressed data, was "ezyquant-execution-0.0.3.tar", last modified: Tue May  2 10:16:41 2023, max compression
```

## Comparing `ezyquant-execution-0.0.2.tar` & `ezyquant-execution-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:50:37.427486 ezyquant-execution-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-18 07:50:37.427486 ezyquant-execution-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:50:37.427486 ezyquant-execution-0.0.2/ezyquant_execution/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)    14364 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/executing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/realtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:50:37.427486 ezyquant-execution-0.0.2/ezyquant_execution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-18 07:50:37.000000 ezyquant-execution-0.0.2/ezyquant_execution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-18 07:50:37.000000 ezyquant-execution-0.0.2/ezyquant_execution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:50:37.000000 ezyquant-execution-0.0.2/ezyquant_execution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 07:50:37.000000 ezyquant-execution-0.0.2/ezyquant_execution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 07:50:37.000000 ezyquant-execution-0.0.2/ezyquant_execution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-18 07:50:37.427486 ezyquant-execution-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:16:41.775104 ezyquant-execution-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-02 10:16:23.000000 ezyquant-execution-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-02 10:16:41.775104 ezyquant-execution-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-02 10:16:23.000000 ezyquant-execution-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:16:41.775104 ezyquant-execution-0.0.3/ezyquant_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 10:16:23.000000 ezyquant-execution-0.0.3/ezyquant_execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 10:16:23.000000 ezyquant-execution-0.0.3/ezyquant_execution/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-02 10:16:23.000000 ezyquant-execution-0.0.3/ezyquant_execution/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-05-02 10:16:23.000000 ezyquant-execution-0.0.3/ezyquant_execution/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-05-02 10:16:23.000000 ezyquant-execution-0.0.3/ezyquant_execution/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-02 10:16:23.000000 ezyquant-execution-0.0.3/ezyquant_execution/executing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-02 10:16:23.000000 ezyquant-execution-0.0.3/ezyquant_execution/realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-02 10:16:23.000000 ezyquant-execution-0.0.3/ezyquant_execution/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:16:41.775104 ezyquant-execution-0.0.3/ezyquant_execution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-02 10:16:41.000000 ezyquant-execution-0.0.3/ezyquant_execution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-02 10:16:41.000000 ezyquant-execution-0.0.3/ezyquant_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:16:41.000000 ezyquant-execution-0.0.3/ezyquant_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 10:16:41.000000 ezyquant-execution-0.0.3/ezyquant_execution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 10:16:41.000000 ezyquant-execution-0.0.3/ezyquant_execution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-02 10:16:41.775104 ezyquant-execution-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-02 10:16:23.000000 ezyquant-execution-0.0.3/setup.py
```

### Comparing `ezyquant-execution-0.0.2/LICENSE.txt` & `ezyquant-execution-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.2/PKG-INFO` & `ezyquant-execution-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant-execution
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ezyquant execution
 Home-page: https://pydoc.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-execution-0.0.2/ezyquant_execution/constant.py` & `ezyquant-execution-0.0.3/ezyquant_execution/constant.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.2/ezyquant_execution/context.py` & `ezyquant-execution-0.0.3/ezyquant_execution/context.py`

 * *Files 9% similar despite different names*

```diff
@@ -335,14 +335,44 @@
                 warnings.warn(
                     f"Cancel order {i.order_no} failed: {i.error_response['message']}"
                 )
 
         return out
 
     """
+    Validate order functions
+    """
+
+    def is_buy_cash_sufficient(
+        self, volume: float, price: float, pct_commission: float = 0.0
+    ) -> bool:
+        """Check if the cash is sufficient for buy order.
+
+        Parameters
+        ----------
+        volume: float
+            volume
+        price: float
+            price
+        pct_commission: float
+            percentage of commission example 0.01 for 1%
+        """
+        return self.cash_balance >= volume * price * (1 + pct_commission)
+
+    def is_sell_volume_sufficient(self, volume: float) -> bool:
+        """Check if the volume is sufficient for sell order.
+
+        Parameters
+        ----------
+        volume: float
+            volume
+        """
+        return self.volume >= volume
+
+    """
     Settrade SDK functions
     """
 
     @property
     def _acc_no_kw(self) -> dict:
         return (
             {"account_no": self.account_no}
```

### Comparing `ezyquant-execution-0.0.2/ezyquant_execution/entity.py` & `ezyquant-execution-0.0.3/ezyquant_execution/entity.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.2/ezyquant_execution/executing.py` & `ezyquant-execution-0.0.3/ezyquant_execution/executing.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.2/ezyquant_execution/realtime.py` & `ezyquant-execution-0.0.3/ezyquant_execution/realtime.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.2/ezyquant_execution/utils.py` & `ezyquant-execution-0.0.3/ezyquant_execution/utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.2/ezyquant_execution.egg-info/PKG-INFO` & `ezyquant-execution-0.0.3/ezyquant_execution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant-execution
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ezyquant execution
 Home-page: https://pydoc.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-execution-0.0.2/setup.py` & `ezyquant-execution-0.0.3/setup.py`

 * *Files identical despite different names*

