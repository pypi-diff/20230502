# Comparing `tmp/starrail-toolkit-0.2.0.tar.gz` & `tmp/starrail-toolkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.2.0.tar", last modified: Mon May  1 16:53:28 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.3.0.tar", last modified: Tue May  2 18:11:20 2023, max compression
```

## Comparing `starrail-toolkit-0.2.0.tar` & `starrail-toolkit-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,43 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.895466 starrail-toolkit-0.2.0/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-04-29 06:29:57.000000 starrail-toolkit-0.2.0/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     2417 2023-05-01 16:53:28.895319 starrail-toolkit-0.2.0/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     1910 2023-05-01 16:51:58.000000 starrail-toolkit-0.2.0/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-01 16:53:28.895503 starrail-toolkit-0.2.0/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.892528 starrail-toolkit-0.2.0/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      724 2023-05-01 08:24:52.000000 starrail-toolkit-0.2.0/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1257 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.893125 starrail-toolkit-0.2.0/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      957 2023-05-01 15:00:08.000000 starrail-toolkit-0.2.0/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)       71 2023-05-01 08:24:52.000000 starrail-toolkit-0.2.0/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1133 2023-05-01 16:49:09.000000 starrail-toolkit-0.2.0/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.894162 starrail-toolkit-0.2.0/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      817 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3077 2023-05-01 15:06:41.000000 starrail-toolkit-0.2.0/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5088 2023-05-01 14:41:54.000000 starrail-toolkit-0.2.0/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3365 2023-05-01 16:53:15.000000 starrail-toolkit-0.2.0/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3448 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.894271 starrail-toolkit-0.2.0/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-01 08:02:28.000000 starrail-toolkit-0.2.0/starrail/gui/__init__.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.894445 starrail-toolkit-0.2.0/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-04-30 15:17:38.000000 starrail-toolkit-0.2.0/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      546 2023-04-30 15:36:19.000000 starrail-toolkit-0.2.0/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)       22 2023-05-01 14:42:38.000000 starrail-toolkit-0.2.0/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-01 16:53:28.895150 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     2417 2023-05-01 16:53:28.000000 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)      700 2023-05-01 16:53:28.000000 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-01 16:53:28.000000 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-01 16:53:28.000000 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       46 2023-05-01 16:53:28.000000 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-01 16:53:28.000000 starrail-toolkit-0.2.0/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.093640 starrail-toolkit-0.3.0/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-04-29 06:29:57.000000 starrail-toolkit-0.3.0/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3353 2023-05-02 18:11:20.093516 starrail-toolkit-0.3.0/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2846 2023-05-02 18:09:34.000000 starrail-toolkit-0.3.0/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-02 18:11:20.093675 starrail-toolkit-0.3.0/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.089565 starrail-toolkit-0.3.0/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      724 2023-05-01 17:01:35.000000 starrail-toolkit-0.3.0/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      996 2023-05-02 10:02:46.000000 starrail-toolkit-0.3.0/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.090248 starrail-toolkit-0.3.0/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1364 2023-05-02 18:09:52.000000 starrail-toolkit-0.3.0/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      285 2023-05-02 10:06:31.000000 starrail-toolkit-0.3.0/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1211 2023-05-02 18:03:42.000000 starrail-toolkit-0.3.0/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.091412 starrail-toolkit-0.3.0/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      817 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-02 17:49:24.000000 starrail-toolkit-0.3.0/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5088 2023-05-02 17:23:42.000000 starrail-toolkit-0.3.0/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3365 2023-05-02 07:38:24.000000 starrail-toolkit-0.3.0/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3448 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.091650 starrail-toolkit-0.3.0/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-01 17:01:35.000000 starrail-toolkit-0.3.0/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      183 2023-05-02 10:06:34.000000 starrail-toolkit-0.3.0/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.092117 starrail-toolkit-0.3.0/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/utils/__init__.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.092664 starrail-toolkit-0.3.0/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      408 2023-05-02 17:44:53.000000 starrail-toolkit-0.3.0/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1387 2023-05-02 17:50:07.000000 starrail-toolkit-0.3.0/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)       68 2023-05-02 15:17:12.000000 starrail-toolkit-0.3.0/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-02 17:37:53.000000 starrail-toolkit-0.3.0/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-02 16:15:22.000000 starrail-toolkit-0.3.0/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-02 18:03:04.000000 starrail-toolkit-0.3.0/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)       22 2023-05-02 18:09:46.000000 starrail-toolkit-0.3.0/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.093337 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3353 2023-05-02 18:11:20.000000 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)      918 2023-05-02 18:11:20.000000 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-02 18:11:20.000000 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-02 18:11:20.000000 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       46 2023-05-02 18:11:20.000000 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-02 18:11:20.000000 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.2.0/LICENSE` & `starrail-toolkit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.2.0/PKG-INFO` & `starrail-toolkit-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,77 @@
-Metadata-Version: 2.1
-Name: starrail-toolkit
-Version: 0.2.0
-Summary: Honkai Star Rail Toolkit
-Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
-Author: LittleNyima
-Author-email: littlenyima@163.com
-License: GPLv3
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 《崩坏：星穹铁道》工具箱
 
