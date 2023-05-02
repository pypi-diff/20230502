# Comparing `tmp/edc_model-0.3.8-py3-none-any.whl.zip` & `tmp/edc_model-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 46380 bytes, number of entries: 50
+Zip file size: 46447 bytes, number of entries: 50
 -rw-r--r--  2.0 unx      236 b- defN 21-Jul-15 03:45 edc_model/__init__.py
 -rw-r--r--  2.0 unx     1008 b- defN 21-Feb-04 19:59 edc_model/apps.py
 -rw-r--r--  2.0 unx      175 b- defN 21-Feb-04 19:59 edc_model/choices.py
 -rw-r--r--  2.0 unx      278 b- defN 21-Mar-01 03:48 edc_model/constants.py
 -rw-r--r--  2.0 unx      929 b- defN 21-Mar-01 03:48 edc_model/stubs.py
--rw-r--r--  2.0 unx     4290 b- defN 21-Aug-08 18:52 edc_model/utils.py
+-rw-r--r--  2.0 unx     4485 b- defN 21-Aug-10 05:37 edc_model/utils.py
 -rw-r--r--  2.0 unx     1104 b- defN 21-Aug-08 22:50 edc_model/models/__init__.py
 -rw-r--r--  2.0 unx      802 b- defN 20-Jul-29 19:16 edc_model/models/address_mixin.py
 -rw-r--r--  2.0 unx      587 b- defN 20-Jul-29 19:16 edc_model/models/base_model.py
 -rw-r--r--  2.0 unx      390 b- defN 21-Feb-04 19:59 edc_model/models/base_uuid_model.py
 -rw-r--r--  2.0 unx     1064 b- defN 21-Mar-01 03:48 edc_model/models/historical_records.py
 -rw-r--r--  2.0 unx      547 b- defN 21-Feb-19 22:07 edc_model/models/report_status_model_mixin.py
 -rw-r--r--  2.0 unx     2470 b- defN 21-Mar-01 03:48 edc_model/models/url_model_mixin.py
@@ -40,13 +40,13 @@
 -rw-r--r--  2.0 unx      294 b- defN 21-Feb-04 19:59 edc_model/validators/__init__.py
 -rw-r--r--  2.0 unx       42 b- defN 20-Jun-23 03:26 edc_model/validators/bp.py
 -rw-r--r--  2.0 unx      154 b- defN 21-Feb-04 19:59 edc_model/validators/date.py
 -rw-r--r--  2.0 unx       64 b- defN 20-Oct-02 17:04 edc_model/validators/duration.py
 -rw-r--r--  2.0 unx       51 b- defN 20-Jun-23 03:26 edc_model/validators/phone.py
 -rw-r--r--  2.0 unx       40 b- defN 20-Oct-02 17:39 edc_model/widgets/__init__.py
 -rw-r--r--  2.0 unx     1210 b- defN 20-Oct-02 17:39 edc_model/widgets/slider_widget.py
--rw-r--r--  2.0 unx    35149 b- defN 21-Aug-08 22:51 edc_model-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3072 b- defN 21-Aug-08 22:51 edc_model-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Aug-08 22:51 edc_model-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 21-Aug-08 22:51 edc_model-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4419 b- defN 21-Aug-08 22:51 edc_model-0.3.8.dist-info/RECORD
-50 files, 95939 bytes uncompressed, 39240 bytes compressed:  59.1%
+-rw-r--r--  2.0 unx    35149 b- defN 21-Aug-10 05:37 edc_model-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3072 b- defN 21-Aug-10 05:37 edc_model-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Aug-10 05:37 edc_model-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 21-Aug-10 05:37 edc_model-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4419 b- defN 21-Aug-10 05:37 edc_model-0.3.9.dist-info/RECORD
+50 files, 96134 bytes uncompressed, 39307 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -129,23 +129,23 @@
 
 Filename: edc_model/widgets/__init__.py
 Comment: 
 
 Filename: edc_model/widgets/slider_widget.py
 Comment: 
 
-Filename: edc_model-0.3.8.dist-info/LICENSE
+Filename: edc_model-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: edc_model-0.3.8.dist-info/METADATA
+Filename: edc_model-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: edc_model-0.3.8.dist-info/WHEEL
+Filename: edc_model-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: edc_model-0.3.8.dist-info/top_level.txt
+Filename: edc_model-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: edc_model-0.3.8.dist-info/RECORD
+Filename: edc_model-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edc_model/utils.py

```diff
@@ -132,7 +132,16 @@
     try:
         model_cls.objects.get(**opts)
     except ObjectDoesNotExist:
         raise forms.ValidationError(
             f"Complete the `{model_cls._meta.verbose_name}` CRF first."
         )
     return True
+
+
+def is_inline_model(instance):
+    """See also, edc-crf inline model mixin."""
+    try:
+        instance._meta.crf_inline_parent
+    except AttributeError:
+        return False
+    return True
```

