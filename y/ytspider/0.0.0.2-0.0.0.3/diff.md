# Comparing `tmp/ytspider-0.0.0.2.tar.gz` & `tmp/ytspider-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytspider-0.0.0.2.tar", last modified: Sun Apr 30 20:46:22 2023, max compression
+gzip compressed data, was "ytspider-0.0.0.3.tar", last modified: Tue May  2 17:37:29 2023, max compression
```

## Comparing `ytspider-0.0.0.2.tar` & `ytspider-0.0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 20:46:22.756679 ytspider-0.0.0.2/
--rw-rw-rw-   0        0        0      377 2023-04-30 20:46:22.756679 ytspider-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-04-30 18:25:19.000000 ytspider-0.0.0.2/README.md
--rw-rw-rw-   0        0        0      115 2023-04-30 20:46:22.757672 ytspider-0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-04-30 20:46:15.000000 ytspider-0.0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 20:46:22.691512 ytspider-0.0.0.2/src/
--rw-rw-rw-   0        0        0       45 2023-04-30 20:45:34.000000 ytspider-0.0.0.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 20:46:22.739201 ytspider-0.0.0.2/src/utils/
--rw-rw-rw-   0        0        0        0 2023-04-30 20:26:12.000000 ytspider-0.0.0.2/src/utils/__init__.py
--rw-rw-rw-   0        0        0     1969 2023-04-30 11:28:54.000000 ytspider-0.0.0.2/src/utils/client.py
--rw-rw-rw-   0        0        0     1620 2023-04-30 19:47:31.000000 ytspider-0.0.0.2/src/utils/context.py
--rw-rw-rw-   0        0        0     2984 2023-04-30 19:47:34.000000 ytspider-0.0.0.2/src/utils/decorator.py
--rw-rw-rw-   0        0        0     7572 2023-04-30 19:47:25.000000 ytspider-0.0.0.2/src/utils/handler.py
--rw-rw-rw-   0        0        0      707 2023-04-30 11:29:20.000000 ytspider-0.0.0.2/src/utils/playback_context.py
--rw-rw-rw-   0        0        0     2567 2023-04-30 19:47:40.000000 ytspider-0.0.0.2/src/utils/request.py
--rw-rw-rw-   0        0        0      951 2023-04-30 11:18:54.000000 ytspider-0.0.0.2/src/utils/signals_info.py
--rw-rw-rw-   0        0        0     5788 2023-04-30 20:20:02.000000 ytspider-0.0.0.2/src/ytspider.py
-drwxrwxrwx   0        0        0        0 2023-04-30 20:46:22.754667 ytspider-0.0.0.2/ytspider.egg-info/
--rw-rw-rw-   0        0        0      377 2023-04-30 20:46:22.000000 ytspider-0.0.0.2/ytspider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-04-30 20:46:22.000000 ytspider-0.0.0.2/ytspider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 20:46:22.000000 ytspider-0.0.0.2/ytspider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 20:46:22.000000 ytspider-0.0.0.2/ytspider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 20:46:22.000000 ytspider-0.0.0.2/ytspider.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 17:37:29.650541 ytspider-0.0.0.3/
+-rw-rw-rw-   0        0        0      377 2023-05-02 17:37:29.650541 ytspider-0.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-04-30 18:25:19.000000 ytspider-0.0.0.3/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-02 17:37:29.650541 ytspider-0.0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-05-02 17:36:59.000000 ytspider-0.0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:37:29.555648 ytspider-0.0.0.3/src/
+-rw-rw-rw-   0        0        0       45 2023-04-30 20:45:34.000000 ytspider-0.0.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:37:29.618361 ytspider-0.0.0.3/src/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-30 20:26:12.000000 ytspider-0.0.0.3/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     1969 2023-04-30 11:28:54.000000 ytspider-0.0.0.3/src/utils/client.py
+-rw-rw-rw-   0        0        0     1670 2023-05-01 20:14:19.000000 ytspider-0.0.0.3/src/utils/context.py
+-rw-rw-rw-   0        0        0     2938 2023-05-01 20:13:59.000000 ytspider-0.0.0.3/src/utils/decorator.py
+-rw-rw-rw-   0        0        0     7605 2023-05-02 17:30:12.000000 ytspider-0.0.0.3/src/utils/handler.py
+-rw-rw-rw-   0        0        0      707 2023-04-30 11:29:20.000000 ytspider-0.0.0.3/src/utils/playback_context.py
+-rw-rw-rw-   0        0        0     2607 2023-05-02 00:21:25.000000 ytspider-0.0.0.3/src/utils/request.py
+-rw-rw-rw-   0        0        0      951 2023-04-30 11:18:54.000000 ytspider-0.0.0.3/src/utils/signals_info.py
+-rw-rw-rw-   0        0        0     6866 2023-05-02 16:57:42.000000 ytspider-0.0.0.3/src/ytspider.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:37:29.649735 ytspider-0.0.0.3/ytspider.egg-info/
+-rw-rw-rw-   0        0        0      377 2023-05-02 17:37:29.000000 ytspider-0.0.0.3/ytspider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-05-02 17:37:29.000000 ytspider-0.0.0.3/ytspider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:37:29.000000 ytspider-0.0.0.3/ytspider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 17:37:29.000000 ytspider-0.0.0.3/ytspider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 17:37:29.000000 ytspider-0.0.0.3/ytspider.egg-info/top_level.txt
```

### Comparing `ytspider-0.0.0.2/README.md` & `ytspider-0.0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.2/setup.py` & `ytspider-0.0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='ytspider',
     description="YouTube scraper, videos, channels, playlists, comments and transcriptions",
