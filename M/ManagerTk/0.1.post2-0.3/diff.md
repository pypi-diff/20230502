# Comparing `tmp/ManagerTk-0.1.post2.tar.gz` & `tmp/ManagerTk-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ManagerTk-0.1.post2.tar", last modified: Tue May  2 16:53:54 2023, max compression
+gzip compressed data, was "ManagerTk-0.3.tar", last modified: Tue Feb 21 21:42:05 2023, max compression
```

## Comparing `ManagerTk-0.1.post2.tar` & `ManagerTk-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:54.696175 ManagerTk-0.1.post2/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:50:29.000000 ManagerTk-0.1.post2/License.txt
--rw-rw-rw-   0        0        0     3343 2023-05-02 16:53:54.695130 ManagerTk-0.1.post2/PKG-INFO
--rw-rw-rw-   0        0        0     2821 2023-05-02 16:29:44.000000 ManagerTk-0.1.post2/README.md
--rw-rw-rw-   0        0        0      544 2023-05-02 16:53:42.000000 ManagerTk-0.1.post2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 16:53:54.696704 ManagerTk-0.1.post2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:54.677281 ManagerTk-0.1.post2/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:54.690915 ManagerTk-0.1.post2/src/ManagerTk.egg-info/
--rw-rw-rw-   0        0        0     3343 2023-05-02 16:53:54.000000 ManagerTk-0.1.post2/src/ManagerTk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-05-02 16:53:54.000000 ManagerTk-0.1.post2/src/ManagerTk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:53:54.000000 ManagerTk-0.1.post2/src/ManagerTk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-02 16:53:54.000000 ManagerTk-0.1.post2/src/ManagerTk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5264 2023-04-30 07:51:28.000000 ManagerTk-0.1.post2/src/ManagerTk.py
+drwxrwxrwx   0        0        0        0 2023-02-21 21:42:05.379660 ManagerTk-0.3/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:50:29.000000 ManagerTk-0.3/License.txt
+-rw-rw-rw-   0        0        0      550 2023-02-21 21:42:05.378086 ManagerTk-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-02-21 09:48:40.000000 ManagerTk-0.3/README.md
+-rw-rw-rw-   0        0        0      500 2023-02-21 21:41:10.000000 ManagerTk-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-02-21 21:42:05.379660 ManagerTk-0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-02-21 21:42:05.354575 ManagerTk-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-02-21 21:42:05.373952 ManagerTk-0.3/src/ManagerTk.egg-info/
+-rw-rw-rw-   0        0        0      550 2023-02-21 21:42:05.000000 ManagerTk-0.3/src/ManagerTk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-02-21 21:42:05.000000 ManagerTk-0.3/src/ManagerTk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-21 21:42:05.000000 ManagerTk-0.3/src/ManagerTk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-02-21 21:42:05.000000 ManagerTk-0.3/src/ManagerTk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3858 2023-02-21 21:29:02.000000 ManagerTk-0.3/src/ManagerTk.py
```

### Comparing `ManagerTk-0.1.post2/License.txt` & `ManagerTk-0.3/License.txt`

 * *Files identical despite different names*

### Comparing `ManagerTk-0.1.post2/src/ManagerTk.py` & `ManagerTk-0.3/src/ManagerTk.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,95 @@
-from tkinter import messagebox
 from tkinter import *
-import tkinter
-from PIL import ImageTk, Image
-from io import BytesIO
 from time import sleep
-import requests
-import base64
-import os
-
-
+import re
 coords = [0,0]
 debug = False
 boolc = False
 window = None
 time_cview = 0
-
 def interface(window):
-    "Bind motion mouse in dubplicate window."
     window.bind('<Motion>', move)
-
 def move(event):
-    "Subfunction for interface, call while move mouse and print coordinates to console."
     global coords
     coords[0] = event.x
     coords[1] = event.y
     if(boolc):
-        try:sleep(time_cview); print(coords[0], coords[1])
-        except:raise TypeError("Read Documentation[About bind mouse motion] | time_cview should be integer or float.")
+        try:sleep(time_cview);print(coords[0], coords[1])
+        except:raise TypeError("time_cview SHOULD be integer or float.")
         
-def run(window):
-    "Run bind mouse motion in dublicate window."
-    interface(window)
-
-def coord_view(window,boolc):
-    "Creating dublicate window for viewing mouse coordinates."
-    interface(window)
+def run(window):interface(window)
 
+def coord_view(window,boolc):"Creating dublicate window for viewing coordinates(x,y)."; interface(window)
 def typely(listm):
-    "Looks on types in page type."
+    "Looks on types."
     typely = True
     for coord in listm:
-        try:
-            for coords in coord[1]:
-                try:
-                    ex = coord[1][0] + coord[1][1]
-                except:
-                    typely = False
-                finally:
-                    if(typely == True):return True
-                    else: return False
-        except:
-            return False
+        for coords in coord[1]:
+            try:
+                ex = coord[1][0] + coord[1][1]
+            except:
+                typely = False
+            finally:
+                if(typely == True):return True
+                else: return False
                     
 def create_mpage(window,ui_page,size):
