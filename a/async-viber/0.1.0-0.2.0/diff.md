# Comparing `tmp/async-viber-0.1.0.tar.gz` & `tmp/async-viber-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-viber-0.1.0.tar", last modified: Wed Apr 19 00:21:31 2023, max compression
+gzip compressed data, was "async-viber-0.2.0.tar", last modified: Tue May  2 12:36:14 2023, max compression
```

## Comparing `async-viber-0.1.0.tar` & `async-viber-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,44 @@
--rw-r--r--   0        0        0      499 2023-04-18 23:30:01.850945 async-viber-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       19 2023-04-18 23:24:28.738176 async-viber-0.1.0/README.md
--rw-r--r--   0        0        0      137 2023-04-19 00:13:34.104045 async-viber-0.1.0/tests/__main__.py
--rw-r--r--   0        0        0      131 2023-04-19 00:17:16.217227 async-viber-0.1.0/viber/__init__.py
--rw-r--r--   0        0        0       21 2023-04-09 18:52:32.193753 async-viber-0.1.0/viber/bot/__init__.py
--rw-r--r--   0        0        0     2318 2023-04-18 23:33:17.810327 async-viber-0.1.0/viber/bot/api.py
--rw-r--r--   0        0        0     2269 2023-04-09 18:52:32.256235 async-viber-0.1.0/viber/bot/base.py
--rw-r--r--   0        0        0     6335 2023-04-09 18:52:32.303114 async-viber-0.1.0/viber/bot/bot.py
--rw-r--r--   0        0        0        0 2023-04-09 18:52:32.334191 async-viber-0.1.0/viber/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 18:52:32.349844 async-viber-0.1.0/viber/contrib/fsm_storage/__init__.py
--rw-r--r--   0        0        0     7966 2023-04-09 18:52:32.381284 async-viber-0.1.0/viber/contrib/fsm_storage/mongo.py
--rw-r--r--   0        0        0       47 2023-04-09 18:52:32.412876 async-viber-0.1.0/viber/dispatcher/__init__.py
--rw-r--r--   0        0        0     5597 2023-04-18 23:33:17.782712 async-viber-0.1.0/viber/dispatcher/dispatcher.py
--rw-r--r--   0        0        0      299 2023-04-09 18:52:32.554142 async-viber-0.1.0/viber/dispatcher/filters/__init__.py
--rw-r--r--   0        0        0    11179 2023-04-19 00:15:35.765335 async-viber-0.1.0/viber/dispatcher/filters/builtin.py
--rw-r--r--   0        0        0     2517 2023-04-09 18:52:32.601238 async-viber-0.1.0/viber/dispatcher/filters/factory.py
--rw-r--r--   0        0        0     8412 2023-04-09 18:52:32.632936 async-viber-0.1.0/viber/dispatcher/filters/filters.py
--rw-r--r--   0        0        0     5176 2023-04-09 18:52:32.664196 async-viber-0.1.0/viber/dispatcher/filters/state.py
--rw-r--r--   0        0        0     4130 2023-04-09 18:52:32.459932 async-viber-0.1.0/viber/dispatcher/handler.py
--rw-r--r--   0        0        0    15575 2023-04-09 18:52:32.491409 async-viber-0.1.0/viber/dispatcher/storage.py
--rw-r--r--   0        0        0     6945 2023-04-19 00:14:02.352359 async-viber-0.1.0/viber/dispatcher/webhook.py
--rw-r--r--   0        0        0      830 2023-04-19 00:18:11.418290 async-viber-0.1.0/viber/loader.py
--rw-r--r--   0        0        0      452 2023-04-09 18:52:32.711066 async-viber-0.1.0/viber/types/__init__.py
--rw-r--r--   0        0        0     8109 2023-04-09 18:52:32.758012 async-viber-0.1.0/viber/types/base.py
--rw-r--r--   0        0        0       76 2023-04-09 18:52:32.796831 async-viber-0.1.0/viber/types/callback_query.py
--rw-r--r--   0        0        0      164 2023-04-09 18:52:32.812457 async-viber-0.1.0/viber/types/contact.py
--rw-r--r--   0        0        0      274 2023-04-09 18:52:32.844238 async-viber-0.1.0/viber/types/conversation_started.py
--rw-r--r--   0        0        0     5728 2023-04-09 18:52:32.876025 async-viber-0.1.0/viber/types/fields.py
--rw-r--r--   0        0        0     3019 2023-04-09 18:52:32.907776 async-viber-0.1.0/viber/types/inline_keyboard.py
--rw-r--r--   0        0        0     3139 2023-04-09 18:52:32.939562 async-viber-0.1.0/viber/types/message.py
--rw-r--r--   0        0        0      126 2023-04-09 18:52:32.955367 async-viber-0.1.0/viber/types/message_id.py
--rw-r--r--   0        0        0     3127 2023-04-09 18:52:32.986719 async-viber-0.1.0/viber/types/reply_keyboard.py
--rw-r--r--   0        0        0     1702 2023-04-09 18:52:33.018376 async-viber-0.1.0/viber/types/update.py
--rw-r--r--   0        0        0      270 2023-04-09 18:52:33.034198 async-viber-0.1.0/viber/types/user.py
--rw-r--r--   0        0        0        0 2023-04-09 18:52:33.065693 async-viber-0.1.0/viber/utils/__init__.py
--rw-r--r--   0        0        0     5539 2023-04-09 18:52:33.097256 async-viber-0.1.0/viber/utils/deprecated.py
--rw-r--r--   0        0        0     3134 2023-04-09 18:52:33.128897 async-viber-0.1.0/viber/utils/exceptions.py
--rw-r--r--   0        0        0     5779 2023-04-09 18:52:33.160375 async-viber-0.1.0/viber/utils/helper.py
--rw-r--r--   0        0        0     2688 2023-04-18 23:33:17.893745 async-viber-0.1.0/viber/utils/payload.py
--rw-r--r--   0        0        0      200 1970-01-01 00:00:00.000000 async-viber-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      519 2023-05-02 12:35:04.997388 async-viber-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       19 2023-04-18 23:24:28.738176 async-viber-0.2.0/README.md
+-rw-r--r--   0        0        0      137 2023-04-19 00:13:34.104045 async-viber-0.2.0/tests/__main__.py
+-rw-r--r--   0        0        0      443 2023-04-24 03:34:25.616731 async-viber-0.2.0/viber/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-09 18:52:32.193753 async-viber-0.2.0/viber/bot/__init__.py
+-rw-r--r--   0        0        0     2318 2023-04-18 23:33:17.810327 async-viber-0.2.0/viber/bot/api.py
+-rw-r--r--   0        0        0     2269 2023-04-09 18:52:32.256235 async-viber-0.2.0/viber/bot/base.py
+-rw-r--r--   0        0        0     6335 2023-04-09 18:52:32.303114 async-viber-0.2.0/viber/bot/bot.py
+-rw-r--r--   0        0        0      853 2023-04-19 18:14:28.151846 async-viber-0.2.0/viber/buttons.py
+-rw-r--r--   0        0        0      370 2023-04-19 17:07:46.414120 async-viber-0.2.0/viber/config.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:52:32.334191 async-viber-0.2.0/viber/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:52:32.349844 async-viber-0.2.0/viber/contrib/fsm_storage/__init__.py
+-rw-r--r--   0        0        0     7966 2023-04-09 18:52:32.381284 async-viber-0.2.0/viber/contrib/fsm_storage/mongo.py
+-rw-r--r--   0        0        0       93 2023-04-19 16:06:44.807189 async-viber-0.2.0/viber/dispatcher/__init__.py
+-rw-r--r--   0        0        0     8139 2023-05-02 12:34:10.876845 async-viber-0.2.0/viber/dispatcher/dispatcher.py
+-rw-r--r--   0        0        0      299 2023-04-09 18:52:32.554142 async-viber-0.2.0/viber/dispatcher/filters/__init__.py
+-rw-r--r--   0        0        0    11194 2023-04-19 22:32:40.400509 async-viber-0.2.0/viber/dispatcher/filters/builtin.py
+-rw-r--r--   0        0        0     2517 2023-04-09 18:52:32.601238 async-viber-0.2.0/viber/dispatcher/filters/factory.py
+-rw-r--r--   0        0        0     8412 2023-04-09 18:52:32.632936 async-viber-0.2.0/viber/dispatcher/filters/filters.py
+-rw-r--r--   0        0        0     5176 2023-04-09 18:52:32.664196 async-viber-0.2.0/viber/dispatcher/filters/state.py
+-rw-r--r--   0        0        0     4130 2023-04-09 18:52:32.459932 async-viber-0.2.0/viber/dispatcher/handler.py
+-rw-r--r--   0        0        0    15575 2023-04-09 18:52:32.491409 async-viber-0.2.0/viber/dispatcher/storage.py
+-rw-r--r--   0        0        0     6621 2023-04-19 21:25:14.337180 async-viber-0.2.0/viber/dispatcher/webhook.py
+-rw-r--r--   0        0        0      653 2023-04-25 07:49:51.625224 async-viber-0.2.0/viber/helpers.py
+-rw-r--r--   0        0        0      723 2023-04-19 18:13:08.175112 async-viber-0.2.0/viber/keyboards.py
+-rw-r--r--   0        0        0      952 2023-04-19 17:07:46.439870 async-viber-0.2.0/viber/loader.py
+-rw-r--r--   0        0        0      512 2023-04-19 21:25:14.316488 async-viber-0.2.0/viber/types/__init__.py
+-rw-r--r--   0        0        0     8109 2023-04-09 18:52:32.758012 async-viber-0.2.0/viber/types/base.py
+-rw-r--r--   0        0        0       76 2023-04-09 18:52:32.796831 async-viber-0.2.0/viber/types/callback_query.py
+-rw-r--r--   0        0        0      164 2023-04-09 18:52:32.812457 async-viber-0.2.0/viber/types/contact.py
+-rw-r--r--   0        0        0      274 2023-04-09 18:52:32.844238 async-viber-0.2.0/viber/types/conversation_started.py
+-rw-r--r--   0        0        0     5728 2023-04-09 18:52:32.876025 async-viber-0.2.0/viber/types/fields.py
+-rw-r--r--   0        0        0     3019 2023-04-09 18:52:32.907776 async-viber-0.2.0/viber/types/inline_keyboard.py
+-rw-r--r--   0        0        0     3001 2023-04-24 03:31:17.171701 async-viber-0.2.0/viber/types/message.py
+-rw-r--r--   0        0        0      126 2023-04-09 18:52:32.955367 async-viber-0.2.0/viber/types/message_id.py
+-rw-r--r--   0        0        0     3127 2023-04-09 18:52:32.986719 async-viber-0.2.0/viber/types/reply_keyboard.py
+-rw-r--r--   0        0        0     1702 2023-04-09 18:52:33.018376 async-viber-0.2.0/viber/types/update.py
+-rw-r--r--   0        0        0      270 2023-04-09 18:52:33.034198 async-viber-0.2.0/viber/types/user.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:52:33.065693 async-viber-0.2.0/viber/utils/__init__.py
+-rw-r--r--   0        0        0     5539 2023-04-09 18:52:33.097256 async-viber-0.2.0/viber/utils/deprecated.py
+-rw-r--r--   0        0        0     3134 2023-04-09 18:52:33.128897 async-viber-0.2.0/viber/utils/exceptions.py
+-rw-r--r--   0        0        0     5779 2023-04-09 18:52:33.160375 async-viber-0.2.0/viber/utils/helper.py
+-rw-r--r--   0        0        0     2688 2023-04-18 23:33:17.893745 async-viber-0.2.0/viber/utils/payload.py
+-rw-r--r--   0        0        0      200 1970-01-01 00:00:00.000000 async-viber-0.2.0/PKG-INFO
```

### Comparing `async-viber-0.1.0/viber/bot/api.py` & `async-viber-0.2.0/viber/bot/api.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/bot/base.py` & `async-viber-0.2.0/viber/bot/base.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/bot/bot.py` & `async-viber-0.2.0/viber/bot/bot.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/contrib/fsm_storage/mongo.py` & `async-viber-0.2.0/viber/contrib/fsm_storage/mongo.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/dispatcher/filters/builtin.py` & `async-viber-0.2.0/viber/dispatcher/filters/builtin.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
 
     @abstractmethod
     def cast_update(self, obj):
         """Cast update-obj to string for matching"""
 
     @staticmethod
     def make_regexp(text: str):