## Comparing `edc_model-0.3.8.dist-info/LICENSE` & `edc_model-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edc_model-0.3.8.dist-info/METADATA` & `edc_model-0.3.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-model
-Version: 0.3.8
+Version: 0.3.9
 Summary: Base model mixins clinicedc/edc projects.
 Home-page: http://github.com/clinicedc/edc-model
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django base models fields forms admin
 Platform: UNKNOWN
```

## Comparing `edc_model-0.3.8.dist-info/RECORD` & `edc_model-0.3.9.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 edc_model/__init__.py,sha256=MngExhC6oJSwghNFqnHsVdwNS9XyqyNppFYjnRpSOCE,236
 edc_model/apps.py,sha256=sbvjDdbO6axiYrzyCEVPNNiq-jT9-S9thHruriV4nNM,1008
 edc_model/choices.py,sha256=FppisMDKr02-MF5aTrfsfVHuw4h1juiCa_Gy0SlhQ9I,175
 edc_model/constants.py,sha256=jPTR6t1jgXl7VqjWFVFiuccVQUPxOqLhUuefHqiozgM,278
 edc_model/stubs.py,sha256=T3MQreogCsr5KNOZDDj4Wbctv1FSfLZzGLPJDxjXP6g,929
-edc_model/utils.py,sha256=bIrgTyx30Y1Ik6o8CVJdvdOlpQ3f523cd3HFFe8CFag,4290
+edc_model/utils.py,sha256=3r7qEHBU0-1SwRFioFjyH24kNrJ_-ApuYmzqJLI0wxg,4485
 edc_model/models/__init__.py,sha256=42GyKtXf2CNm02117MtEAdBdVyIlGpuUQGf9_KTRz9o,1104
 edc_model/models/address_mixin.py,sha256=ud03rmVMukMCqlaY4jZ-YkPQjBeeY0l0c_P5xAK-EOk,802
 edc_model/models/base_model.py,sha256=U9z_XNBhHG0l3uR1peLTCaODH_N8gW5dDr-Rr30kzzM,587
 edc_model/models/base_uuid_model.py,sha256=kvRIjw8gMSC3okz1R9X19Cb4BO2wS-qkT3GSSc1OPB8,390
 edc_model/models/historical_records.py,sha256=1NfApg1WEl_lJJTdknYNMmr-7Zz4XhXU-3qn9F2iRjY,1064
 edc_model/models/report_status_model_mixin.py,sha256=2lOc8mK8heHbacE_TY8rh-cUt4bdcyuNAX_kcUcZJaM,547
 edc_model/models/url_model_mixin.py,sha256=9qiGot7kRBuDvx5nMNPa1p2eFnJPoaYaaLO1flb8D0U,2470
@@ -39,12 +39,12 @@
 edc_model/validators/__init__.py,sha256=m4sQd0G3pPECpfuMVT-kM9WxgLKLgEL6L_5oO34Ftms,294
 edc_model/validators/bp.py,sha256=2WVgRVaNxxpz_o4COcNTaoqrDq4XKAjjgaA5ySacniw,42
 edc_model/validators/date.py,sha256=z8GLFDRSsdZYlgDn7No8RI0A02IPmlapibOy_ft9kis,154
 edc_model/validators/duration.py,sha256=nlqZ0O8PoHLUSSFg4gip0dYVJHVOTsVh6Dl64GoBD3w,64
 edc_model/validators/phone.py,sha256=phjGF_ykiOYVekqvKDIlHRFMX8Vm6ABl6ZmWOUKMGoA,51
 edc_model/widgets/__init__.py,sha256=Q1L6XHWfrMmlOq4iBSvOatqudtp7_Vf3C3pPvxgVwGg,40
 edc_model/widgets/slider_widget.py,sha256=qf9l165S0MvXBSSWbprvAvjXuQuZZcAN097M9UgyedE,1210
-edc_model-0.3.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-edc_model-0.3.8.dist-info/METADATA,sha256=SzFuNNDE3CBXjfFIEMrMIoH9TDbkgTJxHr_3gcMRe8U,3072
-edc_model-0.3.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-edc_model-0.3.8.dist-info/top_level.txt,sha256=KFGQtN1EJrHmcHVh7U9K67pCCAbSkB5efkhk6qyfSQE,10
-edc_model-0.3.8.dist-info/RECORD,,
+edc_model-0.3.9.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+edc_model-0.3.9.dist-info/METADATA,sha256=PRVr0yrso3KFnt8ZAmmTXPrwvd0fNgtTnsE-YrwUIbg,3072
+edc_model-0.3.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+edc_model-0.3.9.dist-info/top_level.txt,sha256=KFGQtN1EJrHmcHVh7U9K67pCCAbSkB5efkhk6qyfSQE,10
+edc_model-0.3.9.dist-info/RECORD,,
```