-    version='0.0.0.2',
+    version='0.0.0.3',
     license='MIT',
     author="Zeyad Khalid",
     maintainer_email='zeyad.khalid@must.edu.eg',
     author_email='zeyadpro99@gmail.com',
     package_dir={"ytspider":"src"},
     packages=find_packages(),#["ytspider","ytspider.utils"],
     py_modules=["ytspider.py"],
```

### Comparing `ytspider-0.0.0.2/src/utils/client.py` & `ytspider-0.0.0.3/src/utils/client.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.2/src/utils/context.py` & `ytspider-0.0.0.3/src/utils/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,22 +26,26 @@
     def replace(self, key, value):
         context_str = json.dumps(self.context)
         context_str = context_str.replace(key, value)
         self.context = json.loads(context_str)
         return self
 
     def replaceVideoId(self, value):
-        return self.replace(self.defaultId, value)
+        self.replace(self.defaultId, value)
+        self.defaultId = value
+        return self
 
     def add(self, key, value):
         self.context[key] = value
         return self
 
     def remove(self, key):
         del self.context[key]
         return self
 
     def get(self):
         return self.context
 
     def getDefaultVideoId(self):
         return self.defaultId
+
+
```

### Comparing `ytspider-0.0.0.2/src/utils/decorator.py` & `ytspider-0.0.0.3/src/utils/decorator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .handler import *
 
+
 class ScrapingDecorator:
     def __init__(self, defaultHandler=BaseHandler()):
 
         if not isinstance(defaultHandler, BaseHandler):
             raise ValueError(
                 "Argument (defaultHandler) must be a subclass of BaseHandler or 'scrape' or 'ignore'")
  
@@ -25,23 +26,23 @@
         self.attachHandler(handler)
 
 class VideosScraper(ScrapingDecorator):
     def __init__(self, videosDefaultHandler=VideosDefaultHandler()):
         if videosDefaultHandler is None or commentDefaultHandler == 'ignore':
             videosDefaultHandler = VideosDefaultHandler()
         elif videosDefaultHandler == 'scrape':
-            videosDefaultHandler = VideosScrapingHandler(self.itemId)
+            videosDefaultHandler = VideosScrapingHandler()
 
         super(VideosScraper, self).__init__(videosDefaultHandler)
 
         self.updateHandler(videosDefaultHandler)
 
     def withVideos(self, n_videos=29):
 
-        handler = VideosScrapingHandler(self.itemId, n_videos=n_videos)
+        handler = VideosScrapingHandler(n_videos=n_videos)
         self.updateHandler(handler)
         return self
 
 
 class TranscriptScraper(ScrapingDecorator):
     def __init__(self, transcriptDefaultHandler=TranscriptionDefaultHandler()):
         if transcriptDefaultHandler is None or transcriptDefaultHandler == 'ignore':
@@ -58,18 +59,18 @@
         return self
 
 class CommentScraper(ScrapingDecorator):
     def __init__(self, commentDefaultHandler=CommentDefaultHandler()):
         if commentDefaultHandler is None or commentDefaultHandler == 'ignore':
             commentDefaultHandler = CommentDefaultHandler()
         elif commentDefaultHandler == 'scrape':
-            commentDefaultHandler = CommentScrapingHandler(self.itemId)
+            commentDefaultHandler = CommentScrapingHandler()
 
         super(CommentScraper, self).__init__(commentDefaultHandler)
 
         self.updateHandler(commentDefaultHandler)
 
     def withComments(self, n_comments=15):
 
