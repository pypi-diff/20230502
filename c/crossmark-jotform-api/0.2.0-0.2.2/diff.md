# Comparing `tmp/crossmark-jotform-api-0.2.0.tar.gz` & `tmp/crossmark-jotform-api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.2.0.tar", last modified: Mon May  1 20:35:55 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.2.2.tar", last modified: Tue May  2 03:49:32 2023, max compression
```

## Comparing `crossmark-jotform-api-0.2.0.tar` & `crossmark-jotform-api-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 20:35:55.765782 crossmark-jotform-api-0.2.0/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2237 2023-05-01 20:35:55.764786 crossmark-jotform-api-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-05-01 20:35:29.000000 crossmark-jotform-api-0.2.0/README.md
--rw-rw-rw-   0        0        0      789 2023-05-01 20:34:46.000000 crossmark-jotform-api-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 20:35:55.765782 crossmark-jotform-api-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 20:35:55.736780 crossmark-jotform-api-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 20:35:55.747783 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    12272 2023-05-01 20:34:38.000000 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-05-01 20:35:55.760781 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     2237 2023-05-01 20:35:55.000000 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-01 20:35:55.000000 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 20:35:55.000000 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-01 20:35:55.000000 crossmark-jotform-api-0.2.0/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 03:49:32.286161 crossmark-jotform-api-0.2.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2280 2023-05-02 03:49:32.285164 crossmark-jotform-api-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-05-02 03:49:01.000000 crossmark-jotform-api-0.2.2/README.md
+-rw-rw-rw-   0        0        0      789 2023-05-02 03:45:42.000000 crossmark-jotform-api-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 03:49:32.286161 crossmark-jotform-api-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 03:49:32.261161 crossmark-jotform-api-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 03:49:32.270166 crossmark-jotform-api-0.2.2/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    12638 2023-05-02 03:47:51.000000 crossmark-jotform-api-0.2.2/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:49:32.282166 crossmark-jotform-api-0.2.2/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2280 2023-05-02 03:49:32.000000 crossmark-jotform-api-0.2.2/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-02 03:49:32.000000 crossmark-jotform-api-0.2.2/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 03:49:32.000000 crossmark-jotform-api-0.2.2/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-02 03:49:32.000000 crossmark-jotform-api-0.2.2/src/crossmark_jotform_api.egg-info/top_level.txt
```

### Comparing `crossmark-jotform-api-0.2.0/LICENSE` & `crossmark-jotform-api-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.2.0/PKG-INFO` & `crossmark-jotform-api-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.2.0
+Version: 0.2.2
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -33,7 +33,8 @@
 
 # jotform api library for python
 specilized for jotform api and crossmark needs
 
 # updates
 - 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
 - 2023-05-01: added a logic for get_emails function. and added a TODO there.
+- 2023-05-01: setted set_answer function.
```

### Comparing `crossmark-jotform-api-0.2.0/pyproject.toml` & `crossmark-jotform-api-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.2.0"
+version = "0.2.2"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.2.0/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.2.2/src/crossmark_jotform_api/jotForm.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def __print(self, text):
         if self.debug:
             print(text)
 
     def __set_get_submission_data(self, submissions):
         submissions_dict = {}
         for i in submissions:
-            submissions_dict[i["id"]] = jotFormSubmission(i)
+            submissions_dict[i["id"]] = JotFormSubmission(i)
         # sorted_tuples = sorted(submissions_dict.items(), key=lambda x: x[1].id, reverse=True)
         # submissions_dict = dict(sorted_tuples)
         return submissions_dict
 
     def get_submission_ids(self):
         return self.submission_ids
 
@@ -113,14 +113,15 @@
 
     def update_submission_answer(self, submission_id, answer_id, answer):
         self.update()
         query = f'submission[{answer_id}]={answer}'
         url = f"https://api.jotform.com/submission/{submission_id}?apiKey={self.api_key}&{query}"
         response = requests.request("POST", url, timeout=self.timeout)
         if response.status_code == 200:
+            self.submission_data[submission_id].set_answer(answer_id, answer)
             return True
         else:
             return False
 
     def set_url_param(self, key, value):
         value = str(value)
         if key in self.url:
@@ -208,15 +209,15 @@
                 self.__print(
                     f"[INFO] Its been {int(its_been/60)} minutes. Updating submission data...")
                 self.set_data()
                 self.update_timestamp = now
             self.updating_process = False
 
 
-class jotFormSubmission(ABC):
+class JotFormSubmission(ABC):
     def __init__(self, submission_object):
         self.id = submission_object['id']
         self.form_id = submission_object['form_id']
         self.ip = submission_object['ip']
         self.created_at = submission_object['created_at']
         self.status = submission_object['status']
         self.new = submission_object['new']
@@ -267,14 +268,20 @@
                 'type': _type,
                 'text': text,
                 'file': file,
                 'selectedFields': selectedFields
             })
         return answers_arr
 
+    def set_answer(self, answer_id:str, answer_value:str):
+        for i in range(len(self.answers_arr)):
+            if self.answers_arr[i]['key'] == answer_id:
+                self.answers_arr[i]['answer'] = answer_value
+        self.answers[answer_id]['answer'] = answer_value
+
     def get_answers(self):
         return self.answers_arr
 
     def get_answer_by_text(self, text):
         for answer in self.answers_arr:
             if answer['text'] and text and answer['text'].upper() == text.upper():
                 return answer
```

### Comparing `crossmark-jotform-api-0.2.0/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.2.2/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.2.0
+Version: 0.2.2
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -33,7 +33,8 @@
 
 # jotform api library for python
 specilized for jotform api and crossmark needs
 
 # updates
 - 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
 - 2023-05-01: added a logic for get_emails function. and added a TODO there.
+- 2023-05-01: setted set_answer function.
```

