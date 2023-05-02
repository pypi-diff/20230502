# Comparing `tmp/mbta-gtfs-sqlite-0.9.0.tar.gz` & `tmp/mbta-gtfs-sqlite-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbta-gtfs-sqlite-0.9.0.tar", max compression
+gzip compressed data, was "mbta-gtfs-sqlite-0.9.1.tar", max compression
```

## Comparing `mbta-gtfs-sqlite-0.9.0.tar` & `mbta-gtfs-sqlite-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       59 2023-05-01 19:07:59.003673 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/__init__.py
--rw-r--r--   0        0        0     2522 2023-05-01 19:40:06.198381 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/archive.py
--rw-r--r--   0        0        0     2368 2023-05-01 20:08:17.551242 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/build.py
--rw-r--r--   0        0        0      312 2023-04-30 02:20:13.261136 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/compact.py
--rw-r--r--   0        0        0     2917 2023-05-01 19:08:24.868631 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/feed.py
--rw-r--r--   0        0        0     6281 2023-05-01 18:28:34.679685 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/ingest.py
--rw-r--r--   0        0        0      300 2023-05-01 19:08:24.816733 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/__init__.py
--rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/base.py
--rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/calendar.py
--rw-r--r--   0        0        0     1452 2023-05-01 18:55:03.550890 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/calendar_attributes.py
--rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/calendar_dates.py
--rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/feed_info.py
--rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/lines.py
--rw-r--r--   0        0        0     1177 2023-04-30 02:22:19.299183 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/route_patterns.py
--rw-r--r--   0        0        0     1540 2023-04-30 02:22:29.021433 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/routes.py
--rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/shapes.py
--rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/stop_times.py
--rw-r--r--   0        0        0     2222 2023-05-01 19:08:24.872868 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/stops.py
--rw-r--r--   0        0        0     1641 2023-04-30 02:22:51.048772 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/transfers.py
--rw-r--r--   0        0        0     1866 2023-05-01 19:08:24.861186 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/trips.py
--rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/reader.py
--rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/session.py
--rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/utils/decorators.py
--rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/utils/enum.py
--rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/utils/indexes.py
--rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/utils/time.py
--rw-r--r--   0        0        0      454 2023-05-01 20:05:02.693316 mbta-gtfs-sqlite-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      742 2023-05-01 20:10:01.191046 mbta-gtfs-sqlite-0.9.0/setup.py
--rw-r--r--   0        0        0      494 2023-05-01 20:10:01.191297 mbta-gtfs-sqlite-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-05-01 19:07:59.003673 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-01 20:26:55.513197 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/archive.py
+-rw-r--r--   0        0        0     2433 2023-05-01 20:21:33.810772 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/build.py
+-rw-r--r--   0        0        0      312 2023-04-30 02:20:13.261136 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/compact.py
+-rw-r--r--   0        0        0     3310 2023-05-01 20:37:55.264919 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/feed.py
+-rw-r--r--   0        0        0     6281 2023-05-01 18:28:34.679685 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/ingest.py
+-rw-r--r--   0        0        0      300 2023-05-01 19:08:24.816733 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/__init__.py
+-rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/base.py
+-rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/calendar.py
+-rw-r--r--   0        0        0     1452 2023-05-01 18:55:03.550890 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/calendar_attributes.py
+-rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/calendar_dates.py
+-rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/feed_info.py
+-rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/lines.py
+-rw-r--r--   0        0        0     1177 2023-04-30 02:22:19.299183 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/route_patterns.py
+-rw-r--r--   0        0        0     1540 2023-04-30 02:22:29.021433 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/routes.py
+-rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/shapes.py
+-rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/stop_times.py
+-rw-r--r--   0        0        0     2222 2023-05-01 19:08:24.872868 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/stops.py
+-rw-r--r--   0        0        0     1641 2023-04-30 02:22:51.048772 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/transfers.py
+-rw-r--r--   0        0        0     1866 2023-05-01 19:08:24.861186 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/trips.py
+-rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/reader.py
+-rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/session.py
+-rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/utils/decorators.py
+-rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/utils/enum.py
+-rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/utils/indexes.py
+-rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/utils/time.py
+-rw-r--r--   0        0        0      454 2023-05-01 20:40:28.651354 mbta-gtfs-sqlite-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      742 2023-05-01 20:40:48.833900 mbta-gtfs-sqlite-0.9.1/setup.py
+-rw-r--r--   0        0        0      494 2023-05-01 20:40:48.834145 mbta-gtfs-sqlite-0.9.1/PKG-INFO
```

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/archive.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/archive.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/build.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,22 @@
             remove(db_path)
             remove(compact_db_path)
         except FileNotFoundError:
             pass
         raise ex
 
 
-def build_local_feed_entry(feed: GtfsFeed):
+def build_local_feed_entry(feed: GtfsFeed, compact_only=False):
     ensure_subdirectory(feed)
     (zip_path, feed_path, db_path, compact_db_path) = (
         path.join(feed.local_subdirectory, entity)
         for entity in ("data.zip", "feed", "gtfs.sqlite3", "gtfs_compact.sqlite3")
     )
     download_feed_zip(feed.url, zip_path)
     unzip_feed(zip_path, feed_path)
     result = GtfsFeedDownloadResult(
         url=feed.url,
         zip_md5_checksum=get_zip_checksum(zip_path),
     )
     ingest_feed_to_sqlite(feed_path, db_path, compact_db_path, result)
+    if compact_only:
+        remove(db_path)
```

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/feed.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/feed.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,69 +4,77 @@
 from dataclasses import dataclass
 from functools import cached_property
 
 
 if TYPE_CHECKING:
     from .archive import MbtaGtfsArchive
 
