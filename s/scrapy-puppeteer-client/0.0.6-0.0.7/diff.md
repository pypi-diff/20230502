# Comparing `tmp/scrapy-puppeteer-client-0.0.6.tar.gz` & `tmp/scrapy-puppeteer-client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-puppeteer-client-0.0.6.tar", last modified: Tue Aug  2 13:35:03 2022, max compression
+gzip compressed data, was "scrapy-puppeteer-client-0.0.7.tar", last modified: Tue May  2 09:27:56 2023, max compression
```

## Comparing `scrapy-puppeteer-client-0.0.6.tar` & `scrapy-puppeteer-client-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:35:03.479180 scrapy-puppeteer-client-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-08-02 13:34:55.000000 scrapy-puppeteer-client-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4677 2022-08-02 13:35:03.479180 scrapy-puppeteer-client-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-08-02 13:34:55.000000 scrapy-puppeteer-client-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:35:03.479180 scrapy-puppeteer-client-0.0.6/scrapy_puppeteer_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4677 2022-08-02 13:35:03.000000 scrapy-puppeteer-client-0.0.6/scrapy_puppeteer_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-08-02 13:35:03.000000 scrapy-puppeteer-client-0.0.6/scrapy_puppeteer_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 13:35:03.000000 scrapy-puppeteer-client-0.0.6/scrapy_puppeteer_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-02 13:35:03.000000 scrapy-puppeteer-client-0.0.6/scrapy_puppeteer_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:35:03.479180 scrapy-puppeteer-client-0.0.6/scrapypuppeteer/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-02 13:34:55.000000 scrapy-puppeteer-client-0.0.6/scrapypuppeteer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8086 2022-08-02 13:34:55.000000 scrapy-puppeteer-client-0.0.6/scrapypuppeteer/actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5242 2022-08-02 13:34:55.000000 scrapy-puppeteer-client-0.0.6/scrapypuppeteer/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-08-02 13:34:55.000000 scrapy-puppeteer-client-0.0.6/scrapypuppeteer/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2898 2022-08-02 13:34:55.000000 scrapy-puppeteer-client-0.0.6/scrapypuppeteer/response.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-02 13:35:03.479180 scrapy-puppeteer-client-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-08-02 13:34:55.000000 scrapy-puppeteer-client-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:27:56.176780 scrapy-puppeteer-client-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-02 09:27:56.176780 scrapy-puppeteer-client-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:27:56.172780 scrapy-puppeteer-client-0.0.7/scrapy_puppeteer_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-02 09:27:56.000000 scrapy-puppeteer-client-0.0.7/scrapy_puppeteer_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-02 09:27:56.000000 scrapy-puppeteer-client-0.0.7/scrapy_puppeteer_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:27:56.000000 scrapy-puppeteer-client-0.0.7/scrapy_puppeteer_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 09:27:56.000000 scrapy-puppeteer-client-0.0.7/scrapy_puppeteer_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:27:56.176780 scrapy-puppeteer-client-0.0.7/scrapypuppeteer/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/scrapypuppeteer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/scrapypuppeteer/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/scrapypuppeteer/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/scrapypuppeteer/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/scrapypuppeteer/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:27:56.176780 scrapy-puppeteer-client-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/setup.py
```

### Comparing `scrapy-puppeteer-client-0.0.6/LICENSE` & `scrapy-puppeteer-client-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-puppeteer-client-0.0.6/PKG-INFO` & `scrapy-puppeteer-client-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: scrapy-puppeteer-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library to use Puppeteer-managed browser in Scrapy spiders
 Home-page: https://github.com/ispras/scrapy-puppeteer
 Author: MODIS @ ISP RAS
 Maintainer: Maksim Varlamov
 Maintainer-email: varlamov@ispras.ru
 License: BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Framework :: Scrapy
 Classifier: Intended Audience :: Developers
@@ -113,16 +112,19 @@
 On your first request service will create new incognito browser context and new page in it.
 Their ids will be in returned in response object as `context_id` and `page_id` attributes.
 Following such response means passing context and page ids to next request.
 You also may specify requests context and page ids directly.
 
 Once your spider is closed, middleware will take care of closing all used browser contexts.
 
+One may customize which `PuppeteerRequest`'s headers will be sent to remote website by the service 
+via `include_headers` attribute in request or globally with `PUPPETEER_INCLUDE_HEADERS` setting. 
+Available values are True (all headers), False (no headers) or list of header names.
+By default, only cookies are sent.
+
 ## TODO
 
 - [x] skeleton that could handle goto, click, scroll, and actions
 - [ ] headers and cookies management
 - [ ] proxy support for puppeteer
 - [ ] error handling for requests
 - [ ] har support
