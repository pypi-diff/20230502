# Comparing `tmp/autosrt-1.2.4.tar.gz` & `tmp/autosrt-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.2.4.tar", last modified: Sun Apr 30 23:47:31 2023, max compression
+gzip compressed data, was "autosrt-1.2.5.tar", last modified: Tue May  2 08:56:38 2023, max compression
```

## Comparing `autosrt-1.2.4.tar` & `autosrt-1.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 23:47:31.335685 autosrt-1.2.4/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.2.4/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-04-30 23:47:31.335685 autosrt-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 23:47:31.294480 autosrt-1.2.4/autosrt/
--rw-rw-rw-   0        0        0     9271 2023-04-30 23:38:40.000000 autosrt-1.2.4/autosrt/__init__.py
--rw-rw-rw-   0        0        0    32560 2023-04-30 13:27:29.000000 autosrt-1.2.4/autosrt/autosrt.py
-drwxrwxrwx   0        0        0        0 2023-04-30 23:47:31.310961 autosrt-1.2.4/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-04-30 23:47:30.000000 autosrt-1.2.4/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-30 23:47:30.000000 autosrt-1.2.4/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 23:47:30.000000 autosrt-1.2.4/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-30 23:47:30.000000 autosrt-1.2.4/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      137 2023-04-30 23:47:30.000000 autosrt-1.2.4/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-30 23:47:30.000000 autosrt-1.2.4/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-30 23:47:31.337934 autosrt-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1583 2023-04-30 23:38:55.000000 autosrt-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 23:47:31.334189 autosrt-1.2.4/test/
--rw-rw-rw-   0        0        0     6874 2023-04-30 02:05:08.000000 autosrt-1.2.4/test/test1.py
--rw-rw-rw-   0        0        0     4087 2023-04-30 02:05:48.000000 autosrt-1.2.4/test/test2.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:56:38.341295 autosrt-1.2.5/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-05-02 08:56:38.342045 autosrt-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 08:56:38.287353 autosrt-1.2.5/autosrt/
+-rw-rw-rw-   0        0        0     9271 2023-05-01 18:14:03.000000 autosrt-1.2.5/autosrt/__init__.py
+-rw-rw-rw-   0        0        0    33442 2023-05-02 08:53:08.000000 autosrt-1.2.5/autosrt/autosrt.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:56:38.313575 autosrt-1.2.5/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-05-02 08:56:37.000000 autosrt-1.2.5/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-05-02 08:56:37.000000 autosrt-1.2.5/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 08:56:37.000000 autosrt-1.2.5/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-02 08:56:37.000000 autosrt-1.2.5/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      137 2023-05-02 08:56:37.000000 autosrt-1.2.5/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 08:56:37.000000 autosrt-1.2.5/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-05-02 08:56:38.343544 autosrt-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1583 2023-05-01 18:14:19.000000 autosrt-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:56:38.339047 autosrt-1.2.5/test/
+-rw-rw-rw-   0        0        0     6874 2023-04-30 02:05:08.000000 autosrt-1.2.5/test/test1.py
+-rw-rw-rw-   0        0        0     4087 2023-04-30 02:05:48.000000 autosrt-1.2.5/test/test2.py
```

### Comparing `autosrt-1.2.4/LICENSE` & `autosrt-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.4/PKG-INFO` & `autosrt-1.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.2.4
+Version: 1.2.5
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.2.4/README.md` & `autosrt-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.4/autosrt/__init__.py` & `autosrt-1.2.5/autosrt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     parser.add_argument('-S', '--src-language', help="Language code of the audio language spoken in video/audio source_path", default="en")
     parser.add_argument('-D', '--dst-language', help="Desired translation language code for the subtitles", default=None)
     parser.add_argument('-ll', '--list-languages', help="List all supported languages", action='store_true')
     parser.add_argument('-o', '--output', help="Output file path for subtitles (by default, subtitles are saved in the same directory and named with the source_path base name)")
     parser.add_argument('-F', '--format', help="Desired subtitle format", default="srt")
     parser.add_argument('-lf', '--list-formats', help="List all supported subtitle formats", action='store_true')
     parser.add_argument('-C', '--concurrency', help="Number of concurrent API requests to make", type=int, default=10)
-    parser.add_argument('-v', '--version', action='version', version='1.2.4')
+    parser.add_argument('-v', '--version', action='version', version='1.2.5')
 
     args = parser.parse_args()
 
     language = Language()
 
     if args.list_languages:
         print("List of supported languages:")
```

### Comparing `autosrt-1.2.4/autosrt/autosrt.py` & `autosrt-1.2.5/autosrt/autosrt.py`

 * *Files 2% similar despite different names*

```diff
@@ -666,89 +666,106 @@
 
         except Exception as e:
             print(e)
             return
 
 
 class SpeechRecognizer(object):