-FEED_FILES = [
-    "gtfs.sqlite3",
-    "gtfs_compact.sqlite3",
-]
+DB_FILE = "gtfs.sqlite3"
+DB_COMPACT_FILE = "gtfs_compact.sqlite3"
+ALL_DB_FILES = [DB_FILE, DB_COMPACT_FILE]
 
 
 @dataclass
 class GtfsFeed(object):
     archive: "MbtaGtfsArchive"
     key: str
     url: str
     version: str
     start_date: date
     end_date: date
 
+    def __post_init__(self):
+        self.compact_only = False
+
     def __repr__(self):
         return f"GtfsFeed({self.key})"
 
     @cached_property
     def local_subdirectory(self):
         return path.join(self.archive.local_archive_path, self.key)
 
+    def required_feed_files(self):
+        return ALL_DB_FILES if not self.compact_only else [DB_COMPACT_FILE]
+
+    def use_compact_only(self, enabled: bool = True):
+        self.compact_only = enabled
+
     def exists_locally(self):
-        for file in FEED_FILES:
+        for file in self.required_feed_files():
             if not path.exists(path.join(self.local_subdirectory, file)):
                 return False
         return True
 
     def exists_remotely(self):
         try:
             remote_objects = self.archive.s3_bucket.objects.filter(Prefix=self.key)
         except RuntimeError:
             return False
-        for file in FEED_FILES:
+        for file in self.required_feed_files():
             if not any(obj.key.endswith(file) for obj in remote_objects):
                 return False
         return True
 
     def build_locally(self):
         from .build import build_local_feed_entry
 
-        build_local_feed_entry(self)
+        build_local_feed_entry(self, self.compact_only)
 
     def download_from_s3(self):
         if not self.exists_remotely():
             raise RuntimeError("Feed does not exist remotely")
-        for file in FEED_FILES:
+        for file in self.required_feed_files():
             self.archive.s3_bucket.download_file(
                 f"{self.key}/{file}", path.join(self.local_subdirectory, file)
             )
 
     def upload_to_s3(self):
         if not self.exists_locally():
             raise RuntimeError("Feed does not exist locally")
-        for file in FEED_FILES:
+        for file in self.required_feed_files():
             self.archive.s3_bucket.upload_file(
                 path.join(self.local_subdirectory, file), f"{self.key}/{file}"
             )
 
     def download_or_build(self):
         if self.exists_locally():
             return
```

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/ingest.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/ingest.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/base.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/base.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/calendar.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/calendar.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/calendar_attributes.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/calendar_attributes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/calendar_dates.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/calendar_dates.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/feed_info.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/feed_info.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/lines.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/lines.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/route_patterns.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/route_patterns.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/routes.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/routes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/stop_times.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/stop_times.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/stops.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/stops.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/transfers.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/transfers.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/models/trips.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/models/trips.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/reader.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/reader.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/utils/indexes.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/utils/indexes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/mbta_gtfs_sqlite/utils/time.py` & `mbta-gtfs-sqlite-0.9.1/mbta_gtfs_sqlite/utils/time.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.0/setup.py` & `mbta-gtfs-sqlite-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['SQLAlchemy>=2.0.7,<3.0.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'mbta-gtfs-sqlite',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': "Query the MBTA's static GTFS feeds using sqlite",
     'long_description': None,
     'author': 'Ian Reynolds',
     'author_email': 'ireynolds@transitmatters.info',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

