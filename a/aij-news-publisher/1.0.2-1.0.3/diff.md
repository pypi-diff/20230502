# Comparing `tmp/aij-news-publisher-1.0.2.tar.gz` & `tmp/aij-news-publisher-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-news-publisher-1.0.2.tar", last modified: Tue May  2 21:38:43 2023, max compression
+gzip compressed data, was "aij-news-publisher-1.0.3.tar", last modified: Tue May  2 21:50:28 2023, max compression
```

## Comparing `aij-news-publisher-1.0.2.tar` & `aij-news-publisher-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     4314 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.2/README.md
--rw-rw-rw-   0        0        0     6281 2023-05-02 21:38:32.000000 aij-news-publisher-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/
--rw-rw-rw-   0        0        0     4314 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      118 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 21:38:44.000000 aij-news-publisher-1.0.2/src/news_publisher/
--rw-rw-rw-   0        0        0      594 2023-05-02 21:26:06.000000 aij-news-publisher-1.0.2/src/news_publisher/__init__.py
--rw-rw-rw-   0        0        0     3293 2023-05-02 19:39:04.000000 aij-news-publisher-1.0.2/src/news_publisher/news_publisher.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     4314 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.3/README.md
+-rw-rw-rw-   0        0        0     6331 2023-05-02 21:50:16.000000 aij-news-publisher-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/
+-rw-rw-rw-   0        0        0     4314 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      147 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/news_publisher/
+-rw-rw-rw-   0        0        0      583 2023-05-02 21:50:00.000000 aij-news-publisher-1.0.3/src/news_publisher/__init__.py
+-rw-rw-rw-   0        0        0     3255 2023-05-02 21:48:22.000000 aij-news-publisher-1.0.3/src/news_publisher/api_server.py
+-rw-rw-rw-   0        0        0     2942 2023-05-02 21:47:28.000000 aij-news-publisher-1.0.3/src/news_publisher/db_server.py
```

### Comparing `aij-news-publisher-1.0.2/LICENSE.txt` & `aij-news-publisher-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.2/PKG-INFO` & `aij-news-publisher-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-publisher
-Version: 1.0.2
+Version: 1.0.3
 Summary: AI Journalist News Publisher package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-news-publisher-1.0.2/README.md` & `aij-news-publisher-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.2/pyproject.toml` & `aij-news-publisher-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-news-publisher"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.2"
+version = "1.0.3"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist News Publisher package"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -103,15 +103,18 @@
     "peppercorn",
     "requests",
     "beautifulsoup4",
     "newsapi-python",
     "pandas",
     "numpy",
     "matplotlib",
-    "pika"
+    "pika",
+    "sqlalchemy",
+    "pytest",
+    "pytest-cov"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
```

### Comparing `aij-news-publisher-1.0.2/src/aij_news_publisher.egg-info/PKG-INFO` & `aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-publisher
-Version: 1.0.2
+Version: 1.0.3
 Summary: AI Journalist News Publisher package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-news-publisher-1.0.2/src/news_publisher/__init__.py` & `aij-news-publisher-1.0.3/src/news_publisher/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from news_publisher.news_server import NewsPublisher
+from news_publisher.api_server import NewsPublisher
 
 
 def main():
     """
     The main function to run the server and publish the news articles to the RabbitMQ queue
     """
     print('Server is being initialized...')
@@ -12,10 +12,10 @@
     # get the api key from the environment variable. If it is not set, use argument parser to get the api key
     api_key = os.environ.get('NEWSAPI_ORG')
 
     # create an instance of the NewsPublisher class
     api = NewsPublisher(api_key)
 
     # get the news from the newsapi
-    api.publish_news_data()
+    api.publish()
 
     print('Server is now running...')
```

### Comparing `aij-news-publisher-1.0.2/src/news_publisher/news_publisher.py` & `aij-news-publisher-1.0.3/src/news_publisher/api_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,44 +29,40 @@
         try:
             self.articles = self.api.get_everything(sources=self.sources)
             self.headlines = self.api.get_top_headlines(sources=self.sources)
         except NewsAPIException as api_exception:
             print(f"Could not request results from NewsAPI; {api_exception}")
             print("Loading the news from the database...")
 
-    def publish_news_data(self):
+    def publish(self):
         """
         Publish the news articles to the RabbitMQ queue one by one and save the news to the database
         """
         try:
-            self.publish_news_one_by_one()
+            """
+            Publish the news articles to the RabbitMQ queue one by one...
+            """
+            for _article in self.articles['articles']:
+                _body = json.dumps(_article).encode('utf-8')
+                self.channel.basic_publish(exchange='', routing_key=self.queue_name, body=_body)
+                print(f"Published a news article to the queue: {_article['title']}")
+                # wait for 1 second before publishing the next article
+                time.sleep(1)
+
+            for _headline in self.headlines['articles']:
+                _body = json.dumps(_headline).encode('utf-8')
+                self.channel.basic_publish(exchange='', routing_key=f"{self.queue_name}_headlines", body=_body)
+                print(f"Published a news headline to the queue: {_headline['title']}")
+                # wait for 1 second before publishing the next article
+                time.sleep(1)
         except NewsAPIException as api_exception:
             print(f"Could not request results from NewsAPI; {api_exception}")
             print("Loading the news from the database...")
             
 
         # do not close the connection until the message is delivered
         if self.connection.is_open:
             self.connection.close()
 
         # call the function again after 60 seconds
         Timer(60, self.publish_news_data).start()
 
-    def publish_news_one_by_one(self):
-        """
-        Publish the news articles to the RabbitMQ queue one by one...
-        """
-        for _article in self.articles['articles']:
-            _body = json.dumps(_article).encode('utf-8')
-            self.channel.basic_publish(exchange='', routing_key=self.queue_name, body=_body)
-            print(f"Published a news article to the queue: {_article['title']}")
-            # wait for 1 second before publishing the next article
-            time.sleep(1)
-
-        for _headline in self.headlines['articles']:
-            _body = json.dumps(_headline).encode('utf-8')
-            self.channel.basic_publish(exchange='', routing_key=f"{self.queue_name}_headlines", body=_body)
-            print(f"Published a news headline to the queue: {_headline['title']}")
-            # wait for 1 second before publishing the next article
-            time.sleep(1)
-
-
```

