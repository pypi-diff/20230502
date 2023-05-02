# Comparing `tmp/jojo-ai-0.1.2.tar.gz` & `tmp/jojo-ai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jojo-ai-0.1.2.tar", last modified: Tue May  2 14:40:50 2023, max compression
+gzip compressed data, was "dist\jojo-ai-0.1.3.tar", last modified: Tue May  2 15:14:51 2023, max compression
```

## Comparing `jojo-ai-0.1.2.tar` & `jojo-ai-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 14:40:50.000000 jojo-ai-0.1.2/
--rw-rw-rw-   0        0        0    11523 2022-08-30 15:00:03.000000 jojo-ai-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      168 2023-05-01 13:35:05.000000 jojo-ai-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1029 2023-05-02 14:40:50.000000 jojo-ai-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-05-01 13:42:45.000000 jojo-ai-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 14:40:50.000000 jojo-ai-0.1.2/ai/
--rw-rw-rw-   0        0        0      190 2023-05-02 14:40:27.000000 jojo-ai-0.1.2/ai/__init__.py
--rw-rw-rw-   0        0        0    30074 2023-05-01 15:39:37.000000 jojo-ai-0.1.2/ai/baidu.py
--rw-rw-rw-   0        0        0     5627 2023-05-02 13:02:01.000000 jojo-ai-0.1.2/ai/baidu_demo.py
-drwxrwxrwx   0        0        0        0 2023-05-02 14:40:50.000000 jojo-ai-0.1.2/jojo_ai.egg-info/
--rw-rw-rw-   0        0        0     1029 2023-05-02 14:40:49.000000 jojo-ai-0.1.2/jojo_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-02 14:40:49.000000 jojo-ai-0.1.2/jojo_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 14:40:49.000000 jojo-ai-0.1.2/jojo_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 14:40:49.000000 jojo-ai-0.1.2/jojo_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2023-05-02 14:40:49.000000 jojo-ai-0.1.2/jojo_ai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 14:40:50.000000 jojo-ai-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2026 2023-05-02 14:40:15.000000 jojo-ai-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:14:51.000000 jojo-ai-0.1.3/
+-rw-rw-rw-   0        0        0    11523 2022-08-30 15:00:03.000000 jojo-ai-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      168 2023-05-01 13:35:05.000000 jojo-ai-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1029 2023-05-02 15:14:51.000000 jojo-ai-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-05-01 13:42:45.000000 jojo-ai-0.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 15:14:51.000000 jojo-ai-0.1.3/ai/
+-rw-rw-rw-   0        0        0      190 2023-05-02 15:14:28.000000 jojo-ai-0.1.3/ai/__init__.py
+-rw-rw-rw-   0        0        0    31557 2023-05-02 15:07:15.000000 jojo-ai-0.1.3/ai/baidu.py
+-rw-rw-rw-   0        0        0     5961 2023-05-02 15:14:04.000000 jojo-ai-0.1.3/ai/baidu_demo.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:14:51.000000 jojo-ai-0.1.3/jojo_ai.egg-info/
+-rw-rw-rw-   0        0        0     1029 2023-05-02 15:14:51.000000 jojo-ai-0.1.3/jojo_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-02 15:14:51.000000 jojo-ai-0.1.3/jojo_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 15:14:51.000000 jojo-ai-0.1.3/jojo_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 15:14:51.000000 jojo-ai-0.1.3/jojo_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2023-05-02 15:14:51.000000 jojo-ai-0.1.3/jojo_ai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 15:14:51.000000 jojo-ai-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2026 2023-05-02 15:14:23.000000 jojo-ai-0.1.3/setup.py
```

### Comparing `jojo-ai-0.1.2/LICENSE.txt` & `jojo-ai-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jojo-ai-0.1.2/PKG-INFO` & `jojo-ai-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jojo-ai
-Version: 0.1.2
+Version: 0.1.3
 Summary: API of AI of Baidu, ChatGPT, etc.
 Home-page: https://www.jostudio.com.cn/python
 Author: JoStudio
 Author-email: jostudio@189.cn
 License: Apache License 2.0
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `jojo-ai-0.1.2/ai/baidu.py` & `jojo-ai-0.1.3/ai/baidu.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             else:
                 return self._error(response_json)
 
     def asr(self, audio_filename):
         """
         语音转文字
 
-        https://ai.baidu.com/ai-doc/SPEECH/Vk38lxily
+        API文档: https://ai.baidu.com/ai-doc/SPEECH/Vk38lxily
 
         :param audio_filename: 语音文件名，格式可以是 .wav, .mp3, .amr, .m4a.
                     必须是16000采样率、单声道
         :return: 返回文字结果
         """
         self._update_token()  # 首先，检查access token
 
@@ -184,15 +184,15 @@
             return self._result(response.json(), 'result')
         return self._error(500, 'error request Baidu ASR')
 
     def tts(self, text, save_filename='', person=0, speed=5, volume=5, pitch=5):
         """
         文字转语音
 
-        https://cloud.baidu.com/doc/SPEECH/s/Gk38y8lzk
+        API文档: https://cloud.baidu.com/doc/SPEECH/s/Gk38y8lzk
 
         :param text: 文字
         :param save_filename: 存盘文件名。如文件名为空，则直接播放声音。
         :param person: (可选) 说话人， 可以是：‘小美’，'小宇’，‘逍遥’，‘丫丫’, '小鹿', '博文', '小童', '小萌', '米朵', '小娇'
         :param speed: (可选)语速，取值0-15，默认为5中语速
         :param volume: (可选) 音量，取值0-15，默认为5中音量（取值为0时为音量最小值，并非为无声）
         :param pitch:  (可选) 音调，取值0-15，默认为5中语调
@@ -302,40 +302,40 @@
 
         return self._error(500, 'error request Baidu OCR')
 
     def ocr(self, image_file):
         """
         通用文字识别
 
-        https://ai.baidu.com/ai-doc/OCR/zk3h7xz52
+        API文档: https://ai.baidu.com/ai-doc/OCR/zk3h7xz52
 
         :param image_file: 图片文件名或URL
         :return: 返回文字识别结果
         """
         return self._ocr_api(image_file, "https://aip.baidubce.com/rest/2.0/ocr/v1/accurate_basic",
                              None, 'words_result')
 
     def ocr_id_card(self, image_file):
         """
         身份证识别
 
-        https://ai.baidu.com/ai-doc/OCR/rk3h7xzck
+        API文档: https://ai.baidu.com/ai-doc/OCR/rk3h7xzck
 
         :param image_file: 身份证图片文件名或URL
         :return: 返回识别结果
         """
         params = {'id_card_side': 'front', 'detect_photo': 'true'}
         return self._ocr_api(image_file, "https://aip.baidubce.com/rest/2.0/ocr/v1/idcard",
                              params)
 
     def ocr_bank_card(self, image_file):
         """
         银行卡识别
 
-        https://ai.baidu.com/ai-doc/OCR/ak3h7xxg3
+        API文档: https://ai.baidu.com/ai-doc/OCR/ak3h7xxg3
 
         :param image_file: 图片文件名或URL
         :return: 返回识别结果
         """
         return self._ocr_api(image_file, "https://aip.baidubce.com/rest/2.0/ocr/v1/bankcard",
                              None, 'result')
 
@@ -353,15 +353,15 @@
             params = {"image": image_file, 'image_type': 'FACE_TOKEN'}
         return params
 
     def face_detect(self, image_file, face_field='', corp_image=True, max_faces=4):
         """
         人脸检测
 
-        https://ai.baidu.com/ai-doc/FACE/yk37c1u4t
+        API文档: https://ai.baidu.com/ai-doc/FACE/yk37c1u4t
 
         :param image_file: 图片文件名或URL
         :param face_field: (可选)脸部信息，逗号分隔, 包括age,expression,face_shape,gender,glasses,
             landmark,landmark150,quality,eye_status,emotion,face_type,mask,spoofing信息
         :param corp_image: (可选)是否显示检测人脸的裁剪图
         :param max_faces:  (可选)最多处理人脸的数目，最大值120
 
@@ -386,15 +386,15 @@
             return self._result(response.json(), 'result')
         return self._error(500, 'error request Baidu face detect')
 
     def face_match(self, image1, image2):
         """
         人脸比对
 
-        https://ai.baidu.com/ai-doc/FACE/Lk37c1tpf
+        API文档: https://ai.baidu.com/ai-doc/FACE/Lk37c1tpf
 
         :param image1: 图片1(文件名或 URL 或 FACE_TOKEN)
         :param image2: 图片2(文件名或 URL 或 FACE_TOKEN)
         :return: 返回比对结果
         """
         self._update_token()  # 首先，检查access token
 
@@ -424,15 +424,15 @@
         Utils.save_file(save_filename, img)
         return save_filename
 
     def face_merge(self, face_image, template_image, save_filename, alpha=0):
         """
         人脸融合
 
-        https://ai.baidu.com/ai-doc/FACE/5k37c1ti0
+        API文档: https://ai.baidu.com/ai-doc/FACE/5k37c1ti0
 
         :param face_image: 目标人脸图片文件名或URL
         :param template_image: 模板图片文件名或URL
         :param save_filename: 存盘文件名
         :param alpha: （可选)融合参数，可选范围 0-1浮点数，保留两位小数，默认(0),
             0代表与目标图人脸最大程度相似（完全换脸），1 代表完全不换脸保留模版图，
             中间值（如0.5）为进行一般的换脸效果。该参数主要用于连续使用制作一组换脸渐变图片
@@ -490,135 +490,171 @@
     def body_count(self, image_file):
         """
         人流量统计.
 
         适用于3米以上的中远距离俯拍，以头部为主要识别目标统计人数，无需正脸、全身照，
         适应各类人流密集场景（如：机场、车展、景区、广场等）；
 
-        https://ai.baidu.com/ai-doc/BODY/7k3cpyy1t
+        API文档: https://ai.baidu.com/ai-doc/BODY/7k3cpyy1t
 
         :param image_file: 图片文件
         :return: 返回检测结果
         """
         api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/body_num"
         return self._image_api(image_file, api_url, 'person_num')
 
     def body_detect(self, image_file):
         """
         人体检测
 
-        https://ai.baidu.com/ai-doc/BODY/Ak3cpyx6v
+        API文档: https://ai.baidu.com/ai-doc/BODY/Ak3cpyx6v
 
         :param image_file: 图像文件
         :return: 返回检测结果
         """
         api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/body_attr"
         return self._image_api(image_file, api_url)
 
     def body_anlysis(self, image_file):
         """
         人体关键点识别.
 
-        https://ai.baidu.com/ai-doc/BODY/0k3cpyxme
+        API文档: https://ai.baidu.com/ai-doc/BODY/0k3cpyxme
 
         :param image_file: 图像文件
         :return: 返回检测结果
         """
         api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/body_analysis"
         return self._image_api(image_file, api_url)
 
     def gesture(self, image_file):
         """
         手势识别
 
-        https://ai.baidu.com/ai-doc/BODY/Ak3cpyx6v
+        API文档: https://ai.baidu.com/ai-doc/BODY/Ak3cpyx6v
 
         :param image_file: 图像文件
         :return: 返回检测结果
         """
         api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/gesture"
         return self._image_api(image_file, api_url)
 
     def classify(self, image_file):
         """
         通用物体和场景识别、分类
 
-        https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Xk3bcxe21
+        API文档: https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Xk3bcxe21
 
         :param image_file: 图像文件
         :return: 返回检测结果
         """
         api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v2/advanced_general"
         return self._image_api(image_file, api_url)
 
     def classify_plant(self, image_file):
         """
         植物识别
 
-        https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Mk3bcxe9i
+        API文档: https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Mk3bcxe9i
 
         :param image_file: 图像文件
         :return: 返回检测结果
         """
         api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/plant"
         return self._image_api(image_file, api_url)
 
     def classify_animal(self, image_file):
         """
         动物识别
 
-        https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Zk3bcxdfr
+        API文档: https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Zk3bcxdfr
 
         :param image_file: 图像文件
         :return: 返回检测结果
         """
         api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/animal"
         return self._image_api(image_file, api_url)
 
     def classify_car(self, image_file):
         """
         车型识别
 
-        https://ai.baidu.com/ai-doc/VEHICLE/tk3hb3eiv
+        API文档: https://ai.baidu.com/ai-doc/VEHICLE/tk3hb3eiv
 
         :param image_file: 图像文件
         :return: 返回检测结果
         """
         api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/car"
         return self._image_api(image_file, api_url)
 
+    def car_detect(self, image_file):
+        """
+        车辆检测
+
+        API文档: https://ai.baidu.com/ai-doc/VEHICLE/rk3hb3flg
+
+        :param image_file: 图像文件
+        :return: 返回检测结果
+        """
+        api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/vehicle_detect"
+        return self._image_api(image_file, api_url)
+
+    def car_attribute(self, image_file):
+        """
+        车辆属性识别
+
+        API文档: https://ai.baidu.com/ai-doc/VEHICLE/mk3hb3fde
+
+        :param image_file: 图像文件
+        :return: 返回检测结果
+        """
+        api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v2/vehicle_attr"
+        return self._image_api(image_file, api_url)
+
+    def car_damage(self, image_file):
+        """
+        车辆外观损伤识别
+
+        API文档: https://ai.baidu.com/ai-doc/VEHICLE/fk3hb3f5w
+
+        :param image_file: 图像文件
+        :return: 返回检测结果
+        """
+        api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/vehicle_damage"
+        return self._image_api(image_file, api_url)
+
     def classify_wine(self, image_file):
         """
         红酒识别
 
-        https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Tk3bcxctf
+        API文档: https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Tk3bcxctf
 
         :param image_file: 图像文件
         :return: 返回检测结果
         """
         api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/redwine"
         return self._image_api(image_file, api_url)
 
     def classify_objects(self, image_file):
         """
         图像主体检测
 
-        https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Wk7em3moi
+        API文档: https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Wk7em3moi
 
         :param image_file: 图像文件
         :return: 返回检测结果
         """
         api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/multi_object_detect"
         return self._image_api(image_file, api_url)
 
     def classify_dish(self, image_file):
         """
         菜品识别
 
-        https://ai.baidu.com/ai-doc/IMAGERECOGNITION/tk3bcxbb0
+        API文档: https://ai.baidu.com/ai-doc/IMAGERECOGNITION/tk3bcxbb0
 
         :param image_file: 图像文件
         :return: 返回检测结果
         """
         api_url = "https://aip.baidubce.com/rest/2.0/image-classify/v2/dish"
         return self._image_api(image_file, api_url)
 
@@ -652,80 +688,80 @@
 
         return self._error(500, 'error request Baidu API')
 
     def nlp_poem(self, topic, index=0):
         """
         智能写诗(七言绝句)
 
-        https://ai.baidu.com/ai-doc/NLP/ak53wc3o3
+        API文档: https://ai.baidu.com/ai-doc/NLP/ak53wc3o3
 
         :param topic: 主题
         :param index: 数值为0，即第一幅。每换一次，数值加1即可，一定数量后会返回之前的结果。
         :return: 返回结果
         """
         api_url = "https://aip.baidubce.com/rpc/2.0/creation/v1/poem"
         return self._text_api(topic, api_url, {'index': index}, 'poem')
 
     def nlp_couplets(self, topic, index=0):
         """
         智能春联
 
-        https://ai.baidu.com/ai-doc/NLP/Ok53wb6dh
+        API文档: https://ai.baidu.com/ai-doc/NLP/Ok53wb6dh
 
         :param topic: 主题
         :param index: 数值为0，即第一幅。每换一次，数值加1即可，一定数量后会返回之前的结果。
         :return: 返回结果
         """
         api_url = "https://aip.baidubce.com/rpc/2.0/creation/v1/couplets"
         return self._text_api(topic, api_url, {'index': index}, 'couplets')
 
     def nlp_bless(self, topic):
         """
         节日祝福语生成
 
-        https://cloud.baidu.com/doc/NLP/s/sl4cg75jk
+        API文档: https://cloud.baidu.com/doc/NLP/s/sl4cg75jk
 
         :param topic: 主题, 节日关键词，目前支持生成祝福语的关键词如下：平安夜 圣诞节 情人节
             元旦 除夕 春节 新年 元宵节 妇女节 清明节 劳动节 端午节 国庆节 中秋节 重阳节 立春
             雨水 惊蛰 春分 清明 谷雨 立夏 小满 芒种 夏至 小暑 大暑 立秋 处暑 白露 秋分 寒露
             霜降 立冬 小雪 大雪 冬至 小寒 大寒 高考
         :return: 返回结果
         """
         api_url = "https://aip.baidubce.com/rpc/2.0/nlp/v1/bless_creation"
         return self._text_api(topic, api_url, None, '')
 
     def nlp_address(self, address_text):
         """
         地址识别
 
-        https://cloud.baidu.com/doc/NLP/s/vk6z52h5n
+        API文档: https://cloud.baidu.com/doc/NLP/s/vk6z52h5n
 
         :param address_text: 地址文字
         :return: 返回结果
         """
         api_url = "https://aip.baidubce.com/rpc/2.0/nlp/v1/address"
         return self._text_api(address_text, api_url, None, '')
 
     def nlp_sentiment(self, text):
         """
         情感倾向分析: 对包含主体主观信息的文本，进行自动情感倾向性判断
 
-        https://cloud.baidu.com/doc/NLP/s/zk6z52hds
+        API文档: https://cloud.baidu.com/doc/NLP/s/zk6z52hds
 
         :param text: 文字
         :return: 返回结果
         """
         api_url = "https://aip.baidubce.com/rpc/2.0/nlp/v1/sentiment_classify"
         return self._text_api(text, api_url, None, '')
 
     def nlp_comment(self, text, industry=8):
         """
         评论观点抽取
 
-        https://cloud.baidu.com/doc/NLP/s/ok6z52g8q
+        API文档: https://cloud.baidu.com/doc/NLP/s/ok6z52g8q
 
         :param text: 评论文字
         :param industry: 行业: 酒店, KTV, 丽人, 美食, 餐饮, 旅游, 健康, 教育, 商业, 房产, 汽车, 生活, 购物, 3C
         :return: 返回结果
         """
         industries = {'酒店': 1, 'KTV': 2, '丽人': 3, '美容': 3, '美食': 4, '餐饮': 4,
                       '旅游': 5, '健康': 6, '教育': 7, '商业': 8, '房产': 9,
@@ -739,15 +775,15 @@
         return self._text_api(text, api_url, {'type': industry},
                               '', add_url='&charset=UTF-8')
 
     def nlp_lexer(self, text):
         """
         词法分析
         
-        https://cloud.baidu.com/doc/NLP/s/fk6z52f2u
+        API文档: https://cloud.baidu.com/doc/NLP/s/fk6z52f2u
         
         :param text:  文字
         :return: 返回分析结果
         """
         api_url = "https://aip.baidubce.com/rpc/2.0/nlp/v1/lexer"
         ret = self._text_api(text, api_url, None, '', add_url='&charset=UTF-8')
         if 'items' in ret:
@@ -759,15 +795,15 @@
             ret['words'] = words
         return ret
 
     def nlp_keywords(self, text):
         """
         关键词提取
 
-        https://cloud.baidu.com/doc/NLP/s/rl9zkamiq
+        API文档: https://cloud.baidu.com/doc/NLP/s/rl9zkamiq
 
         :param text:  文字
         :return: 返回分析结果
         """
         api_url = "https://aip.baidubce.com/rpc/2.0/nlp/v1/txt_keywords_extraction"
         ret = self._text_api([text], api_url, None, '', add_url='&charset=UTF-8')
         if 'results' in ret:
@@ -777,15 +813,15 @@
             ret['keywords'] = words
         return ret
 
     def nlp_summary(self, title, content, summary_len):
         """
         新闻摘要
 
-        https://cloud.baidu.com/doc/NLP/s/Gk6z52hu3
+        API文档: https://cloud.baidu.com/doc/NLP/s/Gk6z52hu3
 
         :param title:  新闻标题
         :param content:  新闻内容
         :param summary_len:  摘要结果的最大长度
         :return: 返回分析结果
         """
         api_url = "https://aip.baidubce.com/rpc/2.0/nlp/v1/news_summary"
@@ -793,30 +829,30 @@
                               {'title': title, 'content': content, 'max_summary_len': summary_len},
                               'summary', add_url='&charset=UTF-8')
 
     def nlp_tags(self, title, content):
         """
         文章标签
 
-        https://cloud.baidu.com/doc/NLP/s/7k6z52ggx
+        API文档: https://cloud.baidu.com/doc/NLP/s/7k6z52ggx
 
         :param title:  文章标题
         :param content:  文章内容
         :return: 返回分析结果
         """
         api_url = "https://aip.baidubce.com/rpc/2.0/nlp/v1/keyword"
         return self._text_api(None, api_url,
                               {'title': title, 'content': content},
                               'items', add_url='&charset=UTF-8')
 
     def nlp_topic(self, title, content):
         """
         文章分类
 
-        https://cloud.baidu.com/doc/NLP/s/wk6z52gxe
+        API文档: https://cloud.baidu.com/doc/NLP/s/wk6z52gxe
 
         :param title:  文章标题
         :param content:  文章内容
         :return: 返回分析结果
         """
         api_url = "https://aip.baidubce.com/rpc/2.0/nlp/v1/topic"
         return self._text_api(None, api_url,
```

