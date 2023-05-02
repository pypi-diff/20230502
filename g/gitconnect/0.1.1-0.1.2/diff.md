# Comparing `tmp/gitconnect-0.1.1.tar.gz` & `tmp/gitconnect-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitconnect-0.1.1.tar", last modified: Thu Mar 30 10:23:56 2023, max compression
+gzip compressed data, was "gitconnect-0.1.2.tar", last modified: Tue May  2 17:12:07 2023, max compression
```

## Comparing `gitconnect-0.1.1.tar` & `gitconnect-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-30 10:23:56.007423 gitconnect-0.1.1/
--rw-r--r--   0 ed        (1000) ed        (1000)      594 2023-03-30 10:23:56.007423 gitconnect-0.1.1/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)     2101 2023-03-30 10:15:36.000000 gitconnect-0.1.1/README.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-30 10:23:56.007423 gitconnect-0.1.1/gitconnect/
--rw-r--r--   0 ed        (1000) ed        (1000)     3161 2023-03-30 09:31:41.000000 gitconnect-0.1.1/gitconnect/GitWrapper.py
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-03-30 08:49:38.000000 gitconnect-0.1.1/gitconnect/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-03-30 10:23:56.007423 gitconnect-0.1.1/gitconnect.egg-info/
--rw-r--r--   0 ed        (1000) ed        (1000)      594 2023-03-30 10:23:55.000000 gitconnect-0.1.1/gitconnect.egg-info/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)      235 2023-03-30 10:23:55.000000 gitconnect-0.1.1/gitconnect.egg-info/SOURCES.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-03-30 10:23:55.000000 gitconnect-0.1.1/gitconnect.egg-info/dependency_links.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        9 2023-03-30 10:23:55.000000 gitconnect-0.1.1/gitconnect.egg-info/requires.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       11 2023-03-30 10:23:55.000000 gitconnect-0.1.1/gitconnect.egg-info/top_level.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-03-30 10:23:56.011423 gitconnect-0.1.1/setup.cfg
--rw-r--r--   0 ed        (1000) ed        (1000)      662 2023-03-30 10:19:38.000000 gitconnect-0.1.1/setup.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-02 17:12:07.773558 gitconnect-0.1.2/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      594 2023-05-02 17:12:07.773558 gitconnect-0.1.2/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)     1783 2023-05-02 08:09:31.000000 gitconnect-0.1.2/README.md
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-02 17:12:07.773558 gitconnect-0.1.2/gitconnect/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)     3161 2023-05-01 15:09:26.000000 gitconnect-0.1.2/gitconnect/GitWrapper.py
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       34 2023-05-02 08:09:25.000000 gitconnect-0.1.2/gitconnect/__init__.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-02 17:12:07.773558 gitconnect-0.1.2/gitconnect.egg-info/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      594 2023-05-02 17:12:07.000000 gitconnect-0.1.2/gitconnect.egg-info/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      235 2023-05-02 17:12:07.000000 gitconnect-0.1.2/gitconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-05-02 17:12:07.000000 gitconnect-0.1.2/gitconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-05-02 17:12:07.000000 gitconnect-0.1.2/gitconnect.egg-info/requires.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       11 2023-05-02 17:12:07.000000 gitconnect-0.1.2/gitconnect.egg-info/top_level.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-05-02 17:12:07.773558 gitconnect-0.1.2/setup.cfg
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      662 2023-05-02 08:45:33.000000 gitconnect-0.1.2/setup.py
```

### Comparing `gitconnect-0.1.1/PKG-INFO` & `gitconnect-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitconnect
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python wrapper for the GitHub API
 Home-page: UNKNOWN
 Author: Ed
 Author-email: ed.a9a6a@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gitconnect-0.1.1/README.md` & `gitconnect-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -24,36 +24,21 @@
 
 Now, you can use the GitWrapper methods to interact with the GitHub API.
 
 ## Example 1: Search for repositories by user and keyword
 ```python
 from gitconnect import GitWrapper
 
-access_token = 'your_access_token_here'
-
+access_token = "place_your_github_token_here"
 wrapper = GitWrapper(access_token)
-user_name ="the_git_user_name_here"
-repos = wrapper.search_repos_by_user(user_name, "python")
-for repo in repos:
-    print(repo.name)
+user_name ="place_the_git_user_name_here"
+repos = wrapper.search_repos_by_user(user_name, "language:py")
+print(repos)
 ```
 
-## Example 2: Get details about a specific repository
-```python
-
-from gitconnect import GitWrapper
-
-access_token = 'your_access_token_here'
-
-wrapper = GitWrapper(access_token)
-user_name ="the_git_user_name_here"
-repo = wrapper.get_repo(user_name, "hello-world")
-print(repo.name)
-print(repo.description)
-```
 
 For more information on how to use GitConnect, please refer to the documentation.
 
 ## Contributing
 
 If you would like to contribute to GitConnect, please follow these steps:
```

### Comparing `gitconnect-0.1.1/gitconnect/GitWrapper.py` & `gitconnect-0.1.2/gitconnect/GitWrapper.py`

 * *Files identical despite different names*

### Comparing `gitconnect-0.1.1/gitconnect.egg-info/PKG-INFO` & `gitconnect-0.1.2/gitconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitconnect
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python wrapper for the GitHub API
 Home-page: UNKNOWN
 Author: Ed
 Author-email: ed.a9a6a@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gitconnect-0.1.1/setup.py` & `gitconnect-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='gitconnect',
-    version='0.1.1',
+    version='0.1.2',
     description='A Python wrapper for the GitHub API',
     author='Ed',
     author_email='ed.a9a6a@gmail.com',
     packages=['gitconnect'],
     install_requires=['requests'],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