-        return re.sub(r'{(.+?)}', r'(?P<\1>.+)', text)
+        return re.sub(r"\\{(.+?)\\}", r"(?P<\1>.+)", re.escape(text))
 
     def __init__(self, button):
         buttons_regexps = []
         if not isinstance(button, (list, tuple, set)):
             button = [button]
 
         for item in button:
```

### Comparing `async-viber-0.1.0/viber/dispatcher/filters/factory.py` & `async-viber-0.2.0/viber/dispatcher/filters/factory.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/dispatcher/filters/filters.py` & `async-viber-0.2.0/viber/dispatcher/filters/filters.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/dispatcher/filters/state.py` & `async-viber-0.2.0/viber/dispatcher/filters/state.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/dispatcher/handler.py` & `async-viber-0.2.0/viber/dispatcher/handler.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/dispatcher/storage.py` & `async-viber-0.2.0/viber/dispatcher/storage.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/dispatcher/webhook.py` & `async-viber-0.2.0/viber/dispatcher/webhook.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 import warnings
 from typing import Optional, Union
 
 from aiohttp import web
 
 from viber.bot import Bot
 from .. import types
-from ..types import base
 from ..utils import helper
 from ..utils.exceptions import TimeoutWarning
 from ..utils.payload import get_md_text
+from viber.types import ReplyKeyboard
 
 BOT_DISPATCHER_KEY = 'BOT_DISPATCHER'
 RESPONSE_TIMEOUT = 55
 
 log = logging.getLogger(__name__)
 
 
