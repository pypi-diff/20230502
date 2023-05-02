# Comparing `tmp/odoo13_addons_oca_account_payment-13.0.20230224.0-py3-none-any.whl.zip` & `tmp/odoo13_addons_oca_account_payment-13.0.20230501.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1593 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1491 b- defN 23-Feb-25 03:08 odoo13_addons_oca_account_payment-13.0.20230224.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-25 03:08 odoo13_addons_oca_account_payment-13.0.20230224.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-25 03:08 odoo13_addons_oca_account_payment-13.0.20230224.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      441 b- defN 23-Feb-25 03:08 odoo13_addons_oca_account_payment-13.0.20230224.0.dist-info/RECORD
-4 files, 2025 bytes uncompressed, 723 bytes compressed:  64.3%
+Zip file size: 1597 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1551 b- defN 23-May-02 03:05 odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 03:05 odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-02 03:05 odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      441 b- defN 23-May-02 03:05 odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/RECORD
+4 files, 2085 bytes uncompressed, 727 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo13_addons_oca_account_payment-13.0.20230224.0.dist-info/METADATA
+Filename: odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo13_addons_oca_account_payment-13.0.20230224.0.dist-info/WHEEL
+Filename: odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo13_addons_oca_account_payment-13.0.20230224.0.dist-info/top_level.txt
+Filename: odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo13_addons_oca_account_payment-13.0.20230224.0.dist-info/RECORD
+Filename: odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo13_addons_oca_account_payment-13.0.20230224.0.dist-info/METADATA` & `odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: odoo13-addons-oca-account-payment
-Version: 13.0.20230224.0
+Version: 13.0.20230501.0
 Summary: Meta package for oca-account-payment Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 13.0
 Requires-Dist: odoo13-addon-account-cash-discount-base
+Requires-Dist: odoo13-addon-account-cash-discount-base-sale
 Requires-Dist: odoo13-addon-account-cash-discount-payment
 Requires-Dist: odoo13-addon-account-cash-discount-write-off
 Requires-Dist: odoo13-addon-account-cash-invoice
 Requires-Dist: odoo13-addon-account-check-date
 Requires-Dist: odoo13-addon-account-check-printing-report-base
 Requires-Dist: odoo13-addon-account-due-list
 Requires-Dist: odoo13-addon-account-due-list-days-overdue
```

