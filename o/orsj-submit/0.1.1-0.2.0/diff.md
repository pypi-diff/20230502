# Comparing `tmp/orsj_submit-0.1.1-py3-none-any.whl.zip` & `tmp/orsj_submit-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 411938 bytes, number of entries: 50
+Zip file size: 411936 bytes, number of entries: 50
 -rw-r--r--  2.0 unx     1153 b- defN 80-Jan-01 00:00 orsj_submit/__init__.py
 -rw-r--r--  2.0 unx       27 b- defN 80-Jan-01 00:00 orsj_submit/__main__.py
 -rw-r--r--  2.0 unx      210 b- defN 80-Jan-01 00:00 orsj_submit/orsj/__init__.py
 -rw-r--r--  2.0 unx   127317 b- defN 80-Jan-01 00:00 orsj_submit/orsj/static/content/bootstrap.css
 -rw-r--r--  2.0 unx    97968 b- defN 80-Jan-01 00:00 orsj_submit/orsj/static/content/bootstrap.min.css
 -rw-r--r--  2.0 unx     3273 b- defN 80-Jan-01 00:00 orsj_submit/orsj/static/content/navbar-fixed-side.css
 -rw-r--r--  2.0 unx     1058 b- defN 80-Jan-01 00:00 orsj_submit/orsj/static/content/site.css
@@ -40,13 +40,13 @@
 -rw-r--r--  2.0 unx      581 b- defN 80-Jan-01 00:00 orsj_submit/orsj/templates/signup.jade
 -rw-r--r--  2.0 unx     3865 b- defN 80-Jan-01 00:00 orsj_submit/orsj/templates/submit.jade
 -rw-r--r--  2.0 unx     1617 b- defN 80-Jan-01 00:00 orsj_submit/orsj/templates/summary.jade
 -rw-r--r--  2.0 unx    13956 b- defN 80-Jan-01 00:00 orsj_submit/orsj/util.py
 -rw-r--r--  2.0 unx    15473 b- defN 80-Jan-01 00:00 orsj_submit/orsj/views.py
 -rw-r--r--  2.0 unx     2321 b- defN 80-Jan-01 00:00 orsj_submit/setting.yml
 -rwxr-xr-x  2.0 unx      175 b- defN 80-Jan-01 00:00 orsj_submit/start_cmd
--rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 orsj_submit-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 orsj_submit-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 80-Jan-01 00:00 orsj_submit-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx     1541 b- defN 80-Jan-01 00:00 orsj_submit-0.1.1.dist-info/METADATA
-?rw-r--r--  2.0 unx     4937 b- defN 16-Jan-01 00:00 orsj_submit-0.1.1.dist-info/RECORD
-50 files, 1401285 bytes uncompressed, 403848 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 orsj_submit-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 orsj_submit-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 80-Jan-01 00:00 orsj_submit-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx     1490 b- defN 80-Jan-01 00:00 orsj_submit-0.2.0.dist-info/METADATA
+?rw-r--r--  2.0 unx     4937 b- defN 16-Jan-01 00:00 orsj_submit-0.2.0.dist-info/RECORD
+50 files, 1401234 bytes uncompressed, 403846 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -129,23 +129,23 @@
 
 Filename: orsj_submit/setting.yml
 Comment: 
 
 Filename: orsj_submit/start_cmd
 Comment: 
 
-Filename: orsj_submit-0.1.1.dist-info/LICENSE
+Filename: orsj_submit-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: orsj_submit-0.1.1.dist-info/WHEEL
+Filename: orsj_submit-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: orsj_submit-0.1.1.dist-info/entry_points.txt
+Filename: orsj_submit-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: orsj_submit-0.1.1.dist-info/METADATA
+Filename: orsj_submit-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: orsj_submit-0.1.1.dist-info/RECORD
+Filename: orsj_submit-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `orsj_submit-0.1.1.dist-info/LICENSE` & `orsj_submit-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `orsj_submit-0.1.1.dist-info/METADATA` & `orsj_submit-0.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: orsj-submit
-Version: 0.1.1
+Version: 0.2.0
 Summary: Web application of 'submitting papers' in ORSJ.
 Home-page: https://github.com/SaitoTsutomu/orsj-submit
 License: Apache-2.0
 Author: SaitoTsutomu
 Author-email: tsutomu7@hotmail.co.jp
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 
 ## Description
```

## Comparing `orsj_submit-0.1.1.dist-info/RECORD` & `orsj_submit-0.2.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -39,12 +39,12 @@
 orsj_submit/orsj/templates/signup.jade,sha256=TvZZdZh99XOKCL1OmjW-VahK2NMkjRzsmmv-7ayIi8A,581
 orsj_submit/orsj/templates/submit.jade,sha256=LZIqtHfObhKiQM1pS68lJGExhsDUox4_PaLON_cggGM,3865
 orsj_submit/orsj/templates/summary.jade,sha256=znIWGwvDDIjVHWw6IZl4c3up3MtNMcxdA_bj1adSTAk,1617
 orsj_submit/orsj/util.py,sha256=KNMJdsgtgXQvL1y6yz_Ggu_qMtYu8xT9f4pp8PtL6bA,13956
 orsj_submit/orsj/views.py,sha256=yZ3zZZXxaNZOcSC9IUm37lvKiC2CKQjUmb1y7V3dfUk,15473
 orsj_submit/setting.yml,sha256=pvMK20XV7AECDJUu2AewxmLa3A7ozAmslbPFCMWH_Dk,2321
 orsj_submit/start_cmd,sha256=VrY8UKNDyqjT0Ypq2HARn0pg6LzT1pUH-B1i24wm0UE,175
-orsj_submit-0.1.1.dist-info/LICENSE,sha256=P4wG11QaWXFTeHpKANPvc83droyjtsKJwzCAbzqFscA,10757
-orsj_submit-0.1.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-orsj_submit-0.1.1.dist-info/entry_points.txt,sha256=j1XgSiEWlPm9S4ZGsFZ_aeB1OfC1nsmfXbL7URy0Jog,48
-orsj_submit-0.1.1.dist-info/METADATA,sha256=VtPAFqL6oK6lI82oaepS43avMj7AVqUVY7QzjX8D5TI,1541
-orsj_submit-0.1.1.dist-info/RECORD,,
+orsj_submit-0.2.0.dist-info/LICENSE,sha256=P4wG11QaWXFTeHpKANPvc83droyjtsKJwzCAbzqFscA,10757
+orsj_submit-0.2.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+orsj_submit-0.2.0.dist-info/entry_points.txt,sha256=j1XgSiEWlPm9S4ZGsFZ_aeB1OfC1nsmfXbL7URy0Jog,48
+orsj_submit-0.2.0.dist-info/METADATA,sha256=0UCQQHmQT4ibPiqDi8LANUERkk1kahHRZmz7UiCEIS4,1490
+orsj_submit-0.2.0.dist-info/RECORD,,
```