### Comparing `jojo-ai-0.1.2/ai/baidu_demo.py` & `jojo-ai-0.1.3/ai/baidu_demo.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import ai
 from pprint import pprint  # pprint() 用于将dict打印得好看些
 
 
 # 以下请写入百度云中创建应用后提供的API Key、Secret Key
 api_key = 'XXXXXXXXXXXXXXXXXXXXXXXXX'
 secret_key = 'XXXXXXXXXXXXXXXXXXXXXXXXX'
+api_key = '8IGsGGa2nQaf8nn47zGnN4Mi'
+secret_key = 'G5NY2NU3WVwzTWIb6EFQ1pVFsc8buy6u'
 
 # 创建 BaiduAI 对象， 代入 api_key, secret_key 两个参数
 b = ai.BaiduAI(api_key, secret_key)
 
 # 调用各个API
 print('====语音转文本')
 texts = b.asr('images/16k.wav')
@@ -47,22 +49,31 @@
 print('====人体关键点识别')
 pprint(b.body_anlysis("images/body_ana.jpg"))
 
 print('====通用物体和场景识别')
 pprint(b.classify("images/notebook.jpg"))
 
 print('====植物识别')
-b.classify_plant("images/plant3.jpg")
+pprint(b.classify_plant("images/plant3.jpg"))
 
 print('====动物识别')
 pprint(b.classify_animal("images/animal3.jpg"))
 
 print('====车型识别')
 pprint(b.classify_car("images/car1.jpg"))
 
