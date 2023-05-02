# Comparing `tmp/cogsgpt-0.0.5.tar.gz` & `tmp/cogsgpt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogsgpt-0.0.5.tar", last modified: Sat Apr 29 15:12:37 2023, max compression
+gzip compressed data, was "cogsgpt-1.0.0.tar", last modified: Tue May  2 14:25:54 2023, max compression
```

## Comparing `cogsgpt-0.0.5.tar` & `cogsgpt-1.0.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.917924 cogsgpt-0.0.5/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-12 05:29:48.000000 cogsgpt-0.0.5/LICENSE
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-24 05:08:50.000000 cogsgpt-0.0.5/MANIFEST.in
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     7365 2023-04-29 15:12:37.917924 cogsgpt-0.0.5/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5622 2023-04-29 15:09:38.000000 cogsgpt-0.0.5/README.md
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.901924 cogsgpt-0.0.5/cogsgpt/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      154 2023-04-29 15:01:53.000000 cogsgpt-0.0.5/cogsgpt/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)    13639 2023-04-29 07:10:23.000000 cogsgpt-0.0.5/cogsgpt/awesome_chat.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.901924 cogsgpt-0.0.5/cogsgpt/cogsmodel/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       92 2023-04-13 04:29:18.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      202 2023-04-25 03:24:15.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/base_model.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.905924 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1058 2023-04-26 07:16:38.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1869 2023-04-26 01:40:24.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/background_remover.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5601 2023-04-28 13:34:38.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/form_recognizer.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     7020 2023-04-27 02:47:18.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/image_analysis_v3.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     6544 2023-04-27 04:13:01.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/image_analysis_v4.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2581 2023-04-28 05:26:48.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/utils.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.909924 cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      599 2023-04-28 03:04:51.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3504 2023-04-27 03:53:31.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1823 2023-04-28 03:12:03.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_generation.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2219 2023-04-27 03:51:10.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_summarize.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1710 2023-04-27 04:05:31.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_translation.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.909924 cogsgpt-0.0.5/cogsgpt/cogsmodel/speech/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       73 2023-04-12 13:18:32.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/speech/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3926 2023-04-27 03:48:02.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/speech/speech.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2835 2023-04-24 07:40:16.000000 cogsgpt-0.0.5/cogsgpt/llm.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      460 2023-04-29 14:44:13.000000 cogsgpt-0.0.5/cogsgpt/logger.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.909924 cogsgpt-0.0.5/cogsgpt/metas/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      316 2023-04-12 04:35:32.000000 cogsgpt-0.0.5/cogsgpt/metas/generate_response_presteps.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2861 2023-04-28 03:41:32.000000 cogsgpt-0.0.5/cogsgpt/metas/parse_task_presteps.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2047 2023-04-28 01:19:48.000000 cogsgpt-0.0.5/cogsgpt/metas/prompts.yaml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     4718 2023-04-28 13:35:33.000000 cogsgpt-0.0.5/cogsgpt/metas/task_metas.yaml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      369 2023-04-27 02:28:37.000000 cogsgpt-0.0.5/cogsgpt/schema.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      892 2023-04-24 07:01:19.000000 cogsgpt-0.0.5/cogsgpt/utils.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.901924 cogsgpt-0.0.5/cogsgpt.egg-info/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     7365 2023-04-29 15:12:37.000000 cogsgpt-0.0.5/cogsgpt.egg-info/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1261 2023-04-29 15:12:37.000000 cogsgpt-0.0.5/cogsgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-29 15:12:37.000000 cogsgpt-0.0.5/cogsgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      189 2023-04-29 15:12:37.000000 cogsgpt-0.0.5/cogsgpt.egg-info/requires.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-29 15:12:37.000000 cogsgpt-0.0.5/cogsgpt.egg-info/top_level.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      932 2023-04-29 15:02:06.000000 cogsgpt-0.0.5/pyproject.toml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-29 15:12:37.917924 cogsgpt-0.0.5/setup.cfg
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.913924 cogsgpt-0.0.5/tests/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1763 2023-04-28 13:14:29.000000 cogsgpt-0.0.5/tests/test_awesome_chat.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      550 2023-04-26 01:38:49.000000 cogsgpt-0.0.5/tests/test_bg_remove.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2840 2023-04-27 02:44:47.000000 cogsgpt-0.0.5/tests/test_form_recognizer.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     4952 2023-04-27 01:52:52.000000 cogsgpt-0.0.5/tests/test_image_analisys.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      602 2023-04-26 14:09:19.000000 cogsgpt-0.0.5/tests/test_speech.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1632 2023-04-26 14:18:48.000000 cogsgpt-0.0.5/tests/test_text_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1232 2023-04-28 03:12:51.000000 cogsgpt-0.0.5/tests/test_text_generation.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1971 2023-04-24 07:02:12.000000 cogsgpt-0.0.5/tests/test_text_summarize.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1195 2023-04-27 04:15:40.000000 cogsgpt-0.0.5/tests/test_text_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.424562 cogsgpt-1.0.0/cogsgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/awesome_chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/cogsgpt/cogsmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/background_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/form_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/image_analysis_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/image_analysis_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/cogsgpt/cogsmodel/speech/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/speech/speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/cogsgpt/metas/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/metas/generate_response_presteps.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/metas/parse_task_presteps.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/metas/prompts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/metas/task_metas.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/cogsgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-02 14:25:54.000000 cogsgpt-1.0.0/cogsgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-02 14:25:54.000000 cogsgpt-1.0.0/cogsgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:25:54.000000 cogsgpt-1.0.0/cogsgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-02 14:25:54.000000 cogsgpt-1.0.0/cogsgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 14:25:54.000000 cogsgpt-1.0.0/cogsgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_awesome_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_bg_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_form_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_image_analisys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_text_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_text_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_text_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_text_translation.py
```

### Comparing `cogsgpt-0.0.5/LICENSE` & `cogsgpt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/PKG-INFO` & `cogsgpt-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 0.0.5
+Version: 1.0.0
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,14 +37,16 @@
 # CogsGPT
 A conversational system which integrates ChatGPT with Azure Cognitive Services to achieve multimodal capabilities.
 
 <a src="https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20Spaces-blue" href="https://huggingface.co/spaces/whiskyboy/CogsGPT">
     <img src="https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20Spaces-blue" alt="Open in Spaces">
 </a>
 
