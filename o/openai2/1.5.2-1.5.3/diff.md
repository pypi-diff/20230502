# Comparing `tmp/openai2-1.5.2.tar.gz` & `tmp/openai2-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.5.2.tar", last modified: Mon May  1 02:01:39 2023, max compression
+gzip compressed data, was "openai2-1.5.3.tar", last modified: Tue May  2 02:44:10 2023, max compression
```

## Comparing `openai2-1.5.2.tar` & `openai2-1.5.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.2/LICENSE
--rw-r--r--   0        0        0     2257 2023-04-30 18:48:25.007298 openai2-1.5.2/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.2/openai2/Licenses of dependent packages/openai/LICENSE
--rw-r--r--   0        0        0       25 2023-03-07 03:18:11.476857 openai2-1.5.2/openai2/__init__.py
--rw-r--r--   0        0        0     2016 2023-03-28 03:12:38.016827 openai2-1.5.2/openai2/openai2.py
--rw-r--r--   0        0        0      634 2023-04-30 19:31:38.138340 openai2-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 openai2-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.3/LICENSE
+-rw-r--r--   0        0        0     2257 2023-04-30 18:48:25.007298 openai2-1.5.3/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.3/openai2/Licenses of dependent packages/openai/LICENSE
+-rw-r--r--   0        0        0       25 2023-03-07 03:18:11.476857 openai2-1.5.3/openai2/__init__.py
+-rw-r--r--   0        0        0     2047 2023-05-02 02:37:21.759092 openai2-1.5.3/openai2/openai2.py
+-rw-r--r--   0        0        0      634 2023-05-02 02:43:09.620811 openai2-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 openai2-1.5.3/PKG-INFO
```

### Comparing `openai2-1.5.2/LICENSE` & `openai2-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.2/README.md` & `openai2-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `openai2-1.5.2/openai2/Licenses of dependent packages/openai/LICENSE` & `openai2-1.5.3/openai2/Licenses of dependent packages/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.2/openai2/openai2.py` & `openai2-1.5.3/openai2/openai2.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,28 +22,30 @@
     def __init__(self, api_key:str, model:str="gpt-3.5-turbo", **kwargs):
         self.api_key = api_key
         self.model = model
         self.messages = []
         self.kwargs = kwargs
 
     def rollback(self, n=1):
-        self.messages = self.messages[:-2*n]
+        self.messages[-2*n:] = []
         for x in self.messages[-2:]:
             print(f"[{x['role']}]: {x['content']}")
     
     def request(self, text:str):
-        self.messages.append({"role": "user", "content": text})
         completion = openai.ChatCompletion.create(
             api_key = self.api_key,
             model = self.model,
-            messages = self.messages,
+            messages = self.messages + [{"role": "user", "content": text}],
              **self.kwargs
         )
         answer:str = completion.choices[0].message['content']
-        self.messages.append({"role": "assistant", "content": answer})
+        self.messages += [
+            {"role": "user", "content": text},
+            {"role": "assistant", "content": answer}
+        ]
         return answer
     
     def dump(self, fpath:str):
         ''' 存档 '''
         jt = jsonDumps(self.messages, ensure_ascii=False)
         Path(fpath).write_text(jt, encoding='utf8')
         return True
```

### Comparing `openai2-1.5.2/pyproject.toml` & `openai2-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "openai2"
-version = "1.5.2"
+version = "1.5.3"
 description = "根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。"
 dependencies = ["openai >=0.27.0"]
 keywords = ["openai2", "openai"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
```

### Comparing `openai2-1.5.2/PKG-INFO` & `openai2-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.5.2
+Version: 1.5.3
 Summary: 根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。
 Keywords: openai2,openai
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: openai >=0.27.0
```

