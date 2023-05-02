# Comparing `tmp/pymicro365-0.0.5.tar.gz` & `tmp/pymicro365-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymicro365-0.0.5.tar", last modified: Tue May  2 18:54:27 2023, max compression
+gzip compressed data, was "pymicro365-0.0.6.tar", last modified: Tue May  2 19:11:32 2023, max compression
```

## Comparing `pymicro365-0.0.5.tar` & `pymicro365-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 18:54:27.031678 pymicro365-0.0.5/
--rw-rw-rw-   0        0        0      340 2023-05-02 18:54:27.030679 pymicro365-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 18:54:27.011731 pymicro365-0.0.5/pymicro365/
--rw-rw-rw-   0        0        0     3267 2023-05-02 18:40:29.000000 pymicro365-0.0.5/pymicro365/__init__.py
--rw-rw-rw-   0        0        0     2989 2023-05-02 18:49:27.000000 pymicro365-0.0.5/pymicro365/pyicalc.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:54:27.029683 pymicro365-0.0.5/pymicro365.egg-info/
--rw-rw-rw-   0        0        0      340 2023-05-02 18:54:26.000000 pymicro365-0.0.5/pymicro365.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-02 18:54:26.000000 pymicro365-0.0.5/pymicro365.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 18:54:26.000000 pymicro365-0.0.5/pymicro365.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-02 18:54:26.000000 pymicro365-0.0.5/pymicro365.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-02 18:54:26.000000 pymicro365-0.0.5/pymicro365.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 18:54:27.032676 pymicro365-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      514 2023-05-02 18:54:13.000000 pymicro365-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:11:32.715316 pymicro365-0.0.6/
+-rw-rw-rw-   0        0        0      340 2023-05-02 19:11:32.714318 pymicro365-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 19:11:32.700353 pymicro365-0.0.6/pymicro365/
+-rw-rw-rw-   0        0        0     3267 2023-05-02 18:40:29.000000 pymicro365-0.0.6/pymicro365/__init__.py
+-rw-rw-rw-   0        0        0     3344 2023-05-02 19:09:34.000000 pymicro365-0.0.6/pymicro365/pyicalc.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:11:32.713320 pymicro365-0.0.6/pymicro365.egg-info/
+-rw-rw-rw-   0        0        0      340 2023-05-02 19:11:32.000000 pymicro365-0.0.6/pymicro365.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-02 19:11:32.000000 pymicro365-0.0.6/pymicro365.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:11:32.000000 pymicro365-0.0.6/pymicro365.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-02 19:11:32.000000 pymicro365-0.0.6/pymicro365.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-02 19:11:32.000000 pymicro365-0.0.6/pymicro365.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 19:11:32.715316 pymicro365-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      514 2023-05-02 19:11:23.000000 pymicro365-0.0.6/setup.py
```

### Comparing `pymicro365-0.0.5/pymicro365/__init__.py` & `pymicro365-0.0.6/pymicro365/__init__.py`

 * *Files identical despite different names*

### Comparing `pymicro365-0.0.5/pymicro365/pyicalc.py` & `pymicro365-0.0.6/pymicro365/pyicalc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 import customtkinter as ct
 import tkinter.messagebox
 from customtkinter import *
 from tkinter.constants import SUNKEN
+def init():
+    def close():
+        exit()
+    window=ct.CTk()
+    window.configure(fg_color="white")
+    window.title('Calculator')
+    window.winfo_width()
+    window.winfo_height()
+    frame=ct.CTkFrame(master=window, fg_color="skyblue")
+    window.resizable(False, False)
+    window.geometry("430x360")
+    frame.pack(padx=5, pady=5, fill='both', expand=True)
+    entry=ct.CTkEntry(master=frame,width=400, height=50, placeholder_text="Enter a number:", placeholder_text_color="orange", font=("Roboto", 20), fg_color="white")
+    entry.grid(row=0,column=0,columnspan=3,ipady=2,pady=2)
+    entry.bind("<Return>", lambda event: equal())
+
+    def myclick(number):
+        entry.insert(ct.END,number)
+
+    def equal():
+        try:
+            y=str(eval(entry.get()))
+            entry.delete(0,ct.END)
+            entry.insert(0,y)
+        except:
+            tkinter.messagebox.showinfo("Error","Syntax Error")
 
-window=ct.CTk()
-window.title('Calculator')
-window.winfo_width()
-window.winfo_height()
-frame=ct.CTkFrame(master=window, fg_color="skyblue")
-window.resizable(False, False)
-window.geometry("430x360")
-frame.pack(padx=5, pady=5, fill='both', expand=True)
-entry=ct.CTkEntry(master=frame,width=400, height=50, placeholder_text="Enter a number:", placeholder_text_color="orange", font=("Roboto", 20))
-entry.grid(row=0,column=0,columnspan=3,ipady=2,pady=2)
-entry.bind("<Return>", lambda event: equal())
-
-def myclick(number):
-    entry.insert(ct.END,number)
-
-def equal():
-    try:
-        y=str(eval(entry.get()))
+    def clear():
         entry.delete(0,ct.END)