+![cogsgpt-demo](./docs/imgs/cogsgpt-demo.png)
+
 *If you find this repo useful, please consider giving it a star! :)*
 
 ## Updates
 - [2023.04.28] **Now you can go to [CogsGPT on Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT) to experience the full capabilities of CogsGPT!!!** We are offering an Azure Cognitive Service resource for FREE to use in the demo. All you need is an OpenAI API key to get started chatting with CogsGPT!
 - [2023.04.25] CogsGPT now supports **image** type output! You can ask CogsGPT to crop a thumbnail of an image, or remove its background.
 - [2023.04.18] Release the first version of CogsGPT!
```

### Comparing `cogsgpt-0.0.5/README.md` & `cogsgpt-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # CogsGPT
 A conversational system which integrates ChatGPT with Azure Cognitive Services to achieve multimodal capabilities.
 
 <a src="https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20Spaces-blue" href="https://huggingface.co/spaces/whiskyboy/CogsGPT">
     <img src="https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20Spaces-blue" alt="Open in Spaces">
 </a>
 
+![cogsgpt-demo](./docs/imgs/cogsgpt-demo.png)
+
 *If you find this repo useful, please consider giving it a star! :)*
 
 ## Updates
 - [2023.04.28] **Now you can go to [CogsGPT on Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT) to experience the full capabilities of CogsGPT!!!** We are offering an Azure Cognitive Service resource for FREE to use in the demo. All you need is an OpenAI API key to get started chatting with CogsGPT!
 - [2023.04.25] CogsGPT now supports **image** type output! You can ask CogsGPT to crop a thumbnail of an image, or remove its background.
 - [2023.04.18] Release the first version of CogsGPT!
