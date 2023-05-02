# Comparing `tmp/cvworld-0.6.tar.gz` & `tmp/cvworld-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cvworld-0.6.tar", last modified: Mon May  1 12:40:51 2023, max compression
+gzip compressed data, was "dist\cvworld-0.7.tar", last modified: Tue May  2 09:07:12 2023, max compression
```

## Comparing `cvworld-0.6.tar` & `cvworld-0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 12:40:51.096792 cvworld-0.6/
--rw-rw-rw-   0        0        0      782 2023-05-01 12:40:51.096792 cvworld-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 12:40:51.096792 cvworld-0.6/cvworld/
--rw-rw-rw-   0        0        0     2400 2023-04-29 06:59:46.304811 cvworld-0.6/cvworld/FaceTrackingModule.py
--rw-rw-rw-   0        0        0     2226 2023-05-01 08:21:19.824516 cvworld-0.6/cvworld/HandTrachkingModule.py
--rw-rw-rw-   0        0        0     2764 2023-05-01 12:27:47.418566 cvworld-0.6/cvworld/Utils.py
--rw-rw-rw-   0        0        0      211 2023-05-01 12:40:07.260554 cvworld-0.6/cvworld/__init__.py
--rw-rw-rw-   0        0        0       39 2023-04-30 07:22:38.469288 cvworld-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1691 2023-05-01 12:40:47.385339 cvworld-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:07:11.992653 cvworld-0.7/
+-rw-rw-rw-   0        0        0      782 2023-05-02 09:07:11.992653 cvworld-0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 09:07:11.992653 cvworld-0.7/cvworld/
+-rw-rw-rw-   0        0        0     2400 2023-04-29 06:59:46.304811 cvworld-0.7/cvworld/FaceTrackingModule.py
+-rw-rw-rw-   0        0        0     2226 2023-05-01 08:21:19.824516 cvworld-0.7/cvworld/HandTrachkingModule.py
+-rw-rw-rw-   0        0        0     2976 2023-05-02 08:39:16.143468 cvworld-0.7/cvworld/Utils.py
+-rw-rw-rw-   0        0        0      211 2023-05-01 12:40:07.260554 cvworld-0.7/cvworld/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-04-30 07:22:38.469288 cvworld-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1691 2023-05-02 08:52:03.818450 cvworld-0.7/setup.py
```

### Comparing `cvworld-0.6/PKG-INFO` & `cvworld-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cvworld
-Version: 0.6
+Version: 0.7
 Summary: Computer Vision Helper Function
 Home-page: https://github.com/user/reponame
 Author: Sethu Raman
 Author-email: sethuramanvr046@gmail.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `cvworld-0.6/cvworld/FaceTrackingModule.py` & `cvworld-0.7/cvworld/FaceTrackingModule.py`

 * *Files identical despite different names*

### Comparing `cvworld-0.6/cvworld/HandTrachkingModule.py` & `cvworld-0.7/cvworld/HandTrachkingModule.py`

 * *Files identical despite different names*

### Comparing `cvworld-0.6/cvworld/Utils.py` & `cvworld-0.7/cvworld/Utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,17 +65,29 @@
     img = cv2.line(img, pt1, pt2, color, t)
     return img
 
 def circle(img, centre, radius, color=(255, 0, 255), t=cv2.FILLED):
     img = cv2.circle(img, centre, radius, color, t)
     return img
 
+def videocapture(img):
+    img = cv2.VideoCapture(img)
+    return img
+
+def imshow(winName, img):
+    img = cv2.imshow(winName, img)
+    return img
+
+def waitkey(delay):
+    img = cv2.waitKey(delay)
+    return img
+
 def main():
-    cap = cv2.VideoCapture(0)
+    cap = videocapture(0)
     while True:
         success, img = cap.read()
         img = edge(img, (5, 5), 0, 75, 100)
-        cv2.imshow("Images", img)
-        cv2.waitKey(1)
+        imshow("EDGES", img)
+        waitkey(0)
 
 if __name__ == "__main__":
     main()
```

### Comparing `cvworld-0.6/setup.py` & `cvworld-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'cvworld',         # How you named your package folder (MyLib)
   packages = ['cvworld'],   # Chose the same as "name"
-  version = '0.6',      # Start with a small number and increase it with every change you make
+  version = '0.7',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Computer Vision Helper Function',   # Give a short description about your library
   author = 'Sethu Raman',                   # Type in your name
   author_email = 'sethuramanvr046@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['ComputerVision', 'FaceDetection', 'HandTracking'],   # Keywords that define your package best
```

