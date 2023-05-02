# Comparing `tmp/vunnel-0.8.1.tar.gz` & `tmp/vunnel-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vunnel-0.8.1.tar", max compression
+gzip compressed data, was "vunnel-0.9.0.tar", max compression
```

## Comparing `vunnel-0.8.1.tar` & `vunnel-0.9.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2023-03-28 18:51:04.427726 vunnel-0.8.1/LICENSE
--rw-r--r--   0        0        0     3574 2023-03-28 18:51:04.427726 vunnel-0.8.1/README.md
--rw-r--r--   0        0        0     7206 2023-03-28 18:51:34.951975 vunnel-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2226 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/__init__.py
--rw-r--r--   0        0        0       34 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/__main__.py
--rw-r--r--   0        0        0       52 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/cli/__init__.py
--rw-r--r--   0        0        0     8451 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/cli/cli.py
--rw-r--r--   0        0        0     3230 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/cli/config.py
--rw-r--r--   0        0        0     8308 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/provider.py
--rw-r--r--   0        0        0     2268 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/providers/__init__.py
--rw-r--r--   0        0        0     1949 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/providers/alpine/__init__.py
--rw-r--r--   0        0        0    10817 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/providers/alpine/parser.py
--rw-r--r--   0        0        0     2128 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/providers/amazon/__init__.py
--rw-r--r--   0        0        0    10062 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/providers/amazon/parser.py
--rw-r--r--   0        0        0     2368 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/providers/centos/__init__.py
--rw-r--r--   0        0        0     5857 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/providers/centos/parser.py
--rw-r--r--   0        0        0     2075 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/providers/chainguard/__init__.py
--rw-r--r--   0        0        0     2294 2023-03-28 18:51:04.427726 vunnel-0.8.1/src/vunnel/providers/debian/__init__.py
--rw-r--r--   0        0        0    22154 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/debian/parser.py
--rw-r--r--   0        0        0     2833 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/github/__init__.py
--rw-r--r--   0        0        0    18569 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/github/parser.py
--rw-r--r--   0        0        0     2447 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/nvd/__init__.py
--rw-r--r--   0        0        0     5598 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/nvd/api.py
--rw-r--r--   0        0        0     2948 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/nvd/manager.py
--rw-r--r--   0        0        0     1968 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/oracle/__init__.py
--rw-r--r--   0        0        0     6144 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/oracle/parser.py
--rw-r--r--   0        0        0     1972 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/rhel/__init__.py
--rw-r--r--   0        0        0    37568 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/rhel/parser.py
--rw-r--r--   0        0        0     2157 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/sles/__init__.py
--rw-r--r--   0        0        0    15909 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/sles/parser.py
--rw-r--r--   0        0        0     2175 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/ubuntu/__init__.py
--rw-r--r--   0        0        0    14635 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/ubuntu/git.py
--rw-r--r--   0        0        0    43019 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/ubuntu/parser.py
--rw-r--r--   0        0        0     2038 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/wolfi/__init__.py
--rw-r--r--   0        0        0     4954 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/providers/wolfi/parser.py
--rw-r--r--   0        0        0     6590 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/result.py
--rw-r--r--   0        0        0     1877 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/schema.py
--rw-r--r--   0        0        0     2020 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/utils/__init__.py
--rw-r--r--   0        0        0     3985 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/utils/fdb.py
--rw-r--r--   0        0        0     9879 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/utils/oval_parser.py
--rw-r--r--   0        0        0    17609 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/utils/oval_v2.py
--rw-r--r--   0        0        0     7823 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/utils/rpm.py
--rw-r--r--   0        0        0     2334 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/utils/vulnerability.py
--rw-r--r--   0        0        0     7840 2023-03-28 18:51:04.431726 vunnel-0.8.1/src/vunnel/workspace.py
--rw-r--r--   0        0        0     5340 1970-01-01 00:00:00.000000 vunnel-0.8.1/setup.py
--rw-r--r--   0        0        0     5384 1970-01-01 00:00:00.000000 vunnel-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 13:15:42.768662 vunnel-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3574 2023-04-27 13:15:42.768662 vunnel-0.9.0/README.md
+-rw-r--r--   0        0        0     7268 2023-04-27 13:16:17.709159 vunnel-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2226 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/__init__.py
+-rw-r--r--   0        0        0       34 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/__main__.py
+-rw-r--r--   0        0        0       52 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/cli/__init__.py
+-rw-r--r--   0        0        0     8451 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/cli/cli.py
+-rw-r--r--   0        0        0     3230 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/cli/config.py
+-rw-r--r--   0        0        0     8308 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/provider.py
+-rw-r--r--   0        0        0     2268 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/__init__.py
+-rw-r--r--   0        0        0     1949 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/alpine/__init__.py
+-rw-r--r--   0        0        0    10817 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/alpine/parser.py
+-rw-r--r--   0        0        0     2128 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/amazon/__init__.py
+-rw-r--r--   0        0        0    10062 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/amazon/parser.py
+-rw-r--r--   0        0        0     2368 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/centos/__init__.py
+-rw-r--r--   0        0        0     5857 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/centos/parser.py
+-rw-r--r--   0        0        0     2075 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/chainguard/__init__.py
+-rw-r--r--   0        0        0     2294 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/debian/__init__.py
+-rw-r--r--   0        0        0    22154 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/debian/parser.py
+-rw-r--r--   0        0        0     2833 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/github/__init__.py
+-rw-r--r--   0        0        0    18569 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/github/parser.py
+-rw-r--r--   0        0        0     2447 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/nvd/__init__.py
+-rw-r--r--   0        0        0     5598 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/nvd/api.py
+-rw-r--r--   0        0        0     2945 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/nvd/manager.py
+-rw-r--r--   0        0        0     1968 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/oracle/__init__.py
+-rw-r--r--   0        0        0     6144 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/oracle/parser.py
+-rw-r--r--   0        0        0     1972 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/rhel/__init__.py
+-rw-r--r--   0        0        0    37128 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/rhel/parser.py
+-rw-r--r--   0        0        0     2157 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/sles/__init__.py
+-rw-r--r--   0        0        0    15895 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/sles/parser.py
+-rw-r--r--   0        0        0     2175 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/ubuntu/__init__.py
+-rw-r--r--   0        0        0    14821 2023-04-27 13:15:42.772662 vunnel-0.9.0/src/vunnel/providers/ubuntu/git.py
+-rw-r--r--   0        0        0    43337 2023-04-27 13:15:42.776662 vunnel-0.9.0/src/vunnel/providers/ubuntu/parser.py
+-rw-r--r--   0        0        0     2038 2023-04-27 13:15:42.776662 vunnel-0.9.0/src/vunnel/providers/wolfi/__init__.py
+-rw-r--r--   0        0        0     4954 2023-04-27 13:15:42.776662 vunnel-0.9.0/src/vunnel/providers/wolfi/parser.py
+-rw-r--r--   0        0        0     6664 2023-04-27 13:15:42.776662 vunnel-0.9.0/src/vunnel/result.py
+-rw-r--r--   0        0        0     1877 2023-04-27 13:15:42.776662 vunnel-0.9.0/src/vunnel/schema.py
+-rw-r--r--   0        0        0     2020 2023-04-27 13:15:42.776662 vunnel-0.9.0/src/vunnel/utils/__init__.py
+-rw-r--r--   0        0        0     3985 2023-04-27 13:15:42.776662 vunnel-0.9.0/src/vunnel/utils/fdb.py
+-rw-r--r--   0        0        0     9879 2023-04-27 13:15:42.776662 vunnel-0.9.0/src/vunnel/utils/oval_parser.py
+-rw-r--r--   0        0        0    17609 2023-04-27 13:15:42.776662 vunnel-0.9.0/src/vunnel/utils/oval_v2.py
+-rw-r--r--   0        0        0     7823 2023-04-27 13:15:42.776662 vunnel-0.9.0/src/vunnel/utils/rpm.py
+-rw-r--r--   0        0        0     2334 2023-04-27 13:15:42.776662 vunnel-0.9.0/src/vunnel/utils/vulnerability.py
+-rw-r--r--   0        0        0     7840 2023-04-27 13:15:42.776662 vunnel-0.9.0/src/vunnel/workspace.py
+-rw-r--r--   0        0        0     5338 1970-01-01 00:00:00.000000 vunnel-0.9.0/setup.py
+-rw-r--r--   0        0        0     5382 1970-01-01 00:00:00.000000 vunnel-0.9.0/PKG-INFO
```

### Comparing `vunnel-0.8.1/LICENSE` & `vunnel-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/README.md` & `vunnel-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/pyproject.toml` & `vunnel-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires-python = ">=3.9.0"
 
 [tool.poetry.scripts]
 vunnel = "vunnel.cli:run"
 
 [tool.poetry]
 name = "vunnel"
