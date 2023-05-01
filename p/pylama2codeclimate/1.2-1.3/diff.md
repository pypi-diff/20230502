# Comparing `tmp/pylama2codeclimate-1.2-py3-none-any.whl.zip` & `tmp/pylama2codeclimate-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 4685 bytes, number of entries: 8
--rw-r--r--  2.0 unx     4307 b- defN 17-Dec-15 05:33 pylama2codeclimate.py
--rw-r--r--  2.0 unx      618 b- defN 17-Dec-15 05:33 pylama2codeclimate-1.2.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx       64 b- defN 17-Dec-15 05:33 pylama2codeclimate-1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx      678 b- defN 17-Dec-15 05:33 pylama2codeclimate-1.2.dist-info/metadata.json
--rw-r--r--  2.0 unx       19 b- defN 17-Dec-15 05:33 pylama2codeclimate-1.2.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 17-Dec-15 05:33 pylama2codeclimate-1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      927 b- defN 17-Dec-15 05:33 pylama2codeclimate-1.2.dist-info/METADATA
--rw-r--r--  2.0 unx      729 b- defN 17-Dec-15 05:33 pylama2codeclimate-1.2.dist-info/RECORD
-8 files, 7434 bytes uncompressed, 3399 bytes compressed:  54.3%
+Zip file size: 4370 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     4306 b- defN 23-May-01 23:05 pylama2codeclimate.py
+-rw-rw-rw-  2.0 unx     1063 b- defN 23-May-01 23:06 pylama2codeclimate-1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      895 b- defN 23-May-01 23:06 pylama2codeclimate-1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-01 23:06 pylama2codeclimate-1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 23-May-01 23:06 pylama2codeclimate-1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-May-01 23:06 pylama2codeclimate-1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      612 b- defN 23-May-01 23:06 pylama2codeclimate-1.3.dist-info/RECORD
+7 files, 7050 bytes uncompressed, 3268 bytes compressed:  53.6%
```

## zipnote {}

```diff
@@ -1,25 +1,22 @@
 Filename: pylama2codeclimate.py
 Comment: 
 
-Filename: pylama2codeclimate-1.2.dist-info/DESCRIPTION.rst
+Filename: pylama2codeclimate-1.3.dist-info/LICENSE
 Comment: 
 
-Filename: pylama2codeclimate-1.2.dist-info/entry_points.txt
+Filename: pylama2codeclimate-1.3.dist-info/METADATA
 Comment: 
 
-Filename: pylama2codeclimate-1.2.dist-info/metadata.json
+Filename: pylama2codeclimate-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pylama2codeclimate-1.2.dist-info/top_level.txt
+Filename: pylama2codeclimate-1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pylama2codeclimate-1.2.dist-info/WHEEL
+Filename: pylama2codeclimate-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pylama2codeclimate-1.2.dist-info/METADATA
-Comment: 
-
-Filename: pylama2codeclimate-1.2.dist-info/RECORD
+Filename: pylama2codeclimate-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylama2codeclimate.py

```diff
@@ -12,15 +12,15 @@
 """
 main.py:22:1: [W] W0611 'logger.domainlogging' imported but unused [pyflakes]
 file1.py:58:1: [E] E0602 undefined name 'SetupNamedSized' [pyflakes]
 file2.py:149:1: [C] C901 'QueueListener._monitor' is too complex (11) [mccabe]
 file2.py:94:1: [W] W0612 local variable 'ret' is assigned to but never used [pyflakes]
 """
 
-parser = re.compile(r'^(?P<path>.*?):(?P<line>\d+?):(?P<column>\d+?): \[(?P<severity>\S)\] (?P<check_name>\S+?) (?P<description>.+) \[(?P<checker>\S+)\]$')
+parser = re.compile(r'^(?P<path>.*?):(?P<line>\d+?):(?P<column>\d+?) \[(?P<severity>\S)\] (?P<check_name>\S+?) (?P<description>.+) \[(?P<checker>\S+)\]$')
 
 
 def issue(check_name, description, categories, location,
           content=None, trace=None, remediation_points=None, severity=None, fingerprint=None, engine_name=None):
     """
     CodeClimate Issue: https://github.com/codeclimate/spec/blob/master/SPEC.md#issues
     :param str  check_name: Required. A unique name representing the static analysis check that emitted this issue.
```

## Comparing `pylama2codeclimate-1.2.dist-info/DESCRIPTION.rst` & `pylama2codeclimate-1.3.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: pylama2codeclimate
+Version: 1.3
+Summary: Converts the (parsable) pylama output to codeclimate.json format
+Home-page: https://gitlab.com/alelec/pylama2codeclimate
+Author: Andrew Leech
+Author-email: andrew@alelec.net
+License: MIT
+License-File: LICENSE
+
 pylama2codeclimate
 ==================
 
 Converts the (parsable) pylama output to codeclimate.json format.
 This was written with the intention of using pylama to analyse python programs and report the output to gitlab ci code quality feature:
 https://docs.gitlab.com/ee/user/project/merge_requests/code_quality_diff.html
 
@@ -13,9 +23,7 @@
       stage: test
       script:
         - pip3 install pylama2codeclimate pylama
         - pylama --format parsable | pylama2codeclimate > codeclimate.json
       artifacts:
         when: always
         paths: [codeclimate.json]
-
-
```

