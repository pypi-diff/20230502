# Comparing `tmp/pymicro365-0.0.4.tar.gz` & `tmp/pymicro365-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymicro365-0.0.4.tar", last modified: Tue May  2 18:45:24 2023, max compression
+gzip compressed data, was "pymicro365-0.0.5.tar", last modified: Tue May  2 18:54:27 2023, max compression
```

## Comparing `pymicro365-0.0.4.tar` & `pymicro365-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 18:45:24.858322 pymicro365-0.0.4/
--rw-rw-rw-   0        0        0      340 2023-05-02 18:45:24.857324 pymicro365-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 18:45:24.846354 pymicro365-0.0.4/pymicro365/
--rw-rw-rw-   0        0        0     3267 2023-05-02 18:40:29.000000 pymicro365-0.0.4/pymicro365/__init__.py
--rw-rw-rw-   0        0        0     2956 2023-05-02 18:24:53.000000 pymicro365-0.0.4/pymicro365/pyicalc.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:45:24.856328 pymicro365-0.0.4/pymicro365.egg-info/
--rw-rw-rw-   0        0        0      340 2023-05-02 18:45:24.000000 pymicro365-0.0.4/pymicro365.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-02 18:45:24.000000 pymicro365-0.0.4/pymicro365.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 18:45:24.000000 pymicro365-0.0.4/pymicro365.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-02 18:45:24.000000 pymicro365-0.0.4/pymicro365.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-02 18:45:24.000000 pymicro365-0.0.4/pymicro365.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 18:45:24.858322 pymicro365-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      514 2023-05-02 18:45:19.000000 pymicro365-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:54:27.031678 pymicro365-0.0.5/
+-rw-rw-rw-   0        0        0      340 2023-05-02 18:54:27.030679 pymicro365-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 18:54:27.011731 pymicro365-0.0.5/pymicro365/
+-rw-rw-rw-   0        0        0     3267 2023-05-02 18:40:29.000000 pymicro365-0.0.5/pymicro365/__init__.py
+-rw-rw-rw-   0        0        0     2989 2023-05-02 18:49:27.000000 pymicro365-0.0.5/pymicro365/pyicalc.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:54:27.029683 pymicro365-0.0.5/pymicro365.egg-info/
+-rw-rw-rw-   0        0        0      340 2023-05-02 18:54:26.000000 pymicro365-0.0.5/pymicro365.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-02 18:54:26.000000 pymicro365-0.0.5/pymicro365.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 18:54:26.000000 pymicro365-0.0.5/pymicro365.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-02 18:54:26.000000 pymicro365-0.0.5/pymicro365.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-02 18:54:26.000000 pymicro365-0.0.5/pymicro365.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 18:54:27.032676 pymicro365-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      514 2023-05-02 18:54:13.000000 pymicro365-0.0.5/setup.py
```

### Comparing `pymicro365-0.0.4/pymicro365/__init__.py` & `pymicro365-0.0.5/pymicro365/__init__.py`

 * *Files identical despite different names*

### Comparing `pymicro365-0.0.4/pymicro365/pyicalc.py` & `pymicro365-0.0.5/pymicro365/pyicalc.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 def equal():
     try:
         y=str(eval(entry.get()))
         entry.delete(0,ct.END)
         entry.insert(0,y)
     except:
         tkinter.messagebox.showinfo("Error","Syntax Error")
+        entry.delete(0, ct.END)
 
 def clear():
     entry.delete(0,ct.END)
     
 button_1=ct.CTkButton(master=frame,text='1',command=lambda:myclick(1))
 button_1.grid(row=1,column=0,pady=4)
 button_2=CTkButton(master=frame,text='2',command=lambda:myclick(2))
```

### Comparing `pymicro365-0.0.4/setup.py` & `pymicro365-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="pymicro365",
-    version="0.0.4",
+    version="0.0.5",
     author="Informatic365",
     author_email="chen.runkang1@gmail.com",
     description="This is a module to simplify closing the PC",
     long_description="This is a module to simplify functions of the MicroSoftware",
     url="https://sites.google.com/view/infocommunity365/projects/pymicro365",
     packages=["pymicro365"],
     python_requires=">=3.10",
```