-        handler = CommentScrapingHandler(self.itemId, n_comments=n_comments)
+        handler = CommentScrapingHandler(n_comments=n_comments)
         self.updateHandler(handler)
         return self
```

### Comparing `ytspider-0.0.0.2/src/utils/handler.py` & `ytspider-0.0.0.3/src/utils/handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,137 +1,140 @@
 from .request import Request
 
 class BaseHandler:
     def __init__(self, name=None):
         self.request = Request()
         self.name = name
 
-    def execute(self):
+    def execute(self, itemId):
 
         return None
 
 
 
 class CommentHandler(BaseHandler):
     def __init__(self, n_comments=0):
         super(CommentHandler, self).__init__(name='comments')
         self.n_comments = n_comments
 
-    def execute(self):
+    def execute(self, itemId):
         return None
 
 
 class CommentDefaultHandler(CommentHandler):
     def __init__(self, n_comments=0):
         super(CommentDefaultHandler, self).__init__(n_comments)
 
-    def execute(self):
+    def execute(self, itemId):
 
         return None
 
 
 class CommentScrapingHandler(CommentHandler):
-    def __init__(self, videoId, n_comments=100):
+    def __init__(self, n_comments=100):
         super(CommentScrapingHandler, self).__init__(n_comments)
-        self.videoId = videoId
         self.url = "https://www.youtube.com/youtubei/v1/next?key=AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8&prettyPrint=false"
 
-    def execute(self):
-        self.request.updateContextState(
-            self.videoId, additional={"continuation": ""})
+    def execute(self, itemId):
+        self.request.updateContextState(itemId, additional={"continuation": ""})
         firstTime = True
         token = ""
         all_comments = []
         while token is not None and len(all_comments) < self.n_comments:
             self.request.updateContextState(additional={"continuation": token})
             result = self.request.send(self.url, method="POST")
             if firstTime:
-                token = result["contents"]["twoColumnWatchNextResults"]["results"]["results"]["contents"][3]["itemSectionRenderer"][
-                    "contents"][0]["continuationItemRenderer"]["continuationEndpoint"]["continuationCommand"]["token"]
-                firstTime = False
+                # Try get token for comment retrieval
+                try:
+                    token = result["contents"]["twoColumnWatchNextResults"]["results"]["results"]["contents"][3]["itemSectionRenderer"]["contents"][0]["continuationItemRenderer"]["continuationEndpoint"]["continuationCommand"]["token"]
+                    firstTime = False
+                # Couldn't get token for comment retrieval
+                except Exception as e:
+                    token = None
             else:
+                # Try get comments
                 try:
-                    token = result["onResponseReceivedEndpoints"][-1]["reloadContinuationItemsCommand"]["continuationItems"][-1][
-                        "continuationItemRenderer"]["continuationEndpoint"]["continuationCommand"]["token"]
                     comments = result["onResponseReceivedEndpoints"][-1]["reloadContinuationItemsCommand"]["continuationItems"][:-1]
-                except:
-                    try:
-                        token = result["onResponseReceivedEndpoints"][-1]["appendContinuationItemsAction"]["continuationItems"][-1][
-                            "continuationItemRenderer"]["continuationEndpoint"]["continuationCommand"]["token"]
-                    except:
-                        token = None
-                    try:
-                        comments = result["onResponseReceivedEndpoints"][-1]["appendContinuationItemsAction"]["continuationItems"][:-1]
-                    except:
-                        comments = []
+                
+                # There are no comments at all (not a single one!)
+                except Exception as e:
+                    comments = []
+                
+                # Try get token, but if comments are < 20, there is no 'continuation' token because there're no more comments
+                try:
+                    token = result["onResponseReceivedEndpoints"][-1]["reloadContinuationItemsCommand"]["continuationItems"][-1]["commentThreadRenderer"]["continuationEndpoint"]["continuationCommand"]["token"]
+                
+                # No more comments
+                except Exception as e:
+                    token = None
+
                 for i in range(len(comments)):
                     comment_texts = comments[i]["commentThreadRenderer"]["comment"]["commentRenderer"]["contentText"]['runs']
                     comment = " ".join(
                         list(map(lambda c: c["text"], comment_texts)))
                     all_comments.append(comment)
         return all_comments
 
 
 
 class TranscriptionHandler(BaseHandler):
     def __init__(self, only_in_langs=[]):
         super(TranscriptionHandler, self).__init__(name='transcripts')
         self.only_in_langs = only_in_langs
 
