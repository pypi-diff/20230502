# Comparing `tmp/xklb-1.26.15.tar.gz` & `tmp/xklb-1.26.18.tar.gz`

## Comparing `xklb-1.26.15.tar` & `xklb-1.26.18.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.15/.gitattributes
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 xklb-1.26.15/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.15/Windows.md
--rw-r--r--   0        0        0   414011 2020-02-02 00:00:00.000000 xklb-1.26.15/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.15/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.15/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.15/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.15/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 xklb-1.26.15/.github/workflows/push.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/__init__.py
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/av.py
--rw-r--r--   0        0        0     6859 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/books.py
--rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/consts.py
--rw-r--r--   0        0        0     7856 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/db.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/dl_config.py
--rw-r--r--   0        0        0    14860 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/dl_extract.py
--rw-r--r--   0        0        0    13555 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/fs_extract.py
--rw-r--r--   0        0        0     6067 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/gui.py
--rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/hn_extract.py
--rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/lb.py
--rw-r--r--   0        0        0    35709 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/play_actions.py
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/playback.py
--rw-r--r--   0        0        0    26512 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/player.py
--rw-r--r--   0        0        0    14708 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/praw_extract.py
--rw-r--r--   0        0        0    16159 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/stats.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/subtitle.py
--rw-r--r--   0        0        0    12089 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21697 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/tube_backend.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/tube_extract.py
--rw-r--r--   0        0        0    28119 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/utils.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17099 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/mining/nfb_ca.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/mining/words.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.15/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.15/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.15/LICENSE
--rw-r--r--   0        0        0    40524 2020-02-02 00:00:00.000000 xklb-1.26.15/README.md
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.26.15/pyproject.toml
--rw-r--r--   0        0        0    44061 2020-02-02 00:00:00.000000 xklb-1.26.15/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.18/.gitattributes
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 xklb-1.26.18/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.18/Windows.md
+-rw-r--r--   0        0        0   414011 2020-02-02 00:00:00.000000 xklb-1.26.18/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.18/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.18/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.18/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.18/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 xklb-1.26.18/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/__init__.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/av.py
+-rw-r--r--   0        0        0     6859 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/books.py
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/consts.py
+-rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/db.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/dl_config.py
+-rw-r--r--   0        0        0    14860 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/gui.py
+-rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/lb.py
+-rw-r--r--   0        0        0    35724 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/play_actions.py
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/playback.py
+-rw-r--r--   0        0        0    26699 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/player.py
+-rw-r--r--   0        0        0    14748 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/stats.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21740 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28159 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/utils.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/mining/nfb_ca.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.18/xklb/scripts/mining/words.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.18/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.18/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.18/LICENSE
+-rw-r--r--   0        0        0    40524 2020-02-02 00:00:00.000000 xklb-1.26.18/README.md
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.26.18/pyproject.toml
+-rw-r--r--   0        0        0    44061 2020-02-02 00:00:00.000000 xklb-1.26.18/PKG-INFO
```

### Comparing `xklb-1.26.15/TODO` & `xklb-1.26.18/TODO`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/Windows.md` & `xklb-1.26.18/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/pdm.lock` & `xklb-1.26.18/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/readme.py` & `xklb-1.26.18/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.26.18/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.26.18/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/.github/workflows/push.yaml` & `xklb-1.26.18/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/av.py` & `xklb-1.26.18/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/books.py` & `xklb-1.26.18/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/consts.py` & `xklb-1.26.18/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/db.py` & `xklb-1.26.18/xklb/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sqlite3
 from pathlib import Path
 from textwrap import dedent
-from typing import Any, Iterable, List, Optional, Union
+from typing import Any, Dict, Iterable, List, Optional, Union
 
 from xklb import consts, utils
 from xklb.utils import log
 
 
 def tracer(sql, params) -> None:
     sql = utils.remove_consecutives(dedent(sql), "\n")
@@ -33,15 +33,15 @@
             return data[0]
 
         def pop_dict(
             self,
             sql: str,
             params: Optional[Union[Iterable, dict]] = None,
             ignore_errors=None,
-        ) -> Optional[Any]:
+        ) -> Optional[Dict]:
             if ignore_errors is None:
                 ignore_errors = ["no such table"]
             try:
                 dg = self.query(sql, params)
                 d = next(dg, None)
             except sqlite3.OperationalError as exc:
                 if any(e in str(exc) for e in ignore_errors):
```

### Comparing `xklb-1.26.15/xklb/dl_config.py` & `xklb-1.26.18/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/dl_extract.py` & `xklb-1.26.18/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/fs_extract.py` & `xklb-1.26.18/xklb/fs_extract.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from pathlib import Path
 from shutil import which
 from timeit import default_timer as timer
 from typing import Dict, List, Optional
 
 from xklb import av, books, consts, db, player, utils
 from xklb.consts import SC, DBType
-from xklb.player import mark_media_deleted
 from xklb.utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
 
     profile = parser.add_mutually_exclusive_group()
