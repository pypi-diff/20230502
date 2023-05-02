# Comparing `tmp/yfjpscraper-0.3.2.tar.gz` & `tmp/yfjpscraper-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yfjpscraper-0.3.2.tar", last modified: Thu Dec 29 03:23:57 2022, max compression
+gzip compressed data, was "yfjpscraper-0.3.3.tar", last modified: Tue May  2 14:05:41 2023, max compression
```

## Comparing `yfjpscraper-0.3.2.tar` & `yfjpscraper-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 zenbook   (1000) zenbook   (1000)        0 2022-12-29 03:23:57.158850 yfjpscraper-0.3.2/
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      192 2022-12-29 03:23:57.158850 yfjpscraper-0.3.2/PKG-INFO
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      292 2021-05-26 00:02:57.000000 yfjpscraper-0.3.2/README.md
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      350 2022-02-16 05:54:12.000000 yfjpscraper-0.3.2/README.rst
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)       38 2022-12-29 03:23:57.158850 yfjpscraper-0.3.2/setup.cfg
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      342 2022-12-29 03:23:28.000000 yfjpscraper-0.3.2/setup.py
-drwxrwxr-x   0 zenbook   (1000) zenbook   (1000)        0 2022-12-29 03:23:57.158850 yfjpscraper-0.3.2/yfjpscraper/
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)     5151 2022-12-29 03:23:02.000000 yfjpscraper-0.3.2/yfjpscraper/__init__.py
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)     4200 2022-11-29 05:35:45.000000 yfjpscraper-0.3.2/yfjpscraper/parser.py
-drwxrwxr-x   0 zenbook   (1000) zenbook   (1000)        0 2022-12-29 03:23:57.158850 yfjpscraper-0.3.2/yfjpscraper.egg-info/
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      192 2022-12-29 03:23:57.000000 yfjpscraper-0.3.2/yfjpscraper.egg-info/PKG-INFO
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      249 2022-12-29 03:23:57.000000 yfjpscraper-0.3.2/yfjpscraper.egg-info/SOURCES.txt
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)        1 2022-12-29 03:23:57.000000 yfjpscraper-0.3.2/yfjpscraper.egg-info/dependency_links.txt
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)       17 2022-12-29 03:23:57.000000 yfjpscraper-0.3.2/yfjpscraper.egg-info/requires.txt
--rw-rw-r--   0 zenbook   (1000) zenbook   (1000)       12 2022-12-29 03:23:57.000000 yfjpscraper-0.3.2/yfjpscraper.egg-info/top_level.txt
+drwxrwxr-x   0 zenbook   (1000) zenbook   (1000)        0 2023-05-02 14:05:41.600674 yfjpscraper-0.3.3/
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      192 2023-05-02 14:05:41.600674 yfjpscraper-0.3.3/PKG-INFO
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      292 2021-05-26 00:02:57.000000 yfjpscraper-0.3.3/README.md
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      350 2022-02-16 05:54:12.000000 yfjpscraper-0.3.3/README.rst
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)       38 2023-05-02 14:05:41.600674 yfjpscraper-0.3.3/setup.cfg
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      342 2023-05-02 14:05:27.000000 yfjpscraper-0.3.3/setup.py
+drwxrwxr-x   0 zenbook   (1000) zenbook   (1000)        0 2023-05-02 14:05:41.600674 yfjpscraper-0.3.3/yfjpscraper/
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)     5275 2023-05-02 14:04:14.000000 yfjpscraper-0.3.3/yfjpscraper/__init__.py
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)     4200 2022-11-29 05:35:45.000000 yfjpscraper-0.3.3/yfjpscraper/parser.py
+drwxrwxr-x   0 zenbook   (1000) zenbook   (1000)        0 2023-05-02 14:05:41.600674 yfjpscraper-0.3.3/yfjpscraper.egg-info/
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      192 2023-05-02 14:05:41.000000 yfjpscraper-0.3.3/yfjpscraper.egg-info/PKG-INFO
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)      249 2023-05-02 14:05:41.000000 yfjpscraper-0.3.3/yfjpscraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)        1 2023-05-02 14:05:41.000000 yfjpscraper-0.3.3/yfjpscraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)       17 2023-05-02 14:05:41.000000 yfjpscraper-0.3.3/yfjpscraper.egg-info/requires.txt
+-rw-rw-r--   0 zenbook   (1000) zenbook   (1000)       12 2023-05-02 14:05:41.000000 yfjpscraper-0.3.3/yfjpscraper.egg-info/top_level.txt
```

### Comparing `yfjpscraper-0.3.2/yfjpscraper/__init__.py` & `yfjpscraper-0.3.3/yfjpscraper/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,16 @@
             "id": query_name,
             "params": inner_params
         }
         logger.info(page_url)
         resp = session.post(
             page_url, data=json.dumps(params).replace(" ", ""), headers=headers
         )
+        if resp.status_code != 200:
+            raise HTTPError(f"status code is {resp.status_code} {page_url=} {params=}")
         json_data = resp.json()
         if get_split is False:
             yield from parse_json_split(json_data)
             get_split = True
         stop = yield from parse_json(json_data)
         if stop:
             break
```

### Comparing `yfjpscraper-0.3.2/yfjpscraper/parser.py` & `yfjpscraper-0.3.3/yfjpscraper/parser.py`

 * *Files identical despite different names*

