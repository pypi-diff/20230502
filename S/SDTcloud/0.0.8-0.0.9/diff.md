# Comparing `tmp/SDTcloud-0.0.8.tar.gz` & `tmp/SDTcloud-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDTcloud-0.0.8.tar", last modified: Tue May  2 05:27:54 2023, max compression
+gzip compressed data, was "SDTcloud-0.0.9.tar", last modified: Tue May  2 05:41:47 2023, max compression
```

## Comparing `SDTcloud-0.0.8.tar` & `SDTcloud-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-02 05:27:54.535745 SDTcloud-0.0.8/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-02 05:27:54.535605 SDTcloud-0.0.8/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)       12 2023-04-27 00:33:43.000000 SDTcloud-0.0.8/README.md
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-02 05:27:54.534592 SDTcloud-0.0.8/SDTcloud/
--rw-r--r--   0 june       (501) staff       (20)       75 2023-04-27 00:34:53.000000 SDTcloud-0.0.8/SDTcloud/__init__.py
--rw-r--r--   0 june       (501) staff       (20)     5090 2023-04-28 07:44:21.000000 SDTcloud-0.0.8/SDTcloud/sdtcloud.py
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-02 05:27:54.535408 SDTcloud-0.0.8/SDTcloud.egg-info/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-02 05:27:54.000000 SDTcloud-0.0.8/SDTcloud.egg-info/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)      188 2023-05-02 05:27:54.000000 SDTcloud-0.0.8/SDTcloud.egg-info/SOURCES.txt
--rw-r--r--   0 june       (501) staff       (20)        1 2023-05-02 05:27:54.000000 SDTcloud-0.0.8/SDTcloud.egg-info/dependency_links.txt
--rw-r--r--   0 june       (501) staff       (20)        9 2023-05-02 05:27:54.000000 SDTcloud-0.0.8/SDTcloud.egg-info/top_level.txt
--rw-r--r--   0 june       (501) staff       (20)       38 2023-05-02 05:27:54.535779 SDTcloud-0.0.8/setup.cfg
--rw-r--r--   0 june       (501) staff       (20)      656 2023-05-02 05:26:59.000000 SDTcloud-0.0.8/setup.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-02 05:41:47.671360 SDTcloud-0.0.9/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-02 05:41:47.671224 SDTcloud-0.0.9/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)       12 2023-04-27 00:33:43.000000 SDTcloud-0.0.9/README.md
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-02 05:41:47.670342 SDTcloud-0.0.9/SDTcloud/
+-rw-r--r--   0 june       (501) staff       (20)       75 2023-04-27 00:34:53.000000 SDTcloud-0.0.9/SDTcloud/__init__.py
+-rw-r--r--   0 june       (501) staff       (20)     5909 2023-05-02 05:40:52.000000 SDTcloud-0.0.9/SDTcloud/sdtcloud.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-02 05:41:47.671039 SDTcloud-0.0.9/SDTcloud.egg-info/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-02 05:41:47.000000 SDTcloud-0.0.9/SDTcloud.egg-info/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)      188 2023-05-02 05:41:47.000000 SDTcloud-0.0.9/SDTcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 june       (501) staff       (20)        1 2023-05-02 05:41:47.000000 SDTcloud-0.0.9/SDTcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 june       (501) staff       (20)        9 2023-05-02 05:41:47.000000 SDTcloud-0.0.9/SDTcloud.egg-info/top_level.txt
+-rw-r--r--   0 june       (501) staff       (20)       38 2023-05-02 05:41:47.671393 SDTcloud-0.0.9/setup.cfg
+-rw-r--r--   0 june       (501) staff       (20)      656 2023-05-02 05:41:44.000000 SDTcloud-0.0.9/setup.py
```

### Comparing `SDTcloud-0.0.8/SDTcloud/sdtcloud.py` & `SDTcloud-0.0.9/SDTcloud/sdtcloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,16 +158,41 @@
             result = json.loads(response.content)
             raise Exception(f"[ERROR] {result}")
 
         open(getPath, "wb").write(response.content)
         print("Success upload...")
     
     # 컨텐츠 등록
-    def fput_content(self):
-        print("fput")
+    def fput_content(self, storageId, folderId, filePath, fileVersion, fileFormat, fileTag):
+        headers = {
+            "Authorization": self.userToken
+        }
+
+        bodys = json.dumps({
+            "storageId": storageId,
+            "folderId": folderId,
+            "version": fileVersion,
+            "format": fileFormat,
+            "tag": fileTag
+        })
+
+        file_open = open(filePath, 'rb')
+
+        files={
+            'request': (None, bodys, 'application/json'),
+            "content": (filePath.split("/")[-1], file_open, 'application/octet-stream')
+        }
+
+        response = requests.request("POST", f"{self.url}/stackbase/v1/contents", headers=headers, files=files)
+        result = json.loads(response.content)
+
+        if response.status_code != 200:
+            raise Exception(f"[ERROR] {result}")
+        
+        return result
         
 
 # print("Login")
 # sdt_client = SDTcloud()
 
 # # print("get List of storage")
 # # sdt_client.get_storage()
```

### Comparing `SDTcloud-0.0.8/setup.py` & `SDTcloud-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SDTcloud", # Replace with your own username
-    version="0.0.8",
+    version="0.0.9",
     author="sujune",
     author_email="hoakw@sdt.inc",
     description="SDT cloud API Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