@@ -217,14 +216,35 @@
         print(f"[{path}] Not found")
         return []
 
     columns = args.db["media"].columns_dict
     scanned_set = set(scanned_files)
 
     try:
+        deleted_set = {
+            d["path"]
+            for d in args.db.query(
+                f"""select path from media
+                where 1=1
+                    and time_deleted > 0
+                    and path like '{path}%'
+                    {'AND time_downloaded > 0' if 'time_downloaded' in columns else ''}
+                """,
+            )
+        }
+    except Exception as e:
+        log.debug(e)
+        pass
+    else:
+        undeleted_files = list(deleted_set.intersection(scanned_set))
+        undeleted_count = player.mark_media_undeleted(args, undeleted_files)
+        if undeleted_count > 0:
+            print(f"[{path}] Marking", undeleted_count, "metadata records as undeleted")
+
+    try:
         existing_set = {
             d["path"]
             for d in args.db.query(
                 f"""select path from media
                 where 1=1
                     and time_deleted = 0
                     and path like '{path}%'
@@ -238,15 +258,15 @@
     else:
         new_files = list(scanned_set - existing_set)
 
         deleted_files = list(existing_set - scanned_set)
         if not new_files and len(deleted_files) >= len(existing_set) and not args.force:
             print(f"[{path}] Path empty or device not mounted. Rerun with -f to mark all subpaths as deleted.")
             return []  # if path not mounted or all files deleted
-        deleted_count = mark_media_deleted(args, deleted_files)
+        deleted_count = player.mark_media_deleted(args, deleted_files)
         if deleted_count > 0:
             print(f"[{path}] Marking", deleted_count, "orphaned metadata records as deleted")
 
     return new_files
 
 
 def _add_folder(args, folder_path: Path) -> None:
```

### Comparing `xklb-1.26.15/xklb/gui.py` & `xklb-1.26.18/xklb/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import NoReturn, Tuple
 
 from xklb.utils import log
 
 
 class UserQuit(BaseException):
     pass
 
@@ -87,26 +87,26 @@
         # bind first letter key
         self.root.bind(true_action[0], lambda _ev: self.return_true())
         self.root.bind(false_action[0], lambda _ev: self.return_false())
 
         self.move_window(*(geom_data or []))
         self.root.mainloop()
 
-    def user_quit(self):
+    def user_quit(self) -> NoReturn:
         raise UserQuit
 
-    def return_true(self):
+    def return_true(self) -> None:
         self.action = True
         self.root.destroy()
 
-    def return_false(self):
+    def return_false(self) -> None:
         self.action = False
         self.root.destroy()
 
-    def move_window(self, window_width=None, window_height=None, x=None, y=None):
+    def move_window(self, window_width=None, window_height=None, x=None, y=None) -> None:
         s_width = window_width or self.root.winfo_screenwidth()
         s_height = window_height or self.root.winfo_screenheight()
 
         # window_width, window_height = 380, 150  # override
         x_coordinate = x or 0
         y_coordinate = y or 0
         self.root.geometry(f"{window_width}x{window_height}+{x_coordinate}+{y_coordinate}")
```

### Comparing `xklb-1.26.15/xklb/hn_extract.py` & `xklb-1.26.18/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/lb.py` & `xklb-1.26.18/xklb/lb.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     if a is None:
         a = []
     subcommands.extend([name, *a])
     aliases = a + consecutive_prefixes(name) + utils.conform([consecutive_prefixes(a) for a in a])
     return subparsers.add_parser(name, aliases=aliases, add_help=False)
 
 
-def create_subcommands_parser():
+def create_subcommands_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         prog="lb",
         description="xk media library",
         epilog="Report bugs here: https://github.com/chapmanjacobd/library/issues/new/choose",
         add_help=False,
     )
     subparsers = parser.add_subparsers()
```

### Comparing `xklb-1.26.15/xklb/play_actions.py` & `xklb-1.26.18/xklb/play_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
         library {action} --multiple-playback 4  # play four media at once, divide by available screens
         library {action} -m 4 --screen-name eDP # play four media at once on specific screen
         library {action} -m 4 --loop --crop     # play four cropped videos on a loop
         library {action} -m 4 --hstack          # use hstack style
 """
 
 
-def parse_args_sort(args):
+def parse_args_sort(args) -> None:
     if args.sort:
         args.sort = " ".join(args.sort)
     elif not args.sort and hasattr(args, "defaults"):
         args.defaults.append("sort")
 
     m_columns = args.db["media"].columns_dict
 
@@ -659,15 +659,15 @@
         [
             args.play_in_order >= consts.SIMILAR,
             args.action == SC.listen and "audiobook" in media_file.lower(),
         ],
     )
 
 
-def transcode(args, path):
+def transcode(args, path) -> str:
     log.debug(path)
     sub_index = subtitle.get_sub_index(args, path)
 
     transcode_dest = str(Path(path).with_suffix(".mkv"))
     temp_video = random_filename(transcode_dest)
 
     maps = ["-map", "0"]
```

### Comparing `xklb-1.26.15/xklb/playback.py` & `xklb-1.26.18/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/player.py` & `xklb-1.26.18/xklb/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             end = int(args.start) + int(args.end)
         else:
             end = int(args.end)
 
     return start, end
 
 
-def get_browser():
+def get_browser() -> Optional[str]:
     default_application = cmd("xdg-mime", "query", "default", "text/html").stdout
     return which(default_application.replace(".desktop", ""))
 
 
 def find_xdg_application(media_file) -> Optional[str]:
     if media_file.startswith("http"):
         return get_browser()
@@ -207,35 +207,39 @@
                     (*chunk_paths,),
                 )
                 modified_row_count += cursor.rowcount
 
     return modified_row_count
 
 
