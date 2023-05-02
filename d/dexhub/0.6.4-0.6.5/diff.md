# Comparing `tmp/dexhub-0.6.4.tar.gz` & `tmp/dexhub-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexhub-0.6.4.tar", last modified: Mon May  1 19:33:09 2023, max compression
+gzip compressed data, was "dexhub-0.6.5.tar", last modified: Tue May  2 19:52:01 2023, max compression
```

## Comparing `dexhub-0.6.4.tar` & `dexhub-0.6.5.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 19:33:09.011076 dexhub-0.6.4/
--rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-01 19:33:09.010931 dexhub-0.6.4/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.6.4/README.md
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 19:33:09.007255 dexhub-0.6.4/dexhub/
--rw-r--r--   0 czhong     (501) staff       (20)     1156 2023-05-01 19:32:51.000000 dexhub-0.6.4/dexhub/__init__.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 19:33:09.009224 dexhub-0.6.4/dexhub/abi/
--rw-r--r--   0 czhong     (501) staff       (20)      250 2023-05-01 18:43:45.000000 dexhub-0.6.4/dexhub/abi/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.6.4/dexhub/abi/arbitrum_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    67846 2023-05-01 18:02:06.000000 dexhub-0.6.4/dexhub/abi/avax_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    22419 2023-03-03 18:30:32.000000 dexhub-0.6.4/dexhub/abi/dfk_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.6.4/dexhub/abi/eth_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.6.4/dexhub/abi/klay_abi.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 19:33:09.010174 dexhub-0.6.4/dexhub/address/
--rw-r--r--   0 czhong     (501) staff       (20)      482 2023-05-01 18:42:42.000000 dexhub-0.6.4/dexhub/address/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.6.4/dexhub/address/arbitrum_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.6.4/dexhub/address/avax_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     4539 2023-03-09 16:49:05.000000 dexhub-0.6.4/dexhub/address/dfk_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.6.4/dexhub/address/eth_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.6.4/dexhub/address/klay_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.6.4/dexhub/address/polygon_address.py
--rw-r--r--   0 czhong     (501) staff       (20)   141917 2023-04-01 13:32:00.000000 dexhub-0.6.4/dexhub/dex.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 19:33:09.010427 dexhub-0.6.4/dexhub/interface/
--rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.6.4/dexhub/interface/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.6.4/dexhub/interface/joe.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 19:33:09.010724 dexhub-0.6.4/dexhub/util/
--rw-r--r--   0 czhong     (501) staff       (20)       40 2023-01-17 19:51:41.000000 dexhub-0.6.4/dexhub/util/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    13947 2022-12-05 20:29:28.000000 dexhub-0.6.4/dexhub/util/helper.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 19:33:09.008275 dexhub-0.6.4/dexhub.egg-info/
--rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-01 19:33:08.000000 dexhub-0.6.4/dexhub.egg-info/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      657 2023-05-01 19:33:08.000000 dexhub-0.6.4/dexhub.egg-info/SOURCES.txt
--rw-r--r--   0 czhong     (501) staff       (20)        1 2023-05-01 19:33:08.000000 dexhub-0.6.4/dexhub.egg-info/dependency_links.txt
--rw-r--r--   0 czhong     (501) staff       (20)        5 2023-05-01 19:33:08.000000 dexhub-0.6.4/dexhub.egg-info/requires.txt
--rw-r--r--   0 czhong     (501) staff       (20)        7 2023-05-01 19:33:08.000000 dexhub-0.6.4/dexhub.egg-info/top_level.txt
--rw-r--r--   0 czhong     (501) staff       (20)       38 2023-05-01 19:33:09.011127 dexhub-0.6.4/setup.cfg
--rw-r--r--   0 czhong     (501) staff       (20)      609 2023-05-01 19:33:04.000000 dexhub-0.6.4/setup.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.819816 dexhub-0.6.5/
+-rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-02 19:52:01.819671 dexhub-0.6.5/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.6.5/README.md
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.815917 dexhub-0.6.5/dexhub/
+-rw-r--r--   0 czhong     (501) staff       (20)     1207 2023-05-02 19:50:21.000000 dexhub-0.6.5/dexhub/__init__.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.817914 dexhub-0.6.5/dexhub/abi/
+-rw-r--r--   0 czhong     (501) staff       (20)      250 2023-05-01 18:43:45.000000 dexhub-0.6.5/dexhub/abi/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.6.5/dexhub/abi/arbitrum_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)   120303 2023-05-02 03:17:30.000000 dexhub-0.6.5/dexhub/abi/avax_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    22419 2023-03-03 18:30:32.000000 dexhub-0.6.5/dexhub/abi/dfk_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.6.5/dexhub/abi/eth_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.6.5/dexhub/abi/klay_abi.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.818778 dexhub-0.6.5/dexhub/address/
+-rw-r--r--   0 czhong     (501) staff       (20)      482 2023-05-01 18:42:42.000000 dexhub-0.6.5/dexhub/address/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.6.5/dexhub/address/arbitrum_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.6.5/dexhub/address/avax_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     4539 2023-03-09 16:49:05.000000 dexhub-0.6.5/dexhub/address/dfk_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.6.5/dexhub/address/eth_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.6.5/dexhub/address/klay_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.6.5/dexhub/address/polygon_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)   141917 2023-04-01 13:32:00.000000 dexhub-0.6.5/dexhub/dex.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.819032 dexhub-0.6.5/dexhub/interface/
+-rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.6.5/dexhub/interface/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.6.5/dexhub/interface/joe.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.819454 dexhub-0.6.5/dexhub/util/
+-rw-r--r--   0 czhong     (501) staff       (20)       83 2023-05-02 19:50:16.000000 dexhub-0.6.5/dexhub/util/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    14052 2023-05-01 20:35:46.000000 dexhub-0.6.5/dexhub/util/helper.py
+-rw-r--r--   0 czhong     (501) staff       (20)      471 2023-05-02 19:50:10.000000 dexhub-0.6.5/dexhub/util/joe_v2.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.816674 dexhub-0.6.5/dexhub.egg-info/
+-rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-02 19:52:01.000000 dexhub-0.6.5/dexhub.egg-info/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      679 2023-05-02 19:52:01.000000 dexhub-0.6.5/dexhub.egg-info/SOURCES.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        1 2023-05-02 19:52:01.000000 dexhub-0.6.5/dexhub.egg-info/dependency_links.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        5 2023-05-02 19:52:01.000000 dexhub-0.6.5/dexhub.egg-info/requires.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        7 2023-05-02 19:52:01.000000 dexhub-0.6.5/dexhub.egg-info/top_level.txt
+-rw-r--r--   0 czhong     (501) staff       (20)       38 2023-05-02 19:52:01.819862 dexhub-0.6.5/setup.cfg
+-rw-r--r--   0 czhong     (501) staff       (20)      609 2023-05-02 19:51:23.000000 dexhub-0.6.5/setup.py
```

### Comparing `dexhub-0.6.4/PKG-INFO` & `dexhub-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexhub
-Version: 0.6.4
+Version: 0.6.5
 Summary: dex connector
 Home-page: https://github.com/elmtlab/aurum
 Author: elmtlab
 Author-email: elmtlab@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dexhub-0.6.4/dexhub/__init__.py` & `dexhub-0.6.5/dexhub/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,18 @@
     JoeV2Factory,JoeV2Pair,JoeV2Route,JoeV2Quote,JoeV2Erc20
 )
 
 from dexhub.util.helper import(
     DexHelper
 )
 
