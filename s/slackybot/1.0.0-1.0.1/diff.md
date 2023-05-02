# Comparing `tmp/slackybot-1.0.0.tar.gz` & `tmp/slackybot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackybot-1.0.0.tar", last modified: Sun Mar 26 20:59:28 2023, max compression
+gzip compressed data, was "slackybot-1.0.1.tar", last modified: Tue May  2 11:30:14 2023, max compression
```

## Comparing `slackybot-1.0.0.tar` & `slackybot-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 20:59:28.502693 slackybot-1.0.0/
--rw-rw-rw-   0        0        0     1088 2023-03-05 21:40:10.000000 slackybot-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2108 2023-03-26 20:59:28.503692 slackybot-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1489 2023-03-26 19:57:28.000000 slackybot-1.0.0/README.md
--rw-rw-rw-   0        0        0       86 2023-03-05 21:48:07.000000 slackybot-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      798 2023-03-26 20:59:28.505693 slackybot-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       75 2023-03-26 20:54:56.000000 slackybot-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-26 20:59:28.460730 slackybot-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-26 20:59:28.481694 slackybot-1.0.0/src/slackybot/
--rw-rw-rw-   0        0        0       25 2023-03-05 21:48:07.000000 slackybot-1.0.0/src/slackybot/__init__.py
--rw-rw-rw-   0        0        0     1795 2023-03-26 15:38:48.000000 slackybot-1.0.0/src/slackybot/exceptions.py
--rw-rw-rw-   0        0        0     1150 2023-03-25 22:25:19.000000 slackybot-1.0.0/src/slackybot/main.py
--rw-rw-rw-   0        0        0     2424 2023-03-26 15:39:06.000000 slackybot-1.0.0/src/slackybot/messaging.py
-drwxrwxrwx   0        0        0        0 2023-03-26 20:59:28.501692 slackybot-1.0.0/src/slackybot/utilities/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:48:07.000000 slackybot-1.0.0/src/slackybot/utilities/__init__.py
--rw-rw-rw-   0        0        0      502 2023-03-20 21:16:42.000000 slackybot-1.0.0/src/slackybot/utilities/config.py
--rw-rw-rw-   0        0        0      198 2023-03-20 21:14:44.000000 slackybot-1.0.0/src/slackybot/utilities/helpers.py
--rw-rw-rw-   0        0        0      521 2023-03-20 20:33:58.000000 slackybot-1.0.0/src/slackybot/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-03-26 20:59:28.496693 slackybot-1.0.0/src/slackybot.egg-info/
--rw-rw-rw-   0        0        0     2108 2023-03-26 20:59:28.000000 slackybot-1.0.0/src/slackybot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-03-26 20:59:28.000000 slackybot-1.0.0/src/slackybot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 20:59:28.000000 slackybot-1.0.0/src/slackybot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-26 20:59:28.000000 slackybot-1.0.0/src/slackybot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-26 20:59:28.000000 slackybot-1.0.0/src/slackybot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 11:30:14.546264 slackybot-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2023-03-05 21:40:10.000000 slackybot-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2341 2023-05-02 11:30:14.546264 slackybot-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1627 2023-05-02 11:28:52.000000 slackybot-1.0.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-02 11:28:52.000000 slackybot-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      882 2023-05-02 11:30:14.549852 slackybot-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       75 2023-05-02 11:28:52.000000 slackybot-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:30:14.394366 slackybot-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 11:30:14.450874 slackybot-1.0.1/src/slackybot/
+-rw-rw-rw-   0        0        0       25 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/__init__.py
+-rw-rw-rw-   0        0        0     1795 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/exceptions.py
+-rw-rw-rw-   0        0        0     1380 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/main.py
+-rw-rw-rw-   0        0        0     2970 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/messaging.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:30:14.532622 slackybot-1.0.1/src/slackybot/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/utilities/__init__.py
+-rw-rw-rw-   0        0        0      502 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/utilities/config.py
+-rw-rw-rw-   0        0        0      198 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/utilities/helpers.py
+-rw-rw-rw-   0        0        0      521 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:30:14.516380 slackybot-1.0.1/src/slackybot.egg-info/
+-rw-rw-rw-   0        0        0     2341 2023-05-02 11:30:14.000000 slackybot-1.0.1/src/slackybot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-05-02 11:30:14.000000 slackybot-1.0.1/src/slackybot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 11:30:14.000000 slackybot-1.0.1/src/slackybot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 11:30:14.000000 slackybot-1.0.1/src/slackybot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-02 11:30:14.000000 slackybot-1.0.1/src/slackybot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 11:30:14.542470 slackybot-1.0.1/tests/
+-rw-rw-rw-   0        0        0     1789 2023-05-02 11:28:52.000000 slackybot-1.0.1/tests/test_slack_message_object.py
+-rw-rw-rw-   0        0        0     1485 2023-05-02 11:28:52.000000 slackybot-1.0.1/tests/test_slack_object.py
```

### Comparing `slackybot-1.0.0/LICENSE` & `slackybot-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slackybot-1.0.0/PKG-INFO` & `slackybot-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: slackybot
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package that helps to interact with the Slack App
 Home-page: https://github.com/michalm138/slackybot
 Author: michalm138
 Author-email: dev.michalm138@gmail.com
