# Comparing `tmp/nonebot_plugin_manga_translator-0.1.1.tar.gz` & `tmp/nonebot_plugin_manga_translator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_manga_translator-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_manga_translator-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_manga_translator-0.1.1.tar` & `nonebot_plugin_manga_translator-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-05-01 18:17:10.001242 nonebot_plugin_manga_translator-0.1.1/LICENSE
--rw-r--r--   0        0        0     5717 2023-05-01 18:17:10.001242 nonebot_plugin_manga_translator-0.1.1/README.md
--rw-r--r--   0        0        0     3999 2023-05-01 18:17:10.001242 nonebot_plugin_manga_translator-0.1.1/nonebot_plugin_manga_translator/__init__.py
--rw-r--r--   0        0        0     5511 2023-05-01 18:17:10.001242 nonebot_plugin_manga_translator-0.1.1/nonebot_plugin_manga_translator/utils.py
--rw-r--r--   0        0        0      529 2023-05-01 18:17:10.001242 nonebot_plugin_manga_translator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6515 1970-01-01 00:00:00.000000 nonebot_plugin_manga_translator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-02 16:20:44.784722 nonebot_plugin_manga_translator-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7701 2023-05-02 16:20:44.784722 nonebot_plugin_manga_translator-0.1.2/README.md
+-rw-r--r--   0        0        0     3999 2023-05-02 16:20:44.784722 nonebot_plugin_manga_translator-0.1.2/nonebot_plugin_manga_translator/__init__.py
+-rw-r--r--   0        0        0     8774 2023-05-02 16:20:44.784722 nonebot_plugin_manga_translator-0.1.2/nonebot_plugin_manga_translator/utils.py
+-rw-r--r--   0        0        0      529 2023-05-02 16:20:44.784722 nonebot_plugin_manga_translator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8499 1970-01-01 00:00:00.000000 nonebot_plugin_manga_translator-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_manga_translator-0.1.1/LICENSE` & `nonebot_plugin_manga_translator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_manga_translator-0.1.1/README.md` & `nonebot_plugin_manga_translator-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -20,111 +20,128 @@
 
 ## 📖简介
 
 1. 适配多种api,将收到的图片翻译并发送翻译后的图片，支持批量操作
 
 2. ⚙️插件配置
 
-这些配置项必填，否则无法使用，请在机器人目录下的.env.*里填写以下选项(至少填一个平台的)
+请在机器人目录下的.env.*里填写以下选项(至少填一个平台的)，获取方式已整理好，见下方
 
-~~个人感觉有道API的效果比百度好很多，但是架不住百度每个月前1w次调用免费啊~~
+~~个人感觉就漫画翻译而言,这几家API的效果大致为有道>=百度≈离线>=火山,且火山翻译对竖版日文的翻译效果很差~~
 
-|       配置项        | 类型  | 默认值 |          示例           | 说明    |
-| :-----------------: | :---: | :-----: | :------------------------: | :------- |
-|     有道翻译API     |   -   |    -    |             -              | -        |
-|   youdao_app_key    |  str  |   ""    |   youdao_app_key="xxxxx"   | 应用ID   |
-|  youdao_app_secret  |  str  |   ""    | youdao_app_secret="xxxxxx" | 应用秘钥 |
-|     百度翻译API     |   -   |    -    |             -              | -        |
-|    baidu_app_id     |  str  |   ""    |    baidu_app_id="66666"    | APP ID   |
-|    baidu_app_key    |  str  |   ""    |   baidu_app_key="xxxxxx"   | 密钥     |
-|     离线翻译API     |   -   |    -    |             -              | -        |
-|    offline_url    |  str  |   ""    |   offline_url="http://127.0.0.1:5003"   | 见下方说明     |
-| 其他翻译API(待更新) |   -   |    -    |             -              | -        |
+|          配置项           | 类型  | 默认值 |                示例                 | 说明              | API定价                                           |
+| :-----------------------: | :---: | :----: | :---------------------------------: | :---------------- | :------------------------------------------------ |
+|        有道翻译API        |   -   |   -    |                  -                  | -                 | 梯度收费，0<月调用量<100w时,0.04元/张                   |
+|      youdao_app_key       |  str  |   ""   |       youdao_app_key="xxxxx"        | 应用ID            |                                                   |
+|     youdao_app_secret     |  str  |   ""   |     youdao_app_secret="xxxxxx"      | 应用秘钥          |                                                   |
+|        百度翻译API        |   -   |   -    |                  -                  | -                 | 每月1万次免费调用量，之后按梯度收费,最高0.04元/次 |
+|       baidu_app_id        |  str  |   ""   |        baidu_app_id="66666"         | APP ID            |                                                   |
+|       baidu_app_key       |  str  |   ""   |       baidu_app_key="xxxxxx"        | 密钥              |                                                   |
+|        火山翻译API        |   -   |   -    |                  -                  | -                 | 每月前100张免费，之后0.04元/张                    |
+|   huoshan_access_key_id   |  str  |   ""   |    huoshan_access_key_id="AK***"    | Access Key ID     |                                                   |
+| huoshan_secret_access_key |  str  |   ""   |  huoshan_secret_access_key="UT**"   | Secret Access Key |                                                   |
+|        离线翻译API        |   -   |   -    |                  -                  | -                 |                                            可能是电费?       |
+|        offline_url        |  str  |   ""   | offline_url="http://127.0.0.1:5003" | 见下方说明        |                                                   |
+|    其他翻译API(待更新)    |   -   |   -    |                  -                  | -                 |                                                   |
 
-## 🌙更新日志
+## 🔑API获取
 
 <details>
-<summary>点击展开</summary>
+<summary>有道翻译</summary>
 