-        entry.insert(0,y)
-    except:
-        tkinter.messagebox.showinfo("Error","Syntax Error")
-        entry.delete(0, ct.END)
-
-def clear():
-    entry.delete(0,ct.END)
-    
-button_1=ct.CTkButton(master=frame,text='1',command=lambda:myclick(1))
-button_1.grid(row=1,column=0,pady=4)
-button_2=CTkButton(master=frame,text='2',command=lambda:myclick(2))
-button_2.grid(row=1,column=1,pady=4)
-button_3=CTkButton(master=frame,text='3',command=lambda:myclick(3))
-button_3.grid(row=1,column=2,pady=4)
-button_4=CTkButton(master=frame,text='4',command=lambda:myclick(4))
-button_4.grid(row=2,column=0,pady=4)
-button_5=CTkButton(master=frame,text='5',command=lambda:myclick(5))
-button_5.grid(row=2,column=1,pady=4)
-button_6=CTkButton(master=frame,text='6',command=lambda:myclick(6))
-button_6.grid(row=2,column=2,pady=4)
-button_7=CTkButton(master=frame,text='7',command=lambda:myclick(7))
-button_7.grid(row=3,column=0,pady=4)
-button_8=CTkButton(master=frame,text='8',command=lambda:myclick(8))
-button_8.grid(row=3,column=1,pady=4)
-button_9=CTkButton(master=frame,text='9',command=lambda:myclick(9))
-button_9.grid(row=3,column=2,pady=4)
-button_0=CTkButton(master=frame,text='0',command=lambda:myclick(0))
-button_0.grid(row=4,column=1,pady=4)
-
-button_add=CTkButton(master=frame,text="+",command=lambda:myclick('+'))
-button_add.grid(row=5,column=0,pady=2)
-
-button_subtract=CTkButton(master=frame,text="-",command=lambda:myclick('-'))
-button_subtract.grid(row=5,column=1,pady=2)
-
-button_multiply=CTkButton(master=frame,text="*",command=lambda:myclick('*'))
-button_multiply.grid(row=5,column=2,pady=2)
-
-button_div=CTkButton(master=frame,text="/",command=lambda:myclick('/'))
-button_div.grid(row=6,column=0,pady=2)
-
-button_clear=CTkButton(master=frame,text="Clear",command=clear)
-button_clear.grid(row=6,column=1,columnspan=2,pady=2)
-
-button_equal=CTkButton(master=frame,text="=",command=equal)
-button_equal.grid(row=7,column=0,columnspan=3,pady=2)
-
-copyright = ct.CTkLabel(frame, text="© Copyright 2022-2023 Informatic365", bg_color="transparent", fg_color="transparent")
-copyright.place(relx=0.005, rely=0.915)
-
-window.bind("<Escape>", lambda event: exit())
-window.mainloop()
+        
+    button_1=ct.CTkButton(master=frame,text='1',command=lambda:myclick(1))
+    button_1.grid(row=1,column=0,pady=4)
+    button_2=CTkButton(master=frame,text='2',command=lambda:myclick(2))
+    button_2.grid(row=1,column=1,pady=4)
+    button_3=CTkButton(master=frame,text='3',command=lambda:myclick(3))
+    button_3.grid(row=1,column=2,pady=4)
+    button_4=CTkButton(master=frame,text='4',command=lambda:myclick(4))
+    button_4.grid(row=2,column=0,pady=4)
+    button_5=CTkButton(master=frame,text='5',command=lambda:myclick(5))
+    button_5.grid(row=2,column=1,pady=4)
+    button_6=CTkButton(master=frame,text='6',command=lambda:myclick(6))
+    button_6.grid(row=2,column=2,pady=4)
+    button_7=CTkButton(master=frame,text='7',command=lambda:myclick(7))
+    button_7.grid(row=3,column=0,pady=4)
+    button_8=CTkButton(master=frame,text='8',command=lambda:myclick(8))
+    button_8.grid(row=3,column=1,pady=4)
+    button_9=CTkButton(master=frame,text='9',command=lambda:myclick(9))
+    button_9.grid(row=3,column=2,pady=4)
+    button_0=CTkButton(master=frame,text='0',command=lambda:myclick(0))
+    button_0.grid(row=4,column=1,pady=4)
+
+    button_add=CTkButton(master=frame,text="+",command=lambda:myclick('+'))
+    button_add.grid(row=5,column=0,pady=2)
+
+    button_subtract=CTkButton(master=frame,text="-",command=lambda:myclick('-'))
+    button_subtract.grid(row=5,column=1,pady=2)
+
+    button_multiply=CTkButton(master=frame,text="*",command=lambda:myclick('*'))
+    button_multiply.grid(row=5,column=2,pady=2)
+
+    button_div=CTkButton(master=frame,text="/",command=lambda:myclick('/'))
+    button_div.grid(row=6,column=0,pady=2)
+
+    button_clear=CTkButton(master=frame,text="Clear",command=clear)
+    button_clear.grid(row=6,column=1,columnspan=2,pady=2)
+
+    button_equal=CTkButton(master=frame,text="=",command=equal)
+    button_equal.grid(row=7,column=0,columnspan=3,pady=2)
+
+    copyright = ct.CTkLabel(frame, text="© Copyright 2022-2023 Informatic365", bg_color="transparent", fg_color="transparent")
+    copyright.place(relx=0.005, rely=0.915)
+
+    window.bind("<Escape>", lambda event: close())
+    window.protocol("WM_DELETE_WINDOW", close)
+    window.mainloop()
```

### Comparing `pymicro365-0.0.5/setup.py` & `pymicro365-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="pymicro365",
-    version="0.0.5",
+    version="0.0.6",
     author="Informatic365",
     author_email="chen.runkang1@gmail.com",
     description="This is a module to simplify closing the PC",
     long_description="This is a module to simplify functions of the MicroSoftware",
     url="https://sites.google.com/view/infocommunity365/projects/pymicro365",
     packages=["pymicro365"],
     python_requires=">=3.10",
```