-version = "0.8.1" # note: this is automagically managed -- no need to manually change this
+version = "0.9.0" # note: this is automagically managed -- no need to manually change this
 description = "vunnel ~= 'vulnerability data funnel'"
 authors = ["Alex Goodman <alex.goodman@anchore.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/anchore/vunnel"
 exclude = [
   "tests/**/*"
@@ -49,15 +49,15 @@
 ijson = ">= 2.5.1, < 3.0"   # note: required for enterprise
 xxhash = "^3.1.0"
 cvss = "^2.6"
 python-dateutil = "^2.8.2"
 defusedxml = "^0.7.1"
 dataclass-wizard = "^0.22.2"
 orjson = "^3.8.6"
-SQLAlchemy = "^1.4.46"
+SQLAlchemy = ">= 1.4.46, < 3.0"  # note: 1.4.x currently required for enterprise
 mergedeep = "^1.3.4"
 future = "^0.18.3"
 importlib-metadata = "^6.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pre-commit = "^3.2.0"
@@ -69,15 +69,15 @@
 pytest-cov = "^4.0.0"
 pytest-picked = "^0.4.6"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.2.1"
 types-PyYAML = "^6.0.12.5"
 types-requests = "^2.28.11.7"
 mypy = "^1.1"
-radon = "^5.1.0"
+radon = ">=5.1,<7.0"
 dunamai = "^1.15.0"
 ruff = "^0.0.254"
 yardstick = {git = "https://github.com/anchore/yardstick", rev = "v0.4.4"}
 tabulate = "0.9.0"
 
 [build-system]
 requires = ["poetry-core>=1.3.0", "poetry-dynamic-versioning"]
```

### Comparing `vunnel-0.8.1/src/vunnel/__init__.py` & `vunnel-0.9.0/src/vunnel/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/cli/cli.py` & `vunnel-0.9.0/src/vunnel/cli/cli.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/cli/config.py` & `vunnel-0.9.0/src/vunnel/cli/config.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/provider.py` & `vunnel-0.9.0/src/vunnel/provider.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/alpine/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/alpine/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/alpine/parser.py` & `vunnel-0.9.0/src/vunnel/providers/alpine/parser.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/amazon/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/amazon/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/amazon/parser.py` & `vunnel-0.9.0/src/vunnel/providers/amazon/parser.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/centos/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/centos/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/centos/parser.py` & `vunnel-0.9.0/src/vunnel/providers/centos/parser.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/chainguard/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/chainguard/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/debian/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/debian/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/debian/parser.py` & `vunnel-0.9.0/src/vunnel/providers/debian/parser.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/github/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/github/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/github/parser.py` & `vunnel-0.9.0/src/vunnel/providers/github/parser.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/nvd/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/nvd/api.py` & `vunnel-0.9.0/src/vunnel/providers/nvd/api.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/nvd/manager.py` & `vunnel-0.9.0/src/vunnel/providers/nvd/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         if not last_updated:
             return False
 
         now = datetime.datetime.now(tz=datetime.timezone.utc)
         days_since_last_sync = (now - last_updated).days
 
         if days_since_last_sync >= NvdAPI.max_date_range_days:
-            self.logger.warning(
+            self.logger.info(
                 f"last sync was {days_since_last_sync} days ago (more than {NvdAPI.max_date_range_days} days, the max range value of the NVD API), downloading all data"
             )
             return False
 
         return True
 
     def _download_all(self) -> Generator[tuple[str, dict[str, Any]], Any, None]:
```

### Comparing `vunnel-0.8.1/src/vunnel/providers/oracle/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/oracle/parser.py` & `vunnel-0.9.0/src/vunnel/providers/oracle/parser.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/rhel/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/rhel/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/rhel/parser.py` & `vunnel-0.9.0/src/vunnel/providers/rhel/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             p = self._fetch_rhsa(rhsa_id, platform)
             if p:
                 fixed_ver, module_name = next(
                     ([item["Version"], item.get("Module")] for item in p["Vulnerability"]["FixedIn"] if item["Name"] == package),
                     [None, None],
                 )
             else:
-                self.logger.warning(f"{rhsa_id} not found for platform {platform}")
+                self.logger.debug(f"{rhsa_id} not found for platform {platform}")
         except:
             self.logger.exception(f"error looking up {package} in {rhsa_id} for {platform}")
 
         return fixed_ver, module_name
 
     def _fetch_rhsa(self, rhsa_id, platform):
         if self.rhsa_dict is not None:  # explicit check to allow for easy testing without actually initializing it
@@ -374,37 +374,32 @@
         if not package or not isinstance(package, str):
             return name, version
 
         if ":" in package:  # tread very carefully, epoch or app streams ahead
             colon_comps = package.split(":", 1)
 
             if colon_comps[0].isdigit():  # epoch in the beginning 1:foo-bar-2.3.4-5.el6_7.8
-                # logger.warning('compliant rpm name with epoch in the beginning')
                 name_other_comps = colon_comps[1].rsplit("-", 2)  # split name-version-release.arch.rpm into max 3 chunks
                 name = name_other_comps[0]  # only the name matters
                 if len(name_other_comps) > 1:  # defaults to rhsa lookup otherwise
                     version = colon_comps[0] + ":" + "-".join(name_other_comps[1:])  # join the rest
             else:
                 name_comps = colon_comps[0].rsplit("-", 1)
                 if len(name_comps) > 1 and name_comps[1].isdigit():  # epoch in the middle foo-bar-1:2.3.4-5.el6_7.8
-                    # logger.warning('compliant rpm name with epoch in the middle')
                     name = name_comps[0]
                     version = name_comps[1] + ":" + colon_comps[1]
                 else:  # not compliant with rpm filename spec, could be an app stream
-                    # logger.warning('non-compliant rpm name with colons and hyphens')
                     name = colon_comps[0]  # best guess for name, fall back to rhsa for version lookup
 
         else:  # no epoch foo-bar-2.3.4-5.el6_7.8 or something else totally different
             if package.count("-") >= 2:  #
-                # logger.warning('may be compliant rpm name without epoch')
                 name_other_comps = package.rsplit("-", 2)  # split name-version-release.arch.rpm into max 3 chunks
                 name = name_other_comps[0]  # only the name matters
                 version = "-".join(name_other_comps[1:])  # join the rest
             else:
-                # logger.warning('non-compliant rpm name without colons and less than 2 hyphens')
                 name = package  # best guess for name, fall back to rhsa for version lookup
 
         return name, version
 
     def _parse_affected_release(self, cve_id, content):
         fixed_ins = []
         ars = content.get("affected_release", [])
@@ -506,31 +501,31 @@
                             final_m = None
                     else:
                         self.logger.debug(f"{cve_id}, platform={ar_obj.platform} : missing package and RHSA ID")
                         final_v = None
                         final_m = None
 
                     if not ar_obj.name or not final_v:
-                        self.logger.warning(
+                        self.logger.debug(
                             f"{cve_id}, platform={ar_obj.platform} : skipping affected release record as all attempts to deduce package name and or version were futile"
                         )
                         continue
 
                     ar_obj.version = final_v  # store the final_v in the object for future usage
                     ar_obj.module = final_m
 
                     prev_ar_obj = final_ar_objs.get((ar_obj.name, ar_obj.platform, ar_obj.module), None)
                     if prev_ar_obj:
                         if rpm.compare_versions(prev_ar_obj.version, ar_obj.version) < 0:
-                            self.logger.warning(
+                            self.logger.debug(
                                 f"{cve_id}, platform={prev_ar_obj.platform}, package={prev_ar_obj.name}, module={prev_ar_obj.module} : multiple fix versions found, {ar_obj.version} > {prev_ar_obj.version}"
                             )
                             final_ar_objs[(ar_obj.name, ar_obj.platform, ar_obj.module)] = ar_obj
                         else:
-                            self.logger.warning(
+                            self.logger.debug(
                                 f"{cve_id}, platform={prev_ar_obj.platform}, package={prev_ar_obj.name}, module={prev_ar_obj.module} : multiple fix versions found, {ar_obj.version} <= {prev_ar_obj.version}"
                             )
                     else:
                         final_ar_objs[(ar_obj.name, ar_obj.platform, ar_obj.module)] = ar_obj
 
                 except Exception:
                     self.logger.exception(f"error processing {cve_id} affected release object: { ar_obj.__dict__}")
@@ -590,15 +585,15 @@
 
                 if "/" in package_name:
                     components = package_name.split("/")
                     package_name = components[1]
                     module = components[0]
 
                 if not package_name:
-                    self.logger.warning(f"package state package_name missing for {cve_id} platform {platform}")
+                    self.logger.debug(f"package state package_name missing for {cve_id} platform {platform}")
                     continue
 
                 state = item.get("fix_state", None)
                 if state in ["Affected", "Fix deferred"]:
                     fixed_ins.append(
                         FixedIn(
                             platform=platform,
@@ -714,15 +709,15 @@
 
             for item in fins:  # process fixed in packages, exclude packages that are still affected
                 if (
                     item.platform,
                     item.package,
                     item.module,
                 ) in platform_package_module_tuples:
-                    self.logger.warning(
+                    self.logger.debug(
                         f"{cve_id}, platform={item.platform}, package={item.package}, module={item.module} : partial fix found but package is still vulnerable. Ignoring fix version {item.version}"
                     )
                     continue
 
                 if item.platform not in platform_artifacts:
                     platform_artifacts[item.platform] = []
```

### Comparing `vunnel-0.8.1/src/vunnel/providers/sles/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/sles/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/sles/parser.py` & `vunnel-0.9.0/src/vunnel/providers/sles/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,31 +105,31 @@
         cls, test_id: str, tests_dict: dict, artifacts_dict: dict, versions_dict: dict
     ) -> tuple[str | None, str | None]:
         name = None
         version = None
 
         test_obj = tests_dict.get(test_id)
         if not test_obj:
-            cls.logger.warning(
+            cls.logger.debug(
                 "test reference not found for %s",
                 test_id,
             )
             return name, version
 
         name_obj = artifacts_dict.get(test_obj.artifact_id)
         if not name_obj:
-            cls.logger.warning(
+            cls.logger.debug(
                 "object reference not found for %s",
                 test_obj.artifact_id,
             )
             return name, version
 
         version_obj = versions_dict.get(test_obj.version_id)
         if not version_obj:
-            cls.logger.warning(
+            cls.logger.debug(
                 "state reference not found for %s",
                 test_obj.version_id,
             )
             return name, version
 
         name = name_obj.name
         version = version_obj.value
@@ -200,15 +200,15 @@
                 continue
 
             result = release_feed.get("sles-ltss-release")
             if result:
                 results.append(result)
                 continue
 
-            cls.logger.warning(
+            cls.logger.debug(
                 "multiple unrecognized release names %s for %s, skipping %s for this namespace",
                 list(release_feed.keys()),
                 version,
                 vulnerability_id,
             )
 
         return results
@@ -251,23 +251,23 @@
                     tests_dict,
                     artifacts_dict,
                     versions_dict,
                 )
 
                 # validate release
                 if not release_name:
-                    cls.logger.warning(
+                    cls.logger.debug(
                         "release name is invalid, skipping %s",
                         vulnerability_obj.name,
                     )
                     continue
 
                 # validate version is inline with major version
                 if not release_version or not release_version.startswith(major_version):
-                    cls.logger.warning(
+                    cls.logger.debug(
                         "%s %s is an unsupported namespace for major version %s, skipping %s for this namespace",
                         release_name,
                         release_version,
                         major_version,
                         vulnerability_obj.name,
                     )
                     continue
@@ -279,15 +279,15 @@
                 fixes = []
                 for test_id in impact_item.affected_test_ids:
                     (
                         pkg_name,
                         pkg_version,
                     ) = cls._get_name_and_version_from_test(test_id, tests_dict, artifacts_dict, versions_dict)
                     if not pkg_name or not pkg_version:
-                        cls.logger.warning(
+                        cls.logger.debug(
                             "package name and or version invalid, skipping fixed-in for %s",
                             test_id,
                         )
                         continue
 
                     fixes.append(
                         FixedIn(
```

### Comparing `vunnel-0.8.1/src/vunnel/providers/ubuntu/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/ubuntu/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/ubuntu/git.py` & `vunnel-0.9.0/src/vunnel/providers/ubuntu/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,19 +61,23 @@
             self.logger.trace("git executable verified using cmd: {}, output: {}".format(self._check_cmd_, out.decode()))
         except:
             self.logger.exception('could not find required "git" executable. Please install git on host')
             raise
 
     def _check(self, destination):
         try:
+            if not os.path.exists(destination):
+                self.logger.debug(f"git working tree not found at {destination}")
+                return False
+
             cmd = self._is_git_repo_cmd_
             out = self._exec_cmd(cmd, cwd=destination)
             self.logger.debug("check for git repository, cmd: {}, output: {}".format(cmd, out.decode()))
         except:
-            self.logger.warning(f"git working tree not found at {destination}")
+            self.logger.debug(f"git working tree not found at {destination}")
             return False
 
         return True
 
     @utils.retry_with_backoff()
     def init_repo(self, force=False):
         if force:
@@ -108,15 +112,15 @@
                     hist[cve] = []
 
                 hist[cve].append(GitRevision(entry.sha, file))
 
         return hist
 
     def prepare_cve_revision_history(self):
-        self.logger.info("building full revision history for all CVEs")
+        self.logger.info("building full revision history for all CVEs.  This may take quite some time.")
         self.cve_rev_history = {}
         out = self._exec_cmd("git log --name-status --no-merges --format=oneline -- retired/ active/", cwd=self.dest)
         self.cve_rev_history = self.parse_full_cve_revision_history(out.decode())
 
     @utils.retry_with_backoff()
     def sync_with_upstream(self):
         try:
@@ -328,15 +332,15 @@
                     # D       active/CVE-2009-1553
                     deleted[cve_id] = components[1]
                 elif components[0].startswith("R"):
                     if components[0] != "R100" and len(components) > 2:
                         updated[cve_id] = components[2]
                 else:
                     # either not a commit line or an irrelevant file, ignore it
-                    self.logger.warning("encountered unknown change symbol {}".format(components[0]))
+                    self.logger.debug("skipping unknown change symbol {}".format(components[0]))
             else:
                 # not a match
                 pass
 
         if updated or deleted:
             deleted = {key: value for key, value in deleted.items() if key not in updated}
             return GitCommitSummary(sha=commit_lines[0][0], updated=updated, deleted=deleted)
```

### Comparing `vunnel-0.8.1/src/vunnel/providers/ubuntu/parser.py` & `vunnel-0.9.0/src/vunnel/providers/ubuntu/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -509,15 +509,15 @@
 
             # If there is a version indicating a fix use it, else 'None' is special keyword for no-fix-available
             if p.status == "released":
                 # Can do version format check here, but requires code from anchore-engine
                 # anchore_engine.services.policy_engine.engine.util.deb.DpkgVersion.from_string(p.get('status'))
                 pkg.Version = p.version
                 if pkg.Version is None:
-                    logger.warn(
+                    logger.debug(
                         'found CVE {} in ubuntu version {} with "released" status for pkg {} but no version for release. Released patches should have version info, but missing in source data. Marking package as not vulnerable'.format(
                             r.Name, r.NamespaceName, pkg.Name
                         )
                     )
                     continue
                     # Strange condition where a release was done but no version found. In this case, we'll omit the FixedIn record.
 
@@ -637,39 +637,40 @@
 
         # process all the updates between last processed and current revisions
         self._process_data(self.vc_workspace, from_rev=last_rev, to_rev=current_rev)
         # save last processed revision to disk
         self._save_last_processed_rev(current_rev)
 
         # load merged state and map it to vulnerabilities
-        self.logger.debug("loading processed CVE content and transforming into vulnerabilities")
-
+        self.logger.info("begin loading processed CVE content and transforming into vulnerabilities")
         for merged_cve in self._merged_cve_iterator():
             yield from map_parsed(merged_cve, self.logger)
+        self.logger.info("finish loading processed CVE content and transforming into vulnerabilities")
 
     def _process_data(self, vc_dir: str, to_rev: str, from_rev: str | None = None):
-        self.logger.debug(f"processing data from git repository: {vc_dir}, from revision: {from_rev}, to revision: {to_rev}")
+        self.logger.info(f"processing data from git repository: {vc_dir}, from revision: {from_rev}, to revision: {to_rev}")
 
         self.git_wrapper.prepare_cve_revision_history()
 
         # gather a list of changed files if the last repo revision processed is available
         updated_paths = []
         deleted_ids = []
         if from_rev and to_rev and from_rev != to_rev:
             self.logger.debug("fetching changes to CVEs between revisions {} and {}".format(from_rev, to_rev))
             modified, removed = self.git_wrapper.get_merged_change_set(from_rev=from_rev, to_rev=to_rev)
             updated_paths = list(modified.values()) if modified else []
             deleted_ids = list(removed.keys()) if removed else []
-            self.logger.debug("detected {} CVE updates (add/modify/rename)".format(len(updated_paths)))
-            self.logger.debug("detected {} CVE deletions".format(len(deleted_ids)))
+            self.logger.info("detected {} CVE updates (add/modify/rename)".format(len(updated_paths)))
+            self.logger.info("detected {} CVE deletions".format(len(deleted_ids)))
 
         # Load cves from active and retired directories and spool merged state to disk
         # note: this is an IO bound operation, so a thread pool will suffice for now
         # but look to a process pool if this becomes a bottleneck
         proc_exception = None
+        self.logger.info("begin processing updates")
         with concurrent.futures.ThreadPoolExecutor(max_workers=self._max_workers) as executor:
 
             def worker(fn, cve_id: str, *args, **kwargs):
                 try:
                     return fn(cve_id, *args, **kwargs)
                 except:
                     self.logger.exception("error processing {}".format(cve_id))
@@ -698,18 +699,22 @@
                     # cancel any scheduled tasks
                     for future in futures:
                         future.cancel()
 
         if proc_exception:
             raise proc_exception
 
+        self.logger.info("finish processing updates")
+
         # Remove merged state of deleted cves
+        self.logger.info("begin processing deletes")
         for cve_id in deleted_ids:
             self.logger.debug("{} is no longer relevant, deleting merged CVE state if any".format(cve_id))
             self._delete_merged_cve(cve_id)
+        self.logger.info("finish processing deletes")
 
     def _process_cve(self, cve_id: str, cve_rel_path: str, f: str, to_rev: str, updated_paths: list[str]):
         if cve_rel_path in updated_paths:
             # merge cves updated since last revision or all if the last processed revision is not available
             # self.logger.debug("CVE updated since last run, processing {}".format(cve_rel_path))
 
             return self._merge_cve(cve_id, cve_rel_path, f, to_rev)
@@ -779,15 +784,15 @@
         :param cve_rel_path:
         :return:
         """
         self.logger.debug(f"reprocessing merged CVE {cve_rel_path}")
         saved_state = self._load_merged_cve(cve_id)
 
         if not saved_state:
-            self.logger.warning(f"no saved state found for {cve_id}")
+            self.logger.debug(f"no saved state found for {cve_id}")
             return
 
         # reprocess only ignored patches
         merged_patches, ignored_patches, to_be_merged_map = self._categorize_patches(saved_state.ignored_patches)
 
         # Found patches that can be merged and or can't be resolved from the saved state, could be a new namespace
         if merged_patches or to_be_merged_map:
```

### Comparing `vunnel-0.8.1/src/vunnel/providers/wolfi/__init__.py` & `vunnel-0.9.0/src/vunnel/providers/wolfi/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/providers/wolfi/parser.py` & `vunnel-0.9.0/src/vunnel/providers/wolfi/parser.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/result.py` & `vunnel-0.9.0/src/vunnel/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,42 +113,42 @@
         return self.conn, self.table
 
     @property
     def db_file_path(self) -> str:
         return os.path.join(self.workspace.results_path, self.filename)
 
     def _create_table(self) -> db.Table:
-        metadata = db.MetaData(self.engine)
+        metadata = db.MetaData()
         table = db.Table(
             self.table_name,
             metadata,
             db.Column("id", db.String(), primary_key=True, index=True),
             db.Column("record", db.LargeBinary()),
         )
-        metadata.create_all()
+        metadata.create_all(self.engine)
         return table
 
     def store(self, identifier: str, record: Envelope) -> None:
         record_str = orjson.dumps(asdict(record))
         conn, table = self.connection()
 
-        # upsert the record conditionally based on the skip_duplicates configuration
+        with conn.begin():
+            # upsert the record conditionally based on the skip_duplicates configuration
+            existing = conn.execute(table.select().where(table.c.id == identifier)).first()
+            if existing:
+                if self.skip_duplicates:
+                    self.logger.warning(f"{identifier!r} entry already written (skipping)")
+                    return
+                self.logger.trace(f"overwriting existing entry: {identifier!r}")  # type: ignore[attr-defined]
+                statement = db.update(table).where(table.c.id == identifier).values(record=record_str)
+            else:
+                self.logger.trace(f"writing record to {identifier!r} key")  # type: ignore[attr-defined]
+                statement = db.insert(table).values(id=identifier, record=record_str)
 
-        existing = conn.execute(table.select().where(table.c.id == identifier)).first()
-        if existing:
-            if self.skip_duplicates:
-                self.logger.warning(f"{identifier!r} entry already written (skipping)")
-                return
-            self.logger.trace(f"overwriting existing entry: {identifier!r}")  # type: ignore[attr-defined]
-            statement = db.update(table).where(table.c.id == identifier).values(record=record_str)
-        else:
-            self.logger.trace(f"writing record to {identifier!r} key")  # type: ignore[attr-defined]
-            statement = db.insert(table).values(id=identifier, record=record_str)
-
-        conn.execute(statement)
+            conn.execute(statement)
 
     def close(self) -> None:
         if self.conn:
             self.conn.close()
             self.engine.dispose()
 
             self.conn = None
```

### Comparing `vunnel-0.8.1/src/vunnel/schema.py` & `vunnel-0.9.0/src/vunnel/schema.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/utils/__init__.py` & `vunnel-0.9.0/src/vunnel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/utils/fdb.py` & `vunnel-0.9.0/src/vunnel/utils/fdb.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/utils/oval_parser.py` & `vunnel-0.9.0/src/vunnel/utils/oval_parser.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/utils/oval_v2.py` & `vunnel-0.9.0/src/vunnel/utils/oval_v2.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/utils/rpm.py` & `vunnel-0.9.0/src/vunnel/utils/rpm.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/utils/vulnerability.py` & `vunnel-0.9.0/src/vunnel/utils/vulnerability.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/src/vunnel/workspace.py` & `vunnel-0.9.0/src/vunnel/workspace.py`

 * *Files identical despite different names*

### Comparing `vunnel-0.8.1/setup.py` & `vunnel-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'vunnel.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=5.4.1,<6.0',
- 'SQLAlchemy>=1.4.46,<2.0.0',
+ 'SQLAlchemy>=1.4.46,<3.0',
  'click>=8.1.3,<9.0.0',
  'colorlog>=6.7.0,<7.0.0',
  'cvss>=2.6,<3.0',
  'dataclass-wizard>=0.22.2,<0.23.0',
  'defusedxml>=0.7.1,<0.8.0',
  'future>=0.18.3,<0.19.0',
  'ijson>=2.5.1,<3.0',
@@ -44,15 +44,15 @@
  'xxhash>=3.1.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['vunnel = vunnel.cli:run']}
 
 setup_kwargs = {
     'name': 'vunnel',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': "vunnel ~= 'vulnerability data funnel'",
     'long_description': '# vunnel\n\nA tool for fetching, transforming, and storing vulnerability data from a variety of sources.\n\n![vunnel-demo](https://user-images.githubusercontent.com/590471/226942827-e19742ef-e66e-4e11-8f9b-fb74c40f1dee.gif)\n\nSupported data sources:\n- Alpine (https://secdb.alpinelinux.org)\n- Amazon (https://alas.aws.amazon.com/AL2/alas.rss & https://alas.aws.amazon.com/AL2022/alas.rss)\n- Debian (https://security-tracker.debian.org/tracker/data/json & https://salsa.debian.org/security-tracker-team/security-tracker/raw/master/data/DSA/list)\n- GitHub Security Advisories (https://api.github.com/graphql)\n- NVD (https://services.nvd.nist.gov/rest/json/cves/2.0)\n- Oracle (https://linux.oracle.com/security/oval)\n- RedHat (https://www.redhat.com/security/data/oval)\n- SLES (https://ftp.suse.com/pub/projects/security/oval)\n- Ubuntu (https://launchpad.net/ubuntu-cve-tracker)\n- Wolfi (https://packages.wolfi.dev)\n\n\n## Installation\n\nWith pip:\n\n```bash\npip install vunnel\n```\n\nWith docker:\n\n```bash\ndocker run \\\n  --rm -it \\\n  -v $(pwd)/data:/data \\\n  -v $(pwd)/.vunnel.yaml:/.vunnel.yaml \\\n    ghcr.io/anchore/vunnel:latest  \\\n      run nvd\n```\nWhere:\n  - the `data` volume keeps the processed data on the host\n  - the `.vunnel.yaml` uses the host application config (if present)\n  - you can swap `latest` for a specific version (same as the git tags)\n\nSee [the vunnel package](https://github.com/anchore/vunnel/pkgs/container/vunnel) for a full listing of available tags.\n\n\n## Getting Started\n\nList the available vulnerability data providers:\n\n```\n$ vunnel list\n\nalpine\namazon\ncentos\ndebian\ngithub\nnvd\noracle\nrhel\nsles\nubuntu\nwolfi\n```\n\nDownload and process a provider:\n\n```\n$ vunnel run wolfi\n\n2023-01-04 13:42:58 root [INFO] running wolfi provider\n2023-01-04 13:42:58 wolfi [INFO] downloading Wolfi secdb https://packages.wolfi.dev/os/security.json\n2023-01-04 13:42:59 wolfi [INFO] wrote 56 entries\n2023-01-04 13:42:59 wolfi [INFO] recording workspace state\n```\n\nYou will see the processed vulnerability data in the local `./data` directory\n\n```\n$ tree data\n\ndata\n└── wolfi\n    ├── checksums\n    ├── metadata.json\n    ├── input\n    │   └── secdb\n    │       └── os\n    │           └── security.json\n    └── results\n        └── wolfi:rolling\n            ├── CVE-2016-2781.json\n            ├── CVE-2017-8806.json\n            ├── CVE-2018-1000156.json\n            └── ...\n```\n\n*Note: to get more verbose output, use `-v`, `-vv`, or `-vvv` (e.g. `vunnel -vv run wolfi`)*\n\nDelete existing input and result data for one or more providers:\n\n```\n$ vunnel clear wolfi\n\n2023-01-04 13:48:31 root [INFO] clearing wolfi provider state\n```\n\nExample config file for changing application behavior:\n\n```yaml\n# .vunnel.yaml\nroot: ./processed-data\n\nlog:\n  level: trace\n\nproviders:\n  wolfi:\n    request_timeout: 125\n    runtime:\n      existing_input: keep\n      existing_results: delete-before-write\n      on_error:\n        action: fail\n        input: keep\n        results: keep\n        retry_count: 3\n        retry_delay: 10\n\n```\n\nUse `vunnel config` to get a better idea of all of the possible configuration options.\n\n\n## FAQ\n\n\n### Can I implement a new provider?\n\nYes you can! See [the provider docs](https://github.com/anchore/vunnel/blob/main/DEVELOPING.md#adding-a-new-provider) for more information.\n\n\n### Why is it called "vunnel"?\n\nThis tool "funnels" vulnerability data into a single spot for easy processing... say "vulnerability data funnel" 100x fast enough and eventually it\'ll slur to "vunnel" :).\n',
     'author': 'Alex Goodman',
     'author_email': 'alex.goodman@anchore.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/anchore/vunnel',
```

### Comparing `vunnel-0.8.1/PKG-INFO` & `vunnel-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vunnel
-Version: 0.8.1
+Version: 0.9.0
 Summary: vunnel ~= 'vulnerability data funnel'
 Home-page: https://github.com/anchore/vunnel
 License: Apache-2.0
 Keywords: vulnerability,data,aggregator,grype,vulnerability-data
 Author: Alex Goodman
 Author-email: alex.goodman@anchore.com
 Requires-Python: >=3.9,<4.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: PyYAML (>=5.4.1,<6.0)
-Requires-Dist: SQLAlchemy (>=1.4.46,<2.0.0)
+Requires-Dist: SQLAlchemy (>=1.4.46,<3.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: cvss (>=2.6,<3.0)
 Requires-Dist: dataclass-wizard (>=0.22.2,<0.23.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: future (>=0.18.3,<0.19.0)
 Requires-Dist: ijson (>=2.5.1,<3.0)
```

