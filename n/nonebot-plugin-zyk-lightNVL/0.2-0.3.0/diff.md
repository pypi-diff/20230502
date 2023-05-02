# Comparing `tmp/nonebot_plugin_zyk_lightNVL-0.2.tar.gz` & `tmp/nonebot_plugin_zyk_lightNVL-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_zyk_lightNVL-0.2.tar", last modified: Mon May  1 13:05:58 2023, max compression
+gzip compressed data, was "nonebot_plugin_zyk_lightNVL-0.3.0.tar", last modified: Tue May  2 13:16:45 2023, max compression
```

## Comparing `nonebot_plugin_zyk_lightNVL-0.2.tar` & `nonebot_plugin_zyk_lightNVL-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 13:05:58.738841 nonebot_plugin_zyk_lightNVL-0.2/
--rw-rw-rw-   0        0        0     1083 2023-04-20 14:30:24.000000 nonebot_plugin_zyk_lightNVL-0.2/LICENSE
--rw-rw-rw-   0        0        0      266 2023-05-01 13:05:58.736841 nonebot_plugin_zyk_lightNVL-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2727 2023-04-20 14:30:24.000000 nonebot_plugin_zyk_lightNVL-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 13:05:58.667837 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/
--rw-rw-rw-   0        0        0     6291 2023-05-01 12:55:09.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/__init__.py
--rw-rw-rw-   0        0        0     1218 2023-05-01 13:04:33.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/config.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:05:58.729840 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/
--rw-rw-rw-   0        0        0    17204 2016-01-24 08:41:06.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/ChangeLog
--rw-rw-rw-   0        0        0     1429 2016-01-24 08:41:06.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/LICENSE.BSD
--rw-rw-rw-   0        0        0     2502 2016-01-24 08:41:06.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/README.md
--rw-rw-rw-   0        0        0     1510 2016-01-24 08:41:06.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/third-party.txt
--rw-rw-rw-   0        0        0        0 2023-05-01 12:57:57.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/template.html
--rw-rw-rw-   0        0        0     4566 2023-05-01 12:55:42.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/work.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:05:58.702839 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/
--rw-rw-rw-   0        0        0      266 2023-05-01 13:05:58.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-05-01 13:05:58.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 13:05:58.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-05-01 13:05:58.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-05-01 13:05:58.000000 nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 13:05:58.741841 nonebot_plugin_zyk_lightNVL-0.2/setup.cfg
--rw-rw-rw-   0        0        0      609 2023-05-01 13:03:10.000000 nonebot_plugin_zyk_lightNVL-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:16:45.071324 nonebot_plugin_zyk_lightNVL-0.3.0/
+-rw-rw-rw-   0        0        0     1083 2023-04-20 14:30:24.000000 nonebot_plugin_zyk_lightNVL-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      318 2023-05-02 13:16:45.070324 nonebot_plugin_zyk_lightNVL-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2710 2023-05-02 13:16:09.000000 nonebot_plugin_zyk_lightNVL-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 13:16:45.033322 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/
+-rw-rw-rw-   0        0        0     8705 2023-05-02 12:59:35.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/__init__.py
+-rw-rw-rw-   0        0        0     1759 2023-05-02 13:06:39.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/config.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:01:17.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/index.html
+drwxrwxrwx   0        0        0        0 2023-05-02 13:16:45.066324 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/phantomjs/
+-rw-rw-rw-   0        0        0    17204 2016-01-24 08:41:06.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/phantomjs/ChangeLog
+-rw-rw-rw-   0        0        0     1429 2016-01-24 08:41:06.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/phantomjs/LICENSE.BSD
+-rw-rw-rw-   0        0        0     2502 2016-01-24 08:41:06.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/phantomjs/README.md
+-rw-rw-rw-   0        0        0     1510 2016-01-24 08:41:06.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/phantomjs/third-party.txt
+-rw-rw-rw-   0        0        0        0 2023-05-01 12:57:57.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/template.html
+-rw-rw-rw-   0        0        0     7115 2023-05-02 12:59:57.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/work.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:16:45.051323 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL.egg-info/
+-rw-rw-rw-   0        0        0      318 2023-05-02 13:16:44.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2023-05-02 13:16:44.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 13:16:44.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-05-02 13:16:44.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-05-02 13:16:44.000000 nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 13:16:45.073324 nonebot_plugin_zyk_lightNVL-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      675 2023-05-02 13:02:46.000000 nonebot_plugin_zyk_lightNVL-0.3.0/setup.py
```

### Comparing `nonebot_plugin_zyk_lightNVL-0.2/LICENSE` & `nonebot_plugin_zyk_lightNVL-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_lightNVL-0.2/README.md` & `nonebot_plugin_zyk_lightNVL-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,115 @@
 # :memo: nonebot_plugin_zyk_lightNVL
 
 *:page_facing_up: 使用本插件前请仔细阅读README*
 
 *本插件基于轻小说网站[哔哩轻小说](https://w.linovelib.com)制作*
 
->说明
+## 更新0.3.0
 
-本插件目前只是半成品，先厚脸皮来占个坑。
-
-目前只支持查询的功能，后面会支持下载。
-
-为什么不做完再发？因为~~懒~~没时间在短期内完成。
+1. 可选使用chorme浏览器工作，速度更快，渲染更优
+2. 新增查看小说目录功能（爆肝中）
 
 ## :cd: 安装方式
+
 - #### 使用pip
-```
+
+```cmd
 pip install nonebot_plugin_zyk_lightNVL
 ```
+
 - #### 使用nb-cli
-```
+
+```cmd
 nb plugin install nonebot_plugin_zyk_lightNVL
 ```
 
 ## :wrench: env配置
 
 |        Name         |   Example   | Type |      Usage       | Required |
 |:-------------------:|:-----------:|:----:|:----------------:|:--------:|
 | light_nvl_username  |     cxk     | str  |   哔哩轻小说账户的用户名    |    No    |
 | light_nvl_password  |   123456    | str  |    哔哩轻小说账户的密码    |    No    |
-|  light_nvl_cookie   | your:cookie | str  |   已经登录的cookie    |    No    |
+|  light_nvl_show_all   | False | bool  |   是否显示所有搜索结果，建议为False    |    No    |
 | light_nvl_retry_num |     50      | int  | 搜索结果发送失败时重新发送的条数 |    No    |
+| light_nvl_browser | chrome | str | 选择的浏览器，默认phantomjs，可选chrome | No |
+| light_nvl_chromedriver_path | path/to/your/chromedriver | str | chromedriver的绝对路径，版本要与你的chrome浏览器一致 | No |
 
 ### 登录说明
-[账号注册](https://w.linovelib.com/register.php)
-
-每次启动时会优先使用env中配置的cookie，如果没有则使用自动保存的cookie登录，如果也没有则以未登录状态继续。
 
-第一次启动则没有自动保存的cookie，需要使用指令来手动登录。
+[账号注册](https://w.linovelib.com/register.php)
 
-每次手动登录成功后将会自动保存cookie。
+获取cookies:
 
-如果已经在浏览器中登录过了，可以直接复制cookie到env配置项中。
+- 启动前先在浏览器中访问[搜索页面](https://w.linovelib.com/search.html)
+- 使用nvl_cookies指令
 
-在有cookie的情况下，无法手动登录。可以使用手动登录指令的*enforce*参数来强制手动登录，一般用于切换账号或cookie异常的情况。
+## :label: 指令
 
+### 登录
 
-## :label: 指令
-### 手动登录
-```
-(COMMAND_START)nvl_login [enforce]
+```cmd
+(COMMAND_START)nvl_login
 
 eg:
     /nvl_login
 ```
-- 可选参数*enforce*用于强制手动登录
+
+### 自动获取cookies
+
+```cmd
+(COMMAND_START)nvl_cookies
+
+eg:
+    /nvl_cookies
 ```
-/nvl_login enforce
+
+用于cookies过期的情况，如果失效请再试一次或重启bot以刷新
+
+### 查找轻小说
+
+#### 使用关键字查找
+
+```cmd
+(COMMAND_START)nvl (key words)
+
+eg:
+    /nvl 回复术士
 ```
 
-### 操作
+#### 使用书页id精确查找
+
+```cmd
+(COMMAND_START)nvl_id (id)
+
+eg:
+    /nvl_id 3636
 ```
-(COMMAND_START)nvl [(info)|bookcase|id (book_id)]
+
+#### 个人书架
+
+```cmd
+(COMMAND_START)nvl_bookcase
 
 eg:
-    /nvl 回复术士
+    /nvl_bookcase
 ```
 
-- 可选参数 *(info)* 、*bookcase*、*id (book_id)* 中**请确保有一个参数存在**。
+只有登录后才可使用
+
+### 查看目录
+
+在bot给你发送了小说的详细信息（一张图片）之后，可以发送`index`和`index_tree`让bot给你发送该小说的目录
+
+- index
+
+用于发送小说的卷数，可进行下一级交互和重复交互
+
+- index_tree
+
+用于发送小说的全部章节（卷数和章数），不可进行下一级交互或重复交互
 
-1. *(info)* 用于查找轻小说，可以是书名、作者、或类型等。
-    ```
-   /nvl 回复术士
-   ```
-2. *bookcase* 用于查看当前账号的书架，只有登录状态才可以使用。
-    ```
-   /nvl bookcase
-   ```
-3. *id (book_id)* 用于导入book_id（可以查看书页，如 `https://w.linovelib.com/novel/3518.html` 中的 `3518`）
-    ```
-   /nvl id 3518
-   ```
 ---
 
 :bug: 如果发现插件有BUG或有建议，欢迎**合理**提*Issue*
 
-:heart: 最后，如果你喜欢本插件，就请给本插件点个:star:吧
+:heart: 最后，如果你喜欢本插件，就请给本插件点个:star:吧
```

### Comparing `nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/ChangeLog` & `nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/phantomjs/ChangeLog`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/LICENSE.BSD` & `nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/phantomjs/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/README.md` & `nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/phantomjs/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL/phantomjs/third-party.txt` & `nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL/phantomjs/third-party.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_lightNVL-0.2/nonebot_plugin_zyk_lightNVL.egg-info/SOURCES.txt` & `nonebot_plugin_zyk_lightNVL-0.3.0/nonebot_plugin_zyk_lightNVL.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 nonebot_plugin_zyk_lightNVL/__init__.py
 nonebot_plugin_zyk_lightNVL/config.py
+nonebot_plugin_zyk_lightNVL/index.html
 nonebot_plugin_zyk_lightNVL/template.html
 nonebot_plugin_zyk_lightNVL/work.py
 nonebot_plugin_zyk_lightNVL.egg-info/PKG-INFO
 nonebot_plugin_zyk_lightNVL.egg-info/SOURCES.txt
 nonebot_plugin_zyk_lightNVL.egg-info/dependency_links.txt
 nonebot_plugin_zyk_lightNVL.egg-info/requires.txt
 nonebot_plugin_zyk_lightNVL.egg-info/top_level.txt
```

### Comparing `nonebot_plugin_zyk_lightNVL-0.2/setup.py` & `nonebot_plugin_zyk_lightNVL-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nonebot_plugin_zyk_lightNVL',
-    version='0.2',
+    version='0.3.0',
     packages=find_packages(),
     url='https://github.com/ZYKsslm/nonebot_plugin_zyk_lightNVL',
     license='MIT LICENSE',
     author='ZYKsslm',
     author_email='3119964735@qq.com',
-    description='A plugin for nonebot2',
-    install_requires=["httpx", "colorama", "lxml", "fake_useragent", "nonebot2", "nonebot_plugin_htmlrender", "nonebot_adapter_onebot", "selenium<=3.3.0", "browser_cookie3"],
-    package_data={"nonebot_plugin_zyk_lightNVL": ["template.html", "phantomjs/*"]}
+    description='A plugin to search light novels based on Bili light novels for nonebot2',
+    install_requires=["httpx", "colorama", "lxml", "fake_useragent", "nonebot2", "nonebot_plugin_htmlrender", "nonebot_adapter_onebot", "selenium==3.3.0", "browser_cookie3"],
+    package_data={"nonebot_plugin_zyk_lightNVL": ["template.html", "index.html", "phantomjs/*"]}
 )
```

