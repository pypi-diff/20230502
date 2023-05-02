# Comparing `tmp/discoger-1.1.0.tar.gz` & `tmp/discoger-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-1.1.0.tar", last modified: Tue May  2 18:35:34 2023, max compression
+gzip compressed data, was "discoger-1.1.1.tar", last modified: Tue May  2 19:35:31 2023, max compression
```

## Comparing `discoger-1.1.0.tar` & `discoger-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:34.640970 discoger-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 18:35:17.000000 discoger-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 18:35:34.640970 discoger-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-02 18:35:17.000000 discoger-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:34.640970 discoger-1.1.0/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:17.000000 discoger-1.1.0/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 18:35:17.000000 discoger-1.1.0/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-02 18:35:17.000000 discoger-1.1.0/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:34.640970 discoger-1.1.0/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 18:35:34.000000 discoger-1.1.0/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 18:35:34.000000 discoger-1.1.0/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:35:34.000000 discoger-1.1.0/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 18:35:34.000000 discoger-1.1.0/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 18:35:34.000000 discoger-1.1.0/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 18:35:34.000000 discoger-1.1.0/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 18:35:34.640970 discoger-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-02 18:35:17.000000 discoger-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:35:31.980555 discoger-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 19:35:17.000000 discoger-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 19:35:31.980555 discoger-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-02 19:35:17.000000 discoger-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:35:31.980555 discoger-1.1.1/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:35:17.000000 discoger-1.1.1/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 19:35:17.000000 discoger-1.1.1/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-05-02 19:35:17.000000 discoger-1.1.1/discoger/discoger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:35:31.980555 discoger-1.1.1/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 19:35:31.000000 discoger-1.1.1/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 19:35:31.000000 discoger-1.1.1/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:35:31.000000 discoger-1.1.1/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 19:35:31.000000 discoger-1.1.1/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 19:35:31.000000 discoger-1.1.1/discoger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 19:35:31.000000 discoger-1.1.1/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 19:35:31.980555 discoger-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-02 19:35:17.000000 discoger-1.1.1/setup.py
```

### Comparing `discoger-1.1.0/LICENSE` & `discoger-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-1.1.0/PKG-INFO` & `discoger-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.0
+Version: 1.1.1
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.0.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.1.1.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.1.0/README.md` & `discoger-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `discoger-1.1.0/discoger/discoger.py` & `discoger-1.1.1/discoger/discoger.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import logging
 logging.basicConfig(format='%(asctime)s %(levelname)s - %(message)s', level=logging.INFO)
 
 home = str(Path.home())
 config_file = Path(home + "/.config/discoger/config.ini")
 database_dir = Path(home + "/.config/discoger/databases")
-
+discogs_url = 'https://www.discogs.com'
 
 if config_file.exists():
     config = configparser.ConfigParser()
     config.read(config_file)
 else:
     logging.error("No config file, please create a config file follwing example")
     raise SystemExit()
@@ -106,15 +106,18 @@
 @bot.message_handler(commands=['list'])
 def get_list(message):
     chat_id = message.chat.id
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     id_list = 0
     all_text = ""
     for i in db["release_list"]:
-        text = "%s: %s - %s %s" % (id_list, i["artist"], i["title"], i["url"])
+        sell_type = i.get("type")
+        if sell_type is None:
+            sell_type = "release"
+        text = "%s: %s - %s %s/%s/%s" % (id_list, i["artist"], i["title"], discogs_url, sell_type, i["release_id"])
         all_text = all_text + "\n" + text
         id_list = id_list + 1
     splitted_text = util.split_string(all_text, 3000)
     for text in splitted_text:
         bot.send_message(chat_id, text, disable_web_page_preview=True)
 
 
@@ -133,17 +136,17 @@
     db.save()
     bot.send_message(chat_id, "% is deleted in following list" % (id_item))
 
 
 def get_info(release_id, type_sell):
     data_last_sell = dict()
     if type_sell == 'master':
-        url = f"https://www.discogs.com/fr/sell/mplistrss?output=rss&master_id={release_id}&ev=mb&format=Vinyl"
+        url = f"{discogs_url}/sell/mplistrss?output=rss&master_id={release_id}&ev=mb&format=Vinyl"
     else:
-        url = f"https://www.discogs.com/fr/sell/mplistrss?output=rss&release_id={release_id}"
+        url = f"{discogs_url}/sell/mplistrss?output=rss&release_id={release_id}"
     feed = feedparser.parse(url)
     try:
         entry = feed.entries[-1]
         data_last_sell["id"] = re.findall(r'\d+', entry["link"])[0]
         data_last_sell["date"] = entry["updated"]
         data_last_sell["url"] = entry["link"]
         data_last_sell["price"] = re.findall(r'... \d?\d?\d\d.\d\d', entry["summary_detail"]["value"])[0]
@@ -166,15 +169,18 @@
 
 
 def scrap_data(chat_id):
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     chat_id = db.get("chat_id")
     for i in range(len(db["release_list"])):
         item = db.search("release_list[%s]" % (str(i)))
-        data_last_sell = get_info(item["release_id"], item["type"])
+        sell_type = item.get("type")
+        if sell_type is None:
+            sell_type = "release"
+        data_last_sell = get_info(item["release_id"], sell_type)
         if data_last_sell:
             if not item["last_sell"] or (item["last_sell"]["id"] != data_last_sell["id"] and item["last_sell"]["date"] < data_last_sell["date"]):
                 logging.info("New item for %s - %s" % (item["artist"], item["title"]))
                 text = "New release for:\n%s - %s\ndate: %s\nprice: %s\n%s" % (item["artist"], item["title"], data_last_sell["date"], data_last_sell["price"], data_last_sell["url"])
                 bot.send_message(chat_id, text, disable_web_page_preview=False)
                 db["release_list"][i]["last_sell"] = data_last_sell
             else:
```

### Comparing `discoger-1.1.0/discoger.egg-info/PKG-INFO` & `discoger-1.1.1/discoger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.0
+Version: 1.1.1
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.0.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.1.1.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.1.0/setup.py` & `discoger-1.1.1/setup.py`

 * *Files identical despite different names*