-def mark_media_deleted(args, paths) -> int:
+def mark_media_deleted(args, paths, time_deleted=consts.APPLICATION_START) -> int:
     paths = utils.conform(paths)
 
     modified_row_count = 0
     if paths:
         df_chunked = utils.chunks(paths, consts.SQLITE_PARAM_LIMIT)
         for chunk_paths in df_chunked:
             with args.db.conn:
                 cursor = args.db.conn.execute(
                     f"""update media
-                    set time_deleted={consts.APPLICATION_START}
+                    set time_deleted={time_deleted}
                     where path in ("""
                     + ",".join(["?"] * len(chunk_paths))
                     + ")",
                     (*chunk_paths,),
                 )
                 modified_row_count += cursor.rowcount
 
     return modified_row_count
 
 
+def mark_media_undeleted(args, paths) -> int:
+    return mark_media_deleted(args, paths, time_deleted=0)
+
+
 def mark_media_deleted_like(args, paths) -> int:
     paths = utils.conform(paths)
 
     modified_row_count = 0
     if paths:
         for p in paths:
             with args.db.conn:
@@ -356,15 +360,15 @@
         sort_expression.replace("month_created", YEAR_MONTH("time_created"))
         .replace("month_modified", YEAR_MONTH("time_modified"))
         .replace("random", "random()")
         .replace("priority", "ntile(1000) over (order by size) desc, duration")
     )
 
 
-def last_chars(candidate):
+def last_chars(candidate) -> str:
     remove_groups = re.split(r"([\W]+|\s+|Ep\d+|x\d+|\.\d+)", candidate)
     log.debug(remove_groups)
 
     remove_chars = ""
     number_of_groups = 1
     while len(remove_chars) < 1:
         remove_chars += remove_groups[-number_of_groups]
@@ -519,15 +523,15 @@
             y = int(ha * h_idx)
             log.debug("geom_walk %s", {"va": va, "ha": ha, "v_idx": v_idx, "h_idx": h_idx, "x": x, "y": y})
             geoms.append([va, ha, x, y])
 
     return geoms
 
 
-def grid_stack(display, qty, swap=False):
+def grid_stack(display, qty, swap=False) -> List[Tuple]:
     if qty == 1:
         return [("--fs", f'--screen-name="{display.name}"', f'--fs-screen-name="{display.name}"')]
     else:
         dv = list(utils.divisor_gen(qty))
         if not dv:
             vh = (qty, 1)
             log.debug("not dv %s", {"dv": dv, "vh": vh})
@@ -540,15 +544,15 @@
     v, h = vh
     if swap:
         h, v = v, h
     holes = geom_walk(display, v=v, h=h)
     return [(hole, f'--screen-name="{display.name}"') for hole in holes]
 
 
-def get_display_by_name(displays, screen_name):  # -> List[screeninfo.Monitor]
+def get_display_by_name(displays, screen_name):  # noqa: ANN201; -> List[screeninfo.Monitor]
     for d in displays:
         if d.name == screen_name:
             return [d]
 
     display_names = '", "'.join([d.name for d in displays])
     raise Exception(f'Display "{screen_name}" not found. I see: "{display_names}"')
