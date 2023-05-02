# Comparing `tmp/nonebot_plugin_questionmark-0.3.1.tar.gz` & `tmp/nonebot_plugin_questionmark-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_questionmark-0.3.1.tar", last modified: Sun Apr  2 11:26:53 2023, max compression
+gzip compressed data, was "nonebot_plugin_questionmark-0.4.0.tar", last modified: Tue May  2 07:33:59 2023, max compression
```

## Comparing `nonebot_plugin_questionmark-0.3.1.tar` & `nonebot_plugin_questionmark-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 11:26:53.414943 nonebot_plugin_questionmark-0.3.1/
--rw-rw-rw-   0        0        0     1088 2023-03-26 12:45:17.000000 nonebot_plugin_questionmark-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1695 2023-04-02 11:26:53.412984 nonebot_plugin_questionmark-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1015 2023-04-02 11:23:15.000000 nonebot_plugin_questionmark-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 11:26:53.384576 nonebot_plugin_questionmark-0.3.1/nonebot_plugin_questionmark/
--rw-rw-rw-   0        0        0      533 2023-04-02 11:23:15.000000 nonebot_plugin_questionmark-0.3.1/nonebot_plugin_questionmark/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 11:26:53.406125 nonebot_plugin_questionmark-0.3.1/nonebot_plugin_questionmark.egg-info/
--rw-rw-rw-   0        0        0     1695 2023-04-02 11:26:52.000000 nonebot_plugin_questionmark-0.3.1/nonebot_plugin_questionmark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-04-02 11:26:53.000000 nonebot_plugin_questionmark-0.3.1/nonebot_plugin_questionmark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 11:26:52.000000 nonebot_plugin_questionmark-0.3.1/nonebot_plugin_questionmark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-02 11:26:52.000000 nonebot_plugin_questionmark-0.3.1/nonebot_plugin_questionmark.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-02 11:26:52.000000 nonebot_plugin_questionmark-0.3.1/nonebot_plugin_questionmark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-02 11:26:53.415924 nonebot_plugin_questionmark-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1046 2023-04-02 11:23:15.000000 nonebot_plugin_questionmark-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:33:59.957285 nonebot_plugin_questionmark-0.4.0/
+-rw-rw-rw-   0        0        0     1088 2023-05-02 07:14:09.000000 nonebot_plugin_questionmark-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     2045 2023-05-02 07:33:59.956309 nonebot_plugin_questionmark-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1392 2023-05-02 07:32:27.000000 nonebot_plugin_questionmark-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 07:33:59.943613 nonebot_plugin_questionmark-0.4.0/nonebot_plugin_questionmark/
+-rw-rw-rw-   0        0        0     1089 2023-05-02 07:32:27.000000 nonebot_plugin_questionmark-0.4.0/nonebot_plugin_questionmark/__init__.py
+-rw-rw-rw-   0        0        0      225 2023-05-02 07:23:34.000000 nonebot_plugin_questionmark-0.4.0/nonebot_plugin_questionmark/config.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:33:59.954356 nonebot_plugin_questionmark-0.4.0/nonebot_plugin_questionmark.egg-info/
+-rw-rw-rw-   0        0        0     2045 2023-05-02 07:33:59.000000 nonebot_plugin_questionmark-0.4.0/nonebot_plugin_questionmark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-05-02 07:33:59.000000 nonebot_plugin_questionmark-0.4.0/nonebot_plugin_questionmark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 07:33:59.000000 nonebot_plugin_questionmark-0.4.0/nonebot_plugin_questionmark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-02 07:33:59.000000 nonebot_plugin_questionmark-0.4.0/nonebot_plugin_questionmark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-05-02 07:33:59.000000 nonebot_plugin_questionmark-0.4.0/nonebot_plugin_questionmark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 07:33:59.957285 nonebot_plugin_questionmark-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1019 2023-05-02 07:29:34.000000 nonebot_plugin_questionmark-0.4.0/setup.py
```

### Comparing `nonebot_plugin_questionmark-0.3.1/LICENSE` & `nonebot_plugin_questionmark-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_questionmark-0.3.1/PKG-INFO` & `nonebot_plugin_questionmark-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot_plugin_questionmark
-Version: 0.3.1
-Summary: 基于 OneBot 适配器的 NoneBot2 行为艺术插件, 有群友或私聊发送全是问号/感叹号的消息时, bot会自动把问号/感叹号方向翻转并发出来
-Home-page: https://github.com/NumberSir/nonebot_plugin_questionmark
-Author: Number_Sir
-Author-email: Number_Sir@126.com
-Keywords: pip,nonebot2,nonebot,nonebot_plugin
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
   
 # Nonebot_Plugin_QuestionMark