-    "Add ui and set size in new window."
     if(typely(ui_page)):
         window.geometry(size)
         for ui in ui_page:
-            ui[0].pack()
-            ui[0].place({"x": ui[1][0], "y": ui[1][1]})
+            ui.pack()
         if(debug == True):
             print("Page ui loaded.")
     else:
-        try:
-            for ui in ui_page:
-                ui[0].pack(side=ui[1][0])
-                ui[0].place(x=ui[1][0], y=ui[1][1])
-        except:
-            for ui in ui_page:
-                ui[0].pack()
-                ui[0].place()
+        raise TypeError("create_mpage(ui_page), ui_page SHOULD be list type.")
+
     
 def redirect_pages(page_ui_1,page_ui_2,side=None):
     "This function makes redirecting from page_1 to page_2, ui reconstruction."
     if(type(page_ui_1) and type(page_ui_2) == list):
-        if(type(side) != list and type(side) != str and side != None): raise TypeError("Read Documentation[About type pages] | redirect_pages(ui_page_1,ui_page_2,side), side should be str type.")
+        if(type(side) != list and type(side) != str and side != None): raise TypeError("redirect_pages(ui_page_1,ui_page_2,side), side SHOULD be str type. \nEXAMPLE:\n\redirect_pages(main,second,'left')\nOR\redirect_pages(ui_page_1,ui_page_2,['top','right',left'])\n\n")
         else:
-            if debug == True: print("Start Redirecting.")
-            for ui_page in page_ui_1:
-                if debug == True: print("Forget object:", ui_page[0])
-                ui_page[0].place_forget()
-                ui_page[0].pack_forget()
+            if debug == True:print("Start Redirecting.")
+            for ui_page_1 in page_ui_1:
+                ui_page_1.pack_forget()
             if(type(side) != list and side != None and type()):
                 for ui_page_2 in page_ui_2:
                     ui_page_2.pack(side=side)
-                    if debug == True: print("Packed ui.")
+                    if debug == True:print("Packed ui.")
             else:
                 if(side in ["bottom","top","right","left"]):
                     side_index = 0
                     for ui_page_2 in page_ui_2:
                         try:
                             ui_page_2.pack(side=side[side_index])
                         except:
-                            raise SyntaxError("Read Documentation[About redirect pages] | if side is a list, count index side should be == count index ui_page_2.")
+                            raise SyntaxError("if side is a list, count index side SHOULD be == count index ui_page_2.\n\n")
                     side_index += 1
-                    if debug: print("Packed ui.")
+                    if debug == True:print("Packed ui.")
                 else:
                     if(typely(page_ui_2)):
                         for sidec in page_ui_2:
-                            if debug: print(sidec[1][0])
+                            print(sidec[1][0])
                             try:
                                 sidec[0].place(x=sidec[1][0],y=sidec[1][1])
-                                if debug: print("x: {},\ny:{}.".format(sidec[1][0],sidec[1][1]))
+                                print("x: {},\ny:{}.".format(sidec[1][0],sidec[1][1]))
                             except:
-                                raise SyntaxError("Read Documentation[About redirect pages] | if side is a list, count index side should be == count index ui_page_2.")
-                            if debug == True: print("Packed ui.")
+                                raise SyntaxError("if side is a list, count index side SHOULD be == count index ui_page_2.\n\n")
+                            if debug == True:print("Packed ui.")
                     else:
-                        raise SyntaxError("Read Documentation[About redirect pages] | list error.")
+                        print("ERROR SYNTAX list.")
                 
     else:
-        raise TypeError("Read Documentation[About redirect pages] | redirect_pages(ui_page), page_ui_1 and page_ui_2 should be list type.")
-
-def add_url_image(window: tkinter.Tk, image_url: str, size=set):
-    "Add image from url address as object(label)."
-    image = BytesIO(requests.get(image_url).content)
-    image_sub_obj = ImageTk.PhotoImage(Image.open(image).resize(size) if size is not set else Image.open(image))
-    image_obj = Label(window, image=image_sub_obj)
-    image_obj.image_sub_obj = image_sub_obj
-    return image_obj
-
-
-
+        raise TypeError("redirect_pages(ui_page), page_ui_1 and page_ui_2 SHOULD be list type.")
+            
 def window_exit(title: str, message: str):
     "Message Box for Exit(two buttons 'Yes','No' and Title text and message text boxs)."
-    output = tkinter.messagebox.askyesno(title=title,message=message)
+    output = messagebox.askyesno(title=title,message=message)
     if(output==True):
         if debug == True:
             print("Program Exit.")
         exit()
 
 
 def documentation():
-    "Show link documentation for ManagerTk."
+    "Show Documentation for ManagerTk."
     print("Documentation: https://pypi.org/project/ManagerTk/")
```

