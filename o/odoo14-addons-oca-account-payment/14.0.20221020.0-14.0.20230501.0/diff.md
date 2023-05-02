# Comparing `tmp/odoo14_addons_oca_account_payment-14.0.20221020.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_account_payment-14.0.20230501.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1620 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1730 b- defN 22-Oct-21 02:46 odoo14_addons_oca_account_payment-14.0.20221020.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-21 02:46 odoo14_addons_oca_account_payment-14.0.20221020.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 22-Oct-21 02:46 odoo14_addons_oca_account_payment-14.0.20221020.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      441 b- defN 22-Oct-21 02:46 odoo14_addons_oca_account_payment-14.0.20221020.0.dist-info/RECORD
-4 files, 2264 bytes uncompressed, 750 bytes compressed:  66.9%
+Zip file size: 1633 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1792 b- defN 23-May-02 03:06 odoo14_addons_oca_account_payment-14.0.20230501.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 03:06 odoo14_addons_oca_account_payment-14.0.20230501.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-02 03:06 odoo14_addons_oca_account_payment-14.0.20230501.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      441 b- defN 23-May-02 03:06 odoo14_addons_oca_account_payment-14.0.20230501.0.dist-info/RECORD
+4 files, 2326 bytes uncompressed, 763 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_account_payment-14.0.20221020.0.dist-info/METADATA
+Filename: odoo14_addons_oca_account_payment-14.0.20230501.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_account_payment-14.0.20221020.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_account_payment-14.0.20230501.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_account_payment-14.0.20221020.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_account_payment-14.0.20230501.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_account_payment-14.0.20221020.0.dist-info/RECORD
+Filename: odoo14_addons_oca_account_payment-14.0.20230501.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_account_payment-14.0.20221020.0.dist-info/METADATA` & `odoo14_addons_oca_account_payment-14.0.20230501.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-account-payment
-Version: 14.0.20221020.0
+Version: 14.0.20230501.0
 Summary: Meta package for oca-account-payment Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -29,10 +29,11 @@
 Requires-Dist: odoo14-addon-account-payment-return-import-iso20022
 Requires-Dist: odoo14-addon-account-payment-term-discount
 Requires-Dist: odoo14-addon-account-payment-term-extension
 Requires-Dist: odoo14-addon-account-payment-terminal
 Requires-Dist: odoo14-addon-account-payment-view-check-number
 Requires-Dist: odoo14-addon-account-payment-widget-amount
 Requires-Dist: odoo14-addon-partner-aging
+Requires-Dist: odoo14-addon-partner-restrict-payment-acquirer
 
 UNKNOWN
```