@@ -41,21 +25,31 @@
 
 - 使用 pip
 
 ```
 pip install -U nonebot_plugin_questionmark
 ```
 
+## 配置项
+```ini
+QM_TRIGGER_RATE=0.3                # 触发回复概率，默认 0.3
+QM_ENABLE_GROUPS=[12345, 114514]   # 白名单群聊，仅列表内群聊可能触发回复
+```
+
 ## 图片示例
 
 <div align="left">
   <img src="https://user-images.githubusercontent.com/52584526/227783077-b490dad2-5e1a-42eb-b455-53f381934497.png" width="500" />
 </div>
 
 ## 更新日志
+> 2023-05-02 v0.4.0
+> - 添加概率触发回复功能
+> - 添加白名单群聊(仅qq可用)功能 [@issue/3](https://github.com/NumberSir/nonebot-plugin-questionmark/issues/3)
+> 
 > 2023-04-02 v0.3.1
 > - 修bug
 > 
 > 2023-03-29 v0.3.0
 > - 优化实现
 >
 > 2023-03-27 v0.2.1
```

#### html2text {}

```diff
@@ -1,23 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_questionmark Version: 0.3.1 Summary:
-åºäº OneBot ééå¨ç NoneBot2 è¡ä¸ºèºæ¯æä»¶,
-æç¾¤åæç§èåéå¨æ¯é®å·/æå¹å·çæ¶æ¯æ¶,
-botä¼èªå¨æé®å·/æå¹å·æ¹åç¿»è½¬å¹¶ååºæ¥ Home-page: https://
-github.com/NumberSir/nonebot_plugin_questionmark Author: Number_Sir Author-
-email: Number_Sir@126.com Keywords: pip,nonebot2,nonebot,nonebot_plugin
-Platform: any Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE
                                    [nonebot]
 # Nonebot_Plugin_QuestionMark _â¨ åºäºOneBotééå¨ç[NoneBot2](https://
                     v2.nonebot.dev/)è¡ä¸ºèºæ¯æä»¶ â¨_
 ## åè½
 æç¾¤åæç§èåéå¨æ¯é®å·`?`,`ï¼`æ`Â¿`ææå¹å·`!`,`ï¼`,`Â¡`çæ¶æ¯æ¶,
 botä¼èªå¨æé®å·/æå¹å·ç¿»è½¬æ¹åååºå» ## å®è£ - ä½¿ç¨ nb-cli
 ``` nb plugin install nonebot_plugin_questionmark ``` - ä½¿ç¨ pip ``` pip
-install -U nonebot_plugin_questionmark ``` ## å¾çç¤ºä¾
+install -U nonebot_plugin_questionmark ``` ## éç½®é¡¹ ```ini
+QM_TRIGGER_RATE=0.3 # è§¦ååå¤æ¦çï¼é»è®¤ 0.3 QM_ENABLE_GROUPS=[12345,
+114514] # ç½ååç¾¤èï¼ä»åè¡¨åç¾¤èå¯è½è§¦ååå¤ ``` ##
+å¾çç¤ºä¾
 [https://user-images.githubusercontent.com/52584526/227783077-b490dad2-5e1a-
 42eb-b455-53f381934497.png]
