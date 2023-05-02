# Comparing `tmp/gokyuzu-2.0.2.tar.gz` & `tmp/gokyuzu-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokyuzu-2.0.2.tar", last modified: Mon Apr 24 18:17:09 2023, max compression
+gzip compressed data, was "gokyuzu-2.0.3.tar", last modified: Tue May  2 16:48:17 2023, max compression
```

## Comparing `gokyuzu-2.0.2.tar` & `gokyuzu-2.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 18:17:09.049122 gokyuzu-2.0.2/
--rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-2.0.2/LICENSE
--rw-r--r--   0 kilic      (501) staff       (20)     6380 2023-04-24 18:17:09.049015 gokyuzu-2.0.2/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)     5604 2023-04-24 18:16:49.000000 gokyuzu-2.0.2/README.md
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 18:17:09.047634 gokyuzu-2.0.2/gokyuzu/
--rw-r--r--   0 kilic      (501) staff       (20)     8586 2023-04-24 18:05:45.000000 gokyuzu-2.0.2/gokyuzu/BlueskyEndpoints.py
--rw-r--r--   0 kilic      (501) staff       (20)      178 2023-04-22 16:36:29.000000 gokyuzu-2.0.2/gokyuzu/BlueskyHelper.py
--rw-r--r--   0 kilic      (501) staff       (20)      224 2023-04-24 17:33:31.000000 gokyuzu-2.0.2/gokyuzu/BlueskyRecords.py
--rw-r--r--   0 kilic      (501) staff       (20)     4015 2023-04-24 17:31:55.000000 gokyuzu-2.0.2/gokyuzu/BlueskySession.py
--rw-r--r--   0 kilic      (501) staff       (20)    30565 2023-04-24 18:16:31.000000 gokyuzu-2.0.2/gokyuzu/__init__.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 18:17:09.048481 gokyuzu-2.0.2/gokyuzu.egg-info/
--rw-r--r--   0 kilic      (501) staff       (20)     6380 2023-04-24 18:17:09.000000 gokyuzu-2.0.2/gokyuzu.egg-info/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      357 2023-04-24 18:17:09.000000 gokyuzu-2.0.2/gokyuzu.egg-info/SOURCES.txt
--rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-24 18:17:09.000000 gokyuzu-2.0.2/gokyuzu.egg-info/dependency_links.txt
--rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-24 18:17:09.000000 gokyuzu-2.0.2/gokyuzu.egg-info/requires.txt
--rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-24 18:17:09.000000 gokyuzu-2.0.2/gokyuzu.egg-info/top_level.txt
--rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-24 18:16:57.000000 gokyuzu-2.0.2/pyproject.toml
--rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-24 18:17:09.049157 gokyuzu-2.0.2/setup.cfg
--rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-24 18:16:58.000000 gokyuzu-2.0.2/setup.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 18:17:09.048700 gokyuzu-2.0.2/tests/
--rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-2.0.2/tests/__init__.py
--rw-r--r--   0 kilic      (501) staff       (20)     4706 2023-04-22 19:03:38.000000 gokyuzu-2.0.2/tests/test_main.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-05-02 16:48:17.800279 gokyuzu-2.0.3/
+-rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-2.0.3/LICENSE
+-rw-r--r--   0 kilic      (501) staff       (20)     6425 2023-05-02 16:48:17.800153 gokyuzu-2.0.3/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)     5650 2023-05-02 16:35:40.000000 gokyuzu-2.0.3/README.md
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-05-02 16:48:17.798564 gokyuzu-2.0.3/gokyuzu/
+-rw-r--r--   0 kilic      (501) staff       (20)     8595 2023-05-02 15:12:35.000000 gokyuzu-2.0.3/gokyuzu/BlueskyEndpoints.py
+-rw-r--r--   0 kilic      (501) staff       (20)      688 2023-05-02 16:34:14.000000 gokyuzu-2.0.3/gokyuzu/BlueskyHelper.py
+-rw-r--r--   0 kilic      (501) staff       (20)      247 2023-05-02 15:06:44.000000 gokyuzu-2.0.3/gokyuzu/BlueskyRecords.py
+-rw-r--r--   0 kilic      (501) staff       (20)     4014 2023-05-02 16:34:27.000000 gokyuzu-2.0.3/gokyuzu/BlueskySession.py
+-rw-r--r--   0 kilic      (501) staff       (20)    31220 2023-05-02 16:26:14.000000 gokyuzu-2.0.3/gokyuzu/__init__.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-05-02 16:48:17.799505 gokyuzu-2.0.3/gokyuzu.egg-info/
+-rw-r--r--   0 kilic      (501) staff       (20)     6425 2023-05-02 16:48:17.000000 gokyuzu-2.0.3/gokyuzu.egg-info/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      357 2023-05-02 16:48:17.000000 gokyuzu-2.0.3/gokyuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 kilic      (501) staff       (20)        1 2023-05-02 16:48:17.000000 gokyuzu-2.0.3/gokyuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       17 2023-05-02 16:48:17.000000 gokyuzu-2.0.3/gokyuzu.egg-info/requires.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       14 2023-05-02 16:48:17.000000 gokyuzu-2.0.3/gokyuzu.egg-info/top_level.txt
+-rw-r--r--   0 kilic      (501) staff       (20)      475 2023-05-02 16:37:49.000000 gokyuzu-2.0.3/pyproject.toml
+-rw-r--r--   0 kilic      (501) staff       (20)       38 2023-05-02 16:48:17.800324 gokyuzu-2.0.3/setup.cfg
+-rw-r--r--   0 kilic      (501) staff       (20)     1028 2023-05-02 16:47:35.000000 gokyuzu-2.0.3/setup.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-05-02 16:48:17.799740 gokyuzu-2.0.3/tests/
+-rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-2.0.3/tests/__init__.py
+-rw-r--r--   0 kilic      (501) staff       (20)     5440 2023-05-02 16:33:19.000000 gokyuzu-2.0.3/tests/test_main.py
```

### Comparing `gokyuzu-2.0.2/PKG-INFO` & `gokyuzu-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 2.0.2
+Version: 2.0.3
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -73,15 +73,15 @@
 
 #### com.atproto.repo
 
 - `def applyWrites( repo, writes, validate=True, swapCommit=None)` 
 - `def createRecord( repo, record, collection, record_key=None, validate=True, swapCommit=None)` 
 - `def deleteRecord( repo, record, collection, swapRecord=None, swapCommit=None)` 
 - `def describeRepo( repo)` 