```

### Comparing `xklb-1.26.15/xklb/praw_extract.py` & `xklb-1.26.18/xklb/praw_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import datetime as dt
 import json
 import sys
 from functools import partial
 from itertools import takewhile
 from pathlib import Path
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Tuple
 
 from xklb import consts, db, utils
 from xklb.utils import log
 
 PRAW_SETUP_INSTRUCTIONS = r"""
 You will need your Reddit user login info, client id, and secret.
 See https://www.reddit.com/wiki/api for client id / secret.
@@ -179,15 +179,15 @@
         "selftext": selftext,
         "title": d.get("title"),
         "total_awards_received": d.get("total_awards_received"),
         "playlist_path": playlist_path,
     }
 
 
-def save_post(args, post_dict, subreddit_path):
+def save_post(args, post_dict, subreddit_path) -> None:
     slim_dict = utils.dict_filter_bool(slim_post_data(post_dict, subreddit_path))
 
     if slim_dict:
         already_downloaded_path = args.db.pop(
             "SELECT path FROM media WHERE webpath =?",
             [slim_dict["path"]],
             ignore_errors=["no such column", "no such table"],
@@ -303,36 +303,36 @@
         for post in takewhile(_takewhile, subreddit.top(time_filter, limit=args.limit)):
             save_post(args, saveable(post), subreddit_path)
 
 
 skip_errors = None
 
 
-def load_module_level_skip_errors():
+def load_module_level_skip_errors() -> Tuple:
     global skip_errors
 
     if skip_errors is None:
         import prawcore
 
         skip_errors = (prawcore.exceptions.NotFound, prawcore.exceptions.Forbidden, prawcore.exceptions.Redirect)
     return skip_errors
 
 
-def process_redditors(args, redditors):
+def process_redditors(args, redditors) -> None:
     load_module_level_skip_errors()
 
     for redditor in redditors:
         try:
             redditor_new(args, redditor)
         except skip_errors as e:
             log.error("[%s] skipping redditor: %s", redditor["name"], e)
             continue
 
 
-def process_subreddits(args, subreddits):
+def process_subreddits(args, subreddits) -> None:
     load_module_level_skip_errors()
 
     for subreddit in subreddits:
         try:
             subreddit_new(args, subreddit)
             subreddit_top(args, subreddit)
         except skip_errors as e:
```

### Comparing `xklb-1.26.15/xklb/stats.py` & `xklb-1.26.18/xklb/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from tabulate import tabulate
 
 from xklb import consts, db, dl_extract, play_actions, tube_backend, utils
 from xklb.player import delete_playlists
 from xklb.utils import human_time, log, pipe_print
 
 
-def parse_args(prog, usage):
+def parse_args(prog, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog,
         usage,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--fields", "-f", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--aggregate", "-a", action="store_true", help=argparse.SUPPRESS)
```

### Comparing `xklb-1.26.15/xklb/subtitle.py` & `xklb-1.26.18/xklb/subtitle.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             log.warning(f"[{video_path}] Could not decode subtitle {path}")
             return []
 
     subtitles = " ".join(list(dict.fromkeys(flatten([sub_to_text(path) for path in paths]))))
     return remove_consecutive_whitespace(subtitles)
 
 
-def is_text_subtitle_stream(s):
+def is_text_subtitle_stream(s) -> bool:
     return s.get("codec_type") == "subtitle" and s.get("codec_name") not in IMAGE_SUBTITLE_CODECS
 
 
 def externalize_internal_subtitles(f, streams=None) -> List[str]:
     if streams is None:
         streams = ffmpeg.probe(f, show_chapters=None)["streams"]
 
@@ -104,24 +104,24 @@
 
     if subtitles:
         return subtitles
 
     return []
 
 
-def get_subtitle_paths(f):
+def get_subtitle_paths(f) -> List[str]:
     internal_subtitles = externalize_internal_subtitles(f)
     if len(internal_subtitles) > 0:
         return internal_subtitles
 
     external_subtitles = get_external(f)
     return external_subtitles
 
 
-def get_sub_index(args, f):
+def get_sub_index(args, f) -> Optional[int]:
     streams = ffmpeg.probe(f)["streams"]
     temp_db = db.connect(args, memory=True)
     temp_db["streams"].insert_all(streams, pk="index")  # type: ignore
     subtitle_index = temp_db.pop(
         f"""select "index" from streams
             where codec_type = "subtitle"
               and codec_name not in ({",".join(['?'] * len(IMAGE_SUBTITLE_CODECS))})
```

### Comparing `xklb-1.26.15/xklb/tabs_actions.py` & `xklb-1.26.18/xklb/tabs_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,41 +121,41 @@
         args.database = args.db
     args.db = db.connect(args)
     log.info(utils.dict_filter_bool(args.__dict__))
 
     return args
 
 
-def tabs_include_string(x):
+def tabs_include_sql(x) -> str:
     return f"""and (
     path like :include{x}
     OR category like :include{x}
     OR frequency like :include{x}
 )"""
 
 
-def tabs_exclude_string(x):
+def tabs_exclude_sql(x) -> str:
     return f"""and (
     path not like :exclude{x}
     AND category not like :exclude{x}
     AND frequency not like :exclude{x}
 )"""
 
 
 def construct_tabs_query(args) -> Tuple[str, dict]:
     args.filter_sql = []
     args.filter_bindings = {}
 
     args.filter_sql.extend([" and " + w for w in args.where])
 
     for idx, inc in enumerate(args.include):
-        args.filter_sql.append(tabs_include_string(idx))
+        args.filter_sql.append(tabs_include_sql(idx))
         args.filter_bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
     for idx, exc in enumerate(args.exclude):