-
-
```

### Comparing `scrapy-puppeteer-client-0.0.6/README.md` & `scrapy-puppeteer-client-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -89,14 +89,19 @@
 On your first request service will create new incognito browser context and new page in it.
 Their ids will be in returned in response object as `context_id` and `page_id` attributes.
 Following such response means passing context and page ids to next request.
 You also may specify requests context and page ids directly.
 
 Once your spider is closed, middleware will take care of closing all used browser contexts.
 
+One may customize which `PuppeteerRequest`'s headers will be sent to remote website by the service 
+via `include_headers` attribute in request or globally with `PUPPETEER_INCLUDE_HEADERS` setting. 
+Available values are True (all headers), False (no headers) or list of header names.
+By default, only cookies are sent.
+
 ## TODO
 
 - [x] skeleton that could handle goto, click, scroll, and actions
 - [ ] headers and cookies management
 - [ ] proxy support for puppeteer
 - [ ] error handling for requests
 - [ ] har support
```

### Comparing `scrapy-puppeteer-client-0.0.6/scrapy_puppeteer_client.egg-info/PKG-INFO` & `scrapy-puppeteer-client-0.0.7/scrapy_puppeteer_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: scrapy-puppeteer-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library to use Puppeteer-managed browser in Scrapy spiders
 Home-page: https://github.com/ispras/scrapy-puppeteer
 Author: MODIS @ ISP RAS
 Maintainer: Maksim Varlamov
 Maintainer-email: varlamov@ispras.ru
 License: BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Framework :: Scrapy
 Classifier: Intended Audience :: Developers
@@ -113,16 +112,19 @@
 On your first request service will create new incognito browser context and new page in it.
 Their ids will be in returned in response object as `context_id` and `page_id` attributes.
 Following such response means passing context and page ids to next request.
 You also may specify requests context and page ids directly.
 
 Once your spider is closed, middleware will take care of closing all used browser contexts.
 
+One may customize which `PuppeteerRequest`'s headers will be sent to remote website by the service 
+via `include_headers` attribute in request or globally with `PUPPETEER_INCLUDE_HEADERS` setting. 
+Available values are True (all headers), False (no headers) or list of header names.
+By default, only cookies are sent.
+
 ## TODO
 
 - [x] skeleton that could handle goto, click, scroll, and actions
 - [ ] headers and cookies management
 - [ ] proxy support for puppeteer
 - [ ] error handling for requests
 - [ ] har support
-
-
```

### Comparing `scrapy-puppeteer-client-0.0.6/scrapypuppeteer/actions.py` & `scrapy-puppeteer-client-0.0.7/scrapypuppeteer/actions.py`

 * *Files identical despite different names*

### Comparing `scrapy-puppeteer-client-0.0.6/scrapypuppeteer/middleware.py` & `scrapy-puppeteer-client-0.0.7/scrapypuppeteer/middleware.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from collections import defaultdict
+from typing import List, Union
 from urllib.parse import urljoin, urlencode
 
 from scrapy import Request, signals
 from scrapy.crawler import Crawler
 from scrapy.http import Headers, TextResponse
 
 from scrapypuppeteer import PuppeteerRequest, PuppeteerHtmlResponse
@@ -15,28 +16,52 @@
     """
     This downloader middleware converts PuppeteerRequest instances to
     Puppeteer service API requests and then converts its responses to
     PuppeteerResponse instances. Additionally it tracks all browser contexts
     that spider uses and performs cleanup request to service once spider
     is closed.
 
-    Puppeteer service URL may be set via PUPPETEER_SERVICE_URL setting.
+    Settings:
+
+    PUPPETEER_SERVICE_URL (str)
+    Service URL, e.g. 'http://localhost:3000'
+
+    PUPPETEER_INCLUDE_HEADERS (bool|list[str])
+    Determines which request headers will be sent to remote site by puppeteer service.
+    Either True (all headers), False (no headers) or list of header names.
+    May be overriden per request.
+    By default, only cookies are sent.
     """
 
-    def __init__(self, crawler: Crawler, service_url: str):
+    SERVICE_URL_SETTING = 'PUPPETEER_SERVICE_URL'
+    INCLUDE_HEADERS_SETTING = 'PUPPETEER_INCLUDE_HEADERS'
+    DEFAULT_INCLUDE_HEADERS = ['Cookie']  # TODO send them separately
+
+    def __init__(self,
+                 crawler: Crawler,
+                 service_url: str,
+                 include_headers: Union[bool, List[str]]):
         self.service_base_url = service_url
+        self.include_headers = include_headers
         self.crawler = crawler
         self.used_contexts = defaultdict(set)
 
     @classmethod
     def from_crawler(cls, crawler):