-## æ´æ°æ¥å¿ > 2023-04-02 v0.3.1 > - ä¿®bug > > 2023-03-29 v0.3.0 > -
-ä¼åå®ç° > > 2023-03-27 v0.2.1 > - ä¼åå®ç° > - æ·»å æå¹å· > >
-2023-03-26 v0.1.0 > - åå¸
+## æ´æ°æ¥å¿ > 2023-05-02 v0.4.0 > - æ·»å æ¦çè§¦ååå¤åè½ > -
+æ·»å ç½ååç¾¤è(ä»qqå¯ç¨)åè½ [@issue/3](https://github.com/
+NumberSir/nonebot-plugin-questionmark/issues/3) > > 2023-04-02 v0.3.1 > -
+ä¿®bug > > 2023-03-29 v0.3.0 > - ä¼åå®ç° > > 2023-03-27 v0.2.1 > -
+ä¼åå®ç° > - æ·»å æå¹å· > > 2023-03-26 v0.1.0 > - åå¸
```

### Comparing `nonebot_plugin_questionmark-0.3.1/nonebot_plugin_questionmark.egg-info/PKG-INFO` & `nonebot_plugin_questionmark-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: nonebot-plugin-questionmark
-Version: 0.3.1
-Summary: 基于 OneBot 适配器的 NoneBot2 行为艺术插件, 有群友或私聊发送全是问号/感叹号的消息时, bot会自动把问号/感叹号方向翻转并发出来
+Name: nonebot_plugin_questionmark
+Version: 0.4.0
+Summary: NoneBot2 行为艺术插件, 有群友或私聊发送全是问号/感叹号的消息时, bot会自动把问号/感叹号方向翻转并发出来
 Home-page: https://github.com/NumberSir/nonebot_plugin_questionmark
 Author: Number_Sir
 Author-email: Number_Sir@126.com
 Keywords: pip,nonebot2,nonebot,nonebot_plugin
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,21 +41,31 @@
 
 - 使用 pip
 
 ```
 pip install -U nonebot_plugin_questionmark
 ```
 
+## 配置项
+```ini
+QM_TRIGGER_RATE=0.3                # 触发回复概率，默认 0.3
+QM_ENABLE_GROUPS=[12345, 114514]   # 白名单群聊，仅列表内群聊可能触发回复
+```
+
 ## 图片示例
 
 <div align="left">
   <img src="https://user-images.githubusercontent.com/52584526/227783077-b490dad2-5e1a-42eb-b455-53f381934497.png" width="500" />
 </div>
 
 ## 更新日志