-        args.filter_sql.append(tabs_exclude_string(idx))
+        args.filter_sql.append(tabs_exclude_sql(idx))
         args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
 
     LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
     OFFSET = f"OFFSET {args.skip}" if args.skip else ""
 
     query = f"""SELECT path
         , frequency
```

### Comparing `xklb-1.26.15/xklb/tabs_extract.py` & `xklb-1.26.18/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/tube_backend.py` & `xklb-1.26.18/xklb/tube_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse, json, sys
 from copy import deepcopy
 from datetime import datetime
 from pathlib import Path
+from types import ModuleType
 from typing import Dict, List, Optional, Tuple
 
 from xklb import consts, fs_extract, utils
 from xklb.consts import DBType
 from xklb.dl_config import (
     prefix_unrecoverable_errors,
     yt_meaningless_errors,
@@ -13,15 +14,15 @@
     yt_unrecoverable_errors,
 )
 from xklb.utils import combine, log, safe_unpack
 
 yt_dlp = None
 
 
-def load_module_level_yt_dlp():
+def load_module_level_yt_dlp() -> ModuleType:
     global yt_dlp
 
     if yt_dlp is None:
         import yt_dlp
     return yt_dlp
```

### Comparing `xklb-1.26.15/xklb/tube_extract.py` & `xklb-1.26.18/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/utils.py` & `xklb-1.26.18/xklb/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
     if not cast_infos:
         log.error("Target chromecast device not found")
         raise SystemExit(53)
 
     return cast_infos[0].host
 
 
-def path_to_mpv_watchlater_md5(path: str):
+def path_to_mpv_watchlater_md5(path: str) -> str:
     return hashlib.md5(path.encode("utf-8")).hexdigest().upper()
 
 
 def mpv_enrich(args, media) -> List[Dict]:
     for m in media:
         md5 = path_to_mpv_watchlater_md5(m["path"])
         metadata_path = Path(args.watch_later_directory, md5)
@@ -454,15 +454,15 @@
             continue
         else:
             filtered_media.append(m)
 
     return filtered_media
 
 
-def safe_int(s):
+def safe_int(s) -> Optional[int]:
     try:
         return int(float(s))
     except Exception:
         return None
 
 
 def mpv_enrich2(args, media) -> List[Dict]:
@@ -908,15 +908,15 @@
 
 
 def confirm(*args, **kwargs) -> bool:
     clear_input()
     return prompt.Confirm.ask(*args, **kwargs, default=False)
 
 
-def connect_mpv(ipc_socket, start_mpv=False):
+def connect_mpv(ipc_socket, start_mpv=False):  # noqa: ANN201
     try:
         from python_mpv_jsonipc import MPV
 
         return MPV(start_mpv, ipc_socket)
     except (ConnectionRefusedError, FileNotFoundError):
         Path(ipc_socket).unlink(missing_ok=True)
```

### Comparing `xklb-1.26.15/xklb/scripts/__init__.py` & `xklb-1.26.18/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/scripts/bigdirs.py` & `xklb-1.26.18/xklb/scripts/bigdirs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from typing import List
+from typing import Dict, List
 
 from tabulate import tabulate
 
 from xklb import db, utils
 from xklb.utils import log
 
 
@@ -40,15 +40,15 @@
     if args.size:
         args.size = utils.parse_human_to_sql(utils.human_to_bytes, "size", args.size)
 
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
-def group_files_by_folder(args, media):
+def group_files_by_folder(args, media) -> List[Dict]:
     d = {}
     for m in media:
         p = m["path"].split("/")
         while len(p) >= 2:
             p.pop()
             parent = "/".join(p) + "/"
 
@@ -73,15 +73,15 @@
                 d.pop(path)
             elif pdict["count"] > (args.upper or 4000):
                 d.pop(path)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
-def group_folders(args, folders):
+def group_folders(args, folders) -> List[Dict]:
     d = {}
     for f in folders:
         p = f["path"].split("/")
         p.pop()
 
         depth = 1 + args.depth
         parent = "/".join(p[:depth]) + "/"
@@ -121,15 +121,15 @@
         order by path
         """,
         ),
     )
     return media
 
 
-def process_bigdirs(args, media):
+def process_bigdirs(args, media) -> List[Dict]:
     folders = group_files_by_folder(args, media)
     if args.depth:
         folders = group_folders(args, folders)
     return sorted(folders, key=lambda x: x["count_deleted"] if args.sort_by_deleted else x["size"] / x["count"])
 
 
 def bigdirs() -> None:
```

### Comparing `xklb-1.26.15/xklb/scripts/christen.py` & `xklb-1.26.18/xklb/scripts/christen.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     parser.add_argument("--verbose", "-v", action="count", default=0)
     args = parser.parse_args()
 
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
-def rename_path(args, b):
+def rename_path(args, b) -> None:
     fixed = utils.clean_path(b, args.dot_space)
 
     if b != fixed.encode():
         printable_p = b.decode("utf-8", "backslashreplace")
         if args.run:
             p = Path(fsdecode(b))
             if not p.is_file():