@@ -197,40 +197,35 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         return await self()
 
 
-class SendMessageOnConversationStarted(BaseResponse):
+class StartResponse(BaseResponse):
     method = None
 
-    __slots__ = ('text', 'parse_mode', 'reply_markup', 'tracking_data')
+    __slots__ = ('text', 'markup', 'tracking_data')
 
-    def __init__(self, text: base.String,
-                 parse_mode: Optional[base.String] = None,
-                 reply_markup: Union[types.ReplyKeyboardMarkup,
-                                     types.InlineKeyboardMarkup,
-                                     None] = None,
-                 tracking_data: Optional[base.String] = None):
+    def __init__(
+            self, text: str,
+            markup: ReplyKeyboard = None,
+            tracking_data: str = None,
+    ):
         self.text = text
-        self.parse_mode = parse_mode
-        self.reply_markup = reply_markup
+        self.markup = markup
         self.tracking_data = tracking_data
 
     def prepare(self):
         bot = Bot.get_current()
-
-        if self.reply_markup is None:
-            keyboard = self.reply_markup
+        if self.markup is None:
+            keyboard = self.markup
         else:
-            keyboard = self.reply_markup.to_python()
-
-        text = get_md_text(self.text, self.parse_mode or bot.parse_mode)
-
+            keyboard = self.markup.to_python()
+        text = get_md_text(self.text, bot.parse_mode)
         return {
             'sender': {'name': bot.name, 'avatar': bot.avatar},
             'min_api_version': bot.min_api_version,
             'type': 'text',
             'text': text,
             'keyboard': keyboard,
             'tracking_data': self.tracking_data,
```

### Comparing `async-viber-0.1.0/viber/types/base.py` & `async-viber-0.2.0/viber/types/base.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/types/fields.py` & `async-viber-0.2.0/viber/types/fields.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/types/inline_keyboard.py` & `async-viber-0.2.0/viber/types/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/types/message.py` & `async-viber-0.2.0/viber/types/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,46 +20,46 @@
     media: base.String = fields.Field()
     contact: Contact = fields.Field(base=Contact)
 
     async def reply(self,
                     text: base.String,
                     parse_mode: Optional[base.String] = None,
                     reply_markup: Union[ReplyKeyboardMarkup,
-                                        InlineKeyboardMarkup,
-                                        None] = None,
+                    InlineKeyboardMarkup,
+                    None] = None,
                     tracking_data: Optional[base.String] = None,
                     ) -> MessageId:
         """Only for compability. Like self.answer()"""
         return await self.answer(text, parse_mode, reply_markup, tracking_data)
 
     async def answer(self,
                      text: base.String,
                      parse_mode: Optional[base.String] = None,
                      reply_markup: Union[ReplyKeyboardMarkup,
-                                         InlineKeyboardMarkup,
-                                         None] = None,
+                     InlineKeyboardMarkup,
+                     None] = None,
                      tracking_data: Optional[base.String] = None,
                      ) -> MessageId:
         return await self.bot.send_message(
             chat_id=self.from_user.id,
             text=text,
             parse_mode=parse_mode,
             reply_markup=reply_markup,
             tracking_data=tracking_data,
         )
 
