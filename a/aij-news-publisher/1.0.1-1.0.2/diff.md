# Comparing `tmp/aij-news-publisher-1.0.1.tar.gz` & `tmp/aij-news-publisher-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-news-publisher-1.0.1.tar", last modified: Tue May  2 21:07:38 2023, max compression
+gzip compressed data, was "aij-news-publisher-1.0.2.tar", last modified: Tue May  2 21:38:43 2023, max compression
```

## Comparing `aij-news-publisher-1.0.1.tar` & `aij-news-publisher-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4390 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.1/README.md
--rw-rw-rw-   0        0        0     6562 2023-05-02 21:06:04.000000 aij-news-publisher-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/
--rw-rw-rw-   0        0        0     4390 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      118 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 21:07:40.000000 aij-news-publisher-1.0.1/src/news_publisher/
--rw-rw-rw-   0        0        0      631 2023-05-02 20:25:50.000000 aij-news-publisher-1.0.1/src/news_publisher/__init__.py
--rw-rw-rw-   0        0        0     3293 2023-05-02 19:39:04.000000 aij-news-publisher-1.0.1/src/news_publisher/news_publisher.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4314 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.2/README.md
+-rw-rw-rw-   0        0        0     6281 2023-05-02 21:38:32.000000 aij-news-publisher-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/
+-rw-rw-rw-   0        0        0     4314 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      118 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/news_publisher/
+-rw-rw-rw-   0        0        0      594 2023-05-02 21:26:06.000000 aij-news-publisher-1.0.2/src/news_publisher/__init__.py
+-rw-rw-rw-   0        0        0     3293 2023-05-02 19:39:04.000000 aij-news-publisher-1.0.2/src/news_publisher/news_publisher.py
```

### Comparing `aij-news-publisher-1.0.1/LICENSE.txt` & `aij-news-publisher-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.1/PKG-INFO` & `aij-news-publisher-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: aij-news-publisher
-Version: 1.0.1
+Version: 1.0.2
 Summary: AI Journalist News Publisher package
 Author-email: Yilmaz Mustafa <dev@mail.be>
