# Comparing `tmp/pygredients-0.1.1.tar.gz` & `tmp/pygredients-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygredients-0.1.1.tar", last modified: Tue May  2 00:34:00 2023, max compression
+gzip compressed data, was "pygredients-0.1.2.tar", last modified: Tue May  2 00:38:01 2023, max compression
```

## Comparing `pygredients-0.1.1.tar` & `pygredients-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:34:00.283007 pygredients-0.1.1/
-drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:34:00.281038 pygredients-0.1.1/.idea/
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      176 2023-04-16 03:27:57.000000 pygredients-0.1.1/.idea/.gitignore
-drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:34:00.281459 pygredients-0.1.1/.idea/inspectionProfiles/
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4819 2023-04-16 03:29:34.000000 pygredients-0.1.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      174 2023-04-16 03:29:34.000000 pygredients-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      185 2023-04-16 03:29:34.000000 pygredients-0.1.1/.idea/misc.xml
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      296 2023-04-16 03:29:34.000000 pygredients-0.1.1/.idea/modules.xml
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      284 2023-04-16 03:29:34.000000 pygredients-0.1.1/.idea/python-design-patterns.iml
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      180 2023-05-01 23:57:57.000000 pygredients-0.1.1/.idea/vcs.xml
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1082 2023-05-01 23:27:20.000000 pygredients-0.1.1/LICENSE.txt
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     2732 2023-05-02 00:34:00.282864 pygredients-0.1.1/PKG-INFO
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1998 2023-05-02 00:14:13.000000 pygredients-0.1.1/README.md
-drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:34:00.281659 pygredients-0.1.1/__pycache__/
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     2873 2023-04-18 20:41:21.000000 pygredients-0.1.1/__pycache__/node.cpython-39.pyc
-drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:34:00.281913 pygredients-0.1.1/_trial_temp/
--rwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-04-18 20:33:46.000000 pygredients-0.1.1/_trial_temp/_trial_marker
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     5155 2023-04-18 20:37:26.000000 pygredients-0.1.1/adapter_linkedlist.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4650 2023-04-18 20:37:26.000000 pygredients-0.1.1/adapter_queue.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4432 2023-04-18 20:37:26.000000 pygredients-0.1.1/adapter_stack.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1872 2023-04-18 20:37:26.000000 pygredients-0.1.1/node.py
-drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:34:00.282645 pygredients-0.1.1/pygredients.egg-info/
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     2732 2023-05-02 00:34:00.000000 pygredients-0.1.1/pygredients.egg-info/PKG-INFO
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      599 2023-05-02 00:34:00.000000 pygredients-0.1.1/pygredients.egg-info/SOURCES.txt
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)        1 2023-05-02 00:34:00.000000 pygredients-0.1.1/pygredients.egg-info/dependency_links.txt
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       13 2023-05-02 00:34:00.000000 pygredients-0.1.1/pygredients.egg-info/requires.txt
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)        1 2023-05-02 00:34:00.000000 pygredients-0.1.1/pygredients.egg-info/top_level.txt
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       38 2023-05-02 00:34:00.283061 pygredients-0.1.1/setup.cfg
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      966 2023-05-02 00:33:42.000000 pygredients-0.1.1/setup.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4259 2023-04-18 20:33:05.000000 pygredients-0.1.1/test_adapter_linkedlist.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     3841 2023-04-18 20:37:26.000000 pygredients-0.1.1/test_adapter_queue.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     3757 2023-04-18 20:33:11.000000 pygredients-0.1.1/test_adapter_stack.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1086 2023-04-18 20:42:06.000000 pygredients-0.1.1/test_node.py
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:38:01.099979 pygredients-0.1.2/
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:38:01.098113 pygredients-0.1.2/.idea/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      176 2023-04-16 03:27:57.000000 pygredients-0.1.2/.idea/.gitignore
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:38:01.098538 pygredients-0.1.2/.idea/inspectionProfiles/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4819 2023-04-16 03:29:34.000000 pygredients-0.1.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      174 2023-04-16 03:29:34.000000 pygredients-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      185 2023-04-16 03:29:34.000000 pygredients-0.1.2/.idea/misc.xml
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      296 2023-04-16 03:29:34.000000 pygredients-0.1.2/.idea/modules.xml
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      284 2023-04-16 03:29:34.000000 pygredients-0.1.2/.idea/python-design-patterns.iml
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      180 2023-05-02 00:36:11.000000 pygredients-0.1.2/.idea/vcs.xml
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1082 2023-05-01 23:27:20.000000 pygredients-0.1.2/LICENSE.txt
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     2745 2023-05-02 00:38:01.099807 pygredients-0.1.2/PKG-INFO
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     2011 2023-05-02 00:37:50.000000 pygredients-0.1.2/README.md
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-01 23:37:49.000000 pygredients-0.1.2/__init__.py
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:38:01.098768 pygredients-0.1.2/__pycache__/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     2873 2023-04-18 20:41:21.000000 pygredients-0.1.2/__pycache__/node.cpython-39.pyc
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:38:01.099017 pygredients-0.1.2/_trial_temp/
+-rwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-04-18 20:33:46.000000 pygredients-0.1.2/_trial_temp/_trial_marker
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     5155 2023-04-18 20:37:26.000000 pygredients-0.1.2/adapter_linkedlist.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4650 2023-04-18 20:37:26.000000 pygredients-0.1.2/adapter_queue.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4432 2023-04-18 20:37:26.000000 pygredients-0.1.2/adapter_stack.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1872 2023-04-18 20:37:26.000000 pygredients-0.1.2/node.py
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:38:01.099610 pygredients-0.1.2/pygredients.egg-info/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     2745 2023-05-02 00:38:00.000000 pygredients-0.1.2/pygredients.egg-info/PKG-INFO
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      611 2023-05-02 00:38:01.000000 pygredients-0.1.2/pygredients.egg-info/SOURCES.txt
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)        1 2023-05-02 00:38:00.000000 pygredients-0.1.2/pygredients.egg-info/dependency_links.txt
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       13 2023-05-02 00:38:00.000000 pygredients-0.1.2/pygredients.egg-info/requires.txt
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)        1 2023-05-02 00:38:00.000000 pygredients-0.1.2/pygredients.egg-info/top_level.txt
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       38 2023-05-02 00:38:01.100022 pygredients-0.1.2/setup.cfg
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      966 2023-05-02 00:37:56.000000 pygredients-0.1.2/setup.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4259 2023-04-18 20:33:05.000000 pygredients-0.1.2/test_adapter_linkedlist.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     3841 2023-04-18 20:37:26.000000 pygredients-0.1.2/test_adapter_queue.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     3757 2023-04-18 20:33:11.000000 pygredients-0.1.2/test_adapter_stack.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1086 2023-04-18 20:42:06.000000 pygredients-0.1.2/test_node.py
```

### Comparing `pygredients-0.1.1/.idea/inspectionProfiles/Project_Default.xml` & `pygredients-0.1.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.1/LICENSE.txt` & `pygredients-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.1/PKG-INFO` & `pygredients-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygredients
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pygredients is an open-source Python library for data structures and algorithms available on PyPi.
 Home-page: https://github.com/FBH514/pygredients
 Author: François Boulay-Handfield
 Author-email: fbhworks@icloud.com
 License: MIT
 Keywords: data structures algorithms
 Platform: UNKNOWN