-- 2023-05-01:
+1. 在[有道智云AI开放平台](https://ai.youdao.com/#/)注册并登录后，进入控制台
+2. 在左侧`自然语言翻译服务`里的`图片翻译`里创建应用，选择服务和接入方式分别为`图片翻译`和`API`，其他项随意。
+![Image text](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/有道翻译.png)
+3. 创建后将`应用ID`和`应用秘钥`按照上面的配置说明分别填入.env.*文件里即可
 
-  - 添加切换api的功能，你可以将某个api优先级设为最高
-  - 适配离线翻译api[manga-image-translator](https://github.com/zyddnys/manga-image-translator),现在你可以体验本地的翻译
+</details>
 
-- 2023-04-28:
+<details>
+<summary>百度翻译</summary>
 
-  插件发布
+   1. 在[百度翻译开放平台](https://api.fanyi.baidu.com/)注册并登录
+   2. 找到`产品服务`的`图片翻译`,申请创建
+   3. 创建后在`管理控制台`的`总览`中找到`APP ID`和`密钥`,根据上面的配置说明填入.env.*文件
+
+</details>
+
+<details>
+<summary>火山翻译</summary>
+
+   1. 根据火山引擎的[文档](https://www.volcengine.com/docs/4640/130872)，按流程注册
+   2. 创建好服务后获取到密钥，分别为`Access Key ID`和`Secret Access Key`，然后点击`Secret Access Key`下的按钮显示出密钥
+   3. 分别根据上面的配置说明填入.env.*文件
+
+</details>
+
+<details>
+<summary>离线翻译</summary>
+(该方案对设备配置要求较高，建议在有足够的硬盘空间、内存、显存，或有一台能为bot处理请求的服务器时考虑使用该方案)
+
+   1. 参考[manga-image-translator](https://github.com/zyddnys/manga-image-translator)的说明，克隆仓库，并安装相关依赖(可能需要额外安装`pydensecrf`)
+   2. 安装好依赖后，在仓库目录下运行
+
+      ```python
+      python -m manga_translator -v --mode web --use-cuda# the demo will be serving on http://127.0.0.1:5003
+      ```
+
+   3. 如果你的设备没有成功安装cuda(要求pytorch的版本和cuda对应，不对应请重装)，请去掉参数`--use-cuda`，如果图片处理过程中爆显存，请改成`--use-cuda-limited`
+
+   4. 你可以访问控制台给出的网址，尝试先本地翻译一张图片，此时会根据选项下载需要的模型(为防止下载失败，也可以提前手动下载)
+   5. 如果bot和翻译器在同一台设备，那么.env填写`offline_url="http://127.0.0.1:5003"`即可，如果不在同一台设备，你**可能**还需要放行防火墙、端口转发等，并且填写内容也会有所变化
+   6. 最后你**可能**还需要修改一下本插件的代码，找到本插件`utils.py`的`offline`函数，根据注释和[文档](https://github.com/zyddnys/manga-image-translator/blob/main/README.md),修改字典`data`，从而指定你想要的OCR模型和翻译模型(目前是用了offline模型,你可以改成别的)
 
 </details>
 
 ## 🎉命令
 
 1. 图片翻译 [图片]：单张图片翻译，也可以先发送/图片翻译再发送图片,可以如下组合
 
     1. 文字+图片
     2. 先文字，后图片
     3. 文字回复图片
 
 2. 多图片翻译 [图片]：n张图片翻译，将会以合并转发消息的形式发出,可以如下组合
 
     1. 先文字，后多张图片 
-    2. 2.文字+图片*n
-3. 切换翻译api [api]: 将该api优先级提到最高，目前有`youdao baidu offline`
+    2. 文字+图片*n
+3. 切换翻译api [api]: 将该api优先级提到最高，目前有`youdao baidu huoshan offline`
 
 未完待续
 
 ## ⭐效果图
 
 <img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图1.jpg" width="300" height="300">
 <img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图2.jpg" width="300" height="300">
 <img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图3.jpg" width="300" height="300">
 <img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图4.PNG" width="300" height="300">
 
-## 🔑API获取
-
-<details>
-<summary>有道翻译</summary>
-
-1. 在[有道智云AI开放平台](https://ai.youdao.com/#/)注册并登录后，进入控制台
-2. 在左侧`自然语言翻译服务`里的`图片翻译`里创建应用，选择服务和接入方式分别为`图片翻译`和`API`，其他项随意。
-![Image text](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/有道翻译.png)
-3. 创建后将`应用ID`和`应用秘钥`按照上面的配置说明分别填入.env.*文件里即可
-
-</details>
+## 🌙更新日志
 
 <details>
-<summary>百度翻译</summary>
-
-   1. 在[百度翻译开放平台](https://api.fanyi.baidu.com/)注册并登录
-   2. 找到`产品服务`的`图片翻译`,申请创建
-   3. 创建后在`管理控制台`的`总览`中找到`APP ID`和`密钥`,根据上面的配置说明填入.env.*文件
+<summary>点击展开</summary>
 
-</details>
+- 2023-05-03:
 
-<details>
-<summary>离线翻译</summary>
-(该方案对设备配置要求较高，建议在有足够的硬盘空间、内存、显存，或有一台能为bot处理请求的服务器时考虑使用该方案)
+  - 更新说明文档
+  - 适配[火山翻译api](https://translate.volcengine.com/api),你可以选择接入火山翻译提供的API
 
-   1. 参考[manga-image-translator](https://github.com/zyddnys/manga-image-translator)的说明，克隆仓库，并安装相关依赖(可能需要额外安装`pydensecrf`)
-   2. 安装好依赖后，在仓库目录下运行
+- 2023-05-01:
 
-      ```python
-      python -m manga_translator -v --mode web --use-cuda# the demo will be serving on http://127.0.0.1:5003
-      ```
+  - 添加切换api的功能，你可以将某个api优先级设为最高
+  - 适配离线翻译api[manga-image-translator](https://github.com/zyddnys/manga-image-translator),现在你可以体验本地的翻译
 
-   3. 如果你的设备没有成功安装cuda(要求pytorch的版本和cuda对应，不对应请重装)，请去掉参数`--use-cuda`，如果图片处理过程中爆显存，请改成`--use-cuda-limited`
+- 2023-04-28:
 
-   4. 你可以访问控制台给出的网址，尝试先本地翻译一张图片，此时会根据选项下载需要的模型(为防止下载失败，也可以提前手动下载)
-   5. 如果bot和翻译器在同一台设备，那么.env填写`offline_url="http://127.0.0.1:5003"`即可，如果不在同一台设备，你**可能**还需要放行防火墙、端口转发等，并且填写内容也会有所变化
-   6. 最后你**可能**还需要修改一下本插件的代码，找到本插件`utils.py`的`offline`函数，根据注释和[文档](https://github.com/zyddnys/manga-image-translator/blob/main/README.md),修改字典`data`，从而指定你想要的OCR模型和翻译模型(目前是用了offline模型,你可以改成别的)
+  - 插件发布
 
 </details>
 
 ## 🐦计划
 
-- [x] 支持部署离线翻译模型
+- [x] 适配离线翻译模型[manga-image-translator](https://github.com/zyddnys/manga-image-translator)
 
-- [ ] 支持更多API
+- [x] 支持更多API
 
 - [ ] 完善插件
 
 ## ✨喜欢的话就点个star✨吧，球球了QAQ
```

#### html2text {}

```diff
@@ -2,54 +2,48 @@
         # nonebot-plugin-manga-translator â¨*åºäºNonebot2çå¾ç/
                             æ¼«ç»ç¿»è¯æä»¶*â¨
 ## ð¿å®è£ éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb:
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨ `nb plugin install
 nonebot_plugin_manga_translator` - ä½¿ç¨pip(ä¸æ¨è):
 ~~ä¸æ¨èå°±æ¯ä¸æ¨èï¼ç¥ç¥ç¥~~ ## ðç®ä» 1.
 ééå¤ç§api,å°æ¶å°çå¾çç¿»è¯å¹¶åéç¿»è¯åçå¾çï¼æ¯ææ¹éæä½
-2. âï¸æä»¶éç½®
-è¿äºéç½®é¡¹å¿å¡«ï¼å¦åæ æ³ä½¿ç¨ï¼è¯·å¨æºå¨äººç®å½ä¸ç.env.*éå¡«åä»¥ä¸éé¡¹
-(è³å°å¡«ä¸ä¸ªå¹³å°ç)
-~~ä¸ªäººæè§æéAPIçæææ¯ç¾åº¦å¥½å¾å¤ï¼ä½æ¯æ¶ä¸ä½ç¾åº¦æ¯ä¸ªæå1wæ¬¡è°ç¨åè´¹å~~
-| éç½®é¡¹ | ç±»å | é»è®¤å¼ | ç¤ºä¾ | è¯´æ | | :-----------------: | :-
---: | :-----: | :------------------------: | :------- | | æéç¿»è¯API | - |
-- | - | - | | youdao_app_key | str | "" | youdao_app_key="xxxxx" | åºç¨ID | |
-youdao_app_secret | str | "" | youdao_app_secret="xxxxxx" | åºç¨ç§é¥ | |
-ç¾åº¦ç¿»è¯API | - | - | - | - | | baidu_app_id | str | "" |
-baidu_app_id="66666" | APP ID | | baidu_app_key | str | "" |
-baidu_app_key="xxxxxx" | å¯é¥ | | ç¦»çº¿ç¿»è¯API | - | - | - | - | |
+2. âï¸æä»¶éç½® è¯·å¨æºå¨äººç®å½ä¸ç.env.*éå¡«åä»¥ä¸éé¡¹
+(è³å°å¡«ä¸ä¸ªå¹³å°ç)ï¼è·åæ¹å¼å·²æ´çå¥½ï¼è§ä¸æ¹
+~~ä¸ªäººæè§å°±æ¼«ç»ç¿»è¯èè¨,è¿å å®¶APIçææå¤§è´ä¸ºæé>=ç¾åº¦âç¦»çº¿>=ç«å±±,ä¸ç«å±±ç¿»è¯å¯¹ç«çæ¥æçç¿»è¯ææå¾å·®~~
+| éç½®é¡¹ | ç±»å | é»è®¤å¼ | ç¤ºä¾ | è¯´æ | APIå®ä»· | | :-----------
+------------: | :---: | :----: | :---------------------------------: | :-------
+--------- | :------------------------------------------------ | |
+æéç¿»è¯API | - | - | - | - |
+æ¢¯åº¦æ¶è´¹ï¼0<æè°ç¨é<100wæ¶,0.04å/å¼  | | youdao_app_key | str | ""
+| youdao_app_key="xxxxx" | åºç¨ID | | | youdao_app_secret | str | "" |
+youdao_app_secret="xxxxxx" | åºç¨ç§é¥ | | | ç¾åº¦ç¿»è¯API | - | - | - | -
+| æ¯æ1ä¸æ¬¡åè´¹è°ç¨éï¼ä¹åææ¢¯åº¦æ¶è´¹,æé«0.04å/æ¬¡ | |
+baidu_app_id | str | "" | baidu_app_id="66666" | APP ID | | | baidu_app_key |
+str | "" | baidu_app_key="xxxxxx" | å¯é¥ | | | ç«å±±ç¿»è¯API | - | - | - |
+- | æ¯æå100å¼ åè´¹ï¼ä¹å0.04å/å¼  | | huoshan_access_key_id | str |
+"" | huoshan_access_key_id="AK***" | Access Key ID | | |
+huoshan_secret_access_key | str | "" | huoshan_secret_access_key="UT**" |
+Secret Access Key | | | ç¦»çº¿ç¿»è¯API | - | - | - | - | å¯è½æ¯çµè´¹? | |
 offline_url | str | "" | offline_url="http://127.0.0.1:5003" | è§ä¸æ¹è¯´æ
-| | å¶ä»ç¿»è¯API(å¾æ´æ°) | - | - | - | - | ## ðæ´æ°æ¥å¿
-ç¹å»å±å¼ - 2023-05-01: -
-æ·»å åæ¢apiçåè½ï¼ä½ å¯ä»¥å°æä¸ªapiä¼åçº§è®¾ä¸ºæé« -
-ééç¦»çº¿ç¿»è¯api[manga-image-translator](https://github.com/zyddnys/manga-
-image-translator),ç°å¨ä½ å¯ä»¥ä½éªæ¬å°çç¿»è¯ - 2023-04-28:
-æä»¶åå¸  ## ðå½ä»¤ 1. å¾çç¿»è¯
-[å¾ç]ï¼åå¼ å¾çç¿»è¯ï¼ä¹å¯ä»¥ååé/
-å¾çç¿»è¯ååéå¾ç,å¯ä»¥å¦ä¸ç»å 1. æå­+å¾ç 2.
-åæå­ï¼åå¾ç 3. æå­åå¤å¾ç 2. å¤å¾çç¿»è¯
-[å¾ç]ï¼nå¼ å¾çç¿»è¯ï¼å°ä¼ä»¥åå¹¶è½¬åæ¶æ¯çå½¢å¼ååº,å¯ä»¥å¦ä¸ç»å
-1. åæå­ï¼åå¤å¼ å¾ç 2. 2.æå­+å¾ç*n 3. åæ¢ç¿»è¯api [api]:
-å°è¯¥apiä¼åçº§æå°æé«ï¼ç®åæ`youdao baidu offline` æªå®å¾ç»­
-## â­ææå¾ [https://github.com/maoxig/nonebot-plugin-manga-translator/
-blob/main/resource/ææå¾1.jpg] [https://github.com/maoxig/nonebot-plugin-
-manga-translator/blob/main/resource/ææå¾2.jpg] [https://github.com/maoxig/
-nonebot-plugin-manga-translator/blob/main/resource/ææå¾3.jpg] [https://
-github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/
-ææå¾4.PNG] ## ðAPIè·å  æéç¿»è¯ 1. å¨
-[æéæºäºAIå¼æ¾å¹³å°](https://ai.youdao.com/#/
+| | | å¶ä»ç¿»è¯API(å¾æ´æ°) | - | - | - | - | | ## ðAPIè·å
+æéç¿»è¯ 1. å¨[æéæºäºAIå¼æ¾å¹³å°](https://ai.youdao.com/#/
 )æ³¨åå¹¶ç»å½åï¼è¿å¥æ§å¶å° 2.
 å¨å·¦ä¾§`èªç¶è¯­è¨ç¿»è¯æå¡`éç`å¾çç¿»è¯`éåå»ºåºç¨ï¼éæ©æå¡åæ¥å¥æ¹å¼åå«ä¸º`å¾çç¿»è¯`å`API`ï¼å¶ä»é¡¹éæã
 ![Image text](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/
 main/resource/æéç¿»è¯.png) 3.
 åå»ºåå°`åºç¨ID`å`åºç¨ç§é¥`æç§ä¸é¢çéç½®è¯´æåå«å¡«å¥.env.*æä»¶éå³å¯
 ç¾åº¦ç¿»è¯ 1. å¨[ç¾åº¦ç¿»è¯å¼æ¾å¹³å°](https://api.fanyi.baidu.com/
 )æ³¨åå¹¶ç»å½ 2. æ¾å°`äº§åæå¡`ç`å¾çç¿»è¯`,ç³è¯·åå»º 3.
 åå»ºåå¨`ç®¡çæ§å¶å°`ç`æ»è§`ä¸­æ¾å°`APP
-ID`å`å¯é¥`,æ ¹æ®ä¸é¢çéç½®è¯´æå¡«å¥.env.*æä»¶   ç¦»çº¿ç¿»è¯
+ID`å`å¯é¥`,æ ¹æ®ä¸é¢çéç½®è¯´æå¡«å¥.env.*æä»¶   ç«å±±ç¿»è¯ 1.
+æ ¹æ®ç«å±±å¼æç[ææ¡£](https://www.volcengine.com/docs/4640/
+130872)ï¼ææµç¨æ³¨å 2.
+åå»ºå¥½æå¡åè·åå°å¯é¥ï¼åå«ä¸º`Access Key ID`å`Secret Access
+Key`ï¼ç¶åç¹å»`Secret Access Key`ä¸çæé®æ¾ç¤ºåºå¯é¥ 3.
+åå«æ ¹æ®ä¸é¢çéç½®è¯´æå¡«å¥.env.*æä»¶   ç¦»çº¿ç¿»è¯
 (è¯¥æ¹æ¡å¯¹è®¾å¤éç½®è¦æ±è¾é«ï¼å»ºè®®å¨æè¶³å¤çç¡¬çç©ºé´ãåå­ãæ¾å­ï¼ææä¸å°è½ä¸ºbotå¤çè¯·æ±çæå¡å¨æ¶èèä½¿ç¨è¯¥æ¹æ¡)
 1. åè[manga-image-translator](https://github.com/zyddnys/manga-image-
 translator)çè¯´æï¼åéä»åºï¼å¹¶å®è£ç¸å³ä¾èµ
 (å¯è½éè¦é¢å¤å®è£`pydensecrf`) 2.
 å®è£å¥½ä¾èµåï¼å¨ä»åºç®å½ä¸è¿è¡ ```python python -
 m manga_translator -v --mode web --use-cuda# the demo will be serving on http:/
 /127.0.0.1:5003 ``` 3. å¦æä½ çè®¾å¤æ²¡ææåå®è£cuda
@@ -61,10 +55,30 @@
 å¦æbotåç¿»è¯å¨å¨åä¸å°è®¾å¤ï¼é£ä¹.envå¡«å`offline_url="http://
 127.0.0.1:
 5003"`å³å¯ï¼å¦æä¸å¨åä¸å°è®¾å¤ï¼ä½ **å¯è½**è¿éè¦æ¾è¡é²ç«å¢ãç«¯å£è½¬åç­ï¼å¹¶ä¸å¡«ååå®¹ä¹ä¼ææåå
 6.
 æåä½ **å¯è½**è¿éè¦ä¿®æ¹ä¸ä¸æ¬æä»¶çä»£ç ï¼æ¾å°æ¬æä»¶`utils.py`ç`offline`å½æ°ï¼æ ¹æ®æ³¨éå
 [ææ¡£](https://github.com/zyddnys/manga-image-translator/blob/main/
 README.md),ä¿®æ¹å­å¸`data`ï¼ä»èæå®ä½ æ³è¦çOCRæ¨¡ååç¿»è¯æ¨¡å
-(ç®åæ¯ç¨äºofflineæ¨¡å,ä½ å¯ä»¥æ¹æå«ç)  ## ð¦è®¡å - [x]
-æ¯æé¨ç½²ç¦»çº¿ç¿»è¯æ¨¡å - [ ] æ¯ææ´å¤API - [ ] å®åæä»¶ ##
+(ç®åæ¯ç¨äºofflineæ¨¡å,ä½ å¯ä»¥æ¹æå«ç)  ## ðå½ä»¤ 1.
+å¾çç¿»è¯ [å¾ç]ï¼åå¼ å¾çç¿»è¯ï¼ä¹å¯ä»¥ååé/
+å¾çç¿»è¯ååéå¾ç,å¯ä»¥å¦ä¸ç»å 1. æå­+å¾ç 2.
+åæå­ï¼åå¾ç 3. æå­åå¤å¾ç 2. å¤å¾çç¿»è¯
+[å¾ç]ï¼nå¼ å¾çç¿»è¯ï¼å°ä¼ä»¥åå¹¶è½¬åæ¶æ¯çå½¢å¼ååº,å¯ä»¥å¦ä¸ç»å
+1. åæå­ï¼åå¤å¼ å¾ç 2. æå­+å¾ç*n 3. åæ¢ç¿»è¯api [api]:
+å°è¯¥apiä¼åçº§æå°æé«ï¼ç®åæ`youdao baidu huoshan offline`
+æªå®å¾ç»­ ## â­ææå¾ [https://github.com/maoxig/nonebot-plugin-manga-
+translator/blob/main/resource/ææå¾1.jpg] [https://github.com/maoxig/
+nonebot-plugin-manga-translator/blob/main/resource/ææå¾2.jpg] [https://
+github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/
+ææå¾3.jpg] [https://github.com/maoxig/nonebot-plugin-manga-translator/
+blob/main/resource/ææå¾4.PNG] ## ðæ´æ°æ¥å¿  ç¹å»å±å¼ - 2023-05-
+03: - æ´æ°è¯´æææ¡£ - éé[ç«å±±ç¿»è¯api](https://
+translate.volcengine.com/api),ä½ å¯ä»¥éæ©æ¥å¥ç«å±±ç¿»è¯æä¾çAPI -
+2023-05-01: -
+æ·»å åæ¢apiçåè½ï¼ä½ å¯ä»¥å°æä¸ªapiä¼åçº§è®¾ä¸ºæé« -
+ééç¦»çº¿ç¿»è¯api[manga-image-translator](https://github.com/zyddnys/manga-
+image-translator),ç°å¨ä½ å¯ä»¥ä½éªæ¬å°çç¿»è¯ - 2023-04-28: -
+æä»¶åå¸  ## ð¦è®¡å - [x] ééç¦»çº¿ç¿»è¯æ¨¡å[manga-image-
+translator](https://github.com/zyddnys/manga-image-translator) - [x]
+æ¯ææ´å¤API - [ ] å®åæä»¶ ##
 â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ
```

### Comparing `nonebot_plugin_manga_translator-0.1.1/nonebot_plugin_manga_translator/__init__.py` & `nonebot_plugin_manga_translator-0.1.2/nonebot_plugin_manga_translator/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_manga_translator-0.1.1/pyproject.toml` & `nonebot_plugin_manga_translator-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-manga-translator"
-version = "0.1.1"
+version = "0.1.2"
 description = "基于nonebot2的适配多种api的图片/漫画翻译插件"
 authors = ["xenophon <674550338@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_manga_translator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_manga_translator-0.1.1/PKG-INFO` & `nonebot_plugin_manga_translator-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-manga-translator
-Version: 0.1.1
+Version: 0.1.2
 Summary: 基于nonebot2的适配多种api的图片/漫画翻译插件
 License: MIT
 Author: xenophon
 Author-email: 674550338@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -41,112 +41,129 @@
 
 ## 📖简介
 
 1. 适配多种api,将收到的图片翻译并发送翻译后的图片，支持批量操作
 
 2. ⚙️插件配置
 
-这些配置项必填，否则无法使用，请在机器人目录下的.env.*里填写以下选项(至少填一个平台的)
+请在机器人目录下的.env.*里填写以下选项(至少填一个平台的)，获取方式已整理好，见下方
 
-~~个人感觉有道API的效果比百度好很多，但是架不住百度每个月前1w次调用免费啊~~
+~~个人感觉就漫画翻译而言,这几家API的效果大致为有道>=百度≈离线>=火山,且火山翻译对竖版日文的翻译效果很差~~
 
-|       配置项        | 类型  | 默认值 |          示例           | 说明    |
-| :-----------------: | :---: | :-----: | :------------------------: | :------- |
-|     有道翻译API     |   -   |    -    |             -              | -        |
-|   youdao_app_key    |  str  |   ""    |   youdao_app_key="xxxxx"   | 应用ID   |
-|  youdao_app_secret  |  str  |   ""    | youdao_app_secret="xxxxxx" | 应用秘钥 |
-|     百度翻译API     |   -   |    -    |             -              | -        |
-|    baidu_app_id     |  str  |   ""    |    baidu_app_id="66666"    | APP ID   |
-|    baidu_app_key    |  str  |   ""    |   baidu_app_key="xxxxxx"   | 密钥     |
-|     离线翻译API     |   -   |    -    |             -              | -        |
-|    offline_url    |  str  |   ""    |   offline_url="http://127.0.0.1:5003"   | 见下方说明     |
-| 其他翻译API(待更新) |   -   |    -    |             -              | -        |
+|          配置项           | 类型  | 默认值 |                示例                 | 说明              | API定价                                           |
+| :-----------------------: | :---: | :----: | :---------------------------------: | :---------------- | :------------------------------------------------ |
+|        有道翻译API        |   -   |   -    |                  -                  | -                 | 梯度收费，0<月调用量<100w时,0.04元/张                   |
+|      youdao_app_key       |  str  |   ""   |       youdao_app_key="xxxxx"        | 应用ID            |                                                   |
+|     youdao_app_secret     |  str  |   ""   |     youdao_app_secret="xxxxxx"      | 应用秘钥          |                                                   |
+|        百度翻译API        |   -   |   -    |                  -                  | -                 | 每月1万次免费调用量，之后按梯度收费,最高0.04元/次 |
+|       baidu_app_id        |  str  |   ""   |        baidu_app_id="66666"         | APP ID            |                                                   |
+|       baidu_app_key       |  str  |   ""   |       baidu_app_key="xxxxxx"        | 密钥              |                                                   |
+|        火山翻译API        |   -   |   -    |                  -                  | -                 | 每月前100张免费，之后0.04元/张                    |
+|   huoshan_access_key_id   |  str  |   ""   |    huoshan_access_key_id="AK***"    | Access Key ID     |                                                   |
+| huoshan_secret_access_key |  str  |   ""   |  huoshan_secret_access_key="UT**"   | Secret Access Key |                                                   |
+|        离线翻译API        |   -   |   -    |                  -                  | -                 |                                            可能是电费?       |
+|        offline_url        |  str  |   ""   | offline_url="http://127.0.0.1:5003" | 见下方说明        |                                                   |
+|    其他翻译API(待更新)    |   -   |   -    |                  -                  | -                 |                                                   |
 
-## 🌙更新日志
+## 🔑API获取
 
 <details>
-<summary>点击展开</summary>
+<summary>有道翻译</summary>
 
-- 2023-05-01:
+1. 在[有道智云AI开放平台](https://ai.youdao.com/#/)注册并登录后，进入控制台
+2. 在左侧`自然语言翻译服务`里的`图片翻译`里创建应用，选择服务和接入方式分别为`图片翻译`和`API`，其他项随意。
+![Image text](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/有道翻译.png)
+3. 创建后将`应用ID`和`应用秘钥`按照上面的配置说明分别填入.env.*文件里即可
 
-  - 添加切换api的功能，你可以将某个api优先级设为最高
-  - 适配离线翻译api[manga-image-translator](https://github.com/zyddnys/manga-image-translator),现在你可以体验本地的翻译
+</details>
 
-- 2023-04-28:
+<details>
+<summary>百度翻译</summary>
 
-  插件发布
+   1. 在[百度翻译开放平台](https://api.fanyi.baidu.com/)注册并登录
+   2. 找到`产品服务`的`图片翻译`,申请创建
+   3. 创建后在`管理控制台`的`总览`中找到`APP ID`和`密钥`,根据上面的配置说明填入.env.*文件
+
+</details>
+
+<details>
+<summary>火山翻译</summary>
+
+   1. 根据火山引擎的[文档](https://www.volcengine.com/docs/4640/130872)，按流程注册
+   2. 创建好服务后获取到密钥，分别为`Access Key ID`和`Secret Access Key`，然后点击`Secret Access Key`下的按钮显示出密钥
+   3. 分别根据上面的配置说明填入.env.*文件
+
+</details>
+
+<details>
+<summary>离线翻译</summary>
+(该方案对设备配置要求较高，建议在有足够的硬盘空间、内存、显存，或有一台能为bot处理请求的服务器时考虑使用该方案)
+
+   1. 参考[manga-image-translator](https://github.com/zyddnys/manga-image-translator)的说明，克隆仓库，并安装相关依赖(可能需要额外安装`pydensecrf`)
+   2. 安装好依赖后，在仓库目录下运行
+
+      ```python
+      python -m manga_translator -v --mode web --use-cuda# the demo will be serving on http://127.0.0.1:5003
+      ```
+
+   3. 如果你的设备没有成功安装cuda(要求pytorch的版本和cuda对应，不对应请重装)，请去掉参数`--use-cuda`，如果图片处理过程中爆显存，请改成`--use-cuda-limited`
+
+   4. 你可以访问控制台给出的网址，尝试先本地翻译一张图片，此时会根据选项下载需要的模型(为防止下载失败，也可以提前手动下载)
+   5. 如果bot和翻译器在同一台设备，那么.env填写`offline_url="http://127.0.0.1:5003"`即可，如果不在同一台设备，你**可能**还需要放行防火墙、端口转发等，并且填写内容也会有所变化
+   6. 最后你**可能**还需要修改一下本插件的代码，找到本插件`utils.py`的`offline`函数，根据注释和[文档](https://github.com/zyddnys/manga-image-translator/blob/main/README.md),修改字典`data`，从而指定你想要的OCR模型和翻译模型(目前是用了offline模型,你可以改成别的)
 
 </details>
 
 ## 🎉命令
 
 1. 图片翻译 [图片]：单张图片翻译，也可以先发送/图片翻译再发送图片,可以如下组合
 
     1. 文字+图片
     2. 先文字，后图片
     3. 文字回复图片
 
 2. 多图片翻译 [图片]：n张图片翻译，将会以合并转发消息的形式发出,可以如下组合
 
     1. 先文字，后多张图片 
-    2. 2.文字+图片*n
-3. 切换翻译api [api]: 将该api优先级提到最高，目前有`youdao baidu offline`
+    2. 文字+图片*n
+3. 切换翻译api [api]: 将该api优先级提到最高，目前有`youdao baidu huoshan offline`
 
 未完待续
 
 ## ⭐效果图
 
 <img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图1.jpg" width="300" height="300">
 <img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图2.jpg" width="300" height="300">
 <img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图3.jpg" width="300" height="300">
 <img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图4.PNG" width="300" height="300">
 
-## 🔑API获取
-
-<details>
-<summary>有道翻译</summary>
-
-1. 在[有道智云AI开放平台](https://ai.youdao.com/#/)注册并登录后，进入控制台
-2. 在左侧`自然语言翻译服务`里的`图片翻译`里创建应用，选择服务和接入方式分别为`图片翻译`和`API`，其他项随意。
-![Image text](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/有道翻译.png)
-3. 创建后将`应用ID`和`应用秘钥`按照上面的配置说明分别填入.env.*文件里即可
-
-</details>
+## 🌙更新日志
 
 <details>
-<summary>百度翻译</summary>
-
-   1. 在[百度翻译开放平台](https://api.fanyi.baidu.com/)注册并登录
-   2. 找到`产品服务`的`图片翻译`,申请创建
-   3. 创建后在`管理控制台`的`总览`中找到`APP ID`和`密钥`,根据上面的配置说明填入.env.*文件
+<summary>点击展开</summary>
 
-</details>
+- 2023-05-03:
 
-<details>
-<summary>离线翻译</summary>
-(该方案对设备配置要求较高，建议在有足够的硬盘空间、内存、显存，或有一台能为bot处理请求的服务器时考虑使用该方案)
+  - 更新说明文档
+  - 适配[火山翻译api](https://translate.volcengine.com/api),你可以选择接入火山翻译提供的API
 
-   1. 参考[manga-image-translator](https://github.com/zyddnys/manga-image-translator)的说明，克隆仓库，并安装相关依赖(可能需要额外安装`pydensecrf`)
-   2. 安装好依赖后，在仓库目录下运行
+- 2023-05-01:
 
-      ```python
-      python -m manga_translator -v --mode web --use-cuda# the demo will be serving on http://127.0.0.1:5003
-      ```
+  - 添加切换api的功能，你可以将某个api优先级设为最高
+  - 适配离线翻译api[manga-image-translator](https://github.com/zyddnys/manga-image-translator),现在你可以体验本地的翻译
 
-   3. 如果你的设备没有成功安装cuda(要求pytorch的版本和cuda对应，不对应请重装)，请去掉参数`--use-cuda`，如果图片处理过程中爆显存，请改成`--use-cuda-limited`
+- 2023-04-28:
 
-   4. 你可以访问控制台给出的网址，尝试先本地翻译一张图片，此时会根据选项下载需要的模型(为防止下载失败，也可以提前手动下载)
-   5. 如果bot和翻译器在同一台设备，那么.env填写`offline_url="http://127.0.0.1:5003"`即可，如果不在同一台设备，你**可能**还需要放行防火墙、端口转发等，并且填写内容也会有所变化
-   6. 最后你**可能**还需要修改一下本插件的代码，找到本插件`utils.py`的`offline`函数，根据注释和[文档](https://github.com/zyddnys/manga-image-translator/blob/main/README.md),修改字典`data`，从而指定你想要的OCR模型和翻译模型(目前是用了offline模型,你可以改成别的)
+  - 插件发布
 
 </details>
 
 ## 🐦计划
 
-- [x] 支持部署离线翻译模型
+- [x] 适配离线翻译模型[manga-image-translator](https://github.com/zyddnys/manga-image-translator)
 
-- [ ] 支持更多API
+- [x] 支持更多API
 
 - [ ] 完善插件
 
 ## ✨喜欢的话就点个star✨吧，球球了QAQ
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-manga-translator Version: 0.1.1
+Metadata-Version: 2.1 Name: nonebot-plugin-manga-translator Version: 0.1.2
 Summary: åºäºnonebot2çééå¤ç§apiçå¾ç/æ¼«ç»ç¿»è¯æä»¶ License:
 MIT Author: xenophon Author-email: 674550338@qq.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.1.1,<10.0.0) Requires-Dist: httpx (>=0.23.0,<0.24.0)
@@ -13,54 +13,48 @@
         # nonebot-plugin-manga-translator â¨*åºäºNonebot2çå¾ç/
                             æ¼«ç»ç¿»è¯æä»¶*â¨
 ## ð¿å®è£ éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb:
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨ `nb plugin install
 nonebot_plugin_manga_translator` - ä½¿ç¨pip(ä¸æ¨è):
 ~~ä¸æ¨èå°±æ¯ä¸æ¨èï¼ç¥ç¥ç¥~~ ## ðç®ä» 1.
 ééå¤ç§api,å°æ¶å°çå¾çç¿»è¯å¹¶åéç¿»è¯åçå¾çï¼æ¯ææ¹éæä½
-2. âï¸æä»¶éç½®
-è¿äºéç½®é¡¹å¿å¡«ï¼å¦åæ æ³ä½¿ç¨ï¼è¯·å¨æºå¨äººç®å½ä¸ç.env.*éå¡«åä»¥ä¸éé¡¹
-(è³å°å¡«ä¸ä¸ªå¹³å°ç)
-~~ä¸ªäººæè§æéAPIçæææ¯ç¾åº¦å¥½å¾å¤ï¼ä½æ¯æ¶ä¸ä½ç¾åº¦æ¯ä¸ªæå1wæ¬¡è°ç¨åè´¹å~~
-| éç½®é¡¹ | ç±»å | é»è®¤å¼ | ç¤ºä¾ | è¯´æ | | :-----------------: | :-
---: | :-----: | :------------------------: | :------- | | æéç¿»è¯API | - |
-- | - | - | | youdao_app_key | str | "" | youdao_app_key="xxxxx" | åºç¨ID | |
-youdao_app_secret | str | "" | youdao_app_secret="xxxxxx" | åºç¨ç§é¥ | |
-ç¾åº¦ç¿»è¯API | - | - | - | - | | baidu_app_id | str | "" |
-baidu_app_id="66666" | APP ID | | baidu_app_key | str | "" |
-baidu_app_key="xxxxxx" | å¯é¥ | | ç¦»çº¿ç¿»è¯API | - | - | - | - | |
+2. âï¸æä»¶éç½® è¯·å¨æºå¨äººç®å½ä¸ç.env.*éå¡«åä»¥ä¸éé¡¹
+(è³å°å¡«ä¸ä¸ªå¹³å°ç)ï¼è·åæ¹å¼å·²æ´çå¥½ï¼è§ä¸æ¹
+~~ä¸ªäººæè§å°±æ¼«ç»ç¿»è¯èè¨,è¿å å®¶APIçææå¤§è´ä¸ºæé>=ç¾åº¦âç¦»çº¿>=ç«å±±,ä¸ç«å±±ç¿»è¯å¯¹ç«çæ¥æçç¿»è¯ææå¾å·®~~
+| éç½®é¡¹ | ç±»å | é»è®¤å¼ | ç¤ºä¾ | è¯´æ | APIå®ä»· | | :-----------
+------------: | :---: | :----: | :---------------------------------: | :-------
+--------- | :------------------------------------------------ | |
+æéç¿»è¯API | - | - | - | - |
+æ¢¯åº¦æ¶è´¹ï¼0<æè°ç¨é<100wæ¶,0.04å/å¼  | | youdao_app_key | str | ""
+| youdao_app_key="xxxxx" | åºç¨ID | | | youdao_app_secret | str | "" |
+youdao_app_secret="xxxxxx" | åºç¨ç§é¥ | | | ç¾åº¦ç¿»è¯API | - | - | - | -
+| æ¯æ1ä¸æ¬¡åè´¹è°ç¨éï¼ä¹åææ¢¯åº¦æ¶è´¹,æé«0.04å/æ¬¡ | |
+baidu_app_id | str | "" | baidu_app_id="66666" | APP ID | | | baidu_app_key |
+str | "" | baidu_app_key="xxxxxx" | å¯é¥ | | | ç«å±±ç¿»è¯API | - | - | - |
+- | æ¯æå100å¼ åè´¹ï¼ä¹å0.04å/å¼  | | huoshan_access_key_id | str |
+"" | huoshan_access_key_id="AK***" | Access Key ID | | |
+huoshan_secret_access_key | str | "" | huoshan_secret_access_key="UT**" |
+Secret Access Key | | | ç¦»çº¿ç¿»è¯API | - | - | - | - | å¯è½æ¯çµè´¹? | |
 offline_url | str | "" | offline_url="http://127.0.0.1:5003" | è§ä¸æ¹è¯´æ
-| | å¶ä»ç¿»è¯API(å¾æ´æ°) | - | - | - | - | ## ðæ´æ°æ¥å¿
-ç¹å»å±å¼ - 2023-05-01: -
-æ·»å åæ¢apiçåè½ï¼ä½ å¯ä»¥å°æä¸ªapiä¼åçº§è®¾ä¸ºæé« -
-ééç¦»çº¿ç¿»è¯api[manga-image-translator](https://github.com/zyddnys/manga-
-image-translator),ç°å¨ä½ å¯ä»¥ä½éªæ¬å°çç¿»è¯ - 2023-04-28:
-æä»¶åå¸  ## ðå½ä»¤ 1. å¾çç¿»è¯
-[å¾ç]ï¼åå¼ å¾çç¿»è¯ï¼ä¹å¯ä»¥ååé/
-å¾çç¿»è¯ååéå¾ç,å¯ä»¥å¦ä¸ç»å 1. æå­+å¾ç 2.
-åæå­ï¼åå¾ç 3. æå­åå¤å¾ç 2. å¤å¾çç¿»è¯
-[å¾ç]ï¼nå¼ å¾çç¿»è¯ï¼å°ä¼ä»¥åå¹¶è½¬åæ¶æ¯çå½¢å¼ååº,å¯ä»¥å¦ä¸ç»å
-1. åæå­ï¼åå¤å¼ å¾ç 2. 2.æå­+å¾ç*n 3. åæ¢ç¿»è¯api [api]:
-å°è¯¥apiä¼åçº§æå°æé«ï¼ç®åæ`youdao baidu offline` æªå®å¾ç»­
-## â­ææå¾ [https://github.com/maoxig/nonebot-plugin-manga-translator/
-blob/main/resource/ææå¾1.jpg] [https://github.com/maoxig/nonebot-plugin-
-manga-translator/blob/main/resource/ææå¾2.jpg] [https://github.com/maoxig/
-nonebot-plugin-manga-translator/blob/main/resource/ææå¾3.jpg] [https://
-github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/
-ææå¾4.PNG] ## ðAPIè·å  æéç¿»è¯ 1. å¨
-[æéæºäºAIå¼æ¾å¹³å°](https://ai.youdao.com/#/
+| | | å¶ä»ç¿»è¯API(å¾æ´æ°) | - | - | - | - | | ## ðAPIè·å
+æéç¿»è¯ 1. å¨[æéæºäºAIå¼æ¾å¹³å°](https://ai.youdao.com/#/
 )æ³¨åå¹¶ç»å½åï¼è¿å¥æ§å¶å° 2.
 å¨å·¦ä¾§`èªç¶è¯­è¨ç¿»è¯æå¡`éç`å¾çç¿»è¯`éåå»ºåºç¨ï¼éæ©æå¡åæ¥å¥æ¹å¼åå«ä¸º`å¾çç¿»è¯`å`API`ï¼å¶ä»é¡¹éæã
 ![Image text](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/
 main/resource/æéç¿»è¯.png) 3.
 åå»ºåå°`åºç¨ID`å`åºç¨ç§é¥`æç§ä¸é¢çéç½®è¯´æåå«å¡«å¥.env.*æä»¶éå³å¯
 ç¾åº¦ç¿»è¯ 1. å¨[ç¾åº¦ç¿»è¯å¼æ¾å¹³å°](https://api.fanyi.baidu.com/
 )æ³¨åå¹¶ç»å½ 2. æ¾å°`äº§åæå¡`ç`å¾çç¿»è¯`,ç³è¯·åå»º 3.
 åå»ºåå¨`ç®¡çæ§å¶å°`ç`æ»è§`ä¸­æ¾å°`APP
-ID`å`å¯é¥`,æ ¹æ®ä¸é¢çéç½®è¯´æå¡«å¥.env.*æä»¶   ç¦»çº¿ç¿»è¯
+ID`å`å¯é¥`,æ ¹æ®ä¸é¢çéç½®è¯´æå¡«å¥.env.*æä»¶   ç«å±±ç¿»è¯ 1.
+æ ¹æ®ç«å±±å¼æç[ææ¡£](https://www.volcengine.com/docs/4640/
+130872)ï¼ææµç¨æ³¨å 2.
+åå»ºå¥½æå¡åè·åå°å¯é¥ï¼åå«ä¸º`Access Key ID`å`Secret Access
+Key`ï¼ç¶åç¹å»`Secret Access Key`ä¸çæé®æ¾ç¤ºåºå¯é¥ 3.
+åå«æ ¹æ®ä¸é¢çéç½®è¯´æå¡«å¥.env.*æä»¶   ç¦»çº¿ç¿»è¯
 (è¯¥æ¹æ¡å¯¹è®¾å¤éç½®è¦æ±è¾é«ï¼å»ºè®®å¨æè¶³å¤çç¡¬çç©ºé´ãåå­ãæ¾å­ï¼ææä¸å°è½ä¸ºbotå¤çè¯·æ±çæå¡å¨æ¶èèä½¿ç¨è¯¥æ¹æ¡)
 1. åè[manga-image-translator](https://github.com/zyddnys/manga-image-
 translator)çè¯´æï¼åéä»åºï¼å¹¶å®è£ç¸å³ä¾èµ
 (å¯è½éè¦é¢å¤å®è£`pydensecrf`) 2.
 å®è£å¥½ä¾èµåï¼å¨ä»åºç®å½ä¸è¿è¡ ```python python -
 m manga_translator -v --mode web --use-cuda# the demo will be serving on http:/
 /127.0.0.1:5003 ``` 3. å¦æä½ çè®¾å¤æ²¡ææåå®è£cuda
@@ -72,10 +66,30 @@
 å¦æbotåç¿»è¯å¨å¨åä¸å°è®¾å¤ï¼é£ä¹.envå¡«å`offline_url="http://
 127.0.0.1:
 5003"`å³å¯ï¼å¦æä¸å¨åä¸å°è®¾å¤ï¼ä½ **å¯è½**è¿éè¦æ¾è¡é²ç«å¢ãç«¯å£è½¬åç­ï¼å¹¶ä¸å¡«ååå®¹ä¹ä¼ææåå
 6.
 æåä½ **å¯è½**è¿éè¦ä¿®æ¹ä¸ä¸æ¬æä»¶çä»£ç ï¼æ¾å°æ¬æä»¶`utils.py`ç`offline`å½æ°ï¼æ ¹æ®æ³¨éå
 [ææ¡£](https://github.com/zyddnys/manga-image-translator/blob/main/
 README.md),ä¿®æ¹å­å¸`data`ï¼ä»èæå®ä½ æ³è¦çOCRæ¨¡ååç¿»è¯æ¨¡å
-(ç®åæ¯ç¨äºofflineæ¨¡å,ä½ å¯ä»¥æ¹æå«ç)  ## ð¦è®¡å - [x]
-æ¯æé¨ç½²ç¦»çº¿ç¿»è¯æ¨¡å - [ ] æ¯ææ´å¤API - [ ] å®åæä»¶ ##
+(ç®åæ¯ç¨äºofflineæ¨¡å,ä½ å¯ä»¥æ¹æå«ç)  ## ðå½ä»¤ 1.
+å¾çç¿»è¯ [å¾ç]ï¼åå¼ å¾çç¿»è¯ï¼ä¹å¯ä»¥ååé/
+å¾çç¿»è¯ååéå¾ç,å¯ä»¥å¦ä¸ç»å 1. æå­+å¾ç 2.
+åæå­ï¼åå¾ç 3. æå­åå¤å¾ç 2. å¤å¾çç¿»è¯
+[å¾ç]ï¼nå¼ å¾çç¿»è¯ï¼å°ä¼ä»¥åå¹¶è½¬åæ¶æ¯çå½¢å¼ååº,å¯ä»¥å¦ä¸ç»å
+1. åæå­ï¼åå¤å¼ å¾ç 2. æå­+å¾ç*n 3. åæ¢ç¿»è¯api [api]:
+å°è¯¥apiä¼åçº§æå°æé«ï¼ç®åæ`youdao baidu huoshan offline`
+æªå®å¾ç»­ ## â­ææå¾ [https://github.com/maoxig/nonebot-plugin-manga-
+translator/blob/main/resource/ææå¾1.jpg] [https://github.com/maoxig/
+nonebot-plugin-manga-translator/blob/main/resource/ææå¾2.jpg] [https://
+github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/
+ææå¾3.jpg] [https://github.com/maoxig/nonebot-plugin-manga-translator/
+blob/main/resource/ææå¾4.PNG] ## ðæ´æ°æ¥å¿  ç¹å»å±å¼ - 2023-05-
+03: - æ´æ°è¯´æææ¡£ - éé[ç«å±±ç¿»è¯api](https://
+translate.volcengine.com/api),ä½ å¯ä»¥éæ©æ¥å¥ç«å±±ç¿»è¯æä¾çAPI -
+2023-05-01: -
+æ·»å åæ¢apiçåè½ï¼ä½ å¯ä»¥å°æä¸ªapiä¼åçº§è®¾ä¸ºæé« -
+ééç¦»çº¿ç¿»è¯api[manga-image-translator](https://github.com/zyddnys/manga-
+image-translator),ç°å¨ä½ å¯ä»¥ä½éªæ¬å°çç¿»è¯ - 2023-04-28: -
+æä»¶åå¸  ## ð¦è®¡å - [x] ééç¦»çº¿ç¿»è¯æ¨¡å[manga-image-
+translator](https://github.com/zyddnys/manga-image-translator) - [x]
+æ¯ææ´å¤API - [ ] å®åæä»¶ ##
 â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ
```

