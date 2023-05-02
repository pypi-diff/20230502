# Comparing `tmp/amino.api-1.2b6.tar.gz` & `tmp/amino.api-1.2b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.api-1.2b6.tar", last modified: Sun Apr 30 12:02:57 2023, max compression
+gzip compressed data, was "amino.api-1.2b7.tar", last modified: Tue May  2 19:00:37 2023, max compression
```

## Comparing `amino.api-1.2b6.tar` & `amino.api-1.2b7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 12:02:56.978902 amino.api-1.2b6/
--rw-rw-rw-   0        0        0      773 2023-04-30 12:02:56.978902 amino.api-1.2b6/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.2b6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 12:02:56.924304 amino.api-1.2b6/amino/
--rw-rw-rw-   0        0        0      922 2023-04-30 12:02:36.000000 amino.api-1.2b6/amino/__init__.py
--rw-rw-rw-   0        0        0       50 2023-04-21 21:48:51.000000 amino.api-1.2b6/amino/async_client.py
--rw-rw-rw-   0        0        0       56 2023-04-21 21:48:51.000000 amino.api-1.2b6/amino/async_full_client.py
--rw-rw-rw-   0        0        0       59 2023-04-21 21:48:51.000000 amino.api-1.2b6/amino/async_local_client.py
--rw-rw-rw-   0        0        0       50 2023-04-21 21:48:51.000000 amino.api-1.2b6/amino/async_socket.py
--rw-rw-rw-   0        0        0    36475 2023-04-28 13:47:41.000000 amino.api-1.2b6/amino/client.py
--rw-rw-rw-   0        0        0    18667 2023-04-30 11:43:28.000000 amino.api-1.2b6/amino/full_client.py
--rw-rw-rw-   0        0        0    10956 2023-04-28 22:02:14.000000 amino.api-1.2b6/amino/local_client.py
--rw-rw-rw-   0        0        0    11535 2023-04-21 23:43:16.000000 amino.api-1.2b6/amino/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-30 12:02:56.977911 amino.api-1.2b6/amino/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 21:48:51.000000 amino.api-1.2b6/amino/utils/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-04-28 13:22:02.000000 amino.api-1.2b6/amino/utils/exceptions.py
--rw-rw-rw-   0        0        0     7429 2023-04-22 10:56:39.000000 amino.api-1.2b6/amino/utils/helpers.py
--rw-rw-rw-   0        0        0    14849 2023-04-30 11:43:14.000000 amino.api-1.2b6/amino/utils/objects.py
--rw-rw-rw-   0        0        0     2270 2023-04-22 10:51:46.000000 amino.api-1.2b6/amino/utils/requester.py
--rw-rw-rw-   0        0        0     3660 2023-04-26 13:04:41.000000 amino.api-1.2b6/amino/utils/snippetTools.py
-drwxrwxrwx   0        0        0        0 2023-04-30 12:02:56.950239 amino.api-1.2b6/amino.api.egg-info/
--rw-rw-rw-   0        0        0      773 2023-04-30 12:02:55.000000 amino.api-1.2b6/amino.api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2023-04-30 12:02:55.000000 amino.api-1.2b6/amino.api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 12:02:55.000000 amino.api-1.2b6/amino.api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-30 12:02:55.000000 amino.api-1.2b6/amino.api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-30 12:02:55.000000 amino.api-1.2b6/amino.api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 12:02:56.980779 amino.api-1.2b6/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-04-30 12:02:24.000000 amino.api-1.2b6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:00:37.454611 amino.api-1.2b7/
+-rw-rw-rw-   0        0        0      773 2023-05-02 19:00:37.454611 amino.api-1.2b7/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.2b7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 19:00:37.397599 amino.api-1.2b7/amino/
+-rw-rw-rw-   0        0        0      922 2023-05-01 20:02:04.000000 amino.api-1.2b7/amino/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-04-21 21:48:51.000000 amino.api-1.2b7/amino/async_client.py
+-rw-rw-rw-   0        0        0       56 2023-04-21 21:48:51.000000 amino.api-1.2b7/amino/async_full_client.py
+-rw-rw-rw-   0        0        0       59 2023-04-21 21:48:51.000000 amino.api-1.2b7/amino/async_local_client.py
+-rw-rw-rw-   0        0        0       50 2023-04-21 21:48:51.000000 amino.api-1.2b7/amino/async_socket.py
+-rw-rw-rw-   0        0        0    35999 2023-05-01 19:49:27.000000 amino.api-1.2b7/amino/client.py
+-rw-rw-rw-   0        0        0    18667 2023-04-30 11:43:28.000000 amino.api-1.2b7/amino/full_client.py
+-rw-rw-rw-   0        0        0    41536 2023-05-02 17:40:15.000000 amino.api-1.2b7/amino/local_client.py
+-rw-rw-rw-   0        0        0    11535 2023-04-21 23:43:16.000000 amino.api-1.2b7/amino/socket.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:00:37.453625 amino.api-1.2b7/amino/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 21:48:51.000000 amino.api-1.2b7/amino/utils/__init__.py
+-rw-rw-rw-   0        0        0     1099 2023-04-28 13:22:02.000000 amino.api-1.2b7/amino/utils/exceptions.py
+-rw-rw-rw-   0        0        0     7429 2023-04-22 10:56:39.000000 amino.api-1.2b7/amino/utils/helpers.py
+-rw-rw-rw-   0        0        0    14913 2023-05-02 17:39:22.000000 amino.api-1.2b7/amino/utils/objects.py
+-rw-rw-rw-   0        0        0     2270 2023-04-22 10:51:46.000000 amino.api-1.2b7/amino/utils/requester.py
+-rw-rw-rw-   0        0        0     3660 2023-04-26 13:04:41.000000 amino.api-1.2b7/amino/utils/snippetTools.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:00:37.431614 amino.api-1.2b7/amino.api.egg-info/
+-rw-rw-rw-   0        0        0      773 2023-05-02 19:00:35.000000 amino.api-1.2b7/amino.api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-05-02 19:00:35.000000 amino.api-1.2b7/amino.api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:00:35.000000 amino.api-1.2b7/amino.api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-02 19:00:35.000000 amino.api-1.2b7/amino.api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 19:00:35.000000 amino.api-1.2b7/amino.api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 19:00:37.456626 amino.api-1.2b7/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-05-02 19:00:07.000000 amino.api-1.2b7/setup.py
```

### Comparing `amino.api-1.2b6/PKG-INFO` & `amino.api-1.2b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.2b6
+Version: 1.2b7
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino.API</h1>
```

### Comparing `amino.api-1.2b6/amino/__init__.py` & `amino.api-1.2b7/amino/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from json import loads
 from requests import get
 
 __title__ = 'amino.api'
 __author__ = 'Xsarz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Xsarz'