-<div style="min-height: 275px">
-<img src="https://s1.ax1x.com/2023/04/30/p98Cv26.png" alt="logo" align="left" vertical-align="center" />
-
-```
-Starrail Toolkit
-
-- 主分支版本：0.2.0
-- 开发分支版本：0.2.0
-- PyPI 版本：0.2.0
-```
+<div align="center">
+<img src="https://s1.ax1x.com/2023/04/30/p98Cv26.png" alt="logo" />
 </div>
 
-<br clear="left">
-
 ## 开发状态
 
+| 主分支版本 | 开发分支版本 | PyPI 版本 |
+| :--------: | :----------: | :-------: |
+|   0.3.0    |    0.3.0     |   0.3.0   |
+
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
-- [ ] 支持导出网页版抽卡报告
+- [x] 支持导出网页版抽卡报告
+- [x] 支持中英文多语言导出
 - [ ] 支持 Windows 平台游戏中自动检测 API URL
 - [ ] 实现用户界面并编译到 Windows 与 macOS 平台
 - [ ] 支持自动检查更新
 
-## 导出结果示例
-
-- Excel 结果示例（为保护隐私已隐藏部分信息）
-
-  ![xlsx](https://s1.ax1x.com/2023/05/02/p9GJKts.md.png)
-
-- Markdown 结果示例：
-
-  ![markdown](https://s1.ax1x.com/2023/05/02/p9GJMhn.md.png)
-
 ## 安装方式
 
 目前仅提供命令行版本，用户交互界面版本正在开发中。
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
 pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
 ```
 
+### 从源码安装
+
+若需要使用尚未推送到 PyPI 版本的功能，可通过源码安装：
+
+```shell
+git clone git@github.com:LittleNyima/honkai-starrail-toolkit.git
+cd honkai-starrail-toolkit
+python setup.py install
+```
+
 ## 使用指南
 
 ### 获取抽卡查询 API URL
 
-请参考[【这个教程】](docs/how-to-get-api-url)获取查询链接。
+请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间后过期，过期后需要重新获取。
 
 ### 导出抽卡记录
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
 ```shell
-hksr --api https://api-takumi.mihoyo.com/xxx --export all
+hksr --api https://api-takumi.mihoyo.com/xxx
 ```
 
-参数：`--export` 为导出格式，默认为导出全部格式，若仅需导出部分格式，可将对应参数替换。目前支持的格式有 `csv`、`json`、`md`、`xlsx`，替换方式例如 `--export json xlsx`。
+**参数说明：**
+
+- `--api`：（必选）API URL 地址。*注：未来将支持自动获取 API URL，届时本参数将变为可选。*
+- `--export`：（可选）导出格式选项。默认为导出全部格式，若仅需导出部分格式，可以替换对应参数。目前支持的格式有 `csv`、`html`、`json`、`md`、`xlsx`。例如，若只需要 json 与 xlsx 格式数据，可以替换为 `--export json xlsx`。
+- `--locale`：（可选）控制输出语言。默认为输出简体中文，可选值为 `en`（英语）、`chs`（简体中文）。
+- `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
+
+## 导出结果示例
+
+- Excel 结果示例（为保护隐私已隐藏部分信息）
+
+  <img src="https://s1.ax1x.com/2023/05/02/p9GJKts.png" alt="xlsx" style="width: 600px;" />
+
+- Markdown 结果示例：
+
+  <img src="https://s1.ax1x.com/2023/05/02/p9GYNKf.png" alt="markdown" style="width: 600px;" />
```

### Comparing `starrail-toolkit-0.2.0/setup.py` & `starrail-toolkit-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.2.0/starrail/__init__.py` & `starrail-toolkit-0.3.0/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.2.0/starrail/config.py` & `starrail-toolkit-0.3.0/starrail/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,45 +3,31 @@
 import os
 
 from easydict import EasyDict
 
 userroot = os.path.abspath(os.path.expanduser('~'))
 
 configuration = EasyDict(
-    cache_dir=None,
-    config_path=None,
-    check_update=True,
-)
-
-cli_defaults = EasyDict(
     cache_dir=os.path.join(userroot, '.starrail'),
     config_path=os.path.join(userroot, '.starrail', 'config.json'),
-)
-
-gui_defaults = EasyDict(
-    cache_dir='',
-    config_path='',
+    check_update=True,
 )
 
 
 def export_config(cfg, skip_keys=[]):
     config_path = cfg.config_path
     cfg = copy.deepcopy(cfg)
     for key in skip_keys:
         if key in cfg:
             cfg.pop(key)
     with open(config_path, 'w', encoding='utf-8') as fcfg:
         json.dump(cfg, fcfg, indent=2, ensure_ascii=False)
 
 
-def init_config(cli: bool = False):
-    if cli:
-        configuration.update(cli_defaults)
-    else:
-        configuration.update(gui_defaults)
+def init_config():
 
     os.makedirs(configuration.cache_dir, exist_ok=True)
 
     if os.path.isfile(configuration.config_path):
         with open(configuration.config_path, encoding='utf-8') as fcfg:
             custom_config = json.load(fcfg)
```

### Comparing `starrail-toolkit-0.2.0/starrail/entry/setup.py` & `starrail-toolkit-0.3.0/starrail/entry/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import platform
 
+from starrail.config import init_config
 from starrail.utils.loggings import get_logger, setup_logging
 
 logger = get_logger(__file__)
 
 
 def display_platform_info():
     logger.info(f'PLATFORM:     {platform.platform()}')
     logger.info(f'VERSION:      {platform.version()}')
     logger.info(f'ARCHITECTURE: {platform.architecture()}')
     logger.info(f'MACHINE:      {platform.machine()}')
     logger.info(f'NODE:         {platform.node()}')
     logger.info(f'PROCESSOR:    {platform.processor()}')
     logger.info(f'SYSTEM:       {platform.system()}')
-    logger.info(f'UNAME:        {platform.uname()}')
+    logger.info(f'RELEASE:      {platform.release()}')
 
 
 def display_python_info():
     logger.info(f'PYTHON_BRANCH:         {platform.python_branch()}')
     logger.info(f'PYTHON_BUILD:          {platform.python_build()}')
     logger.info(f'PYTHON_COMPILER:       {platform.python_compiler()}')
     logger.info(f'PYTHON_IMPLEMENTATION: {platform.python_implementation()}')
     logger.info(f'PYTHON_REVISION:       {platform.python_revision()}')
     logger.info(f'PYTHON_VERSION:        {platform.python_version()}')
 
 
-def setup():
-    setup_logging()
+def setup(log_level):
+    setup_logging(log_level)
+    init_config()
     display_platform_info()
     display_python_info()
```

### Comparing `starrail-toolkit-0.2.0/starrail/gacha/database.py` & `starrail-toolkit-0.3.0/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.2.0/starrail/gacha/fetch.py` & `starrail-toolkit-0.3.0/starrail/gacha/fetch.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.2.0/starrail/gacha/fileio.py` & `starrail-toolkit-0.3.0/starrail/gacha/service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,80 +1,104 @@
-import json
+import os
+from datetime import datetime
 
-import pandas as pd
-
-from starrail.gacha.database import DatabaseFactory
+import starrail.gacha.fileio as fileio
+from starrail.gacha.fetch import fetch_json
 from starrail.gacha.parse import GachaDataManager
 from starrail.gacha.type import GachaType
+from starrail.gacha.url import get_api_url, get_url_template
 from starrail.utils import loggings
 
 logger = loggings.get_logger(__file__)
 
 
-def export_as_sql(manager: GachaDataManager, output_path: str) -> None:
-    logger.info(f'Exporting data to cache {output_path}')
-    with DatabaseFactory.get_database(output_path) as db:
-        for gacha_type in GachaType:
-            should_insert = []
-            for entry in manager.gacha[gacha_type.value]:
-                if 'existing' in entry and not entry['existing']:
-                    should_insert.append(entry)
-            logger.info(
-                f'Exporting {gacha_type.name}, '
-                f'totally {len(should_insert)} new items',
-            )
-            rev_insert = reversed(should_insert)
-            for entry in rev_insert:
-                db.add_entry(gacha_type.name, entry)
-
-
-def export_as_json(manager: GachaDataManager, output_path: str) -> None:
-    data_dict = dict()
-    for gacha_type in GachaType:
-        data_dict[gacha_type.name] = manager.gacha[gacha_type.value].tolist()
-    with open(output_path, 'w', encoding='utf-8') as fout:
-        json.dump(data_dict, fout, indent=2, ensure_ascii=False)
-
-
-def export_as_xlsx(manager: GachaDataManager, output_path: str) -> None:
-    with pd.ExcelWriter(output_path) as writer:
-        for gacha_type in GachaType:
-            df = pd.json_normalize(manager.gacha[gacha_type.value].tolist())
-            df.to_excel(writer, sheet_name=gacha_type.name)
+def integers():
+    r = 1
+    while True:
+        yield r
+        r += 1
+
+
+def check_response(payload, code):
+    if payload is None or not 200 <= code < 300:
+        logger.info(f'Whether payload is None: {payload is None}')
+        logger.info(f'Status code: {code}')
+        return False
+    if 'data' not in payload or 'list' not in payload['data']:
+        logger.info(f'Whether payload contains `data`: {"data" in payload}')
+        logger.info(
+            f'Whether payload data contains `list`:'
+            f'{"list" in payload["data"]}',
+        )
+        return False
+    if not payload['data']['list']:
+        logger.info(
+            f'Length of payload.data.list: '
+            f'{len(payload["data"]["list"])}',
+        )
+        return False
+    return True
+
+
+def export_gacha_type(api_template: str, gacha_type: GachaType):
+    r = []
+    end_id = '0'
+    for page in integers():
+        logger.info(f'Downloading page {page} of type {gacha_type.name}')
+        api_url = get_api_url(
+            api_template, end_id, str(gacha_type.value),
+            str(page), '5',
+        )
+        logger.debug(f'Requesting {api_url}')
+        response, code = fetch_json(api_url)
+        if not check_response(response, code):
+            break
+        data_list = response['data']['list']
+        r.extend(data_list)
+        end_id = data_list[-1]['id']
+    return r
+
+
+def export_gacha_from_api(api_url, export):
+    assert api_url, 'API URL should be provided, auto-detect is coming soon'
+    response, code = fetch_json(api_url)
+    valid = check_response(response, code)
+    if not valid:
+        logger.fatal('Error while checking response from api URL, exitting')
+        raise ValueError('Invalid api URL, please check your input')
+
+    api_template = get_url_template(api_url)
+
+    uid = response['data']['list'][0]['uid']
+    manager = GachaDataManager(uid)
+    logger.info(f'Successfully connected to cache of uid {uid}')
+    manager.log_stats()
 
-
-def export_as_csv(manager: GachaDataManager, output_path: str) -> None:
-    data_list = []
-    for gacha_type in GachaType:
-        data_list.extend(manager.gacha[gacha_type.value].tolist())
-    df = pd.json_normalize(data_list)
-    df.to_csv(output_path, encoding='utf-8')
-
-
-def export_as_md(manager: GachaDataManager, output_path: str) -> None:
-    md = '# Gacha Report\n\n'
     for gacha_type in GachaType:
-        md += f'## {gacha_type.name}\n\n'
-        md += '| Type | Count | Basic Prob. | True Prob. | Since Last |\n'
-        md += '| ---- | ----- | ----------- | ---------- | ---------- |\n'
-        stats = manager.gacha[gacha_type.value].stats
-        for item in stats:
-            rtype = item['rank_type']
-            count = item['count']
-            basic = item['basic_prob']
-            compr = item['compr_prob']
-            since_last = item['since_last']
-            md += f'|{rtype}|{count}|{basic}|{compr}|{since_last}|\n'
-        md += '\n'
-        if stats[0]['attempts']:
-            attempt_string = ' '.join(stats[0]['attempts'])
-            average = stats[0]['average']
-            md += 'History of 5-star gacha attempts: '
-            md += f'**{attempt_string}**'
-            md += '\n\n'
-            md += f'Average gacha per 5-star: **{average}**\n\n'
-    with open(output_path, 'w', encoding='utf-8') as fout:
-        fout.write(md)
-
-
-def export_as_html(manager: GachaDataManager, output_path: str) -> None:
-    raise NotImplementedError
+        records = export_gacha_type(api_template, gacha_type)
+        manager.add_records(gacha_type.value, records)
+        manager.gacha[gacha_type.value].sort()
+        logger.info(f'Finish downloading records of {gacha_type.name}')
+
+    fileio.export_as_sql(manager, manager.cache_path)
+
+    manager.log_stats()
+
+    export_hooks = dict(
+        csv=fileio.export_as_csv,
+        html=fileio.export_as_html,
+        json=fileio.export_as_json,
+        md=fileio.export_as_md,
+        xlsx=fileio.export_as_xlsx,
+    )
+    if 'all' in export:
+        export = ['csv', 'html', 'json', 'md', 'xlsx']
+
+    timestamp = datetime.now().strftime('%Y%m%d%H%M%S')
+
+    for format in export:
+        logger.info(f'Exporting gacha data as {format} format')
+        output_dir = os.getcwd()
+        filename = f'HKSR-export-{uid}-{timestamp}.{format}'
+        path = os.path.join(output_dir, filename)
+        export_hooks[format](manager, path)
+        logger.info(f'Gacha data in {format} format is saved to {path}')
```

### Comparing `starrail-toolkit-0.2.0/starrail/gacha/parse.py` & `starrail-toolkit-0.3.0/starrail/gacha/parse.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.2.0/starrail/gacha/url.py` & `starrail-toolkit-0.3.0/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.2.0/starrail/utils/loggings.py` & `starrail-toolkit-0.3.0/starrail/utils/loggings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 import os
 
 from starrail import package_path
 
 
-def setup_logging():
+def setup_logging(log_level):
     format = (
         '%(asctime)s %(name)s Line %(lineno)d - '
         '[%(levelname)s] %(message)s'
     )
     formatter = logging.Formatter(format)
 
     stream = logging.StreamHandler()
     stream.setFormatter(formatter)
     logging.getLogger().addHandler(stream)
-    logging.getLogger().setLevel(logging.DEBUG)
+    logging.getLogger().setLevel(log_level)
 
 
 def get_logger(name):
     if name and os.path.isfile(name):
         name = os.path.relpath(name, package_path)
     return logging.getLogger(name)
```