+from dexhub.util.joe_v2 import(
+    JoeV2Helper
+)
+
 from dexhub.interface.joe import(
     JoeV2Erc20,JoeV2Factory,JoeV2Pair,JoeV2Quote,JoeV2Route
 )
 
 from dexhub.address.avax_address import(
     AddressJoe,AddressAvaxTokens,AddressPangolin
 )
```

### Comparing `dexhub-0.6.4/dexhub/abi/arbitrum_abi.py` & `dexhub-0.6.5/dexhub/abi/arbitrum_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.4/dexhub/abi/dfk_abi.py` & `dexhub-0.6.5/dexhub/abi/dfk_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.4/dexhub/abi/eth_abi.py` & `dexhub-0.6.5/dexhub/abi/eth_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.4/dexhub/abi/klay_abi.py` & `dexhub-0.6.5/dexhub/abi/klay_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.4/dexhub/address/arbitrum_address.py` & `dexhub-0.6.5/dexhub/address/arbitrum_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.4/dexhub/address/avax_address.py` & `dexhub-0.6.5/dexhub/address/avax_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.4/dexhub/address/dfk_address.py` & `dexhub-0.6.5/dexhub/address/dfk_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.4/dexhub/address/eth_address.py` & `dexhub-0.6.5/dexhub/address/eth_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.4/dexhub/address/klay_address.py` & `dexhub-0.6.5/dexhub/address/klay_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.4/dexhub/address/polygon_address.py` & `dexhub-0.6.5/dexhub/address/polygon_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.4/dexhub/dex.py` & `dexhub-0.6.5/dexhub/dex.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.4/dexhub/interface/joe.py` & `dexhub-0.6.5/dexhub/interface/joe.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.4/dexhub/util/helper.py` & `dexhub-0.6.5/dexhub/util/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,7 +301,13 @@
         except TypeError as e:
             print(e)
         except:
             print("####################################")
             print("################error###############")
             print("####################################")
             time.sleep(2)
+
+
+class SpatialHelper:
+    #uniswap v2 <-> uniswap v2 spatial
+    def v2_spatial():
+        print('test')
```

### Comparing `dexhub-0.6.4/dexhub.egg-info/PKG-INFO` & `dexhub-0.6.5/dexhub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexhub
-Version: 0.6.4
+Version: 0.6.5
 Summary: dex connector
 Home-page: https://github.com/elmtlab/aurum
 Author: elmtlab
 Author-email: elmtlab@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dexhub-0.6.4/dexhub.egg-info/SOURCES.txt` & `dexhub-0.6.5/dexhub.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 dexhub/address/dfk_address.py
 dexhub/address/eth_address.py
 dexhub/address/klay_address.py
 dexhub/address/polygon_address.py
 dexhub/interface/__init__.py
 dexhub/interface/joe.py
 dexhub/util/__init__.py
-dexhub/util/helper.py
+dexhub/util/helper.py
+dexhub/util/joe_v2.py
```

### Comparing `dexhub-0.6.4/setup.py` & `dexhub-0.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dexhub",
-    version="0.6.4",
+    version="0.6.5",
     author="elmtlab",
     author_email="elmtlab@outlook.com",
     description="dex connector",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elmtlab/aurum",
     packages=setuptools.find_packages(),
```