+> 2023-05-02 v0.4.0
+> - 添加概率触发回复功能
+> - 添加白名单群聊(仅qq可用)功能 [@issue/3](https://github.com/NumberSir/nonebot-plugin-questionmark/issues/3)
+> 
 > 2023-04-02 v0.3.1
 > - 修bug
 > 
 > 2023-03-29 v0.3.0
 > - 优化实现
 >
 > 2023-03-27 v0.2.1
```

#### html2text {}

```diff
@@ -1,23 +1,27 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-questionmark Version: 0.3.1 Summary:
-åºäº OneBot ééå¨ç NoneBot2 è¡ä¸ºèºæ¯æä»¶,
-æç¾¤åæç§èåéå¨æ¯é®å·/æå¹å·çæ¶æ¯æ¶,
-botä¼èªå¨æé®å·/æå¹å·æ¹åç¿»è½¬å¹¶ååºæ¥ Home-page: https://
-github.com/NumberSir/nonebot_plugin_questionmark Author: Number_Sir Author-
-email: Number_Sir@126.com Keywords: pip,nonebot2,nonebot,nonebot_plugin
-Platform: any Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE
+Metadata-Version: 2.1 Name: nonebot_plugin_questionmark Version: 0.4.0 Summary:
+NoneBot2 è¡ä¸ºèºæ¯æä»¶, æç¾¤åæç§èåéå¨æ¯é®å·/
+æå¹å·çæ¶æ¯æ¶, botä¼èªå¨æé®å·/æå¹å·æ¹åç¿»è½¬å¹¶ååºæ¥
+Home-page: https://github.com/NumberSir/nonebot_plugin_questionmark Author:
+Number_Sir Author-email: Number_Sir@126.com Keywords:
+pip,nonebot2,nonebot,nonebot_plugin Platform: any Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE
                                    [nonebot]
 # Nonebot_Plugin_QuestionMark _â¨ åºäºOneBotééå¨ç[NoneBot2](https://
                     v2.nonebot.dev/)è¡ä¸ºèºæ¯æä»¶ â¨_
 ## åè½
 æç¾¤åæç§èåéå¨æ¯é®å·`?`,`ï¼`æ`Â¿`ææå¹å·`!`,`ï¼`,`Â¡`çæ¶æ¯æ¶,
 botä¼èªå¨æé®å·/æå¹å·ç¿»è½¬æ¹åååºå» ## å®è£ - ä½¿ç¨ nb-cli
 ``` nb plugin install nonebot_plugin_questionmark ``` - ä½¿ç¨ pip ``` pip
-install -U nonebot_plugin_questionmark ``` ## å¾çç¤ºä¾
+install -U nonebot_plugin_questionmark ``` ## éç½®é¡¹ ```ini
+QM_TRIGGER_RATE=0.3 # è§¦ååå¤æ¦çï¼é»è®¤ 0.3 QM_ENABLE_GROUPS=[12345,
+114514] # ç½ååç¾¤èï¼ä»åè¡¨åç¾¤èå¯è½è§¦ååå¤ ``` ##
+å¾çç¤ºä¾
 [https://user-images.githubusercontent.com/52584526/227783077-b490dad2-5e1a-
 42eb-b455-53f381934497.png]
-## æ´æ°æ¥å¿ > 2023-04-02 v0.3.1 > - ä¿®bug > > 2023-03-29 v0.3.0 > -
-ä¼åå®ç° > > 2023-03-27 v0.2.1 > - ä¼åå®ç° > - æ·»å æå¹å· > >
-2023-03-26 v0.1.0 > - åå¸
+## æ´æ°æ¥å¿ > 2023-05-02 v0.4.0 > - æ·»å æ¦çè§¦ååå¤åè½ > -
+æ·»å ç½ååç¾¤è(ä»qqå¯ç¨)åè½ [@issue/3](https://github.com/
+NumberSir/nonebot-plugin-questionmark/issues/3) > > 2023-04-02 v0.3.1 > -
+ä¿®bug > > 2023-03-29 v0.3.0 > - ä¼åå®ç° > > 2023-03-27 v0.2.1 > -
+ä¼åå®ç° > - æ·»å æå¹å· > > 2023-03-26 v0.1.0 > - åå¸
```

### Comparing `nonebot_plugin_questionmark-0.3.1/setup.py` & `nonebot_plugin_questionmark-0.4.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name="nonebot_plugin_questionmark",
-    version="0.3.1",
+    version="0.4.0",
     author="Number_Sir",
     author_email="Number_Sir@126.com",
     keywords=["pip", "nonebot2", "nonebot", "nonebot_plugin"],
-    description="""基于 OneBot 适配器的 NoneBot2 行为艺术插件, 有群友或私聊发送全是问号/感叹号的消息时, bot会自动把问号/感叹号方向翻转并发出来""",
+    description="""NoneBot2 行为艺术插件, 有群友或私聊发送全是问号/感叹号的消息时, bot会自动把问号/感叹号方向翻转并发出来""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/NumberSir/nonebot_plugin_questionmark",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

