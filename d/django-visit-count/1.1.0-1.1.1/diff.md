# Comparing `tmp/django-visit-count-1.1.0.tar.gz` & `tmp/django-visit-count-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-visit-count-1.1.0.tar", last modified: Tue Sep 13 09:11:31 2022, max compression
+gzip compressed data, was "django-visit-count-1.1.1.tar", last modified: Tue May  2 12:35:04 2023, max compression
```

## Comparing `django-visit-count-1.1.0.tar` & `django-visit-count-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 naderi    (1000) users      (984)        0 2022-09-13 09:11:31.459929 django-visit-count-1.1.0/
--rw-r--r--   0 naderi    (1000) users      (984)     1078 2022-09-13 07:32:23.000000 django-visit-count-1.1.0/LICENSE.txt
--rw-r--r--   0 naderi    (1000) users      (984)       84 2022-09-13 07:39:49.000000 django-visit-count-1.1.0/MANIFEST.in
--rw-r--r--   0 naderi    (1000) users      (984)     3056 2022-09-13 09:11:31.459929 django-visit-count-1.1.0/PKG-INFO
--rw-r--r--   0 naderi    (1000) users      (984)     2057 2022-09-13 09:10:33.000000 django-visit-count-1.1.0/README.md
-drwxr-xr-x   0 naderi    (1000) users      (984)        0 2022-09-13 09:11:31.459929 django-visit-count-1.1.0/django_visit_count/
--rw-r--r--   0 naderi    (1000) users      (984)        0 2022-09-13 07:42:10.000000 django-visit-count-1.1.0/django_visit_count/__init__.py
--rw-r--r--   0 naderi    (1000) users      (984)      150 2022-09-13 08:14:58.000000 django-visit-count-1.1.0/django_visit_count/app_settings.py
-drwxr-xr-x   0 naderi    (1000) users      (984)        0 2022-09-13 09:11:31.459929 django-visit-count-1.1.0/django_visit_count/locale/
-drwxr-xr-x   0 naderi    (1000) users      (984)        0 2022-09-13 09:11:31.459929 django-visit-count-1.1.0/django_visit_count/locale/fa/
-drwxr-xr-x   0 naderi    (1000) users      (984)        0 2022-09-13 09:11:31.459929 django-visit-count-1.1.0/django_visit_count/locale/fa/LC_MESSAGES/
--rw-r--r--   0 naderi    (1000) users      (984)      439 2022-09-13 07:47:47.000000 django-visit-count-1.1.0/django_visit_count/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 naderi    (1000) users      (984)      669 2022-09-13 07:47:39.000000 django-visit-count-1.1.0/django_visit_count/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0 naderi    (1000) users      (984)      624 2022-09-13 08:41:33.000000 django-visit-count-1.1.0/django_visit_count/mixins.py
--rw-r--r--   0 naderi    (1000) users      (984)      737 2022-09-13 08:16:19.000000 django-visit-count-1.1.0/django_visit_count/utils.py
-drwxr-xr-x   0 naderi    (1000) users      (984)        0 2022-09-13 09:11:31.459929 django-visit-count-1.1.0/django_visit_count.egg-info/
--rw-r--r--   0 naderi    (1000) users      (984)     3056 2022-09-13 09:11:31.000000 django-visit-count-1.1.0/django_visit_count.egg-info/PKG-INFO
--rw-r--r--   0 naderi    (1000) users      (984)      491 2022-09-13 09:11:31.000000 django-visit-count-1.1.0/django_visit_count.egg-info/SOURCES.txt
--rw-r--r--   0 naderi    (1000) users      (984)        1 2022-09-13 09:11:31.000000 django-visit-count-1.1.0/django_visit_count.egg-info/dependency_links.txt
--rw-r--r--   0 naderi    (1000) users      (984)       51 2022-09-13 09:11:31.000000 django-visit-count-1.1.0/django_visit_count.egg-info/requires.txt
--rw-r--r--   0 naderi    (1000) users      (984)       19 2022-09-13 09:11:31.000000 django-visit-count-1.1.0/django_visit_count.egg-info/top_level.txt
--rw-r--r--   0 naderi    (1000) users      (984)      142 2022-09-13 07:38:52.000000 django-visit-count-1.1.0/pyproject.toml
--rw-r--r--   0 naderi    (1000) users      (984)       38 2022-09-13 09:11:31.459929 django-visit-count-1.1.0/setup.cfg
--rw-r--r--   0 naderi    (1000) users      (984)     1634 2022-09-13 09:10:39.000000 django-visit-count-1.1.0/setup.py
+drwxr-xr-x   0 naderi    (1000) users      (984)        0 2023-05-02 12:35:04.669420 django-visit-count-1.1.1/
+-rw-r--r--   0 naderi    (1000) users      (984)     1078 2022-09-13 07:32:23.000000 django-visit-count-1.1.1/LICENSE.txt
+-rw-r--r--   0 naderi    (1000) users      (984)       84 2022-09-13 07:39:49.000000 django-visit-count-1.1.1/MANIFEST.in
+-rw-r--r--   0 naderi    (1000) users      (984)     3063 2023-05-02 12:35:04.669420 django-visit-count-1.1.1/PKG-INFO
+-rw-r--r--   0 naderi    (1000) users      (984)     2064 2022-11-13 11:41:24.000000 django-visit-count-1.1.1/README.md
+drwxr-xr-x   0 naderi    (1000) users      (984)        0 2023-05-02 12:35:04.669420 django-visit-count-1.1.1/django_visit_count/
+-rw-r--r--   0 naderi    (1000) users      (984)        0 2022-09-13 07:42:10.000000 django-visit-count-1.1.1/django_visit_count/__init__.py
+-rw-r--r--   0 naderi    (1000) users      (984)      150 2022-09-13 08:14:58.000000 django-visit-count-1.1.1/django_visit_count/app_settings.py
+drwxr-xr-x   0 naderi    (1000) users      (984)        0 2023-05-02 12:35:04.669420 django-visit-count-1.1.1/django_visit_count/locale/
+drwxr-xr-x   0 naderi    (1000) users      (984)        0 2023-05-02 12:35:04.669420 django-visit-count-1.1.1/django_visit_count/locale/fa/
+drwxr-xr-x   0 naderi    (1000) users      (984)        0 2023-05-02 12:35:04.669420 django-visit-count-1.1.1/django_visit_count/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 naderi    (1000) users      (984)      439 2022-09-13 07:47:47.000000 django-visit-count-1.1.1/django_visit_count/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 naderi    (1000) users      (984)      669 2022-09-13 07:47:39.000000 django-visit-count-1.1.1/django_visit_count/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0 naderi    (1000) users      (984)      763 2023-05-02 12:32:05.000000 django-visit-count-1.1.1/django_visit_count/mixins.py
+-rw-r--r--   0 naderi    (1000) users      (984)      737 2022-09-13 08:16:19.000000 django-visit-count-1.1.1/django_visit_count/utils.py
+drwxr-xr-x   0 naderi    (1000) users      (984)        0 2023-05-02 12:35:04.669420 django-visit-count-1.1.1/django_visit_count.egg-info/
+-rw-r--r--   0 naderi    (1000) users      (984)     3063 2023-05-02 12:35:04.000000 django-visit-count-1.1.1/django_visit_count.egg-info/PKG-INFO
+-rw-r--r--   0 naderi    (1000) users      (984)      491 2023-05-02 12:35:04.000000 django-visit-count-1.1.1/django_visit_count.egg-info/SOURCES.txt
+-rw-r--r--   0 naderi    (1000) users      (984)        1 2023-05-02 12:35:04.000000 django-visit-count-1.1.1/django_visit_count.egg-info/dependency_links.txt
+-rw-r--r--   0 naderi    (1000) users      (984)       51 2023-05-02 12:35:04.000000 django-visit-count-1.1.1/django_visit_count.egg-info/requires.txt
+-rw-r--r--   0 naderi    (1000) users      (984)       19 2023-05-02 12:35:04.000000 django-visit-count-1.1.1/django_visit_count.egg-info/top_level.txt
+-rw-r--r--   0 naderi    (1000) users      (984)      142 2022-09-13 07:38:52.000000 django-visit-count-1.1.1/pyproject.toml
+-rw-r--r--   0 naderi    (1000) users      (984)       38 2023-05-02 12:35:04.669420 django-visit-count-1.1.1/setup.cfg
+-rw-r--r--   0 naderi    (1000) users      (984)     1634 2023-05-02 12:32:05.000000 django-visit-count-1.1.1/setup.py
```

### Comparing `django-visit-count-1.1.0/LICENSE.txt` & `django-visit-count-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-visit-count-1.1.0/PKG-INFO` & `django-visit-count-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-visit-count
-Version: 1.1.0
+Version: 1.1.1
 Summary: Count visits using cache for Django models
 Home-page: https://github.com/QueraTeam/django-visit-count
 Download-URL: https://pypi.python.org/pypi/django-visit-count
 Author: Mohammad Javad Naderi
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -61,15 +61,15 @@
 ```
 
 Count visits in your view like this:
 
 ```python
 def view_blog_post(request, post_id):
     post = get_object_or_404(MyBlogPost, pk=post_id)
