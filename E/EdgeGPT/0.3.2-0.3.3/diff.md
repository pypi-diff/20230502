# Comparing `tmp/EdgeGPT-0.3.2.tar.gz` & `tmp/EdgeGPT-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.3.2.tar", last modified: Sat Apr 29 13:41:32 2023, max compression
+gzip compressed data, was "EdgeGPT-0.3.3.tar", last modified: Tue May  2 02:47:17 2023, max compression
```

## Comparing `EdgeGPT-0.3.2.tar` & `EdgeGPT-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:41:32.422943 EdgeGPT-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-29 13:40:56.000000 EdgeGPT-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-29 13:41:32.422943 EdgeGPT-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-29 13:41:32.422943 EdgeGPT-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-29 13:40:56.000000 EdgeGPT-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:41:32.422943 EdgeGPT-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:41:32.422943 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22288 2023-04-29 13:40:56.000000 EdgeGPT-0.3.2/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-29 13:40:56.000000 EdgeGPT-0.3.2/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:47:17.171166 EdgeGPT-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 02:46:47.000000 EdgeGPT-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-02 02:47:17.171166 EdgeGPT-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-02 02:47:16.000000 EdgeGPT-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 02:47:17.171166 EdgeGPT-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 02:46:47.000000 EdgeGPT-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:47:17.171166 EdgeGPT-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:47:17.171166 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-02 02:47:17.000000 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 02:47:17.000000 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 02:47:17.000000 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 02:47:17.000000 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-02 02:47:17.000000 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 02:47:17.000000 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25243 2023-05-02 02:46:47.000000 EdgeGPT-0.3.3/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 02:46:47.000000 EdgeGPT-0.3.3/src/ImageGen.py
```

### Comparing `EdgeGPT-0.3.2/LICENSE` & `EdgeGPT-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.2/PKG-INFO` & `EdgeGPT-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.2
+Version: 0.3.3
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -21,15 +21,16 @@
   <img src="https://socialify.git.ci/acheong08/EdgeGPT/image?font=Inter&language=1&logo=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F9%2F9c%2FBing_Fluent_Logo.svg&owner=1&pattern=Floating%20Cogs&theme=Auto" alt="EdgeGPT" width="640" height="320" />
 
 # Edge GPT
 
 _The reverse engineering the chat feature of the new version of Bing_
 
 <a>English</a> -
-<a href="./README_zh.md">中文</a> -
+<a href="./README_zh-cn.md">简体中文</a> -
+<a href="./README_zh-tw.md">繁體中文 (中國臺灣)</a> -
 <a href="./README_es.md">Español</a> -
 <a href="./README_ja.md">日本語</a>
 
 </div>
 
 <p align="center">
   <a href="https://github.com/acheong08/EdgeGPT">
@@ -147,35 +148,35 @@
 
 Three ways to pass in cookies:
 
 - Environment variable: `export COOKIE_FILE=/path/to/cookies.json`.
 - Specify the path to `cookies.json` in the argument `cookie_path` like this:
 
   ```python
-  bot = Chatbot(cookie_path='./cookies.json')
+  bot = await Chatbot.create(cookie_path='./cookies.json')
   ```
 
 - Pass in the cookies directly by the argument `cookies`, like this:
 
   ```python
   with open('./cookies.json', 'r') as f:
       cookies = json.load(f)
-  bot = Chatbot(cookies=cookies)
+  bot = await Chatbot.create(cookies=cookies)
   ```
 
 Use Async for the best experience
 
 Reference code for more advanced example of usage:
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
-    bot = Chatbot()
+    bot = await Chatbot.create()
     print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/sydney/ChatHub"))
     await bot.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.2 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.3 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
-           version of Bing_ English - ä¸­æ - EspaÃ±ol - æ¥æ¬èª
+    version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ_(ä¸­åèºç£) -
+                             EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
 bing.com/chat> (Required) - Required in a supported country with New Bing
 (Chinese mainland VPN required)   ### Checking access (Required)  - Install the
 latest version of Microsoft Edge - Alternatively, you can use any browser and
@@ -44,46 +45,47 @@
 have a file cookies.json in your current working directory ``` bash docker run
 --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json'
 ghcr.io/acheong08/edgegpt ``` You can add any extra flags as following ``` bash
 docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
 cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative ``` ###
 Developer demo Three ways to pass in cookies: - Environment variable: `export
 COOKIE_FILE=/path/to/cookies.json`. - Specify the path to `cookies.json` in the