-    def execute(self):
+    def execute(self, itemId):
         return None
 
 
 class TranscriptionScrapingHandler(TranscriptionHandler):
     def __init__(self, only_in_langs=[]):
         super(TranscriptionScrapingHandler, self).__init__(only_in_langs)
 
-    def execute(self):
+    def execute(self, itemId):
         result = ["One Two THree"]
         return result
 
 
 class TranscriptionDefaultHandler(TranscriptionHandler):
     def __init__(self):
         super(TranscriptionDefaultHandler, self).__init__()
 
-    def execute(self):
+    def execute(self, itemId):
         return None
 
 
 class VideosHandler(BaseHandler):
     def __init__(self, n_videos=0):
         super(VideosHandler, self).__init__(name='videos')
         self.n_videos = n_videos
 
-    def execute(self):
+    def execute(self, itemId):
         return None
 
 
 class VideosDefaultHandler(VideosHandler):
     def __init__(self, n_videos=0):
         super(VideosDefaultHandler, self).__init__(n_videos)
 
-    def execute(self):
+    def execute(self, itemId):
         return None
 
 
 class VideosScrapingHandler(VideosHandler):
-    def __init__(self, itemId, n_videos=29):
+    def __init__(self, n_videos=29):
         super(VideosScrapingHandler, self).__init__(n_videos)
-        self.channelId = itemId
         self.url = "https://www.youtube.com/youtubei/v1/browse?key=AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8&prettyPrint=false"
 
-    def execute(self):
+    def execute(self, itemId):
         params_token = ""
         firstTime = True
         token = ""
         all_videos = []
 
-        self.request.updateContextState(additional={"browseId": self.channelId, "params": params_token})
+        self.request.updateContextState(additional={"browseId": itemId, "params": params_token})
         # Scrape MainPage tab
         result = self.request.send(self.url, "POST")
 
         try:
             # Get param which will route the scraping to Videos Tab
             tabs = result["contents"]["twoColumnBrowseResultsRenderer"]["tabs"]
             if len(tabs) > 2 and tabs[1]["tabRenderer"]["title"] == "Videos":
@@ -154,15 +157,15 @@
                         video["publish_at"] = vidRender["publishedTimeText"]["simpleText"]
 
                         if len(all_videos) >= self.n_videos:
                             return all_videos
                         all_videos.append(video)
                     try:
                         # Set Continuation Parameter
-                        continuationParam = videoItems[-1]["continuationItemRenderer"]["continuationEndpoint"]["continuationCommand"]["token"]
+                        continuationParam = videoItems[-1]["commentThreadRenderer"]["continuationEndpoint"]["continuationCommand"]["token"]
                     except Exception as e:
                         print(e)
                         break
                     self.request.updateContextState(additional={"continuation":continuationParam})
                     result = self.request.send(self.url, "POST")
                     try:
                         videoItems = result["onResponseReceivedActions"][0]["appendContinuationItemsAction"]["continuationItems"]
```

### Comparing `ytspider-0.0.0.2/src/utils/playback_context.py` & `ytspider-0.0.0.3/src/utils/playback_context.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.2/src/utils/request.py` & `ytspider-0.0.0.3/src/utils/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 
 
 from .context import Context
 
