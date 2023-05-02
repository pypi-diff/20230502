# Comparing `tmp/discoger-1.0.5.tar.gz` & `tmp/discoger-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-1.0.5.tar", last modified: Tue May  2 15:02:51 2023, max compression
+gzip compressed data, was "discoger-1.1.0.tar", last modified: Tue May  2 18:35:34 2023, max compression
```

## Comparing `discoger-1.0.5.tar` & `discoger-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:02:51.986456 discoger-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 15:02:38.000000 discoger-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-02 15:02:51.986456 discoger-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-02 15:02:38.000000 discoger-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:02:51.986456 discoger-1.0.5/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:02:38.000000 discoger-1.0.5/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 15:02:38.000000 discoger-1.0.5/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-02 15:02:38.000000 discoger-1.0.5/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:02:51.986456 discoger-1.0.5/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-02 15:02:51.000000 discoger-1.0.5/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 15:02:51.000000 discoger-1.0.5/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:02:51.000000 discoger-1.0.5/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 15:02:51.000000 discoger-1.0.5/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 15:02:51.000000 discoger-1.0.5/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 15:02:51.000000 discoger-1.0.5/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 15:02:51.986456 discoger-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-02 15:02:38.000000 discoger-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:34.640970 discoger-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 18:35:17.000000 discoger-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 18:35:34.640970 discoger-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-02 18:35:17.000000 discoger-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:34.640970 discoger-1.1.0/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:17.000000 discoger-1.1.0/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 18:35:17.000000 discoger-1.1.0/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-02 18:35:17.000000 discoger-1.1.0/discoger/discoger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:34.640970 discoger-1.1.0/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-02 18:35:34.000000 discoger-1.1.0/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 18:35:34.000000 discoger-1.1.0/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:35:34.000000 discoger-1.1.0/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 18:35:34.000000 discoger-1.1.0/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 18:35:34.000000 discoger-1.1.0/discoger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 18:35:34.000000 discoger-1.1.0/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 18:35:34.640970 discoger-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-02 18:35:17.000000 discoger-1.1.0/setup.py
```

### Comparing `discoger-1.0.5/LICENSE` & `discoger-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-1.0.5/discoger/discoger.py` & `discoger-1.1.0/discoger/discoger.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,26 +74,31 @@
         check_discogs(chat_id)
     else:
         db["release_list"] = list()
         db.save()
         bot.send_message(chat_id, "Your discoger following list is empty, send me item url first")
 
 
-@bot.message_handler(regexp="^https://www.discogs.com/.*release/.*")
+@bot.message_handler(regexp="^https://www.discogs.com/.*(release|master)/.*")
 def handle_message(message):
     release_info = dict()
     chat_id = message.chat.id
     release_id = re.findall(r'\d+', message.text)[0]
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     if not db.search("release_list[?release_id=='%s']" % (release_id)):
         relase_all_info = d.release(release_id)
         db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
         release_info["release_id"] = release_id
         release_info["artist"] = relase_all_info.artists[0].name
         release_info["title"] = relase_all_info.title
+        release_info["url"] = message.text
+        if len(re.findall(r'\/master\/\d+', message.text)) == 1:
+            release_info["type"] = "master"
+        else:
+            release_info["type"] = "release"
         release_info["last_sell"] = dict()
         db["release_list"].append(release_info)
         db.save()
         bot.send_message(chat_id, "%s is added in following list" % (release_id))
     else:
         bot.send_message(chat_id, "%s is already in following list" % (release_id))
 
@@ -101,15 +106,15 @@
 @bot.message_handler(commands=['list'])
 def get_list(message):
     chat_id = message.chat.id
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     id_list = 0
     all_text = ""
     for i in db["release_list"]:
-        text = "%s: %s - %s https://www.discogs.com/fr/release/%s" % (id_list, i["artist"], i["title"], i["release_id"])
+        text = "%s: %s - %s %s" % (id_list, i["artist"], i["title"], i["url"])
         all_text = all_text + "\n" + text
         id_list = id_list + 1
     splitted_text = util.split_string(all_text, 3000)
     for text in splitted_text:
         bot.send_message(chat_id, text, disable_web_page_preview=True)
 
 
@@ -125,17 +130,20 @@
     id_item = message.text
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     db["release_list"].pop(int(id_item))
     db.save()
     bot.send_message(chat_id, "% is deleted in following list" % (id_item))
 
 
-def get_info(release_id):
+def get_info(release_id, type_sell):
     data_last_sell = dict()
-    url = f"https://www.discogs.com/fr/sell/mplistrss?output=rss&release_id={release_id}"
+    if type_sell == 'master':
+        url = f"https://www.discogs.com/fr/sell/mplistrss?output=rss&master_id={release_id}&ev=mb&format=Vinyl"
+    else:
+        url = f"https://www.discogs.com/fr/sell/mplistrss?output=rss&release_id={release_id}"
     feed = feedparser.parse(url)
     try:
         entry = feed.entries[-1]
         data_last_sell["id"] = re.findall(r'\d+', entry["link"])[0]
         data_last_sell["date"] = entry["updated"]
         data_last_sell["url"] = entry["link"]
         data_last_sell["price"] = re.findall(r'... \d?\d?\d\d.\d\d', entry["summary_detail"]["value"])[0]
@@ -158,15 +166,15 @@
 
 
 def scrap_data(chat_id):
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     chat_id = db.get("chat_id")
     for i in range(len(db["release_list"])):
         item = db.search("release_list[%s]" % (str(i)))
-        data_last_sell = get_info(item["release_id"])
+        data_last_sell = get_info(item["release_id"], item["type"])
         if data_last_sell:
             if not item["last_sell"] or (item["last_sell"]["id"] != data_last_sell["id"] and item["last_sell"]["date"] < data_last_sell["date"]):
                 logging.info("New item for %s - %s" % (item["artist"], item["title"]))
                 text = "New release for:\n%s - %s\ndate: %s\nprice: %s\n%s" % (item["artist"], item["title"], data_last_sell["date"], data_last_sell["price"], data_last_sell["url"])
                 bot.send_message(chat_id, text, disable_web_page_preview=False)
                 db["release_list"][i]["last_sell"] = data_last_sell
             else:
```

### Comparing `discoger-1.0.5/setup.py` & `discoger-1.1.0/setup.py`

 * *Files identical despite different names*

