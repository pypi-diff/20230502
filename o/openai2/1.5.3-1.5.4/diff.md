# Comparing `tmp/openai2-1.5.3.tar.gz` & `tmp/openai2-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.5.3.tar", last modified: Tue May  2 02:44:10 2023, max compression
+gzip compressed data, was "openai2-1.5.4.tar", last modified: Tue May  2 03:05:00 2023, max compression
```

## Comparing `openai2-1.5.3.tar` & `openai2-1.5.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.3/LICENSE
--rw-r--r--   0        0        0     2257 2023-04-30 18:48:25.007298 openai2-1.5.3/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.3/openai2/Licenses of dependent packages/openai/LICENSE
--rw-r--r--   0        0        0       25 2023-03-07 03:18:11.476857 openai2-1.5.3/openai2/__init__.py
--rw-r--r--   0        0        0     2047 2023-05-02 02:37:21.759092 openai2-1.5.3/openai2/openai2.py
--rw-r--r--   0        0        0      634 2023-05-02 02:43:09.620811 openai2-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 openai2-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.4/LICENSE
+-rw-r--r--   0        0        0     2323 2023-05-02 03:00:54.676633 openai2-1.5.4/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.4/openai2/Licenses of dependent packages/openai/LICENSE
+-rw-r--r--   0        0        0       25 2023-03-07 03:18:11.476857 openai2-1.5.4/openai2/__init__.py
+-rw-r--r--   0        0        0     2047 2023-05-02 02:37:21.759092 openai2-1.5.4/openai2/openai2.py
+-rw-r--r--   0        0        0      634 2023-05-02 03:01:32.472779 openai2-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 openai2-1.5.4/PKG-INFO
```

### Comparing `openai2-1.5.3/LICENSE` & `openai2-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.3/README.md` & `openai2-1.5.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -18,35 +18,33 @@
 
 导入：
 
 ```python
 from openai2 import Chat
 ```
 
-创建会话：
+创建对话：
 
 ```python
 api_key = 'api_key'  # 更换成自己的api_key
 
 talk_1 = Chat(api_key=api_key, model="gpt-3.5-turbo")
 talk_2 = Chat(api_key=api_key, model="gpt-3.5-turbo")
 ```
 
 对话：
 
 ```python
 talk_1.request('数字1的后面是几?')
 # >>> 2
-
 talk_2.request('数字101的后面是几?')
 # >>> 102
 
 talk_1.request('再往后是几?')
 # >>> 3
-
 talk_2.request('再往后是几?')
 # >>> 103
 ```
 
 存档：
 
 ```python
@@ -86,14 +84,20 @@
 # >>> [user]: 数字1的后面是几?
 # >>> [assistant]: 2
 
 talk_4.request('再往后是几?')
 # >>> 3
 ```
 
+修改api_key：
+
+```python
+talk_4.api_key = 'new api_key'
+```
+
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
```

### Comparing `openai2-1.5.3/openai2/Licenses of dependent packages/openai/LICENSE` & `openai2-1.5.4/openai2/Licenses of dependent packages/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.3/openai2/openai2.py` & `openai2-1.5.4/openai2/openai2.py`

 * *Files identical despite different names*

### Comparing `openai2-1.5.3/pyproject.toml` & `openai2-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "openai2"
-version = "1.5.3"
+version = "1.5.4"
 description = "根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。"
 dependencies = ["openai >=0.27.0"]
 keywords = ["openai2", "openai"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
```

### Comparing `openai2-1.5.3/PKG-INFO` & `openai2-1.5.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.5.3
+Version: 1.5.4
 Summary: 根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。
 Keywords: openai2,openai
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: openai >=0.27.0
@@ -30,35 +30,33 @@
 
 导入：
 
 ```python
 from openai2 import Chat
 ```
 
-创建会话：
+创建对话：
 
 ```python
 api_key = 'api_key'  # 更换成自己的api_key
 
 talk_1 = Chat(api_key=api_key, model="gpt-3.5-turbo")
 talk_2 = Chat(api_key=api_key, model="gpt-3.5-turbo")
 ```
 
 对话：
 
 ```python
 talk_1.request('数字1的后面是几?')
 # >>> 2
-
 talk_2.request('数字101的后面是几?')
 # >>> 102
 
 talk_1.request('再往后是几?')
 # >>> 3
-
 talk_2.request('再往后是几?')
 # >>> 103
 ```
 
 存档：
 
 ```python
@@ -98,14 +96,20 @@
 # >>> [user]: 数字1的后面是几?
 # >>> [assistant]: 2
 
 talk_4.request('再往后是几?')
 # >>> 3
 ```
 
+修改api_key：
+
+```python
+talk_4.api_key = 'new api_key'
+```
+
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
```