-Maintainer-email: Intesaaf <intesaaf@gmail.com>, Fatima <fatima@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
         of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `aij-news-publisher-1.0.1/README.md` & `aij-news-publisher-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.1/pyproject.toml` & `aij-news-publisher-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,160 +1,158 @@
-[project]
-# This is the name of your project. The first time you publish this
-# package, this name will be registered for you. It will determine how
-# users can install this project, e.g.:
-#
-# $ pip install sampleproject
-#
-# And where it will live on PyPI: https://pypi.org/project/sampleproject/
-#
-# There are some restrictions on what makes a valid project name
-# specification here:
-# https://packaging.python.org/specifications/core-metadata/#name
-name = "aij-news-publisher"  # Required
-
-# Versions should comply with PEP 440:
-# https://www.python.org/dev/peps/pep-0440/
-#
-# For a discussion on single-sourcing the version, see
-# https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.1"  # Required
-
-# This is a one-line description or tagline of what your project does. This
-# corresponds to the "Summary" metadata field:
-# https://packaging.python.org/specifications/core-metadata/#summary
-description = "AI Journalist News Publisher package"  # Optional
-
-# This is an optional longer description of your project that represents
-# the body of text which users will see when they visit PyPI.
-#
-# Often, this is the same as your README, so you can just read it in from
-# that file directly (as we have already done above)
-#
-# This field corresponds to the "Description" metadata field:
-# https://packaging.python.org/specifications/core-metadata/#description-optional
-readme = "README.md" # Optional
-
-# Specify which Python versions you support. In contrast to the
-# 'Programming Language' classifiers above, 'pip install' will check this
-# and refuse to install the project if the version does not match. See
-# https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-requires-python = ">=3.7"
-
-# This is either text indicating the license for the distribution, or a file
-# that contains the license
-# https://packaging.python.org/en/latest/specifications/core-metadata/#license
-license = { file = "LICENSE.txt" }
-
-# This field adds keywords for your project which will appear on the
-# project page. What does your project relate to?
-#
-# Note that this is a list of additional keywords, separated
-# by commas, to be used to assist searching for the distribution in a
-# larger catalog.
-keywords = ["aij", "setuptools", "development"]  # Optional
-
-# This should be your name or the name of the organization who originally
-# authored the project, and a valid email address corresponding to the name
-# listed.
-authors = [
-    { name = "Yilmaz Mustafa", email = "dev@mail.be" } # Optional
-]
-
-# This should be your name or the names of the organization who currently
-# maintains the project, and a valid email address corresponding to the name
-# listed.
-maintainers = [
-    { name = "Intesaaf", email = "intesaaf@gmail.com" },
-    { name = "Fatima", email = "fatima@gmail.com" }
-    # Optional
-]
-
-# Classifiers help users find your project by categorizing it.
-#
-# For a list of valid classifiers, see https://pypi.org/classifiers/
-classifiers = [# Optional
-    # How mature is this project? Common values are
-    #   3 - Alpha
-    #   4 - Beta
-    #   5 - Production/Stable
-    "Development Status :: 3 - Alpha",
-    # Indicate who your project is intended for
-    "Intended Audience :: Developers",
-    "Topic :: Software Development :: Build Tools",
-    # Pick your license as you wish
-    "License :: OSI Approved :: MIT License",
-    # Specify the Python versions you support here. In particular, ensure
-    # that you indicate you support Python 3. These classifiers are *not*
-    # checked by "pip install". See instead "python_requires" below.
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3 :: Only",
-]
-
-# This field lists other packages that your project depends on to run.
-# Any package you put here will be installed by pip when your project is
-# installed, so they must be valid existing projects.
-#
-# For an analysis of this field vs pip's requirements files see:
-# https://packaging.python.org/discussions/install-requires-vs-requirements/
-dependencies = [# Optional
-    "peppercorn",
-    "requests",
-    "beautifulsoup4",
-    "newsapi-python",
-    "pandas",
-    "numpy",
-    "matplotlib",
-    "pika"
-]
-
-# List additional groups of dependencies here (e.g. development
-# dependencies). Users will be able to install these using the "extras"
-# syntax, for example:
-#
-#   $ pip install sampleproject[dev]
-#
-# Similar to `dependencies` above, these must be valid existing
-# projects.
-[project.optional-dependencies] # Optional
-dev = ["check-manifest"]
-test = ["coverage"]
-
-# List URLs that are relevant to your project
-#
-# This field corresponds to the "Project-URL" and "Home-Page" metadata fields:
-# https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
-# https://packaging.python.org/specifications/core-metadata/#home-page-optional
-#
-# Examples listed include a pattern for specifying where the package tracks
-# issues, where the source is hosted, where to say thanks to the package
-# maintainers, and where to support the project financially. The key is
-# what's used to render the link text on PyPI.
-[project.urls]  # Optional
-"Homepage" = "https://www.codesapien.be/aij/"
-"Bug Reports" = "https://github.com/codesapienbe/aij-news-publisher/issues"
-"Funding" = "https://donate.pypi.org"
-"Say Thanks!" = "http://saythanks.io/to/aij"
-"Source" = "https://github.com/codesapienbe/aij-news-publisher"
-
-# The following would provide a command line executable called `sample`
-# which executes the function `main` from this package when invoked.
-[project.scripts]  # Optional
-aijnp = "news_publisher:main"
-
-# This is configuration specific to the `setuptools` build backend.
-# If you are using a different build backend, you will need to change this.
-[tool.setuptools]
-# If there are data files included in your packages that need to be
-# installed, specify them here.
-package-data = { "db" = ["*.dat"] }
-
-[build-system]
-# These are the assumed default build requirements from pip:
-# https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
-requires = ["setuptools>=43.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
+[project]
+# This is the name of your project. The first time you publish this
+# package, this name will be registered for you. It will determine how
+# users can install this project, e.g.:
+#
+# $ pip install sampleproject
+#
+# And where it will live on PyPI: https://pypi.org/project/sampleproject/
+#
+# There are some restrictions on what makes a valid project name
+# specification here:
+# https://packaging.python.org/specifications/core-metadata/#name
+name = "aij-news-publisher"  # Required
+
+# Versions should comply with PEP 440:
+# https://www.python.org/dev/peps/pep-0440/
+#
+# For a discussion on single-sourcing the version, see
+# https://packaging.python.org/guides/single-sourcing-package-version/
+version = "1.0.2"
+
+# This is a one-line description or tagline of what your project does. This
+# corresponds to the "Summary" metadata field:
+# https://packaging.python.org/specifications/core-metadata/#summary
+description = "AI Journalist News Publisher package"  # Optional
+
+# This is an optional longer description of your project that represents
+# the body of text which users will see when they visit PyPI.
+#
+# Often, this is the same as your README, so you can just read it in from
+# that file directly (as we have already done above)
+#
+# This field corresponds to the "Description" metadata field:
+# https://packaging.python.org/specifications/core-metadata/#description-optional
+readme = "README.md" # Optional
+
+# Specify which Python versions you support. In contrast to the
+# 'Programming Language' classifiers above, 'pip install' will check this
+# and refuse to install the project if the version does not match. See
+# https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
+requires-python = ">=3.7"
+
+# This is either text indicating the license for the distribution, or a file
+# that contains the license
+# https://packaging.python.org/en/latest/specifications/core-metadata/#license
+license = { file = "LICENSE.txt" }
+
+# This field adds keywords for your project which will appear on the
+# project page. What does your project relate to?
+#
+# Note that this is a list of additional keywords, separated
+# by commas, to be used to assist searching for the distribution in a
+# larger catalog.
+keywords = ["aij", "setuptools", "development"]  # Optional
+
+# This should be your name or the name of the organization who originally
+# authored the project, and a valid email address corresponding to the name
+# listed.
+authors = [
+    { name = "Yilmaz Mustafa", email = "dev@mail.be" } # Optional
+]
+
+# This should be your name or the names of the organization who currently
+# maintains the project, and a valid email address corresponding to the name
+# listed.
+maintainers = [
+    # Optional
+]
+
+# Classifiers help users find your project by categorizing it.
+#
+# For a list of valid classifiers, see https://pypi.org/classifiers/
+classifiers = [# Optional
+    # How mature is this project? Common values are
+    #   3 - Alpha
+    #   4 - Beta
+    #   5 - Production/Stable
+    "Development Status :: 3 - Alpha",
+    # Indicate who your project is intended for
+    "Intended Audience :: Developers",
+    "Topic :: Software Development :: Build Tools",
+    # Pick your license as you wish
+    "License :: OSI Approved :: MIT License",
+    # Specify the Python versions you support here. In particular, ensure
+    # that you indicate you support Python 3. These classifiers are *not*
+    # checked by "pip install". See instead "python_requires" below.
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3 :: Only",
+]
+
+# This field lists other packages that your project depends on to run.
+# Any package you put here will be installed by pip when your project is
+# installed, so they must be valid existing projects.
+#
+# For an analysis of this field vs pip's requirements files see:
+# https://packaging.python.org/discussions/install-requires-vs-requirements/
+dependencies = [# Optional
+    "peppercorn",
+    "requests",
+    "beautifulsoup4",
+    "newsapi-python",
+    "pandas",
+    "numpy",
+    "matplotlib",
+    "pika"
+]
+
+# List additional groups of dependencies here (e.g. development
+# dependencies). Users will be able to install these using the "extras"
+# syntax, for example:
+#
+#   $ pip install sampleproject[dev]
+#
+# Similar to `dependencies` above, these must be valid existing
+# projects.
+[project.optional-dependencies] # Optional
+dev = ["check-manifest"]
+test = ["coverage"]
+
+# List URLs that are relevant to your project
+#
+# This field corresponds to the "Project-URL" and "Home-Page" metadata fields:
+# https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
+# https://packaging.python.org/specifications/core-metadata/#home-page-optional
+#
+# Examples listed include a pattern for specifying where the package tracks
+# issues, where the source is hosted, where to say thanks to the package
+# maintainers, and where to support the project financially. The key is
+# what's used to render the link text on PyPI.
+[project.urls]  # Optional
+"Homepage" = "https://www.codesapien.be/aij/"
+"Bug Reports" = "https://github.com/codesapienbe/aij-news-publisher/issues"
+"Funding" = "https://donate.pypi.org"
+"Say Thanks!" = "http://saythanks.io/to/aij"
+"Source" = "https://github.com/codesapienbe/aij-news-publisher"
+
+# The following would provide a command line executable called `sample`
+# which executes the function `main` from this package when invoked.
+[project.scripts]  # Optional
+aijnp = "news_publisher:main"
+
+# This is configuration specific to the `setuptools` build backend.
+# If you are using a different build backend, you will need to change this.
+[tool.setuptools]
+# If there are data files included in your packages that need to be
+# installed, specify them here.
+package-data = { "db" = ["*.dat"] }
+
+[build-system]
+# These are the assumed default build requirements from pip:
+# https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
+requires = ["setuptools>=43.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
```

