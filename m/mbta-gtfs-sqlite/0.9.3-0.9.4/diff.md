# Comparing `tmp/mbta-gtfs-sqlite-0.9.3.tar.gz` & `tmp/mbta-gtfs-sqlite-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbta-gtfs-sqlite-0.9.3.tar", max compression
+gzip compressed data, was "mbta-gtfs-sqlite-0.9.4.tar", max compression
```

## Comparing `mbta-gtfs-sqlite-0.9.3.tar` & `mbta-gtfs-sqlite-0.9.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       59 2023-05-01 19:07:59.003673 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/__init__.py
--rw-r--r--   0        0        0     2522 2023-05-01 20:26:55.513197 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/archive.py
--rw-r--r--   0        0        0     2265 2023-05-02 03:05:44.353658 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/build.py
--rw-r--r--   0        0        0      312 2023-04-30 02:20:13.261136 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/compact.py
--rw-r--r--   0        0        0     4110 2023-05-02 12:21:38.720435 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/feed.py
--rw-r--r--   0        0        0     6281 2023-05-01 18:28:34.679685 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/ingest.py
--rw-r--r--   0        0        0      300 2023-05-01 19:08:24.816733 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/__init__.py
--rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/base.py
--rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/calendar.py
--rw-r--r--   0        0        0     1452 2023-05-01 18:55:03.550890 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/calendar_attributes.py
--rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/calendar_dates.py
--rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/feed_info.py
--rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/lines.py
--rw-r--r--   0        0        0     1177 2023-04-30 02:22:19.299183 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/route_patterns.py
--rw-r--r--   0        0        0     1540 2023-04-30 02:22:29.021433 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/routes.py
--rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/shapes.py
--rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/stop_times.py
--rw-r--r--   0        0        0     2222 2023-05-01 19:08:24.872868 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/stops.py
--rw-r--r--   0        0        0     1641 2023-04-30 02:22:51.048772 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/transfers.py
--rw-r--r--   0        0        0     1866 2023-05-01 19:08:24.861186 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/trips.py
--rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/reader.py
--rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/session.py
--rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/utils/decorators.py
--rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/utils/enum.py
--rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/utils/indexes.py
--rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/utils/time.py
--rw-r--r--   0        0        0      454 2023-05-02 12:26:12.595870 mbta-gtfs-sqlite-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      742 2023-05-02 12:26:28.730221 mbta-gtfs-sqlite-0.9.3/setup.py
--rw-r--r--   0        0        0      494 2023-05-02 12:26:28.730449 mbta-gtfs-sqlite-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-05-02 12:38:56.937705 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-01 20:26:55.513197 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/archive.py
+-rw-r--r--   0        0        0     2265 2023-05-02 03:05:44.353658 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/build.py
+-rw-r--r--   0        0        0      312 2023-04-30 02:20:13.261136 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/compact.py
+-rw-r--r--   0        0        0     4110 2023-05-02 12:21:38.720435 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/feed.py
+-rw-r--r--   0        0        0     6281 2023-05-01 18:28:34.679685 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/ingest.py
+-rw-r--r--   0        0        0      322 2023-05-02 12:51:09.476358 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/__init__.py
+-rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/base.py
+-rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/calendar.py
+-rw-r--r--   0        0        0     1452 2023-05-01 18:55:03.550890 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/calendar_attributes.py
+-rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/calendar_dates.py
+-rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/feed_info.py
+-rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/lines.py
+-rw-r--r--   0        0        0     1177 2023-04-30 02:22:19.299183 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/route_patterns.py
+-rw-r--r--   0        0        0     1540 2023-04-30 02:22:29.021433 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/routes.py
+-rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/shapes.py
+-rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/stop_times.py
+-rw-r--r--   0        0        0     2222 2023-05-01 19:08:24.872868 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/stops.py
+-rw-r--r--   0        0        0     1641 2023-04-30 02:22:51.048772 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/transfers.py
+-rw-r--r--   0        0        0     1866 2023-05-01 19:08:24.861186 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/trips.py
+-rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/reader.py
+-rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/session.py
+-rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/utils/decorators.py
+-rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/utils/enum.py
+-rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/utils/indexes.py
+-rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/utils/time.py
+-rw-r--r--   0        0        0      454 2023-05-02 12:52:03.672251 mbta-gtfs-sqlite-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      742 2023-05-02 12:52:12.735830 mbta-gtfs-sqlite-0.9.4/setup.py
+-rw-r--r--   0        0        0      494 2023-05-02 12:52:12.736078 mbta-gtfs-sqlite-0.9.4/PKG-INFO
```

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/archive.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/archive.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/build.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/build.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/feed.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/feed.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/ingest.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/ingest.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/base.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/base.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/calendar.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/calendar.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/calendar_attributes.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/calendar_attributes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/calendar_dates.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/calendar_dates.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/feed_info.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/feed_info.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/lines.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/lines.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/route_patterns.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/route_patterns.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/routes.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/routes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/stop_times.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/stop_times.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/stops.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/stops.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/transfers.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/transfers.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/models/trips.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/models/trips.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/reader.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/reader.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/utils/indexes.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/utils/indexes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/mbta_gtfs_sqlite/utils/time.py` & `mbta-gtfs-sqlite-0.9.4/mbta_gtfs_sqlite/utils/time.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.3/setup.py` & `mbta-gtfs-sqlite-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['SQLAlchemy>=2.0.7,<3.0.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'mbta-gtfs-sqlite',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': "Query the MBTA's static GTFS feeds using sqlite",
     'long_description': None,
     'author': 'Ian Reynolds',
     'author_email': 'ireynolds@transitmatters.info',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