```

### Comparing `cogsgpt-0.0.5/cogsgpt/awesome_chat.py` & `cogsgpt-1.0.0/cogsgpt/awesome_chat.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/__init__.py` & `cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/__init__.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/background_remover.py` & `cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/background_remover.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/form_recognizer.py` & `cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/form_recognizer.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/image_analysis_v3.py` & `cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/image_analysis_v3.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/image_analysis_v4.py` & `cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/image_analysis_v4.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/utils.py` & `cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/utils.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/__init__.py` & `cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_analysis.py` & `cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_generation.py` & `cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_generation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_summarize.py` & `cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_summarize.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_translation.py` & `cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_translation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/cogsmodel/speech/speech.py` & `cogsgpt-1.0.0/cogsgpt/cogsmodel/speech/speech.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/llm.py` & `cogsgpt-1.0.0/cogsgpt/llm.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/metas/parse_task_presteps.json` & `cogsgpt-1.0.0/cogsgpt/metas/parse_task_presteps.json`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/metas/prompts.yaml` & `cogsgpt-1.0.0/cogsgpt/metas/prompts.yaml`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/metas/task_metas.yaml` & `cogsgpt-1.0.0/cogsgpt/metas/task_metas.yaml`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt/utils.py` & `cogsgpt-1.0.0/cogsgpt/utils.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/cogsgpt.egg-info/PKG-INFO` & `cogsgpt-1.0.0/cogsgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 0.0.5
+Version: 1.0.0
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,14 +37,16 @@
 # CogsGPT
 A conversational system which integrates ChatGPT with Azure Cognitive Services to achieve multimodal capabilities.
 
 <a src="https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20Spaces-blue" href="https://huggingface.co/spaces/whiskyboy/CogsGPT">
     <img src="https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20Spaces-blue" alt="Open in Spaces">
 </a>
 
+![cogsgpt-demo](./docs/imgs/cogsgpt-demo.png)
+
 *If you find this repo useful, please consider giving it a star! :)*
 
 ## Updates
 - [2023.04.28] **Now you can go to [CogsGPT on Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT) to experience the full capabilities of CogsGPT!!!** We are offering an Azure Cognitive Service resource for FREE to use in the demo. All you need is an OpenAI API key to get started chatting with CogsGPT!
 - [2023.04.25] CogsGPT now supports **image** type output! You can ask CogsGPT to crop a thumbnail of an image, or remove its background.
 - [2023.04.18] Release the first version of CogsGPT!
```

### Comparing `cogsgpt-0.0.5/cogsgpt.egg-info/SOURCES.txt` & `cogsgpt-1.0.0/cogsgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/pyproject.toml` & `cogsgpt-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cogsgpt"
-version = "0.0.5"
+version = "1.0.0"
 description = "A multi-modal LLM integrated ChatGPT with Azure Cognitive Service"
 readme = "README.md"
 authors = [{ name = "weitian", email = "weitian.bnu@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `cogsgpt-0.0.5/tests/test_awesome_chat.py` & `cogsgpt-1.0.0/tests/test_awesome_chat.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/tests/test_bg_remove.py` & `cogsgpt-1.0.0/tests/test_bg_remove.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/tests/test_form_recognizer.py` & `cogsgpt-1.0.0/tests/test_form_recognizer.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/tests/test_image_analisys.py` & `cogsgpt-1.0.0/tests/test_image_analisys.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/tests/test_speech.py` & `cogsgpt-1.0.0/tests/test_speech.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/tests/test_text_analysis.py` & `cogsgpt-1.0.0/tests/test_text_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/tests/test_text_generation.py` & `cogsgpt-1.0.0/tests/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/tests/test_text_summarize.py` & `cogsgpt-1.0.0/tests/test_text_summarize.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.5/tests/test_text_translation.py` & `cogsgpt-1.0.0/tests/test_text_translation.py`

 * *Files identical despite different names*

