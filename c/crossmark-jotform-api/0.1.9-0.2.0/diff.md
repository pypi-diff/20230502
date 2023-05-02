# Comparing `tmp/crossmark-jotform-api-0.1.9.tar.gz` & `tmp/crossmark-jotform-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.1.9.tar", last modified: Thu Apr 27 07:04:10 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.2.0.tar", last modified: Mon May  1 20:35:55 2023, max compression
```

## Comparing `crossmark-jotform-api-0.1.9.tar` & `crossmark-jotform-api-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 07:04:10.637871 crossmark-jotform-api-0.1.9/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     2159 2023-04-27 07:04:10.635866 crossmark-jotform-api-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-26 20:32:45.000000 crossmark-jotform-api-0.1.9/README.md
--rw-rw-rw-   0        0        0      789 2023-04-27 07:03:06.000000 crossmark-jotform-api-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 07:04:10.637871 crossmark-jotform-api-0.1.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 07:04:10.617869 crossmark-jotform-api-0.1.9/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 07:04:10.625869 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    12041 2023-04-27 07:03:35.000000 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:04:10.633866 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     2159 2023-04-27 07:04:10.000000 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-04-27 07:04:10.000000 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 07:04:10.000000 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-27 07:04:10.000000 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 20:35:55.765782 crossmark-jotform-api-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2237 2023-05-01 20:35:55.764786 crossmark-jotform-api-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-05-01 20:35:29.000000 crossmark-jotform-api-0.2.0/README.md
+-rw-rw-rw-   0        0        0      789 2023-05-01 20:34:46.000000 crossmark-jotform-api-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 20:35:55.765782 crossmark-jotform-api-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 20:35:55.736780 crossmark-jotform-api-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 20:35:55.747783 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    12272 2023-05-01 20:34:38.000000 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:35:55.760781 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2237 2023-05-01 20:35:55.000000 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-01 20:35:55.000000 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 20:35:55.000000 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-01 20:35:55.000000 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api.egg-info/top_level.txt
```

### Comparing `crossmark-jotform-api-0.1.9/LICENSE` & `crossmark-jotform-api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.1.9/PKG-INFO` & `crossmark-jotform-api-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.1.9
+Version: 0.2.0
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -32,7 +32,8 @@
 License-File: LICENSE
 
 # jotform api library for python
 specilized for jotform api and crossmark needs
 
 # updates
 - 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
+- 2023-05-01: added a logic for get_emails function. and added a TODO there.
```

### Comparing `crossmark-jotform-api-0.1.9/pyproject.toml` & `crossmark-jotform-api-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.1.9/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.2.0/src/crossmark_jotform_api/jotForm.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,14 +227,15 @@
         self.answers_arr = self.set_answers(self.answers)
         self.case_id = self.get_answer_by_text('CASE')['answer']
         self.editor = self.get_answer_by_text('EDITOR')['answer']
         self.status = self.get_answer_by_text('STATUS')['answer']
         self.store = self.get_answer_by_text('STORE')['answer']
         self.GUID = self.get_answer_by_text('GUID')['answer']
         self.client = self.get_answer_by_text('CLIENT')['answer']
+        self.emails = self.get_emails()
 
     def set_answers(self, answers):
         answers_arr = []
         for key, value in answers.items():
             if 'name' in value:
                 name = value['name']
             else:
@@ -288,14 +289,18 @@
     def get_answer_by_key(self, key):
         for answer in self.answers_arr:
             if answer['key'] and key and answer['key'] == key:
                 return answer
         return {'answer': None}
 
     def get_emails(self):
+        # unsave method
+        # TODO: fix this with a better logic that always track if there is a changed happened in the class
+        if self.emails:
+            return self.emails
         emails = []
         for answer in self.answers_arr:
             if answer['type'] == 'control_email':
                 emails.append(answer['answer'])
         return emails
 
     def get_day_from_date(self, date):
```

### Comparing `crossmark-jotform-api-0.1.9/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.2.0/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.1.9
+Version: 0.2.0
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -32,7 +32,8 @@
 License-File: LICENSE
 
 # jotform api library for python
 specilized for jotform api and crossmark needs
 
 # updates
 - 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
+- 2023-05-01: added a logic for get_emails function. and added a TODO there.
```

