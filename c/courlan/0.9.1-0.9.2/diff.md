# Comparing `tmp/courlan-0.9.1.tar.gz` & `tmp/courlan-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "courlan-0.9.1.tar", last modified: Mon Apr 24 16:06:18 2023, max compression
+gzip compressed data, was "courlan-0.9.2.tar", last modified: Tue May  2 16:57:44 2023, max compression
```

## Comparing `courlan-0.9.1.tar` & `courlan-0.9.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-04-24 16:06:18.728592 courlan-0.9.1/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1131 2020-08-31 17:20:52.000000 courlan-0.9.1/CONTRIBUTING.md
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     2698 2023-04-24 16:04:57.000000 courlan-0.9.1/HISTORY.md
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    35141 2020-08-31 17:20:52.000000 courlan-0.9.1/LICENSE
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      160 2022-07-18 17:01:18.000000 courlan-0.9.1/MANIFEST.in
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    17701 2023-04-24 16:06:18.728592 courlan-0.9.1/PKG-INFO
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    16025 2023-04-24 16:04:57.000000 courlan-0.9.1/README.rst
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-04-24 16:06:18.728592 courlan-0.9.1/courlan/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      629 2023-04-24 16:04:57.000000 courlan-0.9.1/courlan/__init__.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     6234 2023-03-07 12:15:30.000000 courlan-0.9.1/courlan/clean.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     3691 2022-07-27 15:47:45.000000 courlan-0.9.1/courlan/cli.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     8447 2023-03-07 11:31:10.000000 courlan-0.9.1/courlan/core.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     7309 2023-03-07 11:39:05.000000 courlan-0.9.1/courlan/filters.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     7223 2023-03-07 12:06:22.000000 courlan-0.9.1/courlan/langinfo.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1637 2023-04-21 11:54:56.000000 courlan-0.9.1/courlan/network.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2022-07-18 15:53:08.000000 courlan-0.9.1/courlan/py.typed
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1786 2022-07-07 18:06:58.000000 courlan-0.9.1/courlan/settings.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    16274 2023-04-24 15:31:49.000000 courlan-0.9.1/courlan/urlstore.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     5794 2023-03-03 12:29:51.000000 courlan-0.9.1/courlan/urlutils.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-04-24 16:06:18.728592 courlan-0.9.1/courlan.egg-info/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    17701 2023-04-24 16:06:18.000000 courlan-0.9.1/courlan.egg-info/PKG-INFO
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      605 2023-04-24 16:06:18.000000 courlan-0.9.1/courlan.egg-info/SOURCES.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2023-04-24 16:06:18.000000 courlan-0.9.1/courlan.egg-info/dependency_links.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       46 2023-04-24 16:06:18.000000 courlan-0.9.1/courlan.egg-info/entry_points.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2023-03-07 12:17:45.000000 courlan-0.9.1/courlan.egg-info/not-zip-safe
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      111 2023-04-24 16:06:18.000000 courlan-0.9.1/courlan.egg-info/requires.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        8 2023-04-24 16:06:18.000000 courlan-0.9.1/courlan.egg-info/top_level.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)   151953 2020-08-31 17:20:52.000000 courlan-0.9.1/courlan_harns-march.jpg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       40 2021-12-07 18:31:00.000000 courlan-0.9.1/pytest.ini
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       38 2023-04-24 16:06:18.728592 courlan-0.9.1/setup.cfg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     3840 2023-03-07 12:11:21.000000 courlan-0.9.1/setup.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-04-24 16:06:18.728592 courlan-0.9.1/tests/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2020-08-31 17:20:52.000000 courlan-0.9.1/tests/__init__.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-04-24 16:06:18.728592 courlan-0.9.1/tests/data/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      324 2021-12-07 18:52:06.000000 courlan-0.9.1/tests/data/input.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    34473 2023-03-07 11:32:47.000000 courlan-0.9.1/tests/unit_tests.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    13038 2023-04-24 15:31:25.000000 courlan-0.9.1/tests/urlstore_tests.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-02 16:57:44.378929 courlan-0.9.2/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1131 2020-08-31 17:20:52.000000 courlan-0.9.2/CONTRIBUTING.md
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2801 2023-05-02 16:57:40.000000 courlan-0.9.2/HISTORY.md
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    35141 2020-08-31 17:20:52.000000 courlan-0.9.2/LICENSE
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      160 2022-07-18 17:01:18.000000 courlan-0.9.2/MANIFEST.in
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    17701 2023-05-02 16:57:44.378929 courlan-0.9.2/PKG-INFO
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16025 2023-04-24 16:04:57.000000 courlan-0.9.2/README.rst
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-02 16:57:44.378929 courlan-0.9.2/courlan/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      629 2023-05-02 16:57:40.000000 courlan-0.9.2/courlan/__init__.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     6212 2023-05-02 14:30:24.000000 courlan-0.9.2/courlan/clean.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3691 2022-07-27 15:47:45.000000 courlan-0.9.2/courlan/cli.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     8447 2023-03-07 11:31:10.000000 courlan-0.9.2/courlan/core.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7320 2023-05-02 14:30:24.000000 courlan-0.9.2/courlan/filters.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7223 2023-03-07 12:06:22.000000 courlan-0.9.2/courlan/langinfo.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1665 2023-05-02 14:30:24.000000 courlan-0.9.2/courlan/network.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2022-07-18 15:53:08.000000 courlan-0.9.2/courlan/py.typed
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1786 2022-07-07 18:06:58.000000 courlan-0.9.2/courlan/settings.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16213 2023-05-02 14:30:24.000000 courlan-0.9.2/courlan/urlstore.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5794 2023-03-03 12:29:51.000000 courlan-0.9.2/courlan/urlutils.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-02 16:57:44.378929 courlan-0.9.2/courlan.egg-info/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    17701 2023-05-02 16:57:44.000000 courlan-0.9.2/courlan.egg-info/PKG-INFO
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      605 2023-05-02 16:57:44.000000 courlan-0.9.2/courlan.egg-info/SOURCES.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2023-05-02 16:57:44.000000 courlan-0.9.2/courlan.egg-info/dependency_links.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       46 2023-05-02 16:57:44.000000 courlan-0.9.2/courlan.egg-info/entry_points.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2023-03-07 12:17:45.000000 courlan-0.9.2/courlan.egg-info/not-zip-safe
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      128 2023-05-02 16:57:44.000000 courlan-0.9.2/courlan.egg-info/requires.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        8 2023-05-02 16:57:44.000000 courlan-0.9.2/courlan.egg-info/top_level.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   151953 2020-08-31 17:20:52.000000 courlan-0.9.2/courlan_harns-march.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       40 2021-12-07 18:31:00.000000 courlan-0.9.2/pytest.ini
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       38 2023-05-02 16:57:44.378929 courlan-0.9.2/setup.cfg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3921 2023-05-02 14:30:24.000000 courlan-0.9.2/setup.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-02 16:57:44.378929 courlan-0.9.2/tests/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2020-08-31 17:20:52.000000 courlan-0.9.2/tests/__init__.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-02 16:57:44.378929 courlan-0.9.2/tests/data/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      324 2021-12-07 18:52:06.000000 courlan-0.9.2/tests/data/input.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    34725 2023-05-02 14:30:24.000000 courlan-0.9.2/tests/unit_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    13036 2023-05-02 14:30:24.000000 courlan-0.9.2/tests/urlstore_tests.py
```

### Comparing `courlan-0.9.1/CONTRIBUTING.md` & `courlan-0.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `courlan-0.9.1/HISTORY.md` & `courlan-0.9.2/HISTORY.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 ## History / Changelog
 
 
+### 0.9.2
+
+- add blogspot archives to type filter
+- maintenance: upgrade ``urllib3`` and review code
+
+
 ### 0.9.1
 
 - network tests: larger throughput
 - UrlStore: optional compression of rules (#21), added `reset()` (#22) and `get_all_counts()` methods
 - UrlStore fixes: `signal` in #18, `total_url_number`
 - updated Readme
```

