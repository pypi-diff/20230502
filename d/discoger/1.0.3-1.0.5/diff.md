# Comparing `tmp/discoger-1.0.3.tar.gz` & `tmp/discoger-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-1.0.3.tar", last modified: Sun Apr 23 17:19:47 2023, max compression
+gzip compressed data, was "discoger-1.0.5.tar", last modified: Tue May  2 15:02:51 2023, max compression
```

## Comparing `discoger-1.0.3.tar` & `discoger-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:19:47.436839 discoger-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 17:19:34.000000 discoger-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-23 17:19:47.436839 discoger-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-23 17:19:34.000000 discoger-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:19:47.436839 discoger-1.0.3/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:19:34.000000 discoger-1.0.3/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-23 17:19:34.000000 discoger-1.0.3/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-04-23 17:19:34.000000 discoger-1.0.3/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:19:47.436839 discoger-1.0.3/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-23 17:19:47.000000 discoger-1.0.3/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-23 17:19:47.000000 discoger-1.0.3/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:19:47.000000 discoger-1.0.3/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 17:19:47.000000 discoger-1.0.3/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 17:19:47.000000 discoger-1.0.3/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 17:19:47.000000 discoger-1.0.3/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 17:19:47.436839 discoger-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-23 17:19:34.000000 discoger-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:02:51.986456 discoger-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 15:02:38.000000 discoger-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-02 15:02:51.986456 discoger-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-02 15:02:38.000000 discoger-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:02:51.986456 discoger-1.0.5/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:02:38.000000 discoger-1.0.5/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 15:02:38.000000 discoger-1.0.5/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-02 15:02:38.000000 discoger-1.0.5/discoger/discoger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:02:51.986456 discoger-1.0.5/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-02 15:02:51.000000 discoger-1.0.5/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 15:02:51.000000 discoger-1.0.5/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:02:51.000000 discoger-1.0.5/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 15:02:51.000000 discoger-1.0.5/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 15:02:51.000000 discoger-1.0.5/discoger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 15:02:51.000000 discoger-1.0.5/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 15:02:51.986456 discoger-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-02 15:02:38.000000 discoger-1.0.5/setup.py
```

### Comparing `discoger-1.0.3/LICENSE` & `discoger-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-1.0.3/PKG-INFO` & `discoger-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.0.3
+Version: 1.0.5
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.0.3.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.0.5.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
         
-        Installation is in three steps, the first is getting credentials from Discogs and Telegram. 
+        Installation is in three steps, the first is getting credentials from Discogs and Telegram.
         You need to create a [Token](https://www.discogs.com/fr/settings/developers).
         
-        For Telegram you need contact []@BotFather](https://t.me/botfather) and follow a few simple steps for get your authorization token.
+        For Telegram you need contact [@BotFather](https://t.me/botfather) and follow a few simple steps for get your authorization token.
         
         ### Configuration
         
         After that you need create config.ini file
         
         ```
         [DEFAULT]
         schedule_time = 30
         
         [discogs]
         secret = dbPVkGbCVVffggfgkdfgmlkknzezsbhmscskncno
-         
+        
         [telegram]
         token = 1766763279:AAFwufBsdfdsfgdfsgfgsfsgdfgsdf
         ```
         
         ### Docker
         
         ```
```

### Comparing `discoger-1.0.3/README.md` & `discoger-1.0.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 Telegram bot for checking if there are new sell in one specific list on Discogs
 
 ## How to use it
 
 ### Installation
 
-Installation is in three steps, the first is getting credentials from Discogs and Telegram. 
+Installation is in three steps, the first is getting credentials from Discogs and Telegram.
 You need to create a [Token](https://www.discogs.com/fr/settings/developers).
 
-For Telegram you need contact []@BotFather](https://t.me/botfather) and follow a few simple steps for get your authorization token.
+For Telegram you need contact [@BotFather](https://t.me/botfather) and follow a few simple steps for get your authorization token.
 
 ### Configuration
 
 After that you need create config.ini file
 
 ```
 [DEFAULT]
 schedule_time = 30
 
 [discogs]
 secret = dbPVkGbCVVffggfgkdfgmlkknzezsbhmscskncno
- 
+
 [telegram]
 token = 1766763279:AAFwufBsdfdsfgdfsgfgsfsgdfgsdf
 ```
 
 ### Docker
 
 ```
```

### Comparing `discoger-1.0.3/discoger/discoger.py` & `discoger-1.0.5/discoger/discoger.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,16 +162,16 @@
     chat_id = db.get("chat_id")
     for i in range(len(db["release_list"])):
         item = db.search("release_list[%s]" % (str(i)))
         data_last_sell = get_info(item["release_id"])
         if data_last_sell:
             if not item["last_sell"] or (item["last_sell"]["id"] != data_last_sell["id"] and item["last_sell"]["date"] < data_last_sell["date"]):
                 logging.info("New item for %s - %s" % (item["artist"], item["title"]))
-                text = "New release for :\n%s\ndate: %s\nprice: %s\n%s" % (item["title"], data_last_sell["date"], data_last_sell["price"], data_last_sell["url"])
-                bot.send_message(chat_id, text)
+                text = "New release for:\n%s - %s\ndate: %s\nprice: %s\n%s" % (item["artist"], item["title"], data_last_sell["date"], data_last_sell["price"], data_last_sell["url"])
+                bot.send_message(chat_id, text, disable_web_page_preview=False)
                 db["release_list"][i]["last_sell"] = data_last_sell
             else:
                 logging.info("Not new item for %s - %s" % (db["release_list"][i]["artist"], db["release_list"][i]["title"]))
         else:
             logging.info("Nothing available for %s - %s" % (db["release_list"][i]["artist"], db["release_list"][i]["title"]))
     db.save()
```

### Comparing `discoger-1.0.3/discoger.egg-info/PKG-INFO` & `discoger-1.0.5/discoger.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.0.3
+Version: 1.0.5
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.0.3.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.0.5.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
         
-        Installation is in three steps, the first is getting credentials from Discogs and Telegram. 
+        Installation is in three steps, the first is getting credentials from Discogs and Telegram.
         You need to create a [Token](https://www.discogs.com/fr/settings/developers).
         
-        For Telegram you need contact []@BotFather](https://t.me/botfather) and follow a few simple steps for get your authorization token.
+        For Telegram you need contact [@BotFather](https://t.me/botfather) and follow a few simple steps for get your authorization token.
         
         ### Configuration
         
         After that you need create config.ini file
         
         ```
         [DEFAULT]
         schedule_time = 30
         
         [discogs]
         secret = dbPVkGbCVVffggfgkdfgmlkknzezsbhmscskncno
-         
+        
         [telegram]
         token = 1766763279:AAFwufBsdfdsfgdfsgfgsfsgdfgsdf
         ```
         
         ### Docker
         
         ```
```

### Comparing `discoger-1.0.3/setup.py` & `discoger-1.0.5/setup.py`

 * *Files identical despite different names*