-argument `cookie_path` like this: ```python bot = Chatbot(cookie_path='./
-cookies.json') ``` - Pass in the cookies directly by the argument `cookies`,
-like this: ```python with open('./cookies.json', 'r') as f: cookies = json.load
-(f) bot = Chatbot(cookies=cookies) ``` Use Async for the best experience
-Reference code for more advanced example of usage: ```python import asyncio
-from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = Chatbot
-() print(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/
-sydney/ChatHub")) await bot.close() if __name__ == "__main__": asyncio.run(main
-()) ```    ## Image generator  ```bash $ python3 -m ImageGen -h usage:
-ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --prompt PROMPT [--output-
-dir OUTPUT_DIR] [--quiet] [--asyncio] optional arguments: -h, --help show this
-help message and exit -U U Auth cookie from browser --cookie-file COOKIE_FILE
-File containing auth cookie --prompt PROMPT Prompt to generate images for --
-output-dir OUTPUT_DIR Output directory --quiet Disable pipeline messages --
-asyncio Run ImageGen using asyncio ``` ### Developer demo ```python from
-ImageGen import ImageGen import argparse import json async def async_image_gen
-(args) -> None: async with ImageGenAsync(args.U, args.quiet) as
-image_generator: images = await image_generator.get_images(args.prompt) await
-image_generator.save_images(images, output_dir=args.output_dir) if __name__ ==
-"__main__": parser = argparse.ArgumentParser() parser.add_argument("-U",
-help="Auth cookie from browser", type=str) parser.add_argument("--cookie-file",
-help="File containing auth cookie", type=str) parser.add_argument( "--prompt",
-help="Prompt to generate images for", type=str, required=True, )
-parser.add_argument( "--output-dir", help="Output directory", type=str,
-default="./output", ) parser.add_argument( "--quiet", help="Disable pipeline
-messages", action="store_true" ) parser.add_argument( "--asyncio", help="Run
-ImageGen using asyncio", action="store_true" ) args = parser.parse_args() #
-Load auth cookie with open(args.cookie_file, encoding="utf-8") as file:
-cookie_json = json.load(file) for cookie in cookie_json: if cookie.get("name")
-== "_U": args.U = cookie.get("value") break if args.U is None: raise Exception
-("Could not find auth cookie") if not args.asyncio: # Create image generator
+argument `cookie_path` like this: ```python bot = await Chatbot.create
+(cookie_path='./cookies.json') ``` - Pass in the cookies directly by the
+argument `cookies`, like this: ```python with open('./cookies.json', 'r') as f:
+cookies = json.load(f) bot = await Chatbot.create(cookies=cookies) ``` Use
+Async for the best experience Reference code for more advanced example of
+usage: ```python import asyncio from EdgeGPT import Chatbot, ConversationStyle
+async def main(): bot = await Chatbot.create() print(await bot.ask
+(prompt="Hello world", conversation_style=ConversationStyle.creative,
+wss_link="wss://sydney.bing.com/sydney/ChatHub")) await bot.close() if __name__
+== "__main__": asyncio.run(main()) ```    ## Image generator  ```bash $ python3
+-m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --
+prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio] optional
+arguments: -h, --help show this help message and exit -U U Auth cookie from
+browser --cookie-file COOKIE_FILE File containing auth cookie --prompt PROMPT
+Prompt to generate images for --output-dir OUTPUT_DIR Output directory --quiet
+Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ###
+Developer demo ```python from ImageGen import ImageGen import argparse import
+json async def async_image_gen(args) -> None: async with ImageGenAsync(args.U,
+args.quiet) as image_generator: images = await image_generator.get_images
+(args.prompt) await image_generator.save_images(images,
+output_dir=args.output_dir) if __name__ == "__main__": parser =
+argparse.ArgumentParser() parser.add_argument("-U", help="Auth cookie from
+browser", type=str) parser.add_argument("--cookie-file", help="File containing
+auth cookie", type=str) parser.add_argument( "--prompt", help="Prompt to
+generate images for", type=str, required=True, ) parser.add_argument( "--
+output-dir", help="Output directory", type=str, default="./output", )
+parser.add_argument( "--quiet", help="Disable pipeline messages",
+action="store_true" ) parser.add_argument( "--asyncio", help="Run ImageGen
+using asyncio", action="store_true" ) args = parser.parse_args() # Load auth
+cookie with open(args.cookie_file, encoding="utf-8") as file: cookie_json =
+json.load(file) for cookie in cookie_json: if cookie.get("name") == "_U":
+args.U = cookie.get("value") break if args.U is None: raise Exception("Could
+not find auth cookie") if not args.asyncio: # Create image generator
 image_generator = ImageGen(args.U, args.quiet) image_generator.save_images
 ( image_generator.get_images(args.prompt), output_dir=args.output_dir, ) else:
 asyncio.run(async_image_gen(args)) ```  ## Star History [![Star History Chart]
 (https://api.star-history.com/svg?repos=acheong08/EdgeGPT&type=Date)](https://
 star-history.com/#acheong08/EdgeGPT&Date) ## Contributors This project exists
 thanks to all the people who contribute. [https://contrib.rocks/
 image?repo=acheong08/EdgeGPT]
```

### Comparing `EdgeGPT-0.3.2/README.md` & `EdgeGPT-0.3.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
   <img src="https://socialify.git.ci/acheong08/EdgeGPT/image?font=Inter&language=1&logo=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F9%2F9c%2FBing_Fluent_Logo.svg&owner=1&pattern=Floating%20Cogs&theme=Auto" alt="EdgeGPT" width="640" height="320" />
 
 # Edge GPT
 
 _The reverse engineering the chat feature of the new version of Bing_
 
 <a>English</a> -
-<a href="./README_zh.md">中文</a> -
+<a href="./README_zh-cn.md">简体中文</a> -
+<a href="./README_zh-tw.md">繁體中文 (中國臺灣)</a> -
 <a href="./README_es.md">Español</a> -
 <a href="./README_ja.md">日本語</a>
 
 </div>
 
 <p align="center">
   <a href="https://github.com/acheong08/EdgeGPT">
@@ -128,35 +129,35 @@
 
 Three ways to pass in cookies:
 
 - Environment variable: `export COOKIE_FILE=/path/to/cookies.json`.
 - Specify the path to `cookies.json` in the argument `cookie_path` like this:
 
   ```python
-  bot = Chatbot(cookie_path='./cookies.json')
+  bot = await Chatbot.create(cookie_path='./cookies.json')
   ```
 
 - Pass in the cookies directly by the argument `cookies`, like this:
 
   ```python
   with open('./cookies.json', 'r') as f:
       cookies = json.load(f)
-  bot = Chatbot(cookies=cookies)
+  bot = await Chatbot.create(cookies=cookies)
   ```
 
 Use Async for the best experience
 
 Reference code for more advanced example of usage:
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
-    bot = Chatbot()
+    bot = await Chatbot.create()
     print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/sydney/ChatHub"))
     await bot.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
-           version of Bing_ English - ä¸­æ - EspaÃ±ol - æ¥æ¬èª
+    version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ_(ä¸­åèºç£) -
+                             EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
 bing.com/chat> (Required) - Required in a supported country with New Bing
 (Chinese mainland VPN required)   ### Checking access (Required)  - Install the
 latest version of Microsoft Edge - Alternatively, you can use any browser and
@@ -34,46 +35,47 @@
 have a file cookies.json in your current working directory ``` bash docker run
 --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json'
 ghcr.io/acheong08/edgegpt ``` You can add any extra flags as following ``` bash
 docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
 cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative ``` ###
 Developer demo Three ways to pass in cookies: - Environment variable: `export
 COOKIE_FILE=/path/to/cookies.json`. - Specify the path to `cookies.json` in the
-argument `cookie_path` like this: ```python bot = Chatbot(cookie_path='./
-cookies.json') ``` - Pass in the cookies directly by the argument `cookies`,
-like this: ```python with open('./cookies.json', 'r') as f: cookies = json.load
-(f) bot = Chatbot(cookies=cookies) ``` Use Async for the best experience
-Reference code for more advanced example of usage: ```python import asyncio
-from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = Chatbot
-() print(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/
-sydney/ChatHub")) await bot.close() if __name__ == "__main__": asyncio.run(main
-()) ```    ## Image generator  ```bash $ python3 -m ImageGen -h usage:
-ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --prompt PROMPT [--output-
-dir OUTPUT_DIR] [--quiet] [--asyncio] optional arguments: -h, --help show this
-help message and exit -U U Auth cookie from browser --cookie-file COOKIE_FILE
-File containing auth cookie --prompt PROMPT Prompt to generate images for --
-output-dir OUTPUT_DIR Output directory --quiet Disable pipeline messages --
-asyncio Run ImageGen using asyncio ``` ### Developer demo ```python from
-ImageGen import ImageGen import argparse import json async def async_image_gen
-(args) -> None: async with ImageGenAsync(args.U, args.quiet) as
-image_generator: images = await image_generator.get_images(args.prompt) await
-image_generator.save_images(images, output_dir=args.output_dir) if __name__ ==
-"__main__": parser = argparse.ArgumentParser() parser.add_argument("-U",
-help="Auth cookie from browser", type=str) parser.add_argument("--cookie-file",
-help="File containing auth cookie", type=str) parser.add_argument( "--prompt",
-help="Prompt to generate images for", type=str, required=True, )
-parser.add_argument( "--output-dir", help="Output directory", type=str,
-default="./output", ) parser.add_argument( "--quiet", help="Disable pipeline
-messages", action="store_true" ) parser.add_argument( "--asyncio", help="Run
-ImageGen using asyncio", action="store_true" ) args = parser.parse_args() #
-Load auth cookie with open(args.cookie_file, encoding="utf-8") as file:
-cookie_json = json.load(file) for cookie in cookie_json: if cookie.get("name")
-== "_U": args.U = cookie.get("value") break if args.U is None: raise Exception
-("Could not find auth cookie") if not args.asyncio: # Create image generator
+argument `cookie_path` like this: ```python bot = await Chatbot.create
+(cookie_path='./cookies.json') ``` - Pass in the cookies directly by the
+argument `cookies`, like this: ```python with open('./cookies.json', 'r') as f:
+cookies = json.load(f) bot = await Chatbot.create(cookies=cookies) ``` Use
+Async for the best experience Reference code for more advanced example of
+usage: ```python import asyncio from EdgeGPT import Chatbot, ConversationStyle
+async def main(): bot = await Chatbot.create() print(await bot.ask
+(prompt="Hello world", conversation_style=ConversationStyle.creative,
+wss_link="wss://sydney.bing.com/sydney/ChatHub")) await bot.close() if __name__
+== "__main__": asyncio.run(main()) ```    ## Image generator  ```bash $ python3
+-m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --
+prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio] optional
+arguments: -h, --help show this help message and exit -U U Auth cookie from
+browser --cookie-file COOKIE_FILE File containing auth cookie --prompt PROMPT
+Prompt to generate images for --output-dir OUTPUT_DIR Output directory --quiet
+Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ###
+Developer demo ```python from ImageGen import ImageGen import argparse import
+json async def async_image_gen(args) -> None: async with ImageGenAsync(args.U,
+args.quiet) as image_generator: images = await image_generator.get_images
+(args.prompt) await image_generator.save_images(images,
+output_dir=args.output_dir) if __name__ == "__main__": parser =
+argparse.ArgumentParser() parser.add_argument("-U", help="Auth cookie from
+browser", type=str) parser.add_argument("--cookie-file", help="File containing
+auth cookie", type=str) parser.add_argument( "--prompt", help="Prompt to
+generate images for", type=str, required=True, ) parser.add_argument( "--
+output-dir", help="Output directory", type=str, default="./output", )
+parser.add_argument( "--quiet", help="Disable pipeline messages",
+action="store_true" ) parser.add_argument( "--asyncio", help="Run ImageGen
+using asyncio", action="store_true" ) args = parser.parse_args() # Load auth
+cookie with open(args.cookie_file, encoding="utf-8") as file: cookie_json =
+json.load(file) for cookie in cookie_json: if cookie.get("name") == "_U":
+args.U = cookie.get("value") break if args.U is None: raise Exception("Could
+not find auth cookie") if not args.asyncio: # Create image generator
 image_generator = ImageGen(args.U, args.quiet) image_generator.save_images
 ( image_generator.get_images(args.prompt), output_dir=args.output_dir, ) else:
 asyncio.run(async_image_gen(args)) ```  ## Star History [![Star History Chart]
 (https://api.star-history.com/svg?repos=acheong08/EdgeGPT&type=Date)](https://
 star-history.com/#acheong08/EdgeGPT&Date) ## Contributors This project exists
 thanks to all the people who contribute. [https://contrib.rocks/
 image?repo=acheong08/EdgeGPT]
```

### Comparing `EdgeGPT-0.3.2/setup.py` & `EdgeGPT-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.3.2",
+    version="0.3.3",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.3.2/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.3.3/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.2
+Version: 0.3.3
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -21,15 +21,16 @@
   <img src="https://socialify.git.ci/acheong08/EdgeGPT/image?font=Inter&language=1&logo=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F9%2F9c%2FBing_Fluent_Logo.svg&owner=1&pattern=Floating%20Cogs&theme=Auto" alt="EdgeGPT" width="640" height="320" />
 
 # Edge GPT
 
 _The reverse engineering the chat feature of the new version of Bing_
 
 <a>English</a> -
-<a href="./README_zh.md">中文</a> -
+<a href="./README_zh-cn.md">简体中文</a> -
+<a href="./README_zh-tw.md">繁體中文 (中國臺灣)</a> -
 <a href="./README_es.md">Español</a> -
 <a href="./README_ja.md">日本語</a>
 
 </div>
 
 <p align="center">
   <a href="https://github.com/acheong08/EdgeGPT">
@@ -147,35 +148,35 @@
 
 Three ways to pass in cookies:
 
 - Environment variable: `export COOKIE_FILE=/path/to/cookies.json`.
 - Specify the path to `cookies.json` in the argument `cookie_path` like this:
 
   ```python
-  bot = Chatbot(cookie_path='./cookies.json')
+  bot = await Chatbot.create(cookie_path='./cookies.json')
   ```
 
 - Pass in the cookies directly by the argument `cookies`, like this:
 
   ```python
   with open('./cookies.json', 'r') as f:
       cookies = json.load(f)
-  bot = Chatbot(cookies=cookies)
+  bot = await Chatbot.create(cookies=cookies)
   ```
 
 Use Async for the best experience
 
 Reference code for more advanced example of usage:
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
-    bot = Chatbot()
+    bot = await Chatbot.create()
     print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/sydney/ChatHub"))
     await bot.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.2 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.3 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
-           version of Bing_ English - ä¸­æ - EspaÃ±ol - æ¥æ¬èª
+    version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ_(ä¸­åèºç£) -
+                             EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
 bing.com/chat> (Required) - Required in a supported country with New Bing
 (Chinese mainland VPN required)   ### Checking access (Required)  - Install the
 latest version of Microsoft Edge - Alternatively, you can use any browser and
@@ -44,46 +45,47 @@
 have a file cookies.json in your current working directory ``` bash docker run
 --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json'
 ghcr.io/acheong08/edgegpt ``` You can add any extra flags as following ``` bash
 docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
 cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative ``` ###
 Developer demo Three ways to pass in cookies: - Environment variable: `export
 COOKIE_FILE=/path/to/cookies.json`. - Specify the path to `cookies.json` in the
-argument `cookie_path` like this: ```python bot = Chatbot(cookie_path='./
-cookies.json') ``` - Pass in the cookies directly by the argument `cookies`,
-like this: ```python with open('./cookies.json', 'r') as f: cookies = json.load
-(f) bot = Chatbot(cookies=cookies) ``` Use Async for the best experience
-Reference code for more advanced example of usage: ```python import asyncio
-from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = Chatbot
-() print(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/
-sydney/ChatHub")) await bot.close() if __name__ == "__main__": asyncio.run(main
-()) ```    ## Image generator  ```bash $ python3 -m ImageGen -h usage:
-ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --prompt PROMPT [--output-
-dir OUTPUT_DIR] [--quiet] [--asyncio] optional arguments: -h, --help show this
-help message and exit -U U Auth cookie from browser --cookie-file COOKIE_FILE
-File containing auth cookie --prompt PROMPT Prompt to generate images for --
-output-dir OUTPUT_DIR Output directory --quiet Disable pipeline messages --
-asyncio Run ImageGen using asyncio ``` ### Developer demo ```python from
-ImageGen import ImageGen import argparse import json async def async_image_gen
-(args) -> None: async with ImageGenAsync(args.U, args.quiet) as
-image_generator: images = await image_generator.get_images(args.prompt) await
-image_generator.save_images(images, output_dir=args.output_dir) if __name__ ==
-"__main__": parser = argparse.ArgumentParser() parser.add_argument("-U",
-help="Auth cookie from browser", type=str) parser.add_argument("--cookie-file",
-help="File containing auth cookie", type=str) parser.add_argument( "--prompt",
-help="Prompt to generate images for", type=str, required=True, )
-parser.add_argument( "--output-dir", help="Output directory", type=str,
-default="./output", ) parser.add_argument( "--quiet", help="Disable pipeline
-messages", action="store_true" ) parser.add_argument( "--asyncio", help="Run
-ImageGen using asyncio", action="store_true" ) args = parser.parse_args() #
-Load auth cookie with open(args.cookie_file, encoding="utf-8") as file:
-cookie_json = json.load(file) for cookie in cookie_json: if cookie.get("name")
-== "_U": args.U = cookie.get("value") break if args.U is None: raise Exception
-("Could not find auth cookie") if not args.asyncio: # Create image generator
+argument `cookie_path` like this: ```python bot = await Chatbot.create
+(cookie_path='./cookies.json') ``` - Pass in the cookies directly by the
+argument `cookies`, like this: ```python with open('./cookies.json', 'r') as f:
+cookies = json.load(f) bot = await Chatbot.create(cookies=cookies) ``` Use
+Async for the best experience Reference code for more advanced example of
+usage: ```python import asyncio from EdgeGPT import Chatbot, ConversationStyle
+async def main(): bot = await Chatbot.create() print(await bot.ask
+(prompt="Hello world", conversation_style=ConversationStyle.creative,
+wss_link="wss://sydney.bing.com/sydney/ChatHub")) await bot.close() if __name__
+== "__main__": asyncio.run(main()) ```    ## Image generator  ```bash $ python3
+-m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --
+prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio] optional
+arguments: -h, --help show this help message and exit -U U Auth cookie from
+browser --cookie-file COOKIE_FILE File containing auth cookie --prompt PROMPT
+Prompt to generate images for --output-dir OUTPUT_DIR Output directory --quiet
+Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ###
+Developer demo ```python from ImageGen import ImageGen import argparse import
+json async def async_image_gen(args) -> None: async with ImageGenAsync(args.U,
+args.quiet) as image_generator: images = await image_generator.get_images
+(args.prompt) await image_generator.save_images(images,
+output_dir=args.output_dir) if __name__ == "__main__": parser =
+argparse.ArgumentParser() parser.add_argument("-U", help="Auth cookie from
+browser", type=str) parser.add_argument("--cookie-file", help="File containing
+auth cookie", type=str) parser.add_argument( "--prompt", help="Prompt to
+generate images for", type=str, required=True, ) parser.add_argument( "--
+output-dir", help="Output directory", type=str, default="./output", )
+parser.add_argument( "--quiet", help="Disable pipeline messages",
+action="store_true" ) parser.add_argument( "--asyncio", help="Run ImageGen
+using asyncio", action="store_true" ) args = parser.parse_args() # Load auth
+cookie with open(args.cookie_file, encoding="utf-8") as file: cookie_json =
+json.load(file) for cookie in cookie_json: if cookie.get("name") == "_U":
+args.U = cookie.get("value") break if args.U is None: raise Exception("Could
+not find auth cookie") if not args.asyncio: # Create image generator
 image_generator = ImageGen(args.U, args.quiet) image_generator.save_images
 ( image_generator.get_images(args.prompt), output_dir=args.output_dir, ) else:
 asyncio.run(async_image_gen(args)) ```  ## Star History [![Star History Chart]
 (https://api.star-history.com/svg?repos=acheong08/EdgeGPT&type=Date)](https://
 star-history.com/#acheong08/EdgeGPT&Date) ## Contributors This project exists
 thanks to all the people who contribute. [https://contrib.rocks/
 image?repo=acheong08/EdgeGPT]
```

### Comparing `EdgeGPT-0.3.2/src/EdgeGPT.py` & `EdgeGPT-0.3.3/src/EdgeGPT.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,28 +108,30 @@
         "gencontentv3",
         "dv3sugg",
         "responseos",
         "e2ecachewrite",
         "cachewriteext",
         "nodlcpcwrite",
         "travelansgnd",
+        "nojbfedge",
     ]
     balanced = [
         "nlu_direct_response_filter",
         "deepleo",
         "disable_emoji_spoken_text",
         "responsible_ai_policy_235",
         "enablemm",
         "galileo",
         "dv3sugg",
         "responseos",
         "e2ecachewrite",
         "cachewriteext",
         "nodlcpcwrite",
         "travelansgnd",
+        "nojbfedge",
     ]
     precise = [
         "nlu_direct_response_filter",
         "deepleo",
         "disable_emoji_spoken_text",
         "responsible_ai_policy_235",
         "enablemm",
@@ -138,14 +140,15 @@
         "responseos",
         "e2ecachewrite",
         "cachewriteext",
         "nodlcpcwrite",
         "travelansgnd",
         "h3precise",
         "clgalileo",
+        "nojbfedge",
     ]
 
 
 CONVERSATION_STYLE_TYPE = Optional[
     Union[ConversationStyle, Literal["creative", "balanced", "precise"]]
 ]
 
@@ -185,14 +188,15 @@
         self.invocation_id: int = invocation_id
 
     def update(
         self,
         prompt: str,
         conversation_style: CONVERSATION_STYLE_TYPE,
         options: list | None = None,
+        webpage_context: str | None = None
     ) -> None:
         """
         Updates request object
         """
         if options is None:
             options = [
                 "deepleo",
@@ -252,28 +256,37 @@
                     "conversationId": self.conversation_id,
                 },
             ],
             "invocationId": str(self.invocation_id),
             "target": "chat",
             "type": 4,
         }