-__version__ = '1.2b6'
+__version__ = '1.2b7'
 __newest__ = loads(get("https://pypi.org/pypi/amino.api/json").text)["info"]["version"]
 
 
 
 if __version__ != __newest__:
 	s('cls || clear')
 	print(f'\033[38;5;214m{__title__} made by {__author__}\nPlease update the library. Your version: {__version__}  A new version:{__newest__}\033[0m')
```

### Comparing `amino.api-1.2b6/amino/client.py` & `amino.api-1.2b7/amino/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,21 +310,14 @@
 
 	def watch_ad(self, userId: str = None):
 		data = dumps(self.req.gen.tapjoy_data(userId if userId else self.profile.userId))
 		response = self.req.session.request("POST", "https://ads.tapdaq.com/v4/analytics/reward", proxies=self.req.proxies, verify=self.req.verify, data=data, headers=self.req.gen.tapjoy_headers)
 		return exceptions.check_exceptions(response.text) if response.status_code != 204 else response.status_code
 
 
-	def send_active_obj(self, comId: str, tz: int = None, timers: list = None):
-		#TODO
-		data = json_minify(dumps({"userActiveTimeChunkList": timers if timers else self.req.gen.timers(), "timestamp": int(timestamp() * 1000), "optInAdsFlags": 2147483647, "timezone": tz if tz else self.req.gen.timezone()}))
-		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/community/stats/user-active-time", body=data)
-		return response.status_code
-
-
 	def request_verify_code(self, email: str, resetPassword: bool = False):
 
 		data = {
 			"identity": email,
 			"type": 1,
 			"deviceID": self.req.gen.get_headers(deviceId=self.req.deviceId).get("NDCDEVICEID")
 		}
@@ -481,24 +474,24 @@
 	def get_user_info(self, userId: str):
 
 
 		response = self.req.make_request(method="GET", endpoint=f"/g/s/user-profile/{userId}")
 		return objects.UserProfile(loads(response.text)["userProfile"])
 
 
