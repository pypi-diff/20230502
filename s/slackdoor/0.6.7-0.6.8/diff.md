# Comparing `tmp/slackdoor-0.6.7.tar.gz` & `tmp/slackdoor-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackdoor-0.6.7.tar", max compression
+gzip compressed data, was "slackdoor-0.6.8.tar", max compression
```

## Comparing `slackdoor-0.6.7.tar` & `slackdoor-0.6.8.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     2192 2022-12-10 17:52:41.838669 slackdoor-0.6.7/LICENSE
--rw-r--r--   0        0        0       22 2023-03-15 22:33:01.285987 slackdoor-0.6.7/door/__init__.py
--rw-r--r--   0        0        0    11040 2023-03-15 18:22:18.222845 slackdoor-0.6.7/door/core.py
--rw-r--r--   0        0        0     5142 2023-03-15 18:18:02.515195 slackdoor-0.6.7/door/decorators.py
--rw-r--r--   0        0        0    52953 2023-03-15 18:32:18.532794 slackdoor-0.6.7/door/dispatch.py
--rw-r--r--   0        0        0     5648 2022-12-10 17:52:41.841199 slackdoor-0.6.7/door/models/__init__.py
--rw-r--r--   0        0        0     1637 2023-03-15 18:26:59.708502 slackdoor-0.6.7/door/models/files/file.py
--rw-r--r--   0        0        0    13307 2023-03-15 18:27:19.978281 slackdoor-0.6.7/door/models/messages/message.py
--rw-r--r--   0        0        0      412 2023-03-15 18:18:02.515531 slackdoor-0.6.7/door/plugins/__init__.py
--rw-r--r--   0        0        0     1656 2022-12-10 17:52:41.843014 slackdoor-0.6.7/door/plugins/base.py
--rw-r--r--   0        0        0     2507 2022-12-10 17:52:41.843531 slackdoor-0.6.7/door/plugins/commands/leave.py
--rw-r--r--   0        0        0     2097 2023-03-15 18:18:02.516337 slackdoor-0.6.7/door/plugins/examples/channel_joined.py
--rw-r--r--   0        0        0     3858 2022-12-10 17:52:41.844577 slackdoor-0.6.7/door/plugins/examples/general.py
--rw-r--r--   0        0        0      898 2022-12-10 17:52:41.844936 slackdoor-0.6.7/door/run.py
--rw-r--r--   0        0        0     4298 2023-03-15 18:50:59.374709 slackdoor-0.6.7/door/sentry.py
--rw-r--r--   0        0        0     1895 2023-03-15 18:18:02.512729 slackdoor-0.6.7/door/settings.py
--rw-r--r--   0        0        0    22537 2023-03-15 18:29:02.543125 slackdoor-0.6.7/door/slack.py
--rw-r--r--   0        0        0     7262 2023-03-15 18:29:45.608632 slackdoor-0.6.7/door/utils/__init__.py
--rw-r--r--   0        0        0      980 2023-03-15 18:18:02.509410 slackdoor-0.6.7/door/utils/collections.py
--rw-r--r--   0        0        0     2442 2023-01-29 20:50:33.038675 slackdoor-0.6.7/door/utils/interactive.py
--rw-r--r--   0        0        0      966 2022-12-10 17:52:41.847964 slackdoor-0.6.7/door/utils/plugins.py
--rw-r--r--   0        0        0     2317 2023-03-15 22:33:01.268375 slackdoor-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 slackdoor-0.6.7/setup.py
--rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 slackdoor-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     2192 2022-12-10 17:52:41.000000 slackdoor-0.6.8/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-02 02:28:12.748175 slackdoor-0.6.8/door/__init__.py
+-rw-r--r--   0        0        0    11040 2023-03-15 18:22:18.000000 slackdoor-0.6.8/door/core.py
+-rw-r--r--   0        0        0     5142 2023-03-15 18:18:02.000000 slackdoor-0.6.8/door/decorators.py
+-rw-r--r--   0        0        0    52953 2023-03-15 18:32:18.000000 slackdoor-0.6.8/door/dispatch.py
+-rw-r--r--   0        0        0     5648 2022-12-10 17:52:41.000000 slackdoor-0.6.8/door/models/__init__.py
+-rw-r--r--   0        0        0     1637 2023-03-15 18:26:59.000000 slackdoor-0.6.8/door/models/files/file.py
+-rw-r--r--   0        0        0    13307 2023-03-15 18:27:19.000000 slackdoor-0.6.8/door/models/messages/message.py
+-rw-r--r--   0        0        0      412 2023-03-15 18:18:02.000000 slackdoor-0.6.8/door/plugins/__init__.py
+-rw-r--r--   0        0        0     1656 2022-12-10 17:52:41.000000 slackdoor-0.6.8/door/plugins/base.py
+-rw-r--r--   0        0        0     2507 2022-12-10 17:52:41.000000 slackdoor-0.6.8/door/plugins/commands/leave.py
+-rw-r--r--   0        0        0     2097 2023-03-15 18:18:02.000000 slackdoor-0.6.8/door/plugins/examples/channel_joined.py
+-rw-r--r--   0        0        0     3858 2022-12-10 17:52:41.000000 slackdoor-0.6.8/door/plugins/examples/general.py
+-rw-r--r--   0        0        0      898 2022-12-10 17:52:41.000000 slackdoor-0.6.8/door/run.py
+-rw-r--r--   0        0        0     4298 2023-03-15 18:50:59.000000 slackdoor-0.6.8/door/sentry.py
+-rw-r--r--   0        0        0     1895 2023-03-15 18:18:02.000000 slackdoor-0.6.8/door/settings.py
+-rw-r--r--   0        0        0    22537 2023-03-15 18:29:02.000000 slackdoor-0.6.8/door/slack.py
+-rw-r--r--   0        0        0     7266 2023-05-02 02:26:45.689997 slackdoor-0.6.8/door/utils/__init__.py
+-rw-r--r--   0        0        0      980 2023-03-15 18:18:02.000000 slackdoor-0.6.8/door/utils/collections.py
+-rw-r--r--   0        0        0     2442 2023-01-29 20:50:33.000000 slackdoor-0.6.8/door/utils/interactive.py
+-rw-r--r--   0        0        0      966 2022-12-10 17:52:41.000000 slackdoor-0.6.8/door/utils/plugins.py
+-rw-r--r--   0        0        0     2317 2023-05-02 02:28:12.740232 slackdoor-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 slackdoor-0.6.8/PKG-INFO
```

### Comparing `slackdoor-0.6.7/LICENSE` & `slackdoor-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/core.py` & `slackdoor-0.6.8/door/core.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/decorators.py` & `slackdoor-0.6.8/door/decorators.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/dispatch.py` & `slackdoor-0.6.8/door/dispatch.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/models/__init__.py` & `slackdoor-0.6.8/door/models/__init__.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/models/files/file.py` & `slackdoor-0.6.8/door/models/files/file.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/models/messages/message.py` & `slackdoor-0.6.8/door/models/messages/message.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/plugins/base.py` & `slackdoor-0.6.8/door/plugins/base.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/plugins/commands/leave.py` & `slackdoor-0.6.8/door/plugins/commands/leave.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/plugins/examples/channel_joined.py` & `slackdoor-0.6.8/door/plugins/examples/channel_joined.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/plugins/examples/general.py` & `slackdoor-0.6.8/door/plugins/examples/general.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/run.py` & `slackdoor-0.6.8/door/run.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/sentry.py` & `slackdoor-0.6.8/door/sentry.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/settings.py` & `slackdoor-0.6.8/door/settings.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/slack.py` & `slackdoor-0.6.8/door/slack.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/utils/__init__.py` & `slackdoor-0.6.8/door/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,16 @@
 def deduplicate(items: Iterable) -> list:
     """Remove duplicates in an iterable while preserving order"""
     seen = []
     return [x for x in items if not (x in seen or seen.append(x))]
 
 
 def fix_timestamp(timestamp: str) -> str:
