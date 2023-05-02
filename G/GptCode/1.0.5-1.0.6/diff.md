# Comparing `tmp/GptCode-1.0.5.tar.gz` & `tmp/GptCode-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GptCode-1.0.5.tar", last modified: Tue May  2 07:56:39 2023, max compression
+gzip compressed data, was "GptCode-1.0.6.tar", last modified: Tue May  2 07:59:54 2023, max compression
```

## Comparing `GptCode-1.0.5.tar` & `GptCode-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 07:56:39.144641 GptCode-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-05-02 07:56:39.116019 GptCode-1.0.5/GptCode/
--rw-rw-rw-   0        0        0        0 2023-05-01 13:39:37.000000 GptCode-1.0.5/GptCode/__init__.py
--rw-rw-rw-   0        0        0     4747 2023-05-02 07:55:57.000000 GptCode-1.0.5/GptCode/gpt.py
-drwxrwxrwx   0        0        0        0 2023-05-02 07:56:39.136635 GptCode-1.0.5/GptCode.egg-info/
--rw-rw-rw-   0        0        0      167 2023-05-02 07:56:38.000000 GptCode-1.0.5/GptCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-02 07:56:38.000000 GptCode-1.0.5/GptCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 07:56:38.000000 GptCode-1.0.5/GptCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 07:56:38.000000 GptCode-1.0.5/GptCode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2023-05-02 07:56:39.142637 GptCode-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-02 07:56:39.145637 GptCode-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      371 2023-05-02 07:56:30.000000 GptCode-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:59:54.186029 GptCode-1.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-02 07:59:54.158025 GptCode-1.0.6/GptCode/
+-rw-rw-rw-   0        0        0        0 2023-05-01 13:39:37.000000 GptCode-1.0.6/GptCode/__init__.py
+-rw-rw-rw-   0        0        0     4771 2023-05-02 07:58:08.000000 GptCode-1.0.6/GptCode/gpt.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:59:54.178028 GptCode-1.0.6/GptCode.egg-info/
+-rw-rw-rw-   0        0        0      167 2023-05-02 07:59:53.000000 GptCode-1.0.6/GptCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-05-02 07:59:53.000000 GptCode-1.0.6/GptCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 07:59:53.000000 GptCode-1.0.6/GptCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 07:59:53.000000 GptCode-1.0.6/GptCode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2023-05-02 07:59:54.184028 GptCode-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-02 07:59:54.187029 GptCode-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      371 2023-05-02 07:59:50.000000 GptCode-1.0.6/setup.py
```

### Comparing `GptCode-1.0.5/GptCode/gpt.py` & `GptCode-1.0.6/GptCode/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         :return: 翻译结果
         """
         trans = f"请把以下语言翻译为{aim_language}。"
         response = self.get_answer(messages=self.system_setting_list + [{'role': 'user', 'content': trans+prompt}])
         return response
 
     def extract_picture_prompt(self,prompt):
-        extract = "请从以下句子中提取出对图片的描述，或者想象一下图片的描述，描述请尽量详细。"
+        extract = "以下句子描述了一张图片，请从中提取出对图片的描述，或者想象一下图片的描述，描述请尽量详细。"
         response = self.get_answer(messages=self.system_setting_list + [{'role': 'user', 'content': extract + prompt}])
         return response
 
     def get_answer(self, messages):
         response = openai.ChatCompletion.create(model=self.model, messages=messages)
         answer = response.choices[0].message['content']
         return answer
```