@@ -15,15 +15,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Pygredients
-##### Pygredients is an open-source Python library for data structures and algorithms available on PyPi. 🍎🍊🍋🫐
+
+Version 0.1.2
+
+Pygredients is an open-source Python library for data structures and algorithms available on PyPi. 🍎🍊🍋🫐
 
 ## Installation
 ```pip install pygredients```
 
 ```pip3 install pygredients``` for OSX users
 
 ## Usage
@@ -57,15 +60,15 @@
 # Check if the linked list is empty
 ll.is_empty() # False
 
 # Print the linked list
 print(ll) # [1, 3]
 
 # Limit the length of the linked list
-ll.limit(2)
+ll.limit = 2
 ll.append(4) # ValueError: Cannot append 4 to Linked List as it is full.
 ```
 
 ### Stack
 ```python
 # Create a stack
 stack = Stack()
@@ -90,15 +93,15 @@
 # Check if the stack is empty
 stack.is_empty() # False
 
 # Print the stack
 print(stack) # [1, 2]
 
 # Limit the length of the stack
-stack.limit(2)
+stack.limit = 2
 stack.push(4) # ValueError: Cannot push 4 to Stack as it is full.
 ```
 
 ### Queue
 ```python
 # Create a queue
 queue = Queue()
@@ -123,11 +126,11 @@
 # Check if the queue is empty
 queue.is_empty() # False
 
 # Print the queue
 print(queue) # [2, 3]
 
 # Limit the length of the queue
-queue.limit(2) 
+queue.limit = 2 
 queue.enqueue(4) # ValueError: Cannot enqueue 4 to Queue as it is full.
 ```
```

### Comparing `pygredients-0.1.1/README.md` & `pygredients-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Pygredients
-##### Pygredients is an open-source Python library for data structures and algorithms available on PyPi. 🍎🍊🍋🫐
+
+Version 0.1.2
+
+Pygredients is an open-source Python library for data structures and algorithms available on PyPi. 🍎🍊🍋🫐
 
 ## Installation
 ```pip install pygredients```
 
 ```pip3 install pygredients``` for OSX users
 
 ## Usage
@@ -37,15 +40,15 @@
 # Check if the linked list is empty
 ll.is_empty() # False
 
 # Print the linked list
 print(ll) # [1, 3]
 
 # Limit the length of the linked list
