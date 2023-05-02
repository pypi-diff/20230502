# Comparing `tmp/pokerlib-2.2.0.tar.gz` & `tmp/pokerlib-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerlib-2.2.0.tar", max compression
+gzip compressed data, was "pokerlib-2.2.1.tar", max compression
```

## Comparing `pokerlib-2.2.0.tar` & `pokerlib-2.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.0/LICENSE
--rw-r--r--   0        0        0     6276 2023-04-24 16:13:38.139069 pokerlib-2.2.0/README.md
--rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.0/pokerlib/__init__.py
--rw-r--r--   0        0        0     9058 2023-04-20 19:59:08.048593 pokerlib-2.2.0/pokerlib/_handparser.py
--rw-r--r--   0        0        0     5387 2023-04-20 21:01:45.318611 pokerlib-2.2.0/pokerlib/_player.py
--rw-r--r--   0        0        0    17502 2023-04-24 10:35:35.288769 pokerlib-2.2.0/pokerlib/_round.py
--rw-r--r--   0        0        0     6936 2023-04-07 09:33:14.596230 pokerlib-2.2.0/pokerlib/_table.py
--rw-r--r--   0        0        0     1652 2023-04-20 20:01:46.748594 pokerlib-2.2.0/pokerlib/enums.py
--rw-r--r--   0        0        0      122 2023-04-20 19:44:07.068589 pokerlib-2.2.0/pokerlib/implementations/__init__.py
--rw-r--r--   0        0        0      462 2023-04-20 19:43:30.238589 pokerlib-2.2.0/pokerlib/implementations/_no_muck_showdown_table.py
--rw-r--r--   0        0        0      360 2023-04-20 19:50:58.588591 pokerlib-2.2.0/pokerlib/implementations/_no_muck_table.py
--rw-r--r--   0        0        0      663 2023-04-24 16:14:19.719070 pokerlib-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     7001 1970-01-01 00:00:00.000000 pokerlib-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.1/LICENSE
+-rw-r--r--   0        0        0     6276 2023-05-02 19:42:40.871493 pokerlib-2.2.1/README.md
+-rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.1/pokerlib/__init__.py
+-rw-r--r--   0        0        0     9058 2023-05-02 19:42:16.761493 pokerlib-2.2.1/pokerlib/_handparser.py
+-rw-r--r--   0        0        0     5387 2023-05-02 19:42:16.761493 pokerlib-2.2.1/pokerlib/_player.py
+-rw-r--r--   0        0        0    17719 2023-05-02 19:48:34.711495 pokerlib-2.2.1/pokerlib/_round.py
+-rw-r--r--   0        0        0     6936 2023-04-07 09:33:14.596230 pokerlib-2.2.1/pokerlib/_table.py
+-rw-r--r--   0        0        0     1652 2023-05-02 19:42:16.761493 pokerlib-2.2.1/pokerlib/enums.py
+-rw-r--r--   0        0        0      130 2023-05-02 19:42:16.761493 pokerlib-2.2.1/pokerlib/implementations/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-02 19:42:16.761493 pokerlib-2.2.1/pokerlib/implementations/_no_muck_showdown_table.py
+-rw-r--r--   0        0        0      360 2023-05-02 19:42:16.761493 pokerlib-2.2.1/pokerlib/implementations/_no_muck_table.py
+-rw-r--r--   0        0        0      663 2023-05-02 20:03:26.111499 pokerlib-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7001 1970-01-01 00:00:00.000000 pokerlib-2.2.1/PKG-INFO
```

### Comparing `pokerlib-2.2.0/LICENSE` & `pokerlib-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.0/README.md` & `pokerlib-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.0/pokerlib/_handparser.py` & `pokerlib-2.2.1/pokerlib/_handparser.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.0/pokerlib/_player.py` & `pokerlib-2.2.1/pokerlib/_player.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.0/pokerlib/_round.py` & `pokerlib-2.2.1/pokerlib/_round.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,18 +446,20 @@
 
     def __init__(self, *args):
         self.public_out_queue = deque([])
         self.private_out_queue = deque([])
         super().__init__(*args)
 
     def publicIn(self, player_id, action, raise_by=0):
-        if action is self.PublicInId.SHOW or action is self.PublicInId.MUCK:
-            if player_id in self._muck_optioned_player_ids:
-                self._executeChoice(action, player_id)
-        elif (
+        if self.closed: return # can't do anything if round is closed
+        if self.finished: # if round is finished, only show/muck is allowed
+            if action is self.PublicInId.SHOW or action is self.PublicInId.MUCK:
+                if player_id in self._muck_optioned_player_ids:
+                    self._executeChoice(action, player_id)
+        elif ( # if round is not finished, only valid actions are allowed
             action is self.PublicInId.CHECK or
             action is self.PublicInId.CALL or
             action is self.PublicInId.FOLD or
             action is self.PublicInId.ALLIN or
             action is self.PublicInId.RAISE
         ):
             player = self.current_player
```

### Comparing `pokerlib-2.2.0/pokerlib/_table.py` & `pokerlib-2.2.1/pokerlib/_table.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.0/pokerlib/enums.py` & `pokerlib-2.2.1/pokerlib/enums.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.0/pyproject.toml` & `pokerlib-2.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pokerlib"
-version = "2.2.0"
+version = "2.2.1"
 description = "Python poker library"
 repository = "https://github.com/kuco23/pokerlib/"
 authors = ["kuco23 <nseverkar@gmail.com>"]
 keywords = ['python', 'poker', 'library']
 readme = "README.md"
 classifiers=  [
     'Development Status :: 3 - Alpha',
```

### Comparing `pokerlib-2.2.0/PKG-INFO` & `pokerlib-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerlib
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python poker library
 Home-page: https://github.com/kuco23/pokerlib/
 Keywords: python,poker,library
 Author: kuco23
 Author-email: nseverkar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