```

### Comparing `xklb-1.26.15/xklb/scripts/copy_play_counts.py` & `xklb-1.26.18/xklb/scripts/copy_play_counts.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     Path(args.database).touch()
     args.db = db.connect(args)
     log.info(utils.dict_filter_bool(args.__dict__))
 
     return args
 
 
-def copy_play_count(args, source_db):
+def copy_play_count(args, source_db) -> None:
     args.db.attach("src", Path(source_db).resolve())
 
     modified_row_count = 0
     with args.db.conn:
         sql = f"""
         UPDATE
             main.media
@@ -69,15 +69,15 @@
         """
         cursor = args.db.conn.execute(sql, {"source_prefix": args.source_prefix, "target_prefix": args.target_prefix})
         modified_row_count += cursor.rowcount
 
     log.info("Updated %s rows", modified_row_count)
 
 
-def copy_play_counts():
+def copy_play_counts() -> None:
     args = parse_args()
     for s_db in args.source_dbs:
         copy_play_count(args, s_db)
 
 
 if __name__ == "__main__":
     copy_play_counts()
```

### Comparing `xklb-1.26.15/xklb/scripts/dedupe.py` & `xklb-1.26.18/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/scripts/merge_dbs.py` & `xklb-1.26.18/xklb/scripts/merge_dbs.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,30 +28,30 @@
     Path(args.database).touch()
     args.db = db.connect(args)
     log.info(utils.dict_filter_bool(args.__dict__))
 
     return args
 
 
-def merge_db(args, source_db):
+def merge_db(args, source_db) -> None:
     source_db = str(Path(source_db).resolve())
 
     s_db = db.connect(argparse.Namespace(database=source_db, verbose=args.verbose))
     for table in [s for s in s_db.table_names() if "_fts" not in s and not s.startswith("sqlite_")]:
         log.info("[%s]: %s", source_db, table)
         data = s_db[table].rows
 
         with args.db.conn:
             if args.upsert:
                 args.db[table].upsert_all(data, pk=args.upsert.split(","), alter=True)
             else:
                 args.db[table].insert_all(data, alter=True, replace=True)
 
 
-def merge_dbs():
+def merge_dbs() -> None:
     args = parse_args()
     for s_db in args.source_dbs:
         merge_db(args, s_db)
 
 
 if __name__ == "__main__":
     merge_dbs()
```

### Comparing `xklb-1.26.15/xklb/scripts/merge_online_local.py` & `xklb-1.26.18/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/scripts/move_list.py` & `xklb-1.26.18/xklb/scripts/move_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse, shutil, tempfile
 from copy import deepcopy
 from pathlib import Path
-from typing import List
+from typing import Dict, List, Tuple
 
 import humanize
 from tabulate import tabulate
 
 from xklb import db, player, utils
 from xklb.utils import log
 
@@ -24,15 +24,15 @@
     parser.add_argument("database")
     args = parser.parse_args()
     args.db = db.connect(args)
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
-def group_by_folder(args, media):
+def group_by_folder(args, media) -> List[Dict]:
     d = {}
     for m in media:
         if m["path"].startswith("http"):
             continue
 
         p = m["path"].split("/")
         while len(p) >= 3:
@@ -70,15 +70,15 @@
         ),
     )
 
     folders = group_by_folder(args, media)
     return sorted(folders, key=lambda x: x["size"] / x["count"])
 
 
-def print_some(args, tbl):
+def iterate_and_show_options(args, tbl) -> Tuple[List[Dict], List[Dict]]:
     vew = tbl[-int(args.limit) :] if args.limit else tbl
 
     vew = utils.list_dict_filter_bool(vew, keep_0=False)
     vew = utils.col_resize(vew, "path", 60)
     vew = utils.col_naturalsize(vew, "size")
     print(tabulate(vew, tablefmt="fancy_grid", headers="keys", showindex=False))
     print(len(tbl) - len(vew), "other folders not shown")
@@ -94,15 +94,15 @@
     _total, _used, free = shutil.disk_usage(args.mount_point)
 
     print("Current free space:", humanize.naturalsize(free))
 
     data = get_table(args)
 
     tbl = deepcopy(data)