### Comparing `aij-news-publisher-1.0.1/src/aij_news_publisher.egg-info/PKG-INFO` & `aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: aij-news-publisher
-Version: 1.0.1
+Version: 1.0.2
 Summary: AI Journalist News Publisher package
 Author-email: Yilmaz Mustafa <dev@mail.be>
-Maintainer-email: Intesaaf <intesaaf@gmail.com>, Fatima <fatima@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
         of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `aij-news-publisher-1.0.1/src/news_publisher/__init__.py` & `aij-news-publisher-1.0.2/src/news_publisher/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def main():
     """
     The main function to run the server and publish the news articles to the RabbitMQ queue
     """
     print('Server is being initialized...')
 
     # get the api key from the environment variable. If it is not set, use argument parser to get the api key
-    api_key = os.environ.get('NEWSAPI_ORG') or input("Enter your NewsAPI key: ")
+    api_key = os.environ.get('NEWSAPI_ORG')
 
     # create an instance of the NewsPublisher class
     api = NewsPublisher(api_key)
 
     # get the news from the newsapi
     api.publish_news_data()
```

### Comparing `aij-news-publisher-1.0.1/src/news_publisher/news_publisher.py` & `aij-news-publisher-1.0.2/src/news_publisher/news_publisher.py`

 * *Files identical despite different names*