+Project-URL: Documentation, https://github.com/michalm138/slackybot/blob/main/docs/README.md
 Project-URL: Bug Tracker, https://github.com/michalm138/slackybot/issues
-Project-URL: repository, https://github.com/michalm138/slackybot
+Project-URL: Source Code, https://github.com/michalm138/slackybot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,14 +19,16 @@
 This Python package helps you with sending messages to Slack. It offers an object-oriented approach - every message or reply in a thread is an object, so they can be easily managed.
 
 ## Getting started
 ### Installation
 ```commandline
 python -m pip install slackybot
 ```
+Add following token scopes to your Slack bot:  
+`channels:join` `channels:read` `chat:write` `chat:write.customize` `chat:write.public`
 
 ### Simple usage
 Import and initialize the slack object
 ```python
 from slackybot import Slack
 
 slack = Slack(token='XXX')
```

### Comparing `slackybot-1.0.0/README.md` & `slackybot-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 This Python package helps you with sending messages to Slack. It offers an object-oriented approach - every message or reply in a thread is an object, so they can be easily managed.
 
 ## Getting started
 ### Installation
 ```commandline
 python -m pip install slackybot
 ```
+Add following token scopes to your Slack bot:  
+`channels:join` `channels:read` `chat:write` `chat:write.customize` `chat:write.public`
 
 ### Simple usage
 Import and initialize the slack object
 ```python
 from slackybot import Slack
 
 slack = Slack(token='XXX')
```

### Comparing `slackybot-1.0.0/setup.cfg` & `slackybot-1.0.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6c61 636b 7962 6f74 0d0a 7665   = slackybot..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 300d 0a61  rsion = 1.0.0..a
+00000020: 7273 696f 6e20 3d20 312e 302e 310d 0a61  rsion = 1.0.1..a
 00000030: 7574 686f 7220 3d20 6d69 6368 616c 6d31  uthor = michalm1
 00000040: 3338 0d0a 6175 7468 6f72 5f65 6d61 696c  38..author_email
 00000050: 203d 2064 6576 2e6d 6963 6861 6c6d 3133   = dev.michalm13
 00000060: 3840 676d 6169 6c2e 636f 6d0d 0a64 6573  8@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2041 2050 7974  cription = A Pyt
 00000080: 686f 6e20 7061 636b 6167 6520 7468 6174  hon package that
 00000090: 2068 656c 7073 2074 6f20 696e 7465 7261   helps to intera
@@ -15,36 +15,42 @@
 000000e0: 5345 2e74 7874 0d0a 6c6f 6e67 5f64 6573  SE.txt..long_des
 000000f0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
 00000100: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
 00000110: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
 00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00000130: 6d69 6368 616c 6d31 3338 2f73 6c61 636b  michalm138/slack
 00000140: 7962 6f74 0d0a 7072 6f6a 6563 745f 7572  ybot..project_ur