+        if webpage_context:
+            self.struct["arguments"][0]["previousMessages"] = [{
+                "author": 'user',
+                "description": webpage_context,
+                "contextType": 'WebPage',
+                "messageType": 'Context',
+                "messageId": 'discover-web--page-ping-mriduna-----',
+            }]
         self.invocation_id += 1
 
 
 class _Conversation:
     """
     Conversation API
     """
 
-    def __init__(
-        self,
+    @staticmethod
+    async def create(
         cookies: dict,
         proxy: str | None = None,
     ) -> None:
-        self.struct: dict = {
+        self = _Conversation()
+        self.struct = {
             "conversationId": None,
             "clientId": None,
             "conversationSignature": None,
             "result": {"value": "Success", "message": None},
         }
         self.proxy = proxy
         proxy = (
@@ -282,44 +295,45 @@
             or os.environ.get("ALL_PROXY")
             or os.environ.get("https_proxy")
             or os.environ.get("HTTPS_PROXY")
             or None
         )
         if proxy is not None and proxy.startswith("socks5h://"):
             proxy = "socks5://" + proxy[len("socks5h://") :]
-        self.session = httpx.Client(
+        async with httpx.AsyncClient(
             proxies=proxy,
             timeout=30,
             headers=HEADERS_INIT_CONVER,
-        )
-        for cookie in cookies:
-            self.session.cookies.set(cookie["name"], cookie["value"])
-
-        # Send GET request
-        response = self.session.get(
-            url=os.environ.get("BING_PROXY_URL")
-            or "https://edgeservices.bing.com/edgesvc/turing/conversation/create",
-        )
-        if response.status_code != 200:
-            response = self.session.get(
-                "https://edge.churchless.tech/edgesvc/turing/conversation/create",
+        ) as client:
+            for cookie in cookies:
+                client.cookies.set(cookie["name"], cookie["value"])
+
+            # Send GET request
+            response = await client.get(
+                url = os.environ.get("BING_PROXY_URL")
+                or "https://edgeservices.bing.com/edgesvc/turing/conversation/create",
             )
+            if response.status_code != 200:
+                response = await client.get(
+                    "https://edge.churchless.tech/edgesvc/turing/conversation/create",
+                )
         if response.status_code != 200:
             print(f"Status code: {response.status_code}")
             print(response.text)
             print(response.url)
             raise Exception("Authentication failed")
         try:
             self.struct = response.json()
         except (json.decoder.JSONDecodeError, NotAllowedToAccess) as exc:
             raise Exception(
                 "Authentication failed. You have not been accepted into the beta.",
             ) from exc
         if self.struct["result"]["value"] == "UnauthorizedRequest":
             raise NotAllowedToAccess(self.struct["result"]["message"])
+        return self
 
 
 class _ChatHub:
     """
     Chat API
     """
 
@@ -338,56 +352,94 @@
         self,
         prompt: str,
         wss_link: str,
         cookies: str,
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
+        webpage_context: str | None = None
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         if self.wss and not self.wss.closed:
             await self.wss.close()
         # Check if websocket is closed
         self.wss = await websockets.connect(
             wss_link,
             extra_headers=HEADERS,
             max_size=None,
             ssl=ssl_context,
         )
         await self._initial_handshake()
-        # Construct a ChatHub request
-        self.request.update(
-            prompt=prompt,
-            conversation_style=conversation_style,
-            options=options,
-        )
+        if self.request.invocation_id == 0:
+            # Construct a ChatHub request
+            self.request.update(
+                prompt=prompt,
+                conversation_style=conversation_style,
+                options=options,
+                webpage_context=webpage_context,
+            )
+        else:
+            async with httpx.AsyncClient() as client:
+                response = await client.post(
+                    'https://sydney.bing.com/sydney/UpdateConversation/',
+                    json={
+                        "messages": [
+                            {
+                                "author": "user",
+                                "description": webpage_context,
+                                "contextType": "WebPage",
+                                "messageType": "Context"
+                            }
+                        ],
+                        "conversationId": self.request.conversation_id,
+                        "source": "cib",
+                        "traceId": _get_ran_hex(32),
+                        "participant": {
+                            "id": self.request.client_id
+                        },
+                        "conversationSignature": self.request.conversation_signature
+                    }
+                )
+            if response.status_code != 200:
+                print(f"Status code: {response.status_code}")
+                print(response.text)
+                print(response.url)
+                raise Exception("Update web page context failed")
+            # Construct a ChatHub request
+            self.request.update(
+                prompt=prompt,
+                conversation_style=conversation_style,
+                options=options,
+            )
         # Send request
         await self.wss.send(_append_identifier(self.request.struct))
         final = False
         draw = False
+        resp_txt = ''
+        resp_txt_no_link = ''
         while not final:
             objects = str(await self.wss.recv()).split(DELIMITER)
             for obj in objects:
                 if obj is None or not obj:
                     continue
                 response = json.loads(obj)
                 if response.get("type") != 2 and raw:
                     yield False, response
                 elif response.get("type") == 1 and response["arguments"][0].get(
                     "messages",
                 ):
                     try:
                         if not draw:
-                            resp_txt = response["arguments"][0]["messages"][0][
-                                "adaptiveCards"
-                            ][0]["body"][0].get("text")
-                            if resp_txt is None:
-                                resp_txt = ""
+                            if response["arguments"][0]["messages"][0]["contentOrigin"] != "Apology":
+                                resp_txt = response["arguments"][0]["messages"][0][
+                                    "adaptiveCards"
+                                ][0]["body"][0].get("text", '')
+                                resp_txt_no_link = response["arguments"][0]["messages"][0].get("text", '')
                         yield False, resp_txt
                     except Exception as exc:
                         print(exc)
                         if not draw:
                             continue
                         for item in cookies:
                             if item["name"] == "_U":
@@ -414,14 +466,18 @@
                     if draw:
                         cache = response["item"]["messages"][1]["adaptiveCards"][0][
                             "body"
                         ][0]["text"]
                         response["item"]["messages"][1]["adaptiveCards"][0]["body"][0][
                             "text"
                         ] = (cache + resp_txt)
+                    if response["item"]["messages"][-1]["contentOrigin"] == "Apology" and resp_txt:
+                        response["item"]["messages"][-1]["text"] = resp_txt_no_link
+                        response["item"]["messages"][-1]["adaptiveCards"][0]["body"][0]["text"] = resp_txt
+                        print(f"Preserved the message from being deleted", file=sys.stderr)
                     final = True
                     yield True, response
 
     async def _initial_handshake(self) -> None:
         await self.wss.send(_append_identifier({"protocol": "json", "version": 1}))
         await self.wss.recv()
 
@@ -434,90 +490,96 @@
 
 
 class Chatbot:
     """
     Combines everything to make it seamless
     """
 
-    def __init__(
-        self,
+    @staticmethod
+    async def create(
         cookies: dict = None,
         proxy: str | None = None,
         cookie_path: str = None,
-    ) -> None:
+    ):
+        self = Chatbot()
         if cookies is None:
             cookies = {}
         if cookie_path is not None:
             try:
                 with open(cookie_path, encoding="utf-8") as f:
                     self.cookies = json.load(f)
             except FileNotFoundError as exc:
                 raise FileNotFoundError("Cookie file not found") from exc
         else:
             self.cookies = cookies
-        self.proxy: str | None = proxy
-        self.chat_hub: _ChatHub = _ChatHub(
-            _Conversation(self.cookies, self.proxy),
+        self.proxy = proxy
+        self.chat_hub = _ChatHub(
+            await _Conversation.create(self.cookies, self.proxy),
         )
+        return self
 
     async def ask(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         options: dict = None,
+        webpage_context: str | None = None,
     ) -> dict:
         """
         Ask a question to the bot
         """
         async for final, response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             options=options,
             cookies=self.cookies,
+            webpage_context=webpage_context
         ):
             if final:
                 return response
         await self.chat_hub.wss.close()
         return None
 
     async def ask_stream(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
+        webpage_context: str | None = None,
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         async for response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             raw=raw,
             options=options,
             cookies=self.cookies,
+            webpage_context=webpage_context
         ):
             yield response
 
     async def close(self) -> None:
         """
         Close the connection
         """
         await self.chat_hub.close()
 
     async def reset(self) -> None:
         """
         Reset the conversation
         """
         await self.close()
-        self.chat_hub = _ChatHub(_Conversation(self.cookies))
+        self.chat_hub = _ChatHub(await _Conversation.create(self.cookies))
 
 
 async def _get_input_async(
     session: PromptSession = None,
     completer: WordCompleter = None,
 ) -> str:
     """
@@ -556,15 +618,15 @@
 
 async def async_main(args: argparse.Namespace) -> None:
     """
     Main function
     """
     print("Initializing...")
     print("Enter `alt+enter` or `escape+enter` to send a message")
-    bot = Chatbot(proxy=args.proxy, cookies=args.cookies)
+    bot = await Chatbot.create(proxy=args.proxy, cookies=args.cookies)
     session = _create_session()
     completer = _create_completer(["!help", "!exit", "!reset"])
     initial_prompt = args.prompt
 
     while True:
         print("\nYou:")
         if initial_prompt:
```