### Comparing `courlan-0.9.1/LICENSE` & `courlan-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `courlan-0.9.1/PKG-INFO` & `courlan-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: courlan
-Version: 0.9.1
+Version: 0.9.2
 Summary: Clean, filter and sample URLs to optimize data collection – includes spam, content type and language filters.
 Home-page: https://github.com/adbar/courlan
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: GPLv3+
 Project-URL: Blog, https://adrien.barbaresi.eu/blog/
 Project-URL: Tracker, https://github.com/adbar/courlan/issues
```

### Comparing `courlan-0.9.1/README.rst` & `courlan-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `courlan-0.9.1/courlan/__init__.py` & `courlan-0.9.2/courlan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # meta
 __title__ = "courlan"
 __author__ = "Adrien Barbaresi"
 __license__ = "GNU GPL v3+"
 __copyright__ = "Copyright 2020-2023, Adrien Barbaresi"
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 
 # imports
 from .clean import clean_url, normalize_url, scrub_url
 from .core import check_url, extract_links, sample_urls
 from .filters import is_navigation_page, is_not_crawlable, lang_filter, validate_url
 from .urlstore import UrlStore
```

### Comparing `courlan-0.9.1/courlan/clean.py` & `courlan-0.9.2/courlan/clean.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,24 +127,24 @@
             newqdict[qelem] = qdict[qelem]
         return urlencode(newqdict, doseq=True)
     return parsed_url.query
 
 
 def decode_punycode(string: str) -> str:
     "Probe for punycode in lower-cased hostname and try to decode it."