-00000150: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
-00000160: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
-00000170: 7468 7562 2e63 6f6d 2f6d 6963 6861 6c6d  thub.com/michalm
-00000180: 3133 382f 736c 6163 6b79 626f 742f 6973  138/slackybot/is
-00000190: 7375 6573 0d0a 0972 6570 6f73 6974 6f72  sues...repositor
-000001a0: 7920 3d20 6874 7470 733a 2f2f 6769 7468  y = https://gith
-000001b0: 7562 2e63 6f6d 2f6d 6963 6861 6c6d 3133  ub.com/michalm13
-000001c0: 382f 736c 6163 6b79 626f 740d 0a63 6c61  8/slackybot..cla
-000001d0: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-000001e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000200: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
-00000210: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-00000220: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
-00000230: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000240: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-00000250: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-00000260: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-00000270: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
-00000280: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-00000290: 6571 7569 7265 7320 3d20 3e3d 332e 3130  equires = >=3.10
-000002a0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-000002b0: 6573 203d 200d 0a09 7265 7175 6573 7473  es = ...requests
-000002c0: 3e3d 322e 3238 2e32 0d0a 0d0a 5b6f 7074  >=2.28.2....[opt
-000002d0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-000002e0: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
-000002f0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000300: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000310: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000150: 6c73 203d 200d 0a09 446f 6375 6d65 6e74  ls = ...Document
+00000160: 6174 696f 6e20 3d20 6874 7470 733a 2f2f  ation = https://
+00000170: 6769 7468 7562 2e63 6f6d 2f6d 6963 6861  github.com/micha
+00000180: 6c6d 3133 382f 736c 6163 6b79 626f 742f  lm138/slackybot/
+00000190: 626c 6f62 2f6d 6169 6e2f 646f 6373 2f52  blob/main/docs/R
+000001a0: 4541 444d 452e 6d64 0d0a 0942 7567 2054  EADME.md...Bug T
+000001b0: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
+000001c0: 2f67 6974 6875 622e 636f 6d2f 6d69 6368  /github.com/mich
+000001d0: 616c 6d31 3338 2f73 6c61 636b 7962 6f74  alm138/slackybot
+000001e0: 2f69 7373 7565 730d 0a09 536f 7572 6365  /issues...Source
+000001f0: 2043 6f64 6520 3d20 6874 7470 733a 2f2f   Code = https://
+00000200: 6769 7468 7562 2e63 6f6d 2f6d 6963 6861  github.com/micha
+00000210: 6c6d 3133 382f 736c 6163 6b79 626f 740d  lm138/slackybot.
+00000220: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+00000230: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000240: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000250: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
+00000260: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000270: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
+00000280: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000290: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+000002a0: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
+000002b0: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
+000002c0: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
+000002d0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
+000002e0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+000002f0: 332e 3130 0d0a 696e 7374 616c 6c5f 7265  3.10..install_re
+00000300: 7175 6972 6573 203d 200d 0a09 7265 7175  quires = ...requ
+00000310: 6573 7473 3e3d 322e 3238 2e32 0d0a 0d0a  ests>=2.28.2....
+00000320: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000330: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
+00000340: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
+00000350: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000360: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+00000370: 0d0a                                     ..
```

### Comparing `slackybot-1.0.0/src/slackybot/exceptions.py` & `slackybot-1.0.1/src/slackybot/exceptions.py`

 * *Files identical despite different names*

### Comparing `slackybot-1.0.0/src/slackybot/main.py` & `slackybot-1.0.1/src/slackybot/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 from .messaging import Message
 from .utilities import request_handler, config, helpers
 from . import exceptions
 
 
 class Slack:
 
-    def __init__(self, token=None):
+    def __init__(self, token=None, default_channel=''):
         if not token:
             raise exceptions.SlackInitializeError('Missing token')
         self._token = token
         self._messages = []
+        self._default_channel = default_channel
 
     def send_message(self, channel='', text=''):
-        """
-        Send message to the Slack
-        :param channel: (string) Channel name
-        :param text: (string) Text message
-        :return: (object) SlackMessage
+        """Sends simple text message.
+
+        Args:
+            channel (string): Channel name.
+            text (string): Text to be sent.
+
+        Returns:
+            Object: <Message>
         """
         if output := request_handler.post_request(
             config.data['urls']['post_message'],
-            {'channel': channel, 'text': text},
+            {'channel': channel if channel else self._default_channel, 'text': text},
             self._token,
         ):
             if output['ok']:
                 slack_message = Message(self._token, channel, text, output)
                 self._messages.append(slack_message)
                 return slack_message
             else:
                 raise helpers.get_exception(output)
         else:
             raise exceptions.MessageNotSend
 
     def get_messages(self):
+        """Lists all sent messages.
+
+        Returns:
+            List: Message objects
+        """
         return self._messages[:]
```

### Comparing `slackybot-1.0.0/src/slackybot/messaging.py` & `slackybot-1.0.1/src/slackybot/messaging.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,27 +18,40 @@
     def __srt__(self):
         return f'<{self.__class__.__name__} {self.id}>'
 
     def __repr__(self):
         return f'<{self.__class__.__name__} {self.id}>'
 
     def update(self, text=''):
+        """Updates the message.
+
+        Args:
+            text (string): New text. Old one will be replaced.
+
+        Returns:
+            None
+        """
         if output := request_handler.post_request(
                 config.data['urls']['update_message'],
                 {'channel': self._channel, 'ts': self._ts, 'text': text},
                 self._token,
         ):
             if output['ok']:
                 self.text = text
             else:
                 raise helpers.get_exception(output)
         else:
             raise exceptions.MessageNotUpdated
 
     def delete(self):
+        """Deletes the message.
+
+        Returns:
+            None
+        """
         if self._deleted:
             raise exceptions.MessageAlreadyDeleted
 
         if output := request_handler.post_request(
                 config.data['urls']['delete_message'],
                 {'channel': self._channel, 'ts': self._ts},
                 self._token,
@@ -54,14 +67,23 @@
 class Message(SlackMessage):
 
     def __init__(self, token, channel, text, data):
         super().__init__(token, channel, text, data)
         self._replies = []
 
     def send_reply(self, text=''):
+        """Sends reply in the message thread.
+
+        Args:
+            text (string): Text to be sent.
+
+        Returns:
+            Object: <Reply>
+
+        """
         if output := request_handler.post_request(
                 config.data['urls']['post_message'],
                 {'channel': self.channel, 'thread_ts': self._ts, 'text': text},
                 self._token,
         ):
             if output['ok']:
                 reply = Reply(self._token, self.channel, text, output)
@@ -69,12 +91,17 @@
                 return reply
             else:
                 raise helpers.get_exception(output)
         else:
             raise exceptions.MessageNotSend
 
     def get_replies(self):
+        """Lists all sent replies to the message thread.
+
+        Returns:
+            List: Reply objects
+        """
         return self._replies[:]
 
 
 class Reply(SlackMessage):
     pass
```

### Comparing `slackybot-1.0.0/src/slackybot/utilities/request_handler.py` & `slackybot-1.0.1/src/slackybot/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `slackybot-1.0.0/src/slackybot.egg-info/PKG-INFO` & `slackybot-1.0.1/src/slackybot.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: slackybot
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package that helps to interact with the Slack App
 Home-page: https://github.com/michalm138/slackybot
 Author: michalm138
 Author-email: dev.michalm138@gmail.com
+Project-URL: Documentation, https://github.com/michalm138/slackybot/blob/main/docs/README.md
 Project-URL: Bug Tracker, https://github.com/michalm138/slackybot/issues
-Project-URL: repository, https://github.com/michalm138/slackybot
+Project-URL: Source Code, https://github.com/michalm138/slackybot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,14 +19,16 @@
 This Python package helps you with sending messages to Slack. It offers an object-oriented approach - every message or reply in a thread is an object, so they can be easily managed.
 
 ## Getting started
 ### Installation
 ```commandline
 python -m pip install slackybot
 ```
+Add following token scopes to your Slack bot:  
+`channels:join` `channels:read` `chat:write` `chat:write.customize` `chat:write.public`
 
 ### Simple usage
 Import and initialize the slack object
 ```python
 from slackybot import Slack
 
 slack = Slack(token='XXX')
```

