# Comparing `tmp/discoger-1.1.1.tar.gz` & `tmp/discoger-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-1.1.1.tar", last modified: Tue May  2 19:35:31 2023, max compression
+gzip compressed data, was "discoger-1.1.2.tar", last modified: Tue May  2 20:11:26 2023, max compression
```

## Comparing `discoger-1.1.1.tar` & `discoger-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:35:31.980555 discoger-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 19:35:17.000000 discoger-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 19:35:31.980555 discoger-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-02 19:35:17.000000 discoger-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:35:31.980555 discoger-1.1.1/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:35:17.000000 discoger-1.1.1/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 19:35:17.000000 discoger-1.1.1/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-05-02 19:35:17.000000 discoger-1.1.1/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:35:31.980555 discoger-1.1.1/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 19:35:31.000000 discoger-1.1.1/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 19:35:31.000000 discoger-1.1.1/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:35:31.000000 discoger-1.1.1/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 19:35:31.000000 discoger-1.1.1/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 19:35:31.000000 discoger-1.1.1/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 19:35:31.000000 discoger-1.1.1/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 19:35:31.980555 discoger-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-02 19:35:17.000000 discoger-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:11:26.311903 discoger-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 20:11:08.000000 discoger-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 20:11:26.315903 discoger-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-02 20:11:08.000000 discoger-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:11:26.311903 discoger-1.1.2/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:11:08.000000 discoger-1.1.2/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 20:11:08.000000 discoger-1.1.2/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-02 20:11:08.000000 discoger-1.1.2/discoger/discoger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:11:26.311903 discoger-1.1.2/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 20:11:26.000000 discoger-1.1.2/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 20:11:26.000000 discoger-1.1.2/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:11:26.000000 discoger-1.1.2/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 20:11:26.000000 discoger-1.1.2/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 20:11:26.000000 discoger-1.1.2/discoger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 20:11:26.000000 discoger-1.1.2/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 20:11:26.315903 discoger-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-02 20:11:08.000000 discoger-1.1.2/setup.py
```

### Comparing `discoger-1.1.1/LICENSE` & `discoger-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-1.1.1/PKG-INFO` & `discoger-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.1
+Version: 1.1.2
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.1.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.1.2.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.1.1/README.md` & `discoger-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `discoger-1.1.1/discoger/discoger.py` & `discoger-1.1.2/discoger/discoger.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,22 @@
 if not database_dir.exists():
     database_dir.mkdir(parents=True, exist_ok=True)
 
 token = config["telegram"]["token"]
 secret = secret = config["discogs"]["secret"]
 bot = telebot.TeleBot(token)
 
+commands = {  # command description used in the "help" command
+    '/start': 'Get used to the bot',
+    '/help': 'Gives you information about the available commands',
+    '/list': 'Show all item from your following list',
+    '/delete': 'Delete item from the following list',
+    'https://www.discogs.com/release|master/.*': 'Add release or master release in following list (ex: https://www.discogs.com/release/26741825)'
+}
+
 try:
     d = discogs_client.Client('DiscogsAlert/0.1', user_token=secret)
     me = d.identity()
 except discogs_client.exceptions.HTTPError as e:
     logging.error('Error: Unable to authenticate.')
     raise SystemExit(e)
 
@@ -57,16 +65,19 @@
     markup = types.ReplyKeyboardMarkup()
     itembtna = types.KeyboardButton('/help')
     itembtnb = types.KeyboardButton('/check')
     itembtnc = types.KeyboardButton('/list')
     itembtnd = types.KeyboardButton('/delete')
     markup.row(itembtna, itembtnb)
     markup.row(itembtnc, itembtnd)
-    msg = "What do you want?"
-    bot.send_message(chat_id, msg, reply_markup=markup)
+    help_text = "What do you want?\n"
+    for key in commands:
+        help_text += key + " "
+        help_text += commands[key] + "\n"
+    bot.send_message(chat_id, help_text, reply_markup=markup, disable_web_page_preview=True)
 
 
 @bot.message_handler(commands=['check'])
 def get_check(message):
     chat_id = message.chat.id
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     if db.get("release_list"):
```

### Comparing `discoger-1.1.1/discoger.egg-info/PKG-INFO` & `discoger-1.1.2/discoger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.1
+Version: 1.1.2
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.1.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.1.2.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.1.1/setup.py` & `discoger-1.1.2/setup.py`

 * *Files identical despite different names*