-    # convert Z to +00:00 (RFC 3339 format), or change +0000 to +00:00, so datetime.fromisoformat works
-    return re.sub(r"\+(\d\d)(\d\d)$", r"+\1:\2", timestamp.replace("Z", "+00:00"))
+    # convert Z to +00:00 (RFC 3339 format), or change ±0000 to ±00:00, so datetime.fromisoformat works
+    return re.sub(r"[+-](\d\d)(\d\d)$", r"+\1:\2", timestamp.replace("Z", "+00:00"))
 
 
 def strip_mrkdwn(text: str) -> str:
     """Strip Slack-flavored 'mrkdwn' formatting"""
     text = re.sub(r"\*_((?:\S)(?:.*?))_\*", r"\1", text)  # strip *_..._*
     text = re.sub(r"_\*((?:\S)(?:.*?))\*_", r"\1", text)  # strip *_..._*
     text = re.sub(r"([*_])((?:\S)(?:.*?))(?:\1)", r"\2", text)  # strip *...* or _..._
```

### Comparing `slackdoor-0.6.7/door/utils/collections.py` & `slackdoor-0.6.8/door/utils/collections.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/utils/interactive.py` & `slackdoor-0.6.8/door/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/door/utils/plugins.py` & `slackdoor-0.6.8/door/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.7/pyproject.toml` & `slackdoor-0.6.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 authors = ["Eddy G <eddyg@users.noreply.github.com>"]
 license = "MIT"
 repository = "https://github.com/eddyg/slackdoor"
 packages = [
     {include = "door"}
 ]
 
-version = "0.6.7"
+version = "0.6.8"
 # NOTE: uses the 'poetry_bumpversion' plugin to keep versions in sync
 # Use:
 #   poetry version {patch|minor|major|prepatch|preminor|premajor|prerelease}
 # to bump the version and have it be "authoritative" here and in __init__
 # To tag:
 #   git tag $(awk -F'"' '/^version =/{print $2}' pyproject.toml)
 #   git push -o ci.skip && git push --tags
```

### Comparing `slackdoor-0.6.7/PKG-INFO` & `slackdoor-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slackdoor
-Version: 0.6.7
+Version: 0.6.8
 Summary: An opinionated and powerful chatbot framework for Slack
 Home-page: https://github.com/eddyg/slackdoor
 License: MIT
 Author: Eddy G
 Author-email: eddyg@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