-    def __init__(self, language="en", rate=44100, retries=3, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw"):
+    def __init__(self, language="en", rate=44100, retries=3, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", timeout=30):
         self.language = language
         self.rate = rate
         self.api_key = api_key
         self.retries = retries
+        self.timeout = timeout
 
     def __call__(self, data):
         try:
             for i in range(self.retries):
                 url = "http://www.google.com/speech-api/v2/recognize?client=chromium&lang={lang}&key={key}".format(lang=self.language, key=self.api_key)
-                headers = {"Content-Type": "audio/x-flac; rate=%d" % self.rate}
+                headers = {"Content-Type": "audio/x-flac rate=%d" % self.rate}
 
                 try:
-                    resp = requests.post(url, data=data, headers=headers)
+                    resp = requests.post(url, data=data, headers=headers, timeout=self.timeout)
                 except requests.exceptions.ConnectionError:
-                    continue
+                    try:
+                        resp = httpx.post(url, data=data, headers=headers, timeout=self.timeout)
+                    except httpx.exceptions.NetworkError:
+                        continue
 
                 for line in resp.content.decode('utf-8').split("\n"):
                     try:
                         line = json.loads(line)
                         line = line['result'][0]['alternative'][0]['transcript']
                         return line[:1].upper() + line[1:]
                     except:
                         # no result
                         continue
 
         except KeyboardInterrupt:
-            print("Cancelling transcription")
             return
 
         except Exception as e:
             print(e)
             return
 
 
 class SentenceTranslator(object):
     @staticmethod
-    def GoogleTranslate(text, src, dst):
+    def GoogleTranslate(text, src, dst, timeout=30):
         url = 'https://translate.googleapis.com/translate_a/'
         params = 'single?client=gtx&sl='+src+'&tl='+dst+'&dt=t&q='+text;
         headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)', 'Referer': 'https://translate.google.com',}
+
         try:
-            response = requests.get(url+params, headers=headers)
+            response = requests.get(url+params, headers=headers, timeout=timeout)
             if response.status_code == 200:
                 response_json = response.json()[0]
                 length = len(response_json)
                 translation = ""
                 for i in range(length):
                     translation = translation + response_json[i][0]
                 return translation
             return
 
+        except requests.exceptions.ConnectionError:
+            with httpx.Client() as client:
+                response = client.get(url+params, headers=headers, timeout=timeout)
+                if response.status_code == 200:
+                    response_json = response.json()[0]
+                    length = len(response_json)
+                    translation = ""
+                    for i in range(length):
+                        translation = translation + response_json[i][0]
+                    return translation
+                return
+
         except KeyboardInterrupt:
             print("Cancelling transcription")
             return
 
         except Exception as e:
             print(e)
             return
 
-    def __init__(self, src, dst, patience=-1):
+    def __init__(self, src, dst, patience=-1, timeout=30):
         self.src = src
         self.dst = dst
         self.patience = patience
+        self.timeout = timeout
 
     def __call__(self, sentence):
         try:
             translated_sentence = []
             # handle the special case: empty string.
             if not sentence:
                 return None
-            translated_sentence = self.GoogleTranslate(sentence, src=self.src, dst=self.dst)
+            translated_sentence = self.GoogleTranslate(sentence, src=self.src, dst=self.dst, timeout=self.timeout)
             fail_to_translate = translated_sentence[-1] == '\n'
             while fail_to_translate and patience:
-                translated_sentence = self.GoogleTranslate(translated_sentence, src=self.src, dst=self.dst).text
+                translated_sentence = self.GoogleTranslate(translated_sentence, src=self.src, dst=self.dst, timeout=self.timeout).text
                 if translated_sentence[-1] == '\n':
                     if patience == -1:
                         continue
                     patience -= 1
                 else:
                     fail_to_translate = False
```

### Comparing `autosrt-1.2.4/autosrt.egg-info/PKG-INFO` & `autosrt-1.2.5/autosrt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.2.4
+Version: 1.2.5
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.2.4/setup.py` & `autosrt-1.2.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ]
 
 if sys.platform == "win32":
     install_requires.append("python_magic_bin>=0.4.14")
 
 setup(
     name="autosrt",
-    version="1.2.4",
+    version="1.2.5",
     description="a utility for automatic speech recognition and subtitle generation",
     long_description = long_description,
     author="Bot Bahlul",
     author_email="bot.bahlul@gmail.com",
     url="https://github.com/botbahlul/autosrt",
     packages=["autosrt"],
     entry_points={
```

### Comparing `autosrt-1.2.4/test/test1.py` & `autosrt-1.2.5/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.4/test/test2.py` & `autosrt-1.2.5/test/test2.py`

 * *Files identical despite different names*

