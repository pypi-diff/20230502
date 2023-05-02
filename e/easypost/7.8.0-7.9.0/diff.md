# Comparing `tmp/easypost-7.8.0.tar.gz` & `tmp/easypost-7.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypost-7.8.0.tar", last modified: Wed Jan 11 17:13:55 2023, max compression
+gzip compressed data, was "easypost-7.9.0.tar", last modified: Wed Jan 18 18:04:37 2023, max compression
```

## Comparing `easypost-7.8.0.tar` & `easypost-7.9.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-01-11 17:13:55.340628 easypost-7.8.0/
--rw-r--r--   0 jhammond   (502) staff       (20)     9736 2023-01-11 17:13:22.000000 easypost-7.8.0/CHANGELOG.md
--rw-r--r--   0 jhammond   (502) staff       (20)     1092 2021-11-01 16:53:26.000000 easypost-7.8.0/LICENSE
--rw-r--r--   0 jhammond   (502) staff       (20)       13 2021-11-01 16:53:26.000000 easypost-7.8.0/MANIFEST.in
--rw-r--r--   0 jhammond   (502) staff       (20)     5838 2023-01-11 17:13:55.340729 easypost-7.8.0/PKG-INFO
--rw-r--r--   0 jhammond   (502) staff       (20)     4702 2023-01-11 17:02:39.000000 easypost-7.8.0/README.md
--rw-r--r--   0 jhammond   (502) staff       (20)     2371 2022-07-28 18:15:12.000000 easypost-7.8.0/UPGRADE_GUIDE.md
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-01-11 17:13:55.339210 easypost-7.8.0/easypost/
--rw-r--r--   0 jhammond   (502) staff       (20)     1292 2022-12-01 20:29:16.000000 easypost-7.8.0/easypost/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1939 2022-09-29 21:58:17.000000 easypost-7.8.0/easypost/address.py
--rw-r--r--   0 jhammond   (502) staff       (20)       74 2022-12-01 20:29:16.000000 easypost-7.8.0/easypost/api_key.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2679 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/batch.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-01-11 17:13:55.340419 easypost-7.8.0/easypost/beta/
--rw-r--r--   0 jhammond   (502) staff       (20)       59 2022-08-25 19:10:57.000000 easypost-7.8.0/easypost/beta/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)     7358 2023-01-11 17:02:39.000000 easypost-7.8.0/easypost/beta/referral.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3177 2022-08-11 20:30:53.000000 easypost-7.8.0/easypost/billing.py
--rw-r--r--   0 jhammond   (502) staff       (20)       73 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/brand.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1936 2022-12-01 20:29:16.000000 easypost-7.8.0/easypost/carrier_account.py
--rw-r--r--   0 jhammond   (502) staff       (20)      142 2022-12-01 20:29:16.000000 easypost-7.8.0/easypost/constant.py
--rw-r--r--   0 jhammond   (502) staff       (20)       91 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/customs_info.py
--rw-r--r--   0 jhammond   (502) staff       (20)       91 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/customs_item.py
--rw-r--r--   0 jhammond   (502) staff       (20)     7177 2022-12-01 20:29:16.000000 easypost-7.8.0/easypost/easypost_object.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1545 2022-09-29 21:58:17.000000 easypost-7.8.0/easypost/endshipper.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1082 2022-12-01 20:29:16.000000 easypost-7.8.0/easypost/error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      325 2022-08-11 20:30:53.000000 easypost-7.8.0/easypost/event.py
--rw-r--r--   0 jhammond   (502) staff       (20)      128 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/insurance.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1158 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/order.py
--rw-r--r--   0 jhammond   (502) staff       (20)       86 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/parcel.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1195 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/pickup.py
--rw-r--r--   0 jhammond   (502) staff       (20)       78 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/pickup_rate.py
--rw-r--r--   0 jhammond   (502) staff       (20)       80 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/postage_label.py
--rw-r--r--   0 jhammond   (502) staff       (20)        0 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/py.typed
--rw-r--r--   0 jhammond   (502) staff       (20)       72 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/rate.py
--rw-r--r--   0 jhammond   (502) staff       (20)     5152 2023-01-11 17:02:39.000000 easypost-7.8.0/easypost/referral.py
--rw-r--r--   0 jhammond   (502) staff       (20)      125 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/refund.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1017 2022-08-11 20:30:53.000000 easypost-7.8.0/easypost/report.py
--rw-r--r--   0 jhammond   (502) staff       (20)    13122 2022-08-22 20:51:17.000000 easypost-7.8.0/easypost/requestor.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3788 2022-09-29 21:58:17.000000 easypost-7.8.0/easypost/resource.py
--rw-r--r--   0 jhammond   (502) staff       (20)      605 2022-08-11 20:30:53.000000 easypost-7.8.0/easypost/scanform.py
--rw-r--r--   0 jhammond   (502) staff       (20)     5723 2022-09-21 15:30:40.000000 easypost-7.8.0/easypost/shipment.py
--rw-r--r--   0 jhammond   (502) staff       (20)       81 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/tax_identifier.py
--rw-r--r--   0 jhammond   (502) staff       (20)      670 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/tracker.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3246 2022-12-01 20:29:16.000000 easypost-7.8.0/easypost/user.py
--rw-r--r--   0 jhammond   (502) staff       (20)      966 2022-07-05 19:20:56.000000 easypost-7.8.0/easypost/util.py
--rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-01-11 17:13:22.000000 easypost-7.8.0/easypost/version.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2115 2022-07-28 18:15:12.000000 easypost-7.8.0/easypost/webhook.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-01-11 17:13:55.339915 easypost-7.8.0/easypost.egg-info/
--rw-r--r--   0 jhammond   (502) staff       (20)     5838 2023-01-11 17:13:55.000000 easypost-7.8.0/easypost.egg-info/PKG-INFO
--rw-r--r--   0 jhammond   (502) staff       (20)     1035 2023-01-11 17:13:55.000000 easypost-7.8.0/easypost.egg-info/SOURCES.txt
--rw-r--r--   0 jhammond   (502) staff       (20)        1 2023-01-11 17:13:55.000000 easypost-7.8.0/easypost.egg-info/dependency_links.txt
--rw-r--r--   0 jhammond   (502) staff       (20)      270 2023-01-11 17:13:55.000000 easypost-7.8.0/easypost.egg-info/requires.txt
--rw-r--r--   0 jhammond   (502) staff       (20)        9 2023-01-11 17:13:55.000000 easypost-7.8.0/easypost.egg-info/top_level.txt
--rw-r--r--   0 jhammond   (502) staff       (20)       63 2022-06-27 22:05:20.000000 easypost-7.8.0/pyproject.toml
--rw-r--r--   0 jhammond   (502) staff       (20)       70 2023-01-11 17:13:55.340957 easypost-7.8.0/setup.cfg
--rw-r--r--   0 jhammond   (502) staff       (20)     2142 2023-01-11 17:13:22.000000 easypost-7.8.0/setup.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-01-18 18:04:37.058102 easypost-7.9.0/
+-rw-r--r--   0 jhammond   (502) staff       (20)     9894 2023-01-18 18:04:12.000000 easypost-7.9.0/CHANGELOG.md
+-rw-r--r--   0 jhammond   (502) staff       (20)     1092 2021-11-01 16:53:26.000000 easypost-7.9.0/LICENSE
+-rw-r--r--   0 jhammond   (502) staff       (20)       13 2021-11-01 16:53:26.000000 easypost-7.9.0/MANIFEST.in
+-rw-r--r--   0 jhammond   (502) staff       (20)     5838 2023-01-18 18:04:37.058228 easypost-7.9.0/PKG-INFO
+-rw-r--r--   0 jhammond   (502) staff       (20)     4702 2023-01-11 17:02:39.000000 easypost-7.9.0/README.md
+-rw-r--r--   0 jhammond   (502) staff       (20)     2371 2022-07-28 18:15:12.000000 easypost-7.9.0/UPGRADE_GUIDE.md
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-01-18 18:04:37.056665 easypost-7.9.0/easypost/
+-rw-r--r--   0 jhammond   (502) staff       (20)     1329 2023-01-18 16:33:27.000000 easypost-7.9.0/easypost/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1939 2022-09-29 21:58:17.000000 easypost-7.9.0/easypost/address.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       74 2022-12-01 20:29:16.000000 easypost-7.9.0/easypost/api_key.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2679 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/batch.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-01-18 18:04:37.057858 easypost-7.9.0/easypost/beta/
+-rw-r--r--   0 jhammond   (502) staff       (20)       59 2022-08-25 19:10:57.000000 easypost-7.9.0/easypost/beta/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     7358 2023-01-11 17:02:39.000000 easypost-7.9.0/easypost/beta/referral.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3177 2022-08-11 20:30:53.000000 easypost-7.9.0/easypost/billing.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       73 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/brand.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1936 2022-12-01 20:29:16.000000 easypost-7.9.0/easypost/carrier_account.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      142 2022-12-01 20:29:16.000000 easypost-7.9.0/easypost/constant.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       91 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/customs_info.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       91 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/customs_item.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     7203 2023-01-18 16:33:27.000000 easypost-7.9.0/easypost/easypost_object.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1545 2022-09-29 21:58:17.000000 easypost-7.9.0/easypost/endshipper.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1082 2022-12-01 20:29:16.000000 easypost-7.9.0/easypost/error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1416 2023-01-18 16:33:27.000000 easypost-7.9.0/easypost/event.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      128 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/insurance.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1158 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/order.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       86 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/parcel.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       24 2023-01-18 16:33:27.000000 easypost-7.9.0/easypost/payload.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1234 2023-01-13 21:00:18.000000 easypost-7.9.0/easypost/pickup.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       78 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/pickup_rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       80 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/postage_label.py
+-rw-r--r--   0 jhammond   (502) staff       (20)        0 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/py.typed
+-rw-r--r--   0 jhammond   (502) staff       (20)       72 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     5152 2023-01-11 17:02:39.000000 easypost-7.9.0/easypost/referral.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      125 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/refund.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1017 2022-08-11 20:30:53.000000 easypost-7.9.0/easypost/report.py
+-rw-r--r--   0 jhammond   (502) staff       (20)    13122 2022-08-22 20:51:17.000000 easypost-7.9.0/easypost/requestor.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3788 2022-09-29 21:58:17.000000 easypost-7.9.0/easypost/resource.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      605 2022-08-11 20:30:53.000000 easypost-7.9.0/easypost/scanform.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     5723 2022-09-21 15:30:40.000000 easypost-7.9.0/easypost/shipment.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       81 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/tax_identifier.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      670 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/tracker.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3246 2022-12-01 20:29:16.000000 easypost-7.9.0/easypost/user.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      966 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/util.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-01-18 18:04:12.000000 easypost-7.9.0/easypost/version.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2115 2022-07-28 18:15:12.000000 easypost-7.9.0/easypost/webhook.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-01-18 18:04:37.057442 easypost-7.9.0/easypost.egg-info/
+-rw-r--r--   0 jhammond   (502) staff       (20)     5838 2023-01-18 18:04:37.000000 easypost-7.9.0/easypost.egg-info/PKG-INFO
+-rw-r--r--   0 jhammond   (502) staff       (20)     1055 2023-01-18 18:04:37.000000 easypost-7.9.0/easypost.egg-info/SOURCES.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)        1 2023-01-18 18:04:37.000000 easypost-7.9.0/easypost.egg-info/dependency_links.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)      270 2023-01-18 18:04:37.000000 easypost-7.9.0/easypost.egg-info/requires.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)        9 2023-01-18 18:04:37.000000 easypost-7.9.0/easypost.egg-info/top_level.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)       63 2022-06-27 22:05:20.000000 easypost-7.9.0/pyproject.toml
+-rw-r--r--   0 jhammond   (502) staff       (20)       70 2023-01-18 18:04:37.058498 easypost-7.9.0/setup.cfg
+-rw-r--r--   0 jhammond   (502) staff       (20)     2142 2023-01-18 18:04:12.000000 easypost-7.9.0/setup.py
```

### Comparing `easypost-7.8.0/CHANGELOG.md` & `easypost-7.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # CHANGELOG
 