-	def get_chat_threads(self, start: int = 0, size: int = 25):
+	def get_my_chats(self, start: int = 0, size: int = 25):
 
 		response = self.req.make_request(method="GET", endpoint=f"/g/s/chat/thread?type=joined-me&start={start}&size={size}")
 		return objects.ThreadList(loads(response.text)["threadList"])
 
 
 	def get_chat_thread(self, chatId: str):
 
 		response = self.req.make_request(method="GET", endpoint=f"/g/s/chat/thread/{chatId}")
-		return objects.ThreadList(loads(response.text)["thread"])
+		return objects.Thread(loads(response.text)["thread"])
 
 
 	def get_chat_members(self, chatId: str, start: int = 0, size: int = 25, type: str = "default"):
 
 		response = self.req.make_request(method="GET", endpoint=f"/g/s/chat/thread/{chatId}/member?start={start}&size={size}&type={type}&cv=1.2")
 		return objects.userProfileList(loads(response.text)["memberList"])
 
@@ -549,16 +542,15 @@
 
 		response = self.req.make_request(method="DELETE", endpoint=f"/g/s/chat/thread/{chatId}/member/{userId}?allowRejoin={1 if allowRejoin else 0}")
 		return response.status_code
 
 
 	def get_chat_messages(self, chatId: str, size: int = 25, pageToken: str = None):
 
-		response = self.req.make_request(method="GET",
-			endpoint=f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}{f'&pageToken={pageToken}' if pageToken else ''}")
+		response = self.req.make_request(method="GET",endpoint=f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}{f'&pageToken={pageToken}' if pageToken else ''}")
 		return objects.MessageList(loads(response.text))
 
 
 	def get_message_info(self, chatId: str, messageId: str):
 
 		response = self.req.make_request(method="GET", endpoint=f"/g/s/chat/thread/{chatId}/message/{messageId}")
 		return objects.Message(loads(response.text)["message"])
@@ -720,15 +712,15 @@
 		else:
 			raise exceptions.IncorrectType(type(userId))
 
 
 
 	def unfollow(self, userId: str):
 
-		response = self.req.make_request(method="DELETE", endpoint=f"/g/s/user-profile/{userId}/member/{self.profile.userId}")
+		response = self.req.make_request(method="DELETE", endpoint=f"/g/s/user-profile/{self.profile.userId}/member/{userId}")
 		return response.status_code
 
 	def block(self, userId: str):
 
 		response = self.req.make_request(method="POST", endpoint=f"/g/s/block/{userId}")
 		return response.status_code
```

### Comparing `amino.api-1.2b6/amino/full_client.py` & `amino.api-1.2b7/amino/full_client.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b6/amino/socket.py` & `amino.api-1.2b7/amino/socket.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b6/amino/utils/exceptions.py` & `amino.api-1.2b7/amino/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b6/amino/utils/helpers.py` & `amino.api-1.2b7/amino/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b6/amino/utils/objects.py` & `amino.api-1.2b7/amino/utils/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,14 +293,15 @@
 class WikiFoldes:
 	def __init__(self, data: dict = []):
 		self.json = data
 		self.folders = list()
 		self.wikis = list()
 		self.allFolders = self.Folder(self.json.get("allEntriesItemCategory", {}))
 		self.itemCategory = self.Folder(self.json.get("itemCategory", {}))
+		self.type = self.json.get("childrenWrapper", {}).get("type")
 		for folder in self.json.get("itemCategoryList", []) if self.json.get("itemCategoryList") else self.json.get("childrenWrapper", {}).get("itemCategoryList", []):
 			self.folders.append(self.Folder(folder))
 		for wiki in self.json.get("childrenWrapper", {}).get("itemList", []):
 			self.wikis.append(self.Wiki(wiki))
```

### Comparing `amino.api-1.2b6/amino/utils/requester.py` & `amino.api-1.2b7/amino/utils/requester.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b6/amino/utils/snippetTools.py` & `amino.api-1.2b7/amino/utils/snippetTools.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b6/amino.api.egg-info/PKG-INFO` & `amino.api-1.2b7/amino.api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.2b6
+Version: 1.2b7
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino.API</h1>
```

### Comparing `amino.api-1.2b6/amino.api.egg-info/SOURCES.txt` & `amino.api-1.2b7/amino.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b6/setup.py` & `amino.api-1.2b7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 info = {
 	"name": "amino.api",
-	"version": "1.2b6",
+	"version": "1.2b7",
 	"github_page": "https://github.com/xXxCLOTIxXx/amino.api",
 	"download_link": "https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip",
 	"license": "MIT",
 	"author": "Xsarz",
 	"author_email": "xsarzy@gmail.com",
 	"description": "Library for creating amino bots and scripts.",
 	"long_description": None,
```

