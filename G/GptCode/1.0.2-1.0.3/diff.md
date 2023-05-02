# Comparing `tmp/GptCode-1.0.2.tar.gz` & `tmp/GptCode-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GptCode-1.0.2.tar", last modified: Mon May  1 15:40:20 2023, max compression
+gzip compressed data, was "GptCode-1.0.3.tar", last modified: Tue May  2 06:51:24 2023, max compression
```

## Comparing `GptCode-1.0.2.tar` & `GptCode-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 15:40:20.871071 GptCode-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-01 15:40:20.847314 GptCode-1.0.2/GptCode/
--rw-rw-rw-   0        0        0        0 2023-05-01 13:39:37.000000 GptCode-1.0.2/GptCode/__init__.py
--rw-rw-rw-   0        0        0     2991 2023-05-01 15:38:06.000000 GptCode-1.0.2/GptCode/gpt.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:40:20.865252 GptCode-1.0.2/GptCode.egg-info/
--rw-rw-rw-   0        0        0      165 2023-05-01 15:40:20.000000 GptCode-1.0.2/GptCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-01 15:40:20.000000 GptCode-1.0.2/GptCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 15:40:20.000000 GptCode-1.0.2/GptCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 15:40:20.000000 GptCode-1.0.2/GptCode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      165 2023-05-01 15:40:20.869253 GptCode-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-01 15:40:20.871071 GptCode-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      369 2023-05-01 15:38:52.000000 GptCode-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:51:24.590875 GptCode-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-02 06:51:24.564858 GptCode-1.0.3/GptCode/
+-rw-rw-rw-   0        0        0        0 2023-05-01 13:39:37.000000 GptCode-1.0.3/GptCode/__init__.py
+-rw-rw-rw-   0        0        0     3874 2023-05-02 06:50:46.000000 GptCode-1.0.3/GptCode/gpt.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:51:24.583856 GptCode-1.0.3/GptCode.egg-info/
+-rw-rw-rw-   0        0        0      165 2023-05-02 06:51:24.000000 GptCode-1.0.3/GptCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-05-02 06:51:24.000000 GptCode-1.0.3/GptCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 06:51:24.000000 GptCode-1.0.3/GptCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 06:51:24.000000 GptCode-1.0.3/GptCode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      165 2023-05-02 06:51:24.588873 GptCode-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-02 06:51:24.590875 GptCode-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      369 2023-05-02 06:51:11.000000 GptCode-1.0.3/setup.py
```

### Comparing `GptCode-1.0.2/GptCode/gpt.py` & `GptCode-1.0.3/GptCode/gpt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 import openai
+from PIL import Image
+from io import BytesIO
+import requests
+from IPython.display import display
 
 class Chat:
     def __init__(self, api_key, system_setting=None, language="中文", model="gpt-3.5-turbo") -> None:
 
         # Apply the API key
         openai.api_key = api_key
 
@@ -40,14 +44,36 @@
         return prompt
 
     def get_answer(self, messages):
         response = openai.ChatCompletion.create(model=self.model, messages=messages)
         answer = response.choices[0].message['content']
         return answer
 
+    def painting(self,prompt,image_size = "1024x1024",return_img = False):
+        """
+        :param prompt: 图像描述
+        :param image_size: 图像大小
+        :param return_img: 是否返回图像，若不返回则直接展示
+        :return: 图像
+        """
+        response = openai.Image.create(
+            prompt=prompt,
+            n=1,
+            size=image_size
+        )
+        url = response['data'][0]['url']
+        # 获取图片链接的二进制数据
+        response = requests.get(url)
+        image_data = response.content
+
+        # 将二进制数据转换成图片对象并展示
+        image = Image.open(BytesIO(image_data))
+        if return_img:
+            return response['data'][0]['url']
+        display(image)
     # 提示chatgpt
     def ask(self, prompt,reference=True, use_history=False, history_number=5):
         """
         :param prompt:问题描述
         :param reference: 是否列出参考的资料来源
         :param use_history: 是否参考历史对话信息
         :param history_number: 参考历史对话信息的条数
```