-    async def answer_picture(self,
-                             media: base.String,
-                             text: base.String,
-                             parse_mode: Optional[base.String] = None,
-                             reply_markup: Union[ReplyKeyboardMarkup,
-                                                 InlineKeyboardMarkup,
-                                                 None] = None,
-                             tracking_data: Optional[base.String] = None,
-                             ) -> MessageId:
+    async def answer_photo(self,
+                           media: base.String,
+                           text: base.String,
+                           parse_mode: Optional[base.String] = None,
+                           reply_markup: Union[ReplyKeyboardMarkup,
+                           InlineKeyboardMarkup,
+                           None] = None,
+                           tracking_data: Optional[base.String] = None,
+                           ) -> MessageId:
         return await self.bot.send_picture(
             chat_id=self.from_user.id,
             media=media,
             text=text,
             parse_mode=parse_mode,
             reply_markup=reply_markup,
             tracking_data=tracking_data,
```

### Comparing `async-viber-0.1.0/viber/types/reply_keyboard.py` & `async-viber-0.2.0/viber/types/reply_keyboard.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/types/update.py` & `async-viber-0.2.0/viber/types/update.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/utils/deprecated.py` & `async-viber-0.2.0/viber/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/utils/exceptions.py` & `async-viber-0.2.0/viber/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/utils/helper.py` & `async-viber-0.2.0/viber/utils/helper.py`

 * *Files identical despite different names*

### Comparing `async-viber-0.1.0/viber/utils/payload.py` & `async-viber-0.2.0/viber/utils/payload.py`

 * *Files identical despite different names*