-
+from bs4 import BeautifulSoup
 class Request:
     def __init__(self):
         self.__Context = Context()
         self.__initHeaders()
 
     def __initHeaders(self):
         self.headers = {
@@ -21,15 +21,15 @@
 
     def removeHeaders(self, headerNames):
         for key in headerNames:
             self.headers.pop(key)
 
     def updateContextState(self, videoId=None, replacables={}, additional={}, removables=[]):
         if videoId is not None:
-            self.__Context.replace(self.__Context.defaultId, videoId)
+            self.__Context.replaceVideoId(videoId)
         for key, val in replacables.items():
             if key in self.__Context:
                 self.__Context[key] = val
             else:
                 self.__Context.replace(key, val)
 
         for key, val in additional.items():
@@ -55,26 +55,28 @@
 
         # Merge payloads
         payload = self.__Context.get()
         # if additional_payload is not None and type(additional_payload) == dict:
         #     payt
         #     payload.update(additional_payload)
         if method.upper() == "GET":
-            response = requests.get(url, headers=self.headers)
+            response = requests.get(url, headers = {
+                "Accept":"text/html"
+            })
 
         elif method.upper() == "POST":
             response = requests.post(
                 url,
                 json=payload,
                 headers=self.headers
             )
-        # print(payload)
-        # print(response)
+
         if response.status_code == 200:
             if method.upper() == "GET":
                 return response
             elif method.upper() == "POST":
                 return response.json()
         else:
+            print(response.content)
             raise RuntimeError(f"Request failed ({response.status_code})")
         return None
```

### Comparing `ytspider-0.0.0.2/src/utils/signals_info.py` & `ytspider-0.0.0.3/src/utils/signals_info.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.2/src/ytspider.py` & `ytspider-0.0.0.3/src/ytspider.py`

 * *Files 18% similar despite different names*

```diff
@@ -48,42 +48,49 @@
     def getAllHandlers(self):
         return self.handlers
 
     def executeHandlers(self, itemId):
         results = {}
         for handlerName, handler in self.handlers.items():
 
-            result = handler.execute()
+            result = handler.execute(itemId)
             if result is not None and result != []:
                 results[handlerName] = result
         return results
 
     def scrape(self, itemId, continuation_token=None):
         self.__Response.clear()
         if type(itemId) == str:
-            self.itemId = itemId
-            self.__Response.update({itemId: self.scrapeSingle(itemId)})
+            # self.itemId = itemId
+            # self.__Response.update({itemId: self.scrapeSingle(itemId)})
+            result = self.scrapeSingle(itemId)
+            key = self.itemId if hasattr(self, "itemId") else itemId
+            self.__Response.update({key: result})
         elif type(itemId) == list:
             for i, id in enumerate(itemId):
                 if type(id) == str:
-                    self.itemId = id
-                    self.__Response.update({id: self.scrapeSingle(id)})
+                    # self.itemId = id
+                    # self.__Response.update({id: self.scrapeSingle(id)})
+                    result = self.scrapeSingle(id)
+                    key = self.itemId if hasattr(self, "itemId") else id
+                    self.__Response.update({key: result})
                 else:
                     raise ValueError(
                         f"Invalid data type at index {i}. Expected str")
         return self
 
     def scrapeSingle(self, itemId):
         result = {itemId: None}
         return result
 
     def get(self):
         for itemId in self.__Response.keys():
             self.itemId = itemId
             result = self.executeHandlers(itemId)
+
             if itemId in self.__Response:
                 self.__Response[itemId].update(result)
             else:
                 self.__Response[itemId] = result
         self.restoreDefaultHandlers()
         return self.__Response
 
@@ -113,23 +120,26 @@
     def prepareURL(self, userInput):
         if type(userInput) != str:
             raise ValueError("Argument (screenName) must be a string")
 
         screenNames = re.findall(r"@\w+", userInput)
         if len(screenNames) > 0:
             screenName = screenNames[0]
+        elif "youtube.com" in userInput:
+            screenName = ""
+            self.url = userInput
         else:
             raise ValueError(
-                "Argument (screenName) must have a screen name as '@ChannelName'")
-
+                "Argument (screenName) must have a screen name as '@ChannelName' or a YouTube URL")
         return self.url + screenName.strip("/").strip()
 
     def __postProcessResponse(self, response):
         if isinstance(response, requests.models.Response):
             soup = BeautifulSoup(response.text)
+            # print(list(map(lambda x: x['itemprop'], metas)))
             data = {}
             # FEATURE: add useful meta properties (attributes['property'])
             attributes = {
                 "itemprop": [
                     "channelId",
                     "isFamilyFriendly",
                     "regionsAllowed",
@@ -149,16 +159,30 @@
 
             for criteria in attributes:
                 for metaKey in attributes[criteria]:
                     tag = soup.find("meta", {criteria: metaKey})
                     if tag is not None:
                         tagInnerContent = tag['content']
                         data[metaKey] = tagInnerContent
-        self.itemId = data["channelId"]
-        return data
+        
+        # if "channelId" not in data:
+        #     channelId = 
+        # print(soup.find("meta", {"itemprop":"channelId"}))
+            # channelIds = re.findall(r'"browseId":"([a-zA-Z0-9 _ -]+)"', str(soup))
+            # if len(channelIds) > 0:
+            #     data["channelId"] = channelIds[0]
+        if "channelId" in data:
+            self.itemId = data["channelId"]
+            return data
+        else:
+            return None
 
     def scrapeSingle(self, screenName):
         endpoint = self.prepareURL(screenName)
+        print("HHH")
+        print(endpoint)
         result = self.Request.send(endpoint)
         data = self.__postProcessResponse(result)
+        if not hasattr(self, "itemId"):
+            self.itemId = screenName
         return data
```