-    post.count_visit()
+    post.count_visit(request)
     ...
 ```
 
 ## Advanced Usage
 
 If you need more control, you can use `is_new_visit` function.
```

### Comparing `django-visit-count-1.1.0/README.md` & `django-visit-count-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ```
 
 Count visits in your view like this:
 
 ```python
 def view_blog_post(request, post_id):
     post = get_object_or_404(MyBlogPost, pk=post_id)
-    post.count_visit()
+    post.count_visit(request)
     ...
 ```
 
 ## Advanced Usage
 
 If you need more control, you can use `is_new_visit` function.
```

### Comparing `django-visit-count-1.1.0/django_visit_count/locale/fa/LC_MESSAGES/django.po` & `django-visit-count-1.1.1/django_visit_count/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-visit-count-1.1.0/django_visit_count/utils.py` & `django-visit-count-1.1.1/django_visit_count/utils.py`

 * *Files identical despite different names*

### Comparing `django-visit-count-1.1.0/django_visit_count.egg-info/PKG-INFO` & `django-visit-count-1.1.1/django_visit_count.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-visit-count
-Version: 1.1.0
+Version: 1.1.1
 Summary: Count visits using cache for Django models
 Home-page: https://github.com/QueraTeam/django-visit-count
 Download-URL: https://pypi.python.org/pypi/django-visit-count
 Author: Mohammad Javad Naderi
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -61,15 +61,15 @@
 ```
 
 Count visits in your view like this:
 
 ```python
 def view_blog_post(request, post_id):
     post = get_object_or_404(MyBlogPost, pk=post_id)
-    post.count_visit()
+    post.count_visit(request)
     ...
 ```
 
 ## Advanced Usage
 
 If you need more control, you can use `is_new_visit` function.
```

### Comparing `django-visit-count-1.1.0/setup.py` & `django-visit-count-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 dev_requirements = [
     "pre-commit",
 ]
 
 setup(
     name="django-visit-count",
-    version="1.1.0",
+    version="1.1.1",
     description="Count visits using cache for Django models",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Mohammad Javad Naderi",
     url="https://github.com/QueraTeam/django-visit-count",
     download_url="https://pypi.python.org/pypi/django-visit-count",
     license="MIT",
```