+## v7.9.0 (2023-01-18)
+
+- Adds `all` function to `Pickup` to retrieve all pickups
+- Adds `retrieve_payload` and `retrieve_all_payloads` functions to `Event`
+
 ## v7.8.0 (2023-01-11)
 
 - Adds new beta billing functionality for ReferralCustomer users
   - `add_payment_method` can add a pre-existing Stripe bank account or credit card to your EasyPost account
   - `refund_by_amount` refunds your wallet by a dollar amount
   - `refund_by_payment_log` refunds you wallet by a PaymentLog ID
```

### Comparing `easypost-7.8.0/LICENSE` & `easypost-7.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/PKG-INFO` & `easypost-7.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypost
-Version: 7.8.0
+Version: 7.9.0
 Summary: EasyPost Shipping API Client Library for Python
 Home-page: https://easypost.com/
 Author: EasyPost
 Author-email: support@easypost.com
 Project-URL: Docs, https://www.easypost.com/docs/api
 Project-URL: Tracker, https://github.com/EasyPost/easypost-python/issues
 Project-URL: Source, https://github.com/EasyPost/easypost-python
```

### Comparing `easypost-7.8.0/README.md` & `easypost-7.9.0/README.md`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/UPGRADE_GUIDE.md` & `easypost-7.9.0/UPGRADE_GUIDE.md`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/__init__.py` & `easypost-7.9.0/easypost/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from easypost.customs_item import CustomsItem
 from easypost.endshipper import EndShipper
 from easypost.error import Error
 from easypost.event import Event
 from easypost.insurance import Insurance
 from easypost.order import Order
 from easypost.parcel import Parcel
