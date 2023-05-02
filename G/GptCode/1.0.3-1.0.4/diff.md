# Comparing `tmp/GptCode-1.0.3.tar.gz` & `tmp/GptCode-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GptCode-1.0.3.tar", last modified: Tue May  2 06:51:24 2023, max compression
+gzip compressed data, was "GptCode-1.0.4.tar", last modified: Tue May  2 07:25:02 2023, max compression
```

## Comparing `GptCode-1.0.3.tar` & `GptCode-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 06:51:24.590875 GptCode-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-02 06:51:24.564858 GptCode-1.0.3/GptCode/
--rw-rw-rw-   0        0        0        0 2023-05-01 13:39:37.000000 GptCode-1.0.3/GptCode/__init__.py
--rw-rw-rw-   0        0        0     3874 2023-05-02 06:50:46.000000 GptCode-1.0.3/GptCode/gpt.py
-drwxrwxrwx   0        0        0        0 2023-05-02 06:51:24.583856 GptCode-1.0.3/GptCode.egg-info/
--rw-rw-rw-   0        0        0      165 2023-05-02 06:51:24.000000 GptCode-1.0.3/GptCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-02 06:51:24.000000 GptCode-1.0.3/GptCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 06:51:24.000000 GptCode-1.0.3/GptCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 06:51:24.000000 GptCode-1.0.3/GptCode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      165 2023-05-02 06:51:24.588873 GptCode-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-02 06:51:24.590875 GptCode-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      369 2023-05-02 06:51:11.000000 GptCode-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:25:01.997131 GptCode-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-02 07:25:01.971128 GptCode-1.0.4/GptCode/
+-rw-rw-rw-   0        0        0        0 2023-05-01 13:39:37.000000 GptCode-1.0.4/GptCode/__init__.py
+-rw-rw-rw-   0        0        0     4672 2023-05-02 07:24:16.000000 GptCode-1.0.4/GptCode/gpt.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:25:01.990112 GptCode-1.0.4/GptCode.egg-info/
+-rw-rw-rw-   0        0        0      167 2023-05-02 07:25:01.000000 GptCode-1.0.4/GptCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-05-02 07:25:01.000000 GptCode-1.0.4/GptCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 07:25:01.000000 GptCode-1.0.4/GptCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 07:25:01.000000 GptCode-1.0.4/GptCode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2023-05-02 07:25:01.996115 GptCode-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-02 07:25:01.998113 GptCode-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      371 2023-05-02 07:24:55.000000 GptCode-1.0.4/setup.py
```

### Comparing `GptCode-1.0.3/GptCode/gpt.py` & `GptCode-1.0.4/GptCode/gpt.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,26 +39,43 @@
         ask_type:问题类型
         """
         # 这部分函数有待更新
         tail_message = "列出你所参考的资料来源,请你一步一步来,并仔细思考你的行为逻辑,核查你输出的信息。"
         prompt = prompt + tail_message
         return prompt
 
+    def translate(self,prompt,aim_language = "英语"):
+        """
+        :param prompt: 原始语言
+        :param aim_language: 要翻译成的语种
+        :return: 翻译结果
+        """
+        trans = f"请把以下语言翻译为{aim_language}。"
+        response = self.get_answer(messages=self.system_setting_list + [{'role': 'user', 'content': trans+prompt}])
+        return response
+
+    def extract_picture_prompt(self,prompt):
+        extract = "请从以下句子中提取出对图片的描述，描述请尽量详细。"
+        response = self.get_answer(messages=self.system_setting_list + [{'role': 'user', 'content': extract + prompt}])
+        return response
+
     def get_answer(self, messages):
         response = openai.ChatCompletion.create(model=self.model, messages=messages)
         answer = response.choices[0].message['content']
         return answer
 
     def painting(self,prompt,image_size = "1024x1024",return_img = False):
         """
         :param prompt: 图像描述
         :param image_size: 图像大小
         :param return_img: 是否返回图像，若不返回则直接展示
         :return: 图像
         """
+        prompt = self.extract_picture_prompt(prompt)
+        prompt = self.translate(prompt)
         response = openai.Image.create(
             prompt=prompt,
             n=1,
             size=image_size
         )
         url = response['data'][0]['url']
         # 获取图片链接的二进制数据
```

