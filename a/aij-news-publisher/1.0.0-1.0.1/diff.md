# Comparing `tmp/aij-news-publisher-1.0.0.tar.gz` & `tmp/aij-news-publisher-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-news-publisher-1.0.0.tar", last modified: Tue May  2 20:26:10 2023, max compression
+gzip compressed data, was "aij-news-publisher-1.0.1.tar", last modified: Tue May  2 21:07:38 2023, max compression
```

## Comparing `aij-news-publisher-1.0.0.tar` & `aij-news-publisher-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 20:26:10.000000 aij-news-publisher-1.0.0/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4390 2023-05-02 20:26:12.000000 aij-news-publisher-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.0/README.md
--rw-rw-rw-   0        0        0     6551 2023-05-02 20:00:46.000000 aij-news-publisher-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 20:26:12.000000 aij-news-publisher-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 20:26:10.000000 aij-news-publisher-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 20:26:10.000000 aij-news-publisher-1.0.0/src/aij_news_publisher.egg-info/
--rw-rw-rw-   0        0        0     4390 2023-05-02 20:26:10.000000 aij-news-publisher-1.0.0/src/aij_news_publisher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-05-02 20:26:10.000000 aij-news-publisher-1.0.0/src/aij_news_publisher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 20:26:10.000000 aij-news-publisher-1.0.0/src/aij_news_publisher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-02 20:26:10.000000 aij-news-publisher-1.0.0/src/aij_news_publisher.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      118 2023-05-02 20:26:10.000000 aij-news-publisher-1.0.0/src/aij_news_publisher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-02 20:26:10.000000 aij-news-publisher-1.0.0/src/aij_news_publisher.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 20:26:10.000000 aij-news-publisher-1.0.0/src/news_publisher/
--rw-rw-rw-   0        0        0      631 2023-05-02 20:25:50.000000 aij-news-publisher-1.0.0/src/news_publisher/__init__.py
--rw-rw-rw-   0        0        0     3293 2023-05-02 19:39:04.000000 aij-news-publisher-1.0.0/src/news_publisher/publisher.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4390 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.1/README.md
+-rw-rw-rw-   0        0        0     6562 2023-05-02 21:06:04.000000 aij-news-publisher-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/
+-rw-rw-rw-   0        0        0     4390 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      118 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/news_publisher/
+-rw-rw-rw-   0        0        0      631 2023-05-02 20:25:50.000000 aij-news-publisher-1.0.1/src/news_publisher/__init__.py
+-rw-rw-rw-   0        0        0     3293 2023-05-02 19:39:04.000000 aij-news-publisher-1.0.1/src/news_publisher/news_publisher.py
```

### Comparing `aij-news-publisher-1.0.0/LICENSE.txt` & `aij-news-publisher-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.0/PKG-INFO` & `aij-news-publisher-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-publisher
-Version: 1.0.0
+Version: 1.0.1
 Summary: AI Journalist News Publisher package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 Maintainer-email: Intesaaf <intesaaf@gmail.com>, Fatima <fatima@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `aij-news-publisher-1.0.0/README.md` & `aij-news-publisher-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.0/pyproject.toml` & `aij-news-publisher-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-news-publisher"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.0"  # Required
+version = "1.0.1"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist News Publisher package"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -140,15 +140,15 @@
 "Funding" = "https://donate.pypi.org"
 "Say Thanks!" = "http://saythanks.io/to/aij"
 "Source" = "https://github.com/codesapienbe/aij-news-publisher"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
-aijnp = "aij:main"
+aijnp = "news_publisher:main"
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 package-data = { "db" = ["*.dat"] }
```

### Comparing `aij-news-publisher-1.0.0/src/aij_news_publisher.egg-info/PKG-INFO` & `aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-publisher
-Version: 1.0.0
+Version: 1.0.1
 Summary: AI Journalist News Publisher package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 Maintainer-email: Intesaaf <intesaaf@gmail.com>, Fatima <fatima@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `aij-news-publisher-1.0.0/src/news_publisher/__init__.py` & `aij-news-publisher-1.0.1/src/news_publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.0/src/news_publisher/publisher.py` & `aij-news-publisher-1.0.1/src/news_publisher/news_publisher.py`

 * *Files identical despite different names*

