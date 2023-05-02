# Comparing `tmp/autosrt-1.2.7.tar.gz` & `tmp/autosrt-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.2.7.tar", last modified: Tue May  2 11:40:08 2023, max compression
+gzip compressed data, was "autosrt-1.2.8.tar", last modified: Tue May  2 12:00:43 2023, max compression
```

## Comparing `autosrt-1.2.7.tar` & `autosrt-1.2.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 11:40:08.376031 autosrt-1.2.7/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.2.7/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-05-02 11:40:08.376781 autosrt-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 11:40:08.314552 autosrt-1.2.7/autosrt/
--rw-rw-rw-   0        0        0     9271 2023-05-02 11:36:08.000000 autosrt-1.2.7/autosrt/__init__.py
--rw-rw-rw-   0        0        0    33439 2023-05-02 10:41:14.000000 autosrt-1.2.7/autosrt/autosrt.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:40:08.334780 autosrt-1.2.7/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-05-02 11:40:07.000000 autosrt-1.2.7/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-05-02 11:40:07.000000 autosrt-1.2.7/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 11:40:07.000000 autosrt-1.2.7/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-02 11:40:07.000000 autosrt-1.2.7/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      137 2023-05-02 11:40:07.000000 autosrt-1.2.7/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 11:40:07.000000 autosrt-1.2.7/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-05-02 11:40:08.379031 autosrt-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1663 2023-05-02 11:33:00.000000 autosrt-1.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:40:08.372285 autosrt-1.2.7/test/
--rw-rw-rw-   0        0        0     6874 2023-04-30 02:05:08.000000 autosrt-1.2.7/test/test1.py
--rw-rw-rw-   0        0        0     4087 2023-04-30 02:05:48.000000 autosrt-1.2.7/test/test2.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 12:00:43.670415 autosrt-1.2.8/
+-rwxrwxrwx   0 root         (0) root         (0)     1087 2023-01-06 18:50:17.000000 autosrt-1.2.8/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-01-06 18:50:17.000000 autosrt-1.2.8/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     1987 2023-05-02 12:00:43.671018 autosrt-1.2.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5260 2023-04-30 04:22:31.000000 autosrt-1.2.8/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 12:00:43.662201 autosrt-1.2.8/autosrt/
+-rwxrwxrwx   0 root         (0) root         (0)     9271 2023-05-02 11:58:44.000000 autosrt-1.2.8/autosrt/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    33439 2023-05-02 10:41:14.000000 autosrt-1.2.8/autosrt/autosrt.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 12:00:43.667758 autosrt-1.2.8/autosrt.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1987 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      303 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)      112 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      136 2023-05-02 12:00:43.672433 autosrt-1.2.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1695 2023-05-02 12:00:07.000000 autosrt-1.2.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 12:00:43.669526 autosrt-1.2.8/test/
+-rwxrwxrwx   0 root         (0) root         (0)     6874 2023-04-30 02:05:08.000000 autosrt-1.2.8/test/test1.py
+-rwxrwxrwx   0 root         (0) root         (0)     4087 2023-04-30 02:05:48.000000 autosrt-1.2.8/test/test2.py
```

### Comparing `autosrt-1.2.7/LICENSE` & `autosrt-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.7/PKG-INFO` & `autosrt-1.2.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: autosrt
-Version: 1.2.7
-Summary: a utility for automatic speech recognition and subtitle generation
-Home-page: https://github.com/botbahlul/autosrt
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 botbahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-
-autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+Metadata-Version: 2.1
+Name: autosrt
+Version: 1.2.8
+Summary: a utility for automatic speech recognition and subtitle generation
+Home-page: https://github.com/botbahlul/autosrt
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+        
+        Copyright (c) 2022 botbahlul
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+
+autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
```

### Comparing `autosrt-1.2.7/README.md` & `autosrt-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.7/autosrt/__init__.py` & `autosrt-1.2.8/autosrt/__init__.py`

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
-    parser.add_argument('-v', '--version', action='version', version='1.2.7')
+    parser.add_argument('-v', '--version', action='version', version='1.2.8')
 
     args = parser.parse_args()
 
     language = Language()
 
     if args.list_languages:
         print("List of supported languages:")
```

### Comparing `autosrt-1.2.7/autosrt/autosrt.py` & `autosrt-1.2.8/autosrt/autosrt.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.7/autosrt.egg-info/PKG-INFO` & `autosrt-1.2.8/autosrt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: autosrt
-Version: 1.2.7
-Summary: a utility for automatic speech recognition and subtitle generation
-Home-page: https://github.com/botbahlul/autosrt
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 botbahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-
-autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+Metadata-Version: 2.1
+Name: autosrt
+Version: 1.2.8
+Summary: a utility for automatic speech recognition and subtitle generation
+Home-page: https://github.com/botbahlul/autosrt
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+        
+        Copyright (c) 2022 botbahlul
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+
+autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
```

### Comparing `autosrt-1.2.7/test/test1.py` & `autosrt-1.2.8/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.7/test/test2.py` & `autosrt-1.2.8/test/test2.py`

 * *Files identical despite different names*