-    cur, rest = print_some(args, tbl)
+    cur, rest = iterate_and_show_options(args, tbl)
 
     data = {d["path"]: d for d in data}
 
     utils.set_readline_completion(list(data.keys()))
 
     print(
         """
@@ -126,24 +126,24 @@
             input_path = input("Paste a path: ").strip()
         except EOFError:
             break
         if input_path.lower() in ["done", "q"]:
             break
 
         if input_path.lower() == "more":
-            cur, rest = print_some(args, rest)
+            cur, rest = iterate_and_show_options(args, rest)
             continue
 
         if input_path == "*":
             if cur:
                 selected_paths.update([d["path"] for d in cur])
             else:
                 selected_paths.update(data.keys())
 
-            cur, rest = print_some(args, rest)
+            cur, rest = iterate_and_show_options(args, rest)
         else:
             try:
                 data[input_path]
             except KeyError:
                 continue
 
             if input_path in selected_paths:
```

### Comparing `xklb-1.26.15/xklb/scripts/optimize_db.py` & `xklb-1.26.18/xklb/scripts/optimize_db.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 
 from xklb import db, utils
 from xklb.utils import log
 
 
-def optimize_db():
+def optimize_db() -> None:
     parser = argparse.ArgumentParser(
         prog="library optimize",
         usage="""library optimize DATABASE [--force]
 
     Optimize library databases
 
     The force flag is usually unnecessary and it can take much longer
```

### Comparing `xklb-1.26.15/xklb/scripts/redownload.py` & `xklb-1.26.18/xklb/scripts/redownload.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             WHERE time_deleted = strftime('%s', ?, 'utc')
             AND time_downloaded > 0
         """
         media = list(args.db.query(query, (args.deleted_at,)))
     return media
 
 
-def mark_media_undownloaded(args, deleted_media):
+def mark_media_undownloaded(args, deleted_media) -> None:
     m_columns = args.db["media"].columns_dict
 
     media = deepcopy(deleted_media)
     for d in media:
         d["time_deleted"] = 0
         d["time_modified"] = 0
         d["time_downloaded"] = 0
@@ -136,22 +136,22 @@
 
             d["path"] = d["webpath"]
             args.db["media"].upsert(d, pk="path", alter=True)  # type: ignore
         else:
             args.db["media"].upsert(d, pk="path", alter=True)  # type: ignore
 
 
-def print_deletions(args, deletions):
+def print_deletions(args, deletions) -> None:
     print("Deletions:")
     tbl = deepcopy(deletions)
     print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
     print(f"Showing most recent {args.limit} deletions. Use -l to change this limit")
 
 
-def print_deleted(args, deleted_media):
+def print_deleted(args, deleted_media) -> None:
     tbl = deepcopy(deleted_media)
     tbl = utils.list_dict_filter_bool(tbl, keep_0=False)
     tbl = utils.list_dict_filter_unique(tbl)
     tbl = utils.list_dict_filter_keys(tbl, ["sparseness"])
     tbl = tbl[: int(args.limit)]
     tbl = utils.col_resize(tbl, "path", 25)
     tbl = utils.col_duration(tbl, "duration")
```

### Comparing `xklb-1.26.15/xklb/scripts/relmv.py` & `xklb-1.26.18/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/xklb/scripts/scatter.py` & `xklb-1.26.18/xklb/scripts/scatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse, random, tempfile
 from pathlib import Path
 from statistics import median
-from typing import List
+from typing import Dict, List, Tuple, Union
 
 from humanize import naturalsize
 from tabulate import tabulate
 
 from xklb import consts, db, utils
 from xklb.utils import log
 
@@ -138,15 +138,15 @@
             },
         ),
     )
 
     return media
 
 
-def get_path_stats(args, data):
+def get_path_stats(args, data) -> List[Dict]:
     result = []
     for srcmount in args.srcmounts:
         disk_files = [d for d in data if d["path"].startswith(srcmount)]
         if disk_files:
             result.append(
                 {
                     "mount": srcmount,
@@ -157,25 +157,25 @@
                     "time_modified": median(d["time_modified"] for d in disk_files),
                     "time_scanned": median(d["time_downloaded"] for d in disk_files),
                 },
             )
     return result
 
 
-def print_path_stats(tbl):
+def print_path_stats(tbl) -> None:
     tbl = utils.list_dict_filter_bool(tbl, keep_0=False)
     tbl = utils.col_naturalsize(tbl, "total_size")
     tbl = utils.col_naturalsize(tbl, "median_size")
     for t in consts.TIME_COLUMNS:
         utils.col_naturaldate(tbl, t)
 
     print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
 
 
-def rebin_files(args, disk_stats, all_files):
+def rebin_files(args, disk_stats, all_files) -> Tuple[List, List]:
     total_size = sum(d["size"] for d in all_files)
 
     untouched = []
     to_rebin = []
     full_disks = []
     for disk_stat in disk_stats:
         disk_files = [d for d in all_files if d["path"].startswith(disk_stat["mount"])]
@@ -227,15 +227,15 @@
         file["from_path"] = file["path"]
         file["path"] = file["path"].replace(file["mount"], new_mount)
         rebinned.append(file)
 
     return untouched, rebinned
 
 
-def get_rel_stats(parents, files):
+def get_rel_stats(parents, files) -> List[Dict[str, Union[float, str]]]:
     mount_space = []
     total_used = 1
     for parent in parents:
         used = sum([file["size"] for file in files if file["path"].startswith(parent)])
         total_used += used
         mount_space.append([parent, used])
```

### Comparing `xklb-1.26.15/xklb/scripts/streaming_tab_loader.py` & `xklb-1.26.18/xklb/scripts/streaming_tab_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse, logging, sys
 from time import sleep
+from typing import List
 
 from xklb import db, player, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
@@ -35,19 +36,19 @@
         log.error("Currently only stdin is supported")
         raise NotImplementedError
 
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
-def list_tabs(args):
+def list_tabs(args) -> List:
     return args.bt_api.list_tabs([])
 
 
-def open_tabs(_args, urls):
+def open_tabs(_args, urls) -> None:
     for url in urls:
         utils.cmd(player.get_browser(), url)
 
 
 def streaming_tab_loader() -> None:
     args = parse_args()
```

### Comparing `xklb-1.26.15/xklb/scripts/mining/nfb_ca.py` & `xklb-1.26.18/xklb/scripts/mining/nfb_ca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from xklb.utils import log, pipe_print
 
 
-def get_page_links(url):
+def get_page_links(url) -> None:
     from urllib.parse import urlparse
 
     import requests
     from bs4 import BeautifulSoup
 
     soup = BeautifulSoup(requests.get(url).content, "html.parser")
     film_list = set()
```

### Comparing `xklb-1.26.15/xklb/scripts/mining/nouns.py` & `xklb-1.26.18/xklb/scripts/mining/nouns.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,54 +17,54 @@
     def __init__(self) -> None:
         super().__init__()
         self.reset()
         self.strict = False
         self.convert_charrefs = True
         self.text = StringIO()
 
-    def handle_data(self, data):
+    def handle_data(self, data) -> None:
         self.text.write(data)
 
-    def get_data(self):
+    def get_data(self) -> str:
         return self.text.getvalue()
 
 
-def strip_tags(html):
+def strip_tags(html) -> str:
     s = MLStripper()
     s.feed(html)
     return s.get_data()
 
 
-def is_num(s):
+def is_num(s) -> bool:
     return s.replace(".", "", 1).replace("-", "", 1).isdigit()
 
 
-def printer(parts):
+def printer(parts) -> None:
     for part in parts:
         part = part.strip()
         if not part:
             continue
 
         part_lookup = part.lower()
         if part_lookup in words.stop_words or part_lookup in words.prepositions or is_num(part):
             continue
 
         pipe_print(part)
 
 
-def line_processor(txt):
+def line_processor(txt) -> None:
     txt = strip_tags(txt)
 
     if getattr(line_processor, "RE_NOUNS_SPLIT", None) is None:
         import regex
 
         line_processor.RE_NOUNS_SPLIT = regex.compile(
             r"(?= [a-z]|(?<!\b[A-Z][a-z]*) (?=[A-Z]))|[.?!,\/#$%\^&\*;:{}=\-_`~()]|\,|\'|\"|\^|‘|’|“|”|\n| -| :| _",
         )
 
     parts = line_processor.RE_NOUNS_SPLIT.split(txt)
     printer(parts)
 
 
-def nouns():
+def nouns() -> None:
     for line in sys.stdin:
         line_processor(line)
```

### Comparing `xklb-1.26.15/xklb/scripts/mining/pushshift.py` & `xklb-1.26.18/xklb/scripts/mining/pushshift.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     args.db = db.connect(args)
 
     log.info(utils.dict_filter_bool(args.__dict__))
 
     return args
 
 
-def save_data(args, reddit_posts, media):
+def save_data(args, reddit_posts, media) -> None:
     if len(reddit_posts) > 0:
         args.db["reddit_posts"].insert_all(reddit_posts, alter=True)
         reddit_posts.clear()
     if len(media) > 0:
         args.db["media"].insert_all(media, alter=True)
         media.clear()
```

### Comparing `xklb-1.26.15/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.26.18/xklb/scripts/mining/reddit_selftext.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse, html
+from typing import Set, Tuple
 from urllib.parse import urlparse
 
 from xklb import db, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
@@ -18,15 +19,15 @@
     args = parser.parse_args()
 
     args.db = db.connect(args)
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
-def get_page_links(path, text):
+def get_page_links(path, text) -> Tuple[Set, Set]:
     from bs4 import BeautifulSoup
 
     soup = BeautifulSoup(html.unescape(text), "lxml")
     internal_links = set()
     external_links = set()
 
     for a in soup.findAll("a", attrs={"href": True}):
```

### Comparing `xklb-1.26.15/xklb/scripts/mining/words.py` & `xklb-1.26.18/xklb/scripts/mining/words.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/assets/kotobago.png` & `xklb-1.26.18/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/.gitignore` & `xklb-1.26.18/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/LICENSE` & `xklb-1.26.18/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/README.md` & `xklb-1.26.18/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.015)
+    xk media library subcommands (v1.26.018)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.26.15/pyproject.toml` & `xklb-1.26.18/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.15/PKG-INFO` & `xklb-1.26.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.26.15
+Version: 1.26.18
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -100,15 +100,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.015)
+    xk media library subcommands (v1.26.018)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

