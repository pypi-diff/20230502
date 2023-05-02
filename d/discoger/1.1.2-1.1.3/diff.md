# Comparing `tmp/discoger-1.1.2.tar.gz` & `tmp/discoger-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-1.1.2.tar", last modified: Tue May  2 20:11:26 2023, max compression
+gzip compressed data, was "discoger-1.1.3.tar", last modified: Tue May  2 20:53:56 2023, max compression
```

## Comparing `discoger-1.1.2.tar` & `discoger-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:11:26.311903 discoger-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 20:11:08.000000 discoger-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 20:11:26.315903 discoger-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-02 20:11:08.000000 discoger-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:11:26.311903 discoger-1.1.2/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:11:08.000000 discoger-1.1.2/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 20:11:08.000000 discoger-1.1.2/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-02 20:11:08.000000 discoger-1.1.2/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:11:26.311903 discoger-1.1.2/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 20:11:26.000000 discoger-1.1.2/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 20:11:26.000000 discoger-1.1.2/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:11:26.000000 discoger-1.1.2/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 20:11:26.000000 discoger-1.1.2/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 20:11:26.000000 discoger-1.1.2/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 20:11:26.000000 discoger-1.1.2/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 20:11:26.315903 discoger-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-02 20:11:08.000000 discoger-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:53:56.298656 discoger-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 20:53:33.000000 discoger-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 20:53:56.298656 discoger-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-02 20:53:33.000000 discoger-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:53:56.298656 discoger-1.1.3/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:53:33.000000 discoger-1.1.3/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 20:53:33.000000 discoger-1.1.3/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-05-02 20:53:33.000000 discoger-1.1.3/discoger/discoger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:53:56.298656 discoger-1.1.3/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 20:53:56.000000 discoger-1.1.3/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 20:53:56.000000 discoger-1.1.3/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:53:56.000000 discoger-1.1.3/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 20:53:56.000000 discoger-1.1.3/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 20:53:56.000000 discoger-1.1.3/discoger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 20:53:56.000000 discoger-1.1.3/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 20:53:56.298656 discoger-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-02 20:53:33.000000 discoger-1.1.3/setup.py
```

### Comparing `discoger-1.1.2/LICENSE` & `discoger-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-1.1.2/PKG-INFO` & `discoger-1.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.2
+Version: 1.1.3
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.2.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.1.3.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.1.2/README.md` & `discoger-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `discoger-1.1.2/discoger/discoger.py` & `discoger-1.1.3/discoger/discoger.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 token = config["telegram"]["token"]
 secret = secret = config["discogs"]["secret"]
 bot = telebot.TeleBot(token)
 
 commands = {  # command description used in the "help" command
     '/start': 'Get used to the bot',
     '/help': 'Gives you information about the available commands',
-    '/list': 'Show all item from your following list',
+    '/list': 'Show all items in your following list',
     '/delete': 'Delete item from the following list',
     'https://www.discogs.com/release|master/.*': 'Add release or master release in following list (ex: https://www.discogs.com/release/26741825)'
 }
 
 try:
     d = discogs_client.Client('DiscogsAlert/0.1', user_token=secret)
     me = d.identity()
@@ -53,14 +53,19 @@
     raise SystemExit(e)
 
 
 @bot.message_handler(commands=['help', 'start'])
 def send_welcome(message):
     chat_id = message.chat.id
     msg = "Hi there, I am Discoger bot"
+    db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
+    if not db.get("release_list"):
+        db["release_list"] = list()
+        db["chat_id"] = chat_id
+        db.save()
     bot.reply_to(message, msg)
     process_hi_step(chat_id)
 
 
 def process_hi_step(chat_id):
     markup = types.ReplyKeyboardMarkup()
     itembtna = types.KeyboardButton('/help')
@@ -77,20 +82,18 @@
 
 
 @bot.message_handler(commands=['check'])
 def get_check(message):
     chat_id = message.chat.id
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     if db.get("release_list"):
-        bot.send_message(chat_id, "Okay i check your discogs list")
+        bot.send_message(chat_id, "Okay i'm checkng your following list")
         check_discogs(chat_id)
     else:
-        db["release_list"] = list()
-        db.save()
-        bot.send_message(chat_id, "Your discoger following list is empty, send me item url first")
+        bot.send_message(chat_id, "Your discoger following list is empty, send me a url first")
 
 
 @bot.message_handler(regexp="^https://www.discogs.com/.*(release|master)/.*")
 def handle_message(message):
     release_info = dict()
     chat_id = message.chat.id
     release_id = re.findall(r'\d+', message.text)[0]
@@ -114,26 +117,29 @@
         bot.send_message(chat_id, "%s is already in following list" % (release_id))
 
 
 @bot.message_handler(commands=['list'])
 def get_list(message):
     chat_id = message.chat.id
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
-    id_list = 0
-    all_text = ""
-    for i in db["release_list"]:
-        sell_type = i.get("type")
-        if sell_type is None:
-            sell_type = "release"
-        text = "%s: %s - %s %s/%s/%s" % (id_list, i["artist"], i["title"], discogs_url, sell_type, i["release_id"])
-        all_text = all_text + "\n" + text
-        id_list = id_list + 1
-    splitted_text = util.split_string(all_text, 3000)
-    for text in splitted_text:
-        bot.send_message(chat_id, text, disable_web_page_preview=True)
+    if not db.get("release_list"):
+        bot.send_message(chat_id, "Your discoger following list is empty, send me a url first")
+    else:
+        id_list = 0
+        all_text = ""
+        for i in db["release_list"]:
+            sell_type = i.get("type")
+            if sell_type is None:
+                sell_type = "release"
+            text = "%s: %s - %s %s/%s/%s" % (id_list, i["artist"], i["title"], discogs_url, sell_type, i["release_id"])
+            all_text = all_text + "\n" + text
+            id_list = id_list + 1
+        splitted_text = util.split_string(all_text, 3000)
+        for text in splitted_text:
+            bot.send_message(chat_id, text, disable_web_page_preview=True)
 
 
 @bot.message_handler(commands=['delete'])
 def delete_release(message):
     msg = "Which item do you want delete in your list?"
     answer = bot.reply_to(message, msg)
     bot.register_next_step_handler(answer, process_delete_step)
```

### Comparing `discoger-1.1.2/discoger.egg-info/PKG-INFO` & `discoger-1.1.3/discoger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.2
+Version: 1.1.3
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.2.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.1.3.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.1.2/setup.py` & `discoger-1.1.3/setup.py`

 * *Files identical despite different names*