-ll.limit(2)
+ll.limit = 2
 ll.append(4) # ValueError: Cannot append 4 to Linked List as it is full.
 ```
 
 ### Stack
 ```python
 # Create a stack
 stack = Stack()
@@ -70,15 +73,15 @@
 # Check if the stack is empty
 stack.is_empty() # False
 
 # Print the stack
 print(stack) # [1, 2]
 
 # Limit the length of the stack
-stack.limit(2)
+stack.limit = 2
 stack.push(4) # ValueError: Cannot push 4 to Stack as it is full.
 ```
 
 ### Queue
 ```python
 # Create a queue
 queue = Queue()
@@ -103,10 +106,10 @@
 # Check if the queue is empty
 queue.is_empty() # False
 
 # Print the queue
 print(queue) # [2, 3]
 
 # Limit the length of the queue
-queue.limit(2) 
+queue.limit = 2 
 queue.enqueue(4) # ValueError: Cannot enqueue 4 to Queue as it is full.
 ```
```

### Comparing `pygredients-0.1.1/__pycache__/node.cpython-39.pyc` & `pygredients-0.1.2/__pycache__/node.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.1/adapter_linkedlist.py` & `pygredients-0.1.2/adapter_linkedlist.py`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.1/adapter_queue.py` & `pygredients-0.1.2/adapter_queue.py`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.1/adapter_stack.py` & `pygredients-0.1.2/adapter_stack.py`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.1/node.py` & `pygredients-0.1.2/node.py`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.1/pygredients.egg-info/PKG-INFO` & `pygredients-0.1.2/pygredients.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygredients
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pygredients is an open-source Python library for data structures and algorithms available on PyPi.
 Home-page: https://github.com/FBH514/pygredients
 Author: François Boulay-Handfield
 Author-email: fbhworks@icloud.com
 License: MIT
 Keywords: data structures algorithms
 Platform: UNKNOWN
@@ -15,15 +15,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Pygredients
-##### Pygredients is an open-source Python library for data structures and algorithms available on PyPi. 🍎🍊🍋🫐
+
+Version 0.1.2
+
+Pygredients is an open-source Python library for data structures and algorithms available on PyPi. 🍎🍊🍋🫐
 
 ## Installation
 ```pip install pygredients```
 
 ```pip3 install pygredients``` for OSX users
 
 ## Usage
@@ -57,15 +60,15 @@
 # Check if the linked list is empty
 ll.is_empty() # False
 
 # Print the linked list
 print(ll) # [1, 3]
 
 # Limit the length of the linked list
-ll.limit(2)
+ll.limit = 2
 ll.append(4) # ValueError: Cannot append 4 to Linked List as it is full.
 ```
 
 ### Stack
 ```python
 # Create a stack
 stack = Stack()
@@ -90,15 +93,15 @@
 # Check if the stack is empty
 stack.is_empty() # False
 
 # Print the stack
 print(stack) # [1, 2]
 
 # Limit the length of the stack
-stack.limit(2)
+stack.limit = 2
 stack.push(4) # ValueError: Cannot push 4 to Stack as it is full.
 ```
 
 ### Queue
 ```python
 # Create a queue
 queue = Queue()
@@ -123,11 +126,11 @@
 # Check if the queue is empty
 queue.is_empty() # False
 
 # Print the queue
 print(queue) # [2, 3]
 
 # Limit the length of the queue
-queue.limit(2) 
+queue.limit = 2 
 queue.enqueue(4) # ValueError: Cannot enqueue 4 to Queue as it is full.
 ```
```

### Comparing `pygredients-0.1.1/pygredients.egg-info/SOURCES.txt` & `pygredients-0.1.2/pygredients.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE.txt
 README.md
+__init__.py
 adapter_linkedlist.py
 adapter_queue.py
 adapter_stack.py
 node.py
 setup.py
 test_adapter_linkedlist.py
 test_adapter_queue.py
```

### Comparing `pygredients-0.1.1/setup.py` & `pygredients-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pygredients',
-    version='0.1.1',
+    version='0.1.2',
     description='Pygredients is an open-source Python library for data structures and algorithms available on PyPi.',
     long_description=f"{long_description}",
     long_description_content_type="text/markdown",
     author='François Boulay-Handfield',
     author_email="fbhworks@icloud.com",
     url="https://github.com/FBH514/pygredients",
     license="MIT",
```

### Comparing `pygredients-0.1.1/test_adapter_linkedlist.py` & `pygredients-0.1.2/test_adapter_linkedlist.py`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.1/test_adapter_queue.py` & `pygredients-0.1.2/test_adapter_queue.py`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.1/test_adapter_stack.py` & `pygredients-0.1.2/test_adapter_stack.py`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.1/test_node.py` & `pygredients-0.1.2/test_node.py`

 * *Files identical despite different names*