-- `def getRecord( user_did, collection, record_key, commit=None)` 
+- `def getAdminRecord( user_did, collection, record_key, commit=None)` 
 - `def listRecords( user_did, collection, limit=10, record_key_start=None, record_key_end=None, reverse=False)` 
 - `def putRecord( repo, collection, record_key, record, validate=True, swapRecord=None, swapCommit=None)` 
 - `def uploadBlob( blob_bytes)` 
 - `def uploadImage( image_path)` 
 - `def followRecord( handle=None, user_did=None)` 
 - `def unfollowRecord( handle=None, user_did=None)` 
 
@@ -106,15 +106,15 @@
 #### com.atproto.sync
 
 - `def getBlob( repo_did, blob_cid)` 
 - `def getBlocks( did, cids)` 
 - `def getCheckout( did, commit=None)` 
 - `def getCommitPath( did, latest=None, earliest=None)` 
 - `def getHead( did)` 
-- `def getRecord( did, collection, record_key, commit=None)` 
+- `def getSyncRecord( did, collection, record_key, commit=None)` 
 - `def getRepo( did, earliest=None, latest=None)` 
 - `def listBlobs( did, latest, earliest)` 
 - `def notifyOfUpdate( hostname)` 
 - `def requestCrawl( hostname)` 
 - `def subscribeRepos( cursor)` 
 
 
@@ -172,14 +172,15 @@
 - `def search( query_type="posts", query="")` 
 - `def search_profiles( query)` 
 - `def search_posts( query)` 
 
 #### Other
 
 - `def health()` 
+- `def createLinkFromAtUri( at_uri)`
 - `def quote( text, repo, record_uri, record_cid, createdAt=None)` 
 - `def delete_post( repo, record_key)` 
 - `def comment( text, repo, reply_root_uri, reply_root_cid, reply_parent_uri, reply_parent_cid, createdAt=None)` 
 
 
 ### Development
```

### Comparing `gokyuzu-2.0.2/README.md` & `gokyuzu-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 #### com.atproto.repo
 
 - `def applyWrites( repo, writes, validate=True, swapCommit=None)` 
 - `def createRecord( repo, record, collection, record_key=None, validate=True, swapCommit=None)` 
 - `def deleteRecord( repo, record, collection, swapRecord=None, swapCommit=None)` 
 - `def describeRepo( repo)` 