+from easypost.payload import Payload
 from easypost.pickup import Pickup
 from easypost.pickup_rate import PickupRate
 from easypost.postage_label import PostageLabel
 from easypost.rate import Rate
 from easypost.referral import Referral
 from easypost.refund import Refund
 from easypost.report import Report
```

### Comparing `easypost-7.8.0/easypost/address.py` & `easypost-7.9.0/easypost/address.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/batch.py` & `easypost-7.9.0/easypost/batch.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/beta/referral.py` & `easypost-7.9.0/easypost/beta/referral.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/billing.py` & `easypost-7.9.0/easypost/billing.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/carrier_account.py` & `easypost-7.9.0/easypost/carrier_account.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/easypost_object.py` & `easypost-7.9.0/easypost/easypost_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,28 @@
     Optional,
 )
 
 import easypost
 
 
 EASYPOST_OBJECT_ID_PREFIX_TO_CLASS_NAME_MAP = {
-    "ak": "ApiKey",
     "adr": "Address",
+    "ak": "ApiKey",
     "batch": "Batch",
     "brd": "Brand",
     "ca": "CarrierAccount",
     "cfrep": "Report",
     "cstinfo": "CustomsInfo",
     "cstitem": "CustomsItem",
     "es": "EndShipper",
     "evt": "Event",
     "hook": "Webhook",
     "ins": "Insurance",
     "order": "Order",
+    "payload": "Payload",
     "pickup": "Pickup",
     "pickuprate": "PickupRate",
     "pl": "PostageLabel",
     "plrep": "Report",
     "prcl": "Parcel",
     "rate": "Rate",
     "refrep": "Report",
```

### Comparing `easypost-7.8.0/easypost/endshipper.py` & `easypost-7.9.0/easypost/endshipper.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/error.py` & `easypost-7.9.0/easypost/error.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/order.py` & `easypost-7.9.0/easypost/order.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/pickup.py` & `easypost-7.9.0/easypost/pickup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from typing import List
 
 from easypost.requestor import (
     RequestMethod,
     Requestor,
 )
-from easypost.resource import CreateResource
+from easypost.resource import (
+    AllResource,
+    CreateResource,
+)
 from easypost.util import get_lowest_object_rate
 
 
-class Pickup(CreateResource):
+class Pickup(CreateResource, AllResource):
     def buy(self, **params) -> "Pickup":
         """Buy a pickup."""
         requestor = Requestor(local_api_key=self._api_key)
         url = "%s/%s" % (self.instance_url(), "buy")
         response, api_key = requestor.request(method=RequestMethod.POST, url=url, params=params)
         self.refresh_from(values=response, api_key=api_key)
         return self
```

### Comparing `easypost-7.8.0/easypost/referral.py` & `easypost-7.9.0/easypost/referral.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/report.py` & `easypost-7.9.0/easypost/report.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/requestor.py` & `easypost-7.9.0/easypost/requestor.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/resource.py` & `easypost-7.9.0/easypost/resource.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/scanform.py` & `easypost-7.9.0/easypost/scanform.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/shipment.py` & `easypost-7.9.0/easypost/shipment.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/tracker.py` & `easypost-7.9.0/easypost/tracker.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/user.py` & `easypost-7.9.0/easypost/user.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/util.py` & `easypost-7.9.0/easypost/util.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost/webhook.py` & `easypost-7.9.0/easypost/webhook.py`

 * *Files identical despite different names*

### Comparing `easypost-7.8.0/easypost.egg-info/PKG-INFO` & `easypost-7.9.0/easypost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypost
-Version: 7.8.0
+Version: 7.9.0
 Summary: EasyPost Shipping API Client Library for Python
 Home-page: https://easypost.com/
 Author: EasyPost
 Author-email: support@easypost.com
 Project-URL: Docs, https://www.easypost.com/docs/api
 Project-URL: Tracker, https://github.com/EasyPost/easypost-python/issues
 Project-URL: Source, https://github.com/EasyPost/easypost-python
```

### Comparing `easypost-7.8.0/easypost.egg-info/SOURCES.txt` & `easypost-7.9.0/easypost.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 easypost/easypost_object.py
 easypost/endshipper.py
 easypost/error.py
 easypost/event.py
 easypost/insurance.py
 easypost/order.py
 easypost/parcel.py
+easypost/payload.py
 easypost/pickup.py
 easypost/pickup_rate.py
 easypost/postage_label.py
 easypost/py.typed
 easypost/rate.py
 easypost/referral.py
 easypost/refund.py
```

### Comparing `easypost-7.8.0/setup.py` & `easypost-7.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ]
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="easypost",
-    version="7.8.0",
+    version="7.9.0",
     description="EasyPost Shipping API Client Library for Python",
     author="EasyPost",
     author_email="support@easypost.com",
     url="https://easypost.com/",
     packages=find_packages(
         exclude=[
             "examples",
```