+print('====车辆检测')
+pprint(b.car_detect("images/cars2.jpg"))
+
+print('====车辆属性识别')
+pprint(b.car_attribute("images/car4.jpg"))
+
+print('====车辆外观损伤识别')
+pprint(b.car_damage("images/car_damage1.jpg"))
+
 print('====红酒识别')
 pprint(b.classify_wine("images/wine1.jpg"))
 
 print('====图像主体检测')
 pprint(b.classify_objects("images/objects1.jpg"))
 
 print('====菜品识别')
```

### Comparing `jojo-ai-0.1.2/jojo_ai.egg-info/PKG-INFO` & `jojo-ai-0.1.3/jojo_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jojo-ai
-Version: 0.1.2
+Version: 0.1.3
 Summary: API of AI of Baidu, ChatGPT, etc.
 Home-page: https://www.jostudio.com.cn/python
 Author: JoStudio
 Author-email: jostudio@189.cn
 License: Apache License 2.0
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `jojo-ai-0.1.2/setup.py` & `jojo-ai-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         line = line.strip()
         if line and not line.startswith('#'):
             result.append(line)
     return result
 
 
 setup(name='jojo-ai',  # 包的分发名称
-      version='0.1.2',  # PyPI上只允许一个版本存在，如果后续代码有了任何更改，再次上传需要增加版本号
+      version='0.1.3',  # PyPI上只允许一个版本存在，如果后续代码有了任何更改，再次上传需要增加版本号
       description='API of AI of Baidu, ChatGPT, etc.',  # 项目的简短描述
       long_description=read_file("README.rst"),  # 详细描述，会显示在PyPI的项目描述页面。必须是rst(reStructuredText) 格式的
       author='JoStudio',
       author_email='jostudio@189.cn',
       url='https://www.jostudio.com.cn/python',
       install_requires=['requests'],  # 项目依赖哪些库，这些库会在pip install的时候自动安装
       license='Apache License 2.0',
```