-- `def getRecord( user_did, collection, record_key, commit=None)` 
+- `def getAdminRecord( user_did, collection, record_key, commit=None)` 
 - `def listRecords( user_did, collection, limit=10, record_key_start=None, record_key_end=None, reverse=False)` 
 - `def putRecord( repo, collection, record_key, record, validate=True, swapRecord=None, swapCommit=None)` 
 - `def uploadBlob( blob_bytes)` 
 - `def uploadImage( image_path)` 
 - `def followRecord( handle=None, user_did=None)` 
 - `def unfollowRecord( handle=None, user_did=None)` 
 
@@ -86,15 +86,15 @@
 #### com.atproto.sync
 
 - `def getBlob( repo_did, blob_cid)` 
 - `def getBlocks( did, cids)` 
 - `def getCheckout( did, commit=None)` 
 - `def getCommitPath( did, latest=None, earliest=None)` 
 - `def getHead( did)` 
-- `def getRecord( did, collection, record_key, commit=None)` 
+- `def getSyncRecord( did, collection, record_key, commit=None)` 
 - `def getRepo( did, earliest=None, latest=None)` 
 - `def listBlobs( did, latest, earliest)` 
 - `def notifyOfUpdate( hostname)` 
 - `def requestCrawl( hostname)` 
 - `def subscribeRepos( cursor)` 
 
 
@@ -152,14 +152,15 @@
 - `def search( query_type="posts", query="")` 
 - `def search_profiles( query)` 
 - `def search_posts( query)` 
 
 #### Other
 
 - `def health()` 
+- `def createLinkFromAtUri( at_uri)`
 - `def quote( text, repo, record_uri, record_cid, createdAt=None)` 
 - `def delete_post( repo, record_key)` 
 - `def comment( text, repo, reply_root_uri, reply_root_cid, reply_parent_uri, reply_parent_cid, createdAt=None)` 
 
 
 ### Development
```

### Comparing `gokyuzu-2.0.2/gokyuzu/BlueskyEndpoints.py` & `gokyuzu-2.0.3/gokyuzu/BlueskyEndpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         
     def getModerationReport(self):
         return self.get_url("/xrpc/com.atproto.admin.getModerationReport")
 
     def getModerationReports(self):
         return self.get_url("/xrpc/com.atproto.admin.getModerationReports")
         
-    def getRecord(self):
+    def getAdminRecord(self):
         return self.get_url("/xrpc/com.atproto.admin.getRecord")
         
     def getRepo(self):
         return self.get_url("/xrpc/com.atproto.admin.getRepo")
 
     def resolveModerationReports(self):
         return self.get_url("/xrpc/com.atproto.admin.resolveModerationReports")
@@ -160,15 +160,15 @@
     
     def getCommitPath(self):
         return self.get_url("/xrpc/com.atproto.sync.getCommitPath")
     
     def getHead(self):
         return self.get_url("/xrpc/com.atproto.sync.getHead")
     
-    def getRecord(self):
+    def getSyncRecord(self):
         return self.get_url("/xrpc/com.atproto.sync.getRecord")
     
     def getRepo(self):
         return self.get_url("/xrpc/com.atproto.sync.getRepo")
     
     def listBlobs(self):
         return self.get_url("/xrpc/com.atproto.sync.listBlobs")
```

### Comparing `gokyuzu-2.0.2/gokyuzu/BlueskySession.py` & `gokyuzu-2.0.3/gokyuzu/BlueskySession.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 
-from gokyuzu import BlueskyEndpoints
+from gokyuzu import BlueskyEndpoints, BlueskyHelper
 
 
 class BlueskySession():
     def __init__(self, handle, password):
         self.BSKY_SERVER = "https://bsky.social"
         self.DID = ""
         self.HANDLE = handle
@@ -93,10 +93,10 @@
         return response
     
     def deleteRecord(self, request_data, **kwargs):
         request_url = self.ENDPOINTS.deleteRecord()
         headers = { 'Authorization': f'Bearer {self.getAccessToken()}', 'Content-Type': 'application/json' }
         response = requests.post(request_url, headers=headers, json=request_data, **kwargs)
         return response