-        service_url = crawler.settings.get('PUPPETEER_SERVICE_URL')
+        service_url = crawler.settings.get(cls.SERVICE_URL_SETTING)
         if service_url is None:
             raise ValueError('Puppeteer service URL must be provided')
-        middleware = cls(crawler, service_url)
+        if cls.INCLUDE_HEADERS_SETTING in crawler.settings:
+            try:
+                include_headers = crawler.settings.getbool(cls.INCLUDE_HEADERS_SETTING)
+            except ValueError:
+                include_headers = crawler.settings.getlist(cls.INCLUDE_HEADERS_SETTING)
+        else:
+            include_headers = cls.DEFAULT_INCLUDE_HEADERS
+        middleware = cls(crawler, service_url, include_headers)
         crawler.signals.connect(middleware.close_used_contexts,
                                 signal=signals.spider_closed)
         return middleware
 
     def process_request(self, request, spider):
         if not isinstance(request, PuppeteerRequest):
             return
@@ -72,25 +97,29 @@
             service_params['contextId'] = request.context_id
         if request.page_id is not None:
             service_params['pageId'] = request.page_id
         if request.close_page:
             service_params['closePage'] = 1
         return urlencode(service_params)
 
-    @staticmethod
-    def _serialize_body(action, request):
+    def _serialize_body(self, action, request):
         payload = action.payload()
         if action.content_type == 'application/json':
             if isinstance(payload, dict):
                 # disallow null values in top-level request parameters
                 payload = {k: v for k, v in payload.items() if v is not None}
             proxy = request.meta.get('proxy')
             if proxy:
                 payload['proxy'] = proxy
-            payload['headers'] = request.headers.to_unicode_dict()
+            include_headers = self.include_headers if request.include_headers is None else request.include_headers
+            if include_headers:
+                headers = request.headers.to_unicode_dict()
+                if isinstance(include_headers, list):
+                    headers = {h: headers[h] for h in include_headers if h in headers}
+                payload['headers'] = headers
             return json.dumps(payload)
         return str(payload)
 
     def process_response(self, request, response, spider):
         if not isinstance(response, TextResponse):
             return response
```

### Comparing `scrapy-puppeteer-client-0.0.6/scrapypuppeteer/request.py` & `scrapy-puppeteer-client-0.0.7/scrapypuppeteer/request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union
+from typing import List, Union
 
 from scrapy.http import Request
 
 from scrapypuppeteer.actions import GoTo, PuppeteerServiceAction
 
 
 class PuppeteerRequest(Request):
@@ -11,25 +11,30 @@
     """
 
     def __init__(self,
                  action: Union[str, PuppeteerServiceAction],
                  context_id: str = None,
                  page_id: str = None,
                  close_page: bool = True,
+                 include_headers: Union[bool, List[str]] = None,
                  **kwargs):
         """
 
         :param action: URL or browser action
         :param context_id: puppeteer browser context id; if None (default),
                            new incognito context will be created
         :param page_id: puppeteer browser page id; if None (default), new
                         page will be opened in given context
         :param close_page: whether to close page after request completion;
                            set to False, if you want to continue interacting
                            with the page
+        :param include_headers: determines which headers will be sent to remote
+                                site by puppeteer: either True (all headers),
+                                False (no headers), list of header names
+                                or None (default, let middleware decide)
         :param kwargs:
         """
         url = kwargs.pop('url', None)
         if isinstance(action, str):
             url = action
             navigation_options = kwargs.pop('navigation_options', None)
             wait_options = kwargs.pop('wait_options', None)
@@ -41,12 +46,13 @@
         if url is None:
             raise ValueError('Request is not a goto-request and does not follow a response')
         super().__init__(url, **kwargs)
         self.action = action
         self.context_id = context_id
         self.page_id = page_id
         self.close_page = close_page
+        self.include_headers = include_headers
 
     def replace(self, *args, **kwargs):
-        for x in ['action', 'context_id', 'page_id', 'close_page']:
+        for x in ['action', 'context_id', 'page_id', 'close_page', 'include_headers']:
             kwargs.setdefault(x, getattr(self, x))
         return super().replace(*args, **kwargs)
```

### Comparing `scrapy-puppeteer-client-0.0.6/scrapypuppeteer/response.py` & `scrapy-puppeteer-client-0.0.7/scrapypuppeteer/response.py`

 * *Files identical despite different names*

### Comparing `scrapy-puppeteer-client-0.0.6/setup.py` & `scrapy-puppeteer-client-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(
     name='scrapy-puppeteer-client',
-    version='0.0.6',
+    version='0.0.7',
     description='A library to use Puppeteer-managed browser in Scrapy spiders',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ispras/scrapy-puppeteer',
     author='MODIS @ ISP RAS',
     maintainer='Maksim Varlamov',
     maintainer_email='varlamov@ispras.ru',
```