-    if not "xn--" in string:
+    if "xn--" not in string:
         return string
 
     parts = []
 
     for part in string.split("."):
         if part.lower().startswith("xn--"):
             try:
                 part = part.encode("utf8").decode("idna")
-            except (UnicodeError, UnicodeDecodeError):
+            except UnicodeError:
                 LOGGER.debug("invalid utf/idna string: %s", part)
         parts.append(part)
 
     return ".".join(parts)
 
 
 def normalize_url(
```

### Comparing `courlan-0.9.1/courlan/cli.py` & `courlan-0.9.2/courlan/cli.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.1/courlan/core.py` & `courlan-0.9.2/courlan/core.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.1/courlan/filters.py` & `courlan-0.9.2/courlan/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 from .langinfo import COUNTRY_CODES, LANGUAGE_CODES
 
 
 LOGGER = logging.getLogger(__name__)
 
 # content filters
-WORDPRESS_CONTENT = re.compile(
-    r"/(?:page|seite|user|search|gallery|gall?erie|labels|archives|uploads|modules|attachment)/|/(?:tags?|schlagwort|category|cat|kategorie|kat|auth?or)/[^/]+/?$",
+SITE_STRUCTURE = re.compile(
+    r"/(?:page|seite|user|search|gallery|gall?erie|labels|archives|uploads|modules|attachment)/|/(?:tags?|schlagwort|category|cat|kategorie|kat|auth?or)/[^/]+/?$|/[0-9]+/[0-9]+/$|/[0-9]{4}/$|_archive\.html$",
     re.IGNORECASE,
 )
 FILE_TYPE = re.compile(
     r"\.(atom|json|css|xml|js|jpg|jpeg|png|gif|tiff|pdf|ogg|mp3|m4a|aac|avi|mp4|mov|webm|flv|ico|pls|zip|tar|gz|iso|swf)\b",
     re.IGNORECASE,
 )  # (?=[&?])
 UNDESIRABLE = re.compile(
@@ -103,15 +103,15 @@
     """Filter URLs based on basic formal characteristics"""
     return bool(url.startswith("http") and 10 <= len(url) < 500)
 
 
 def extension_filter(urlpath: str) -> bool:
     """Filter based on file extension"""
     extension_match = EXTENSION_REGEX.search(urlpath)
-    return bool(not extension_match or extension_match[0] in WHITELISTED_EXTENSIONS)
+    return not extension_match or extension_match[0] in WHITELISTED_EXTENSIONS
 
 
 def langcodes_score(language: str, segment: str, score: int) -> int:
     """Use langcodes on selected URL segments and integrate
     them into a score."""
     # see also: https://babel.pocoo.org/en/latest/locale.html
     # test if the code looks like a country or a language
@@ -175,17 +175,15 @@
     """Make sure the target URL is from a suitable type (HTML page with primarily text).
     Strict: Try to filter out other document types, spam, video and adult websites."""
     try:
         # feeds
         if url.endswith(("/feed", "/rss")):
             raise ValueError
         # wordpress website structure
-        if WORDPRESS_CONTENT.search(url) and (
-            not with_nav or not is_navigation_page(url)
-        ):
+        if SITE_STRUCTURE.search(url) and (not with_nav or not is_navigation_page(url)):
             raise ValueError
         # not suitable: ads, adult and embedded content
         if UNDESIRABLE.search(url):
             raise ValueError
         # type hidden in parameters + video content
         if strict and (FILE_TYPE.search(url) or ADULT_AND_VIDEOS.search(url)):
             raise ValueError
```

### Comparing `courlan-0.9.1/courlan/langinfo.py` & `courlan-0.9.2/courlan/langinfo.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.1/courlan/network.py` & `courlan-0.9.2/courlan/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 import logging
 
 import urllib3
 
 
 LOGGER = logging.getLogger(__name__)
+urllib3.disable_warnings()
+
 
 RETRY_STRATEGY = urllib3.util.Retry(
     total=2,
     redirect=2,
     raise_on_redirect=False,
     status_forcelist=[
         429,
```

### Comparing `courlan-0.9.1/courlan/settings.py` & `courlan-0.9.2/courlan/settings.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.1/courlan/urlstore.py` & `courlan-0.9.2/courlan/urlstore.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,24 @@
 import signal
 import sys
 import zlib
 
 from collections import defaultdict, deque
 from datetime import datetime, timedelta
 from threading import Lock
-from typing import Any, DefaultDict, Deque, Dict, List, Optional, Tuple, Union
+from typing import (
+    Any,
+    DefaultDict,
+    Deque,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
 
 from urllib.robotparser import RobotFileParser
 
 from .filters import lang_filter, validate_url
 from .urlutils import get_host_and_path, is_known_link
 
 
@@ -105,18 +114,17 @@
                 hostinfo, urlpath = get_host_and_path(parsed_url)
                 inputdict[hostinfo].append(UrlPathTuple(urlpath, visited))
             except (TypeError, ValueError):
                 LOGGER.warning("Discarding URL: %s", url)
         return inputdict
 
     def _load_urls(self, domain: str) -> Deque[UrlPathTuple]:
-        value = self.urldict[domain].tuples
-        if isinstance(value, bytes):
-            return pickle.loads(bz2.decompress(value))
-        return value
+        if self.compressed:
+            return pickle.loads(bz2.decompress(self.urldict[domain].tuples))  # type: ignore
+        return self.urldict[domain].tuples
 
     def _store_urls(
         self,
         domain: str,
         to_right: Optional[Deque[UrlPathTuple]] = None,
         timestamp: Optional[datetime] = None,
         to_left: Optional[Deque[UrlPathTuple]] = None,
@@ -210,22 +218,20 @@
         if appendleft:
             for host, urltuples in self._buffer_urls(appendleft, visited).items():
                 self._store_urls(host, to_left=urltuples)
 
     def is_known(self, url: str) -> bool:
         "Check if the given URL has already been stored."
         hostinfo, urlpath = get_host_and_path(url)
-        values = self._load_urls(hostinfo)
         # returns False if domain or URL is new
-        return urlpath in {u.urlpath for u in values}
+        return urlpath in {u.urlpath for u in self._load_urls(hostinfo)}
 
     def find_known_urls(self, domain: str) -> List[str]:
         """Get all already known URLs for the given domain (ex. "https://example.org")."""
-        values = self._load_urls(domain)
-        return [domain + u.urlpath for u in values]
+        return [domain + u.urlpath for u in self._load_urls(domain)]
 
     def filter_unknown_urls(self, urls: List[str]) -> List[str]:
         "Take a list of URLs and return the currently unknown ones."
         return self._search_urls(urls, switch=1)
 
     def get_known_domains(self) -> List[str]:
         "Return all known domains as a list."
@@ -238,23 +244,21 @@
         raise KeyError("website not in store")
 
     # URL-BASED QUERIES
 
     def has_been_visited(self, url: str) -> bool:
         "Check if the given URL has already been visited.."
         hostinfo, urlpath = get_host_and_path(url)
-        values = self._load_urls(hostinfo)
-        known_urlpaths = {u.urlpath: u.visited for u in values}
+        known_urlpaths = {u.urlpath: u.visited for u in self._load_urls(hostinfo)}
         # defaults to None, thus False
         return known_urlpaths.get(urlpath) or False
 
     def find_unvisited_urls(self, domain: str) -> List[str]:
         "Get all unvisited URLs for the given domain."
-        values = self._load_urls(domain)
-        return [domain + u.urlpath for u in values if not u.visited]
+        return [domain + u.urlpath for u in self._load_urls(domain) if not u.visited]
 
     def filter_unvisited_urls(self, urls: List[str]) -> List[Union[Any, str]]:
         "Take a list of URLs and return the currently unvisited ones."
         return self._search_urls(urls, switch=2)
 
     def unvisited_websites_number(self) -> int:
         "Return the number of websites for which there are still URLs to visit."
@@ -267,15 +271,15 @@
         # not fully used
         if not self.urldict[domain].all_visited:
             url_tuples = self._load_urls(domain)
             # get first non-seen url
             for url in url_tuples:
                 if not url.visited:
                     # store information
-                    if as_visited is True:
+                    if as_visited:
                         url.visited = True
                         with self._lock:
                             self.urldict[domain].count += 1
                         self._store_urls(domain, url_tuples, timestamp=datetime.now())
                     return domain + url.urlpath
         # nothing to draw from
         with self._lock:
@@ -285,15 +289,15 @@
     def get_download_urls(self, timelimit: int = 10) -> Optional[List[str]]:
         """Get a list of immediately downloadable URLs according to the given
         time limit per domain."""
         with self._lock:
             potential = [d for d in self.urldict if not self.urldict[d].all_visited]
         if not potential:
             self.done = True
-            return None
+            return []
         targets = []
         for domain in potential:
             timestamp = self._timestamp(domain)
             if (
                 timestamp is None
                 or (datetime.now() - timestamp).total_seconds() > timelimit
             ):
@@ -313,16 +317,16 @@
                 self.done = True
                 return []
         # variables init
         per_domain = max_urls // len(potential) or 1
         targets: List[Tuple[float, str]] = []
         # iterate potential domains
         for domain in potential:
-            url_tuples = self._load_urls(domain)
             # load urls
+            url_tuples = self._load_urls(domain)
             urlpaths: List[str] = []
             # get first non-seen urls
             for url in url_tuples:
                 if (
                     len(urlpaths) >= per_domain
                     or (len(targets) + len(urlpaths)) >= max_urls
                 ):
@@ -364,17 +368,16 @@
             )
         self.urldict[website].rules = rules
 
     def get_rules(self, website: str) -> Optional[RobotFileParser]:
         "Return the stored crawling rules for the given website."
         if website in self.urldict:
             if self.compressed:
-                return pickle.loads(zlib.decompress(self.urldict[website].rules))  # type: ignore[arg-type]
-            else:
-                return self.urldict[website].rules
+                return pickle.loads(zlib.decompress(self.urldict[website].rules))  # type: ignore
+            return self.urldict[website].rules
         return None
 
     def get_crawl_delay(self, website: str, default: float = 5) -> float:
         "Return the delay as extracted from robots.txt, or a given default."
         delay = None
         rules = self.get_rules(website)
         try:
@@ -403,16 +406,17 @@
         urls = []
         for domain in self.urldict:
             urls.extend(self.find_known_urls(domain))
         return urls
 
     def print_unvisited_urls(self) -> None:
         "Print all unvisited URLs in store."
-        for domain in self.urldict:
-            print("\n".join(self.find_unvisited_urls(domain)))
+        with self._lock:
+            for domain in self.urldict:
+                print("\n".join(self.find_unvisited_urls(domain)))
 
     def print_urls(self) -> None:
         "Print all URLs in store (URL + TAB + visited or not)."
         for domain in self.urldict:
             print(
                 "\n".join(
                     [
```

### Comparing `courlan-0.9.1/courlan/urlutils.py` & `courlan-0.9.2/courlan/urlutils.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.1/courlan.egg-info/PKG-INFO` & `courlan-0.9.2/courlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: courlan
-Version: 0.9.1
+Version: 0.9.2
 Summary: Clean, filter and sample URLs to optimize data collection – includes spam, content type and language filters.
 Home-page: https://github.com/adbar/courlan
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: GPLv3+
 Project-URL: Blog, https://adrien.barbaresi.eu/blog/
 Project-URL: Tracker, https://github.com/adbar/courlan/issues
```

### Comparing `courlan-0.9.1/courlan.egg-info/SOURCES.txt` & `courlan-0.9.2/courlan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `courlan-0.9.1/courlan_harns-march.jpg` & `courlan-0.9.2/courlan_harns-march.jpg`

 * *Files identical despite different names*

### Comparing `courlan-0.9.1/setup.py` & `courlan-0.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,16 @@
     # package_data={},
     include_package_data=True,
     python_requires=">=3.6",
     install_requires=[
         "langcodes >= 3.3.0",
         "tld == 0.12.6; python_version < '3.7'",
         "tld >= 0.13; python_version >= '3.7'",
-        "urllib3 >= 1.26, < 2",
+        "urllib3 >= 1.26, < 2; python_version < '3.7'",
+        "urllib3 >= 1.26, < 3; python_version >= '3.7'",
     ],
     # extras_require=extras,
     entry_points={
         "console_scripts": ["courlan=courlan.cli:main"],
     },
     # platforms='any',
     tests_require=["pytest"],
```

### Comparing `courlan-0.9.1/tests/unit_tests.py` & `courlan-0.9.2/tests/unit_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,20 +205,29 @@
     assert type_filter("http://example.com/new-video-release", strict=True) is False
     # tags
     assert type_filter("https://de.thecitizen.de/tag/anonymity/") is False
     assert type_filter("https://de.thecitizen.de/tags/anonymity/") is False
     # author
     assert type_filter("http://www.example.org/author/abcde") is False
     assert type_filter("http://www.example.org/autor/abcde/") is False
+    # archives
+    assert type_filter("http://www.example.org/2011/11/") is False
+    assert type_filter("http://www.example.org/2011/") is False
+    assert type_filter("http://www.example.org/2011_archive.html") is False
     # misc
     assert (
         type_filter("http://www.bmbwk.gv.at/forschung/fps/gsk/befragung.xml?style=text")
         is True
     )
-    # assert type_filter('http://www.aec.at/de/archives/prix_archive/prix_projekt.asp?iProjectID=11118') is True
+    assert (
+        type_filter(
+            "http://www.aec.at/de/archives/prix_archive/prix_projekt.asp?iProjectID=11118"
+        )
+        is False
+    )
     # nav
     assert type_filter("http://www.example.org/tag/abcde/", with_nav=False) is False
     assert type_filter("http://www.example.org/tag/abcde/", with_nav=True) is True
     assert type_filter("http://www.example.org/page/10/", with_nav=False) is False
     assert type_filter("http://www.example.org/page/10/", with_nav=True) is True
 
 
@@ -457,17 +466,17 @@
     assert (
         check_url("http://example.com/index.html#term", strict=False)[0]
         == "http://example.com/index.html#term"
     )
     assert check_url("http://example.com/test.js") is None
     assert check_url("http://twitter.com/", strict=True) is None
     assert check_url("http://twitter.com/", strict=False) is not None
-    assert check_url("https://www.httpbin.org/status/200", with_redirects=True) == (
-        "https://www.httpbin.org/status/200",
-        "httpbin.org",
+    assert check_url("https://www.httpbun.org/status/200", with_redirects=True) == (
+        "https://httpbun.org",
+        "httpbun.org",
     )
     # assert check_url('https://www.httpbin.org/status/302', with_redirects=True) == ('https://www.httpbin.org/status/302', 'httpbin.org')
     assert check_url("https://www.httpbin.org/status/404", with_redirects=True) is None
     assert check_url("https://www.ht.or", with_redirects=True) is None
     # recheck type and spam filters
     assert check_url("http://example.org/code/oembed/") is None
     assert check_url("http://cams.com/", strict=False) == (
```

### Comparing `courlan-0.9.1/tests/urlstore_tests.py` & `courlan-0.9.2/tests/urlstore_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
     ).total_seconds() < 0.25
     assert my_urls.urldict["https://www.example.org"].count == 3
     assert my_urls.urldict["https://test.org"].count == 1
     downloadable_urls = my_urls.get_download_urls()  # limit=10
     assert len(downloadable_urls) == 0
     other_store = UrlStore()
     downloadable_urls = other_store.get_download_urls()
-    assert downloadable_urls is None and other_store.done is True
+    assert downloadable_urls == [] and other_store.done is True
 
     # schedule
     schedule = other_store.establish_download_schedule()
     assert schedule == []
     # store exhaustion
     other_store = UrlStore()
     other_store.add_urls(
```