-                
+
```

### Comparing `gokyuzu-2.0.2/gokyuzu/__init__.py` & `gokyuzu-2.0.3/gokyuzu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
             "resolved": resolved,
             "limit": limit,
             "cursor": cursor
         }
         response = self.SESSION.get(request_url, json=request_data)
         return response
         
-    def getRecord(self, uri=None, cid=None):
-        request_url = self.ENDPOINTS.getRecord()
+    def getAdminRecord(self, uri=None, cid=None):
+        request_url = self.ENDPOINTS.getAdminRecord()
         request_data = {}
         if uri is not None:
             request_data['uri'] = uri
         if cid is not None:
             request_data['cid'] = cid
         response = self.SESSION.get(request_url, json=request_data)
         return response
@@ -238,22 +238,18 @@
         request_data = {
             "repo": repo
         }
         response = self.SESSION.postJson(request_url, json=request_data)
         return response
 
     def getRecord(self, user_did, collection, record_key, commit=None):
-        request_url = self.ENDPOINTS.getRecord()
-        request_data = {
-            "repo": user_did,
-            "collection": collection,
-            "rkey": record_key,
-            "cid": commit
-        }
-        response = self.SESSION.postJson(request_url, json=request_data)
+        request_url = self.ENDPOINTS.getRecord() + "?repo={}&collection={}&rkey={}".format(user_did, collection, record_key)
+        if commit is not None:
+            request_url += "&commit={}".format(commit)
+        response = self.SESSION.get(request_url)
         return response
 
     def listRecords(self, user_did, collection, limit=10, record_key_start=None, record_key_end=None, reverse=False):
         request_url = self.ENDPOINTS.listRecords()
         request_data = {
             "repo": user_did,
             "collection": collection,
@@ -497,29 +493,36 @@
         return response
 
     def getHead(self, did):
         request_url = self.ENDPOINTS.getHead() + "?did={}".format(did)
         response = self.SESSION.get(request_url)
         return response
 
-    def getRecord(self, did, collection, record_key, commit=None):
-        request_url = self.ENDPOINTS.getRecord()
+    def getSyncRecord(self, did, collection, record_key, commit=None):
+        request_url = self.ENDPOINTS.getSyncRecord()
         request_data = {
             "did": did,
             "collection": collection,
             "key": record_key
         }
         if commit:
             request_data["commit"] = commit
         
         response = self.SESSION.postJson(request_url, json=request_data)
         return response
 
     def getRepo(self, did, earliest=None, latest=None):
-        request_url = self.ENDPOINTS.getRepo() + "?did{}&earliest={}&latest={}".format(did, earliest, latest)
+        if earliest is not None and latest is not None:
+            request_url = self.ENDPOINTS.getRepo() + "?did={}&earliest={}&latest={}".format(did, earliest, latest)
+        elif earliest is not None:
+            request_url = self.ENDPOINTS.getRepo() + "?did={}&earliest={}".format(did, earliest)
+        elif latest is not None:
+            request_url = self.ENDPOINTS.getRepo() + "?did={}&latest={}".format(did, latest)
+        else:
+            request_url = self.ENDPOINTS.getRepo() + "?did={}".format(did)
         response = self.SESSION.get(request_url)
         return response
     
     def listBlobs(self, did, latest, earliest):
         request_url = self.ENDPOINTS.listBlobs()
         request_data = {
             "did": did,
@@ -797,69 +800,74 @@
     #endregion
 
     #region unspecced
     def health(self):
         request_url = self.ENDPOINTS.health()
         response = self.SESSION.get(request_url)
         return response
+    
+    def createLinkFromAtUri(self, at_uri):
+        did, rkey = BlueskyHelper.analyze_at_uri(at_uri)
+        handle = self.getProfile(did).json().get("handle")
+        return BlueskyHelper.createPostLink(handle, rkey)
 
     def quote(self, text, repo, record_uri, record_cid, createdAt=None):
         if createdAt is None:
             createdAt = BlueskyHelper.getTimestamp()
 
         request_data = {
-            "collection": BlueskyRecords.Post,
+            "collection": str(BlueskyRecords.Post),
             "repo": repo,
             "record":{
                 "text": text,
                 "embed":{
-                "$type": BlueskyRecords.EmbedRecord,
+                "$type": str(BlueskyRecords.EmbedRecord),
                 "record":{
                     "uri": record_uri,
                     "cid": record_cid
                 }
                 },
                 "createdAt": createdAt,
-                "$type": BlueskyRecords.Post
+                "$type": str(BlueskyRecords.Post)
             }
         }
         response = self.SESSION.createRecord(request_data=request_data)
         return response
 
     def delete_post(self, repo, record_key):
         request_data = {
-            "collection": BlueskyRecords.Post,
+            "collection": str(BlueskyRecords.Post),
             "repo": repo,
             "rkey": record_key
         }
         response = self.SESSION.deleteRecord(request_data=request_data)
         return response
 
     # TODO: simplify comment function
     def comment(self, text, repo, reply_root_uri, reply_root_cid, reply_parent_uri, reply_parent_cid, createdAt=None):
         if createdAt is None:
             createdAt = BlueskyHelper.getTimestamp()
 
         request_data = {
-            "collection": BlueskyRecords.Post,
+            "collection": str(BlueskyRecords.Post),
             "repo": repo,
             "record":{
                 "text":text,
                 "reply":{
                     "root":{
                         "uri": reply_root_uri,
                         "cid": reply_root_cid
                     },
                     "parent":{
                         "uri": reply_parent_uri,
                         "cid": reply_parent_cid
                     }
                 },
                 "createdAt": createdAt,
-                "$type": BlueskyRecords.Post
+                "$type": str(BlueskyRecords.Post)
             }
         }
         response = self.SESSION.createRecord(request_data=request_data)
         return response
     
     #endregion
```

### Comparing `gokyuzu-2.0.2/gokyuzu.egg-info/PKG-INFO` & `gokyuzu-2.0.3/gokyuzu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 2.0.2
+Version: 2.0.3
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -73,15 +73,15 @@
 
 #### com.atproto.repo
 
 - `def applyWrites( repo, writes, validate=True, swapCommit=None)` 
 - `def createRecord( repo, record, collection, record_key=None, validate=True, swapCommit=None)` 
 - `def deleteRecord( repo, record, collection, swapRecord=None, swapCommit=None)` 
 - `def describeRepo( repo)` 
-- `def getRecord( user_did, collection, record_key, commit=None)` 
+- `def getAdminRecord( user_did, collection, record_key, commit=None)` 
 - `def listRecords( user_did, collection, limit=10, record_key_start=None, record_key_end=None, reverse=False)` 
 - `def putRecord( repo, collection, record_key, record, validate=True, swapRecord=None, swapCommit=None)` 
 - `def uploadBlob( blob_bytes)` 
 - `def uploadImage( image_path)` 
 - `def followRecord( handle=None, user_did=None)` 
 - `def unfollowRecord( handle=None, user_did=None)` 
 
@@ -106,15 +106,15 @@
 #### com.atproto.sync
 
 - `def getBlob( repo_did, blob_cid)` 
 - `def getBlocks( did, cids)` 
 - `def getCheckout( did, commit=None)` 
 - `def getCommitPath( did, latest=None, earliest=None)` 
 - `def getHead( did)` 
-- `def getRecord( did, collection, record_key, commit=None)` 
+- `def getSyncRecord( did, collection, record_key, commit=None)` 
 - `def getRepo( did, earliest=None, latest=None)` 
 - `def listBlobs( did, latest, earliest)` 
 - `def notifyOfUpdate( hostname)` 
 - `def requestCrawl( hostname)` 
 - `def subscribeRepos( cursor)` 
 
 
@@ -172,14 +172,15 @@
 - `def search( query_type="posts", query="")` 
 - `def search_profiles( query)` 
 - `def search_posts( query)` 
 
 #### Other
 
 - `def health()` 
+- `def createLinkFromAtUri( at_uri)`
 - `def quote( text, repo, record_uri, record_cid, createdAt=None)` 
 - `def delete_post( repo, record_key)` 
 - `def comment( text, repo, reply_root_uri, reply_root_cid, reply_parent_uri, reply_parent_cid, createdAt=None)` 
 
 
 ### Development
```

### Comparing `gokyuzu-2.0.2/setup.py` & `gokyuzu-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gokyuzu',
-    version='2.0.2',
+    version='2.0.3',
     description='bsky.social client library',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Muhammed Kılıç',
     author_email='muhammeddkilicc@gmail.com',
     url='https://github.com/kiliczsh/gokyuzu',
     packages=find_packages(),
     install_requires=[
         'requests>=2.22.0'
     ],
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

