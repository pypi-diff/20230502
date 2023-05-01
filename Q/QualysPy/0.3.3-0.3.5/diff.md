# Comparing `tmp/qualyspy-0.3.3.tar.gz` & `tmp/qualyspy-0.3.5.tar.gz`

## Comparing `qualyspy-0.3.3.tar` & `qualyspy-0.3.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.3.3/.vscode/launch.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.3.3/.vscode/settings.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.3.3/.vscode/tasks.json
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.3.3/debug/build.sh
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.3/debug/dtd.txt
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.3/debug/output.txt
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.3/debug/parse_dtd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.3/debug/quickscan.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.3/debug/remove_cookies.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 qualyspy-0.3.3/debug/test.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.3.3/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.3.3/docs/make.bat
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.3.3/docs/source/conf.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.3.3/docs/source/index.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.3/docs/source/modules.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.3/docs/source/qualyspy.assets.host_list.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.3.3/docs/source/qualyspy.assets.host_list_detection.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.3.3/docs/source/qualyspy.qualysapi.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.3/docs/source/qualyspy.qutils.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.3.3/docs/source/qualyspy.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.3.3/docs/source/qualyspy.scan_configuration.knowledgebase.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/__init__.py
--rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/qualysapi.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/qutils.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/urls.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/asset_mgmt_tagging/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/asset_mgmt_tagging/api_input.py
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/asset_mgmt_tagging/asset.py
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/asset_mgmt_tagging/tag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/assets/__init__.py
--rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/assets/host_list.py
--rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/assets/host_list_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/certview/__init__.py
--rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/certview/certificate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/scan_configuration/__init__.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.3/qualyspy/scan_configuration/knowledgebase.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.3/requirements/deploy.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.3.3/requirements/dev.txt
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.3.3/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.3/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.3.3/README.md
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.3.5/.vscode/launch.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.3.5/.vscode/settings.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.3.5/.vscode/tasks.json
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/build.sh
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/dtd.txt
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/output.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/parse_dtd.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/quickscan.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/remove_cookies.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/test.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/make.bat
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/conf.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/index.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/modules.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/qualyspy.assets.host_list.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/qualyspy.assets.host_list_detection.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/qualyspy.qualysapi.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/qualyspy.qutils.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/qualyspy.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/qualyspy.scan_configuration.knowledgebase.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/__init__.py
+-rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/qualysapi.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/qutils.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/urls.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/api_input.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/asset.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/tag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/assets/__init__.py
+-rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/assets/host_list.py
+-rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/assets/host_list_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/certview/__init__.py
+-rw-r--r--   0        0        0    14938 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/certview/certificate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/scan_configuration/__init__.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/scan_configuration/knowledgebase.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.5/requirements/deploy.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.3.5/requirements/dev.txt
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.5/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.3.5/README.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.3.5/PKG-INFO
```

### Comparing `qualyspy-0.3.3/.vscode/launch.json` & `qualyspy-0.3.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/debug/dtd.txt` & `qualyspy-0.3.5/debug/dtd.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/debug/output.txt` & `qualyspy-0.3.5/debug/output.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/debug/parse_dtd.py` & `qualyspy-0.3.5/debug/parse_dtd.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/debug/quickscan.py` & `qualyspy-0.3.5/debug/quickscan.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/debug/remove_cookies.py` & `qualyspy-0.3.5/debug/remove_cookies.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/docs/Makefile` & `qualyspy-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/docs/make.bat` & `qualyspy-0.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/docs/source/conf.py` & `qualyspy-0.3.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/qualyspy/qualysapi.py` & `qualyspy-0.3.5/qualyspy/qualysapi.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/qualyspy/qutils.py` & `qualyspy-0.3.5/qualyspy/qutils.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/qualyspy/urls.json` & `qualyspy-0.3.5/qualyspy/urls.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/qualyspy/asset_mgmt_tagging/api_input.py` & `qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/api_input.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/qualyspy/asset_mgmt_tagging/asset.py` & `qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/asset.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/qualyspy/asset_mgmt_tagging/tag.py` & `qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 class Tag_Simple_Q_List(pyd.BaseModel):
     count: int | None
     list_: list[dict[str, Tag_Simple]] | None = pyd.Field(None, alias="list")
     set: dict[str, list[Tag_Simple]] | None
     add: dict[str, list[Tag_Simple]] | None
     remove: dict[str, list[Tag_Simple]] | None
-    upydate: dict[str, list[Tag_Simple]] | None
+    update: dict[str, list[Tag_Simple]] | None
 
     class Config:
         orm_mode = True
 
 
 ####################################################################################################
 # Tag
@@ -135,14 +135,23 @@
 
 class Update_Tag:
     def __init__(self, conn: qualysapi.Connection, tag: Tag) -> None:
         self.conn = conn
         self.tag = tag
 
     def __call__(self, input: Tag) -> Response:
+        tag_list_types = ["list_", "set", "add", "remove", "update"]
+        for tag_list_type in tag_list_types:
+            if getattr(input.children, tag_list_type) is not None:
+                for tag in getattr(input.children, tag_list_type)["TagSimple"]:
+                    if getattr(tag, "id", None) is None:
+                        raise ValueError(
+                            f"Tag ID must be specified for each tag in {tag_list_type} tag list."
+                        )
+
         data = {"ServiceRequest": {"data": {"Tag": input.dict(exclude_unset=True)}}}
         r = self.conn.post(qutils.URLS["Update Tag"] + f"/{self.tag.id}", data=data)
         response = parse_response(r)
 
         return response
```

### Comparing `qualyspy-0.3.3/qualyspy/assets/host_list.py` & `qualyspy-0.3.5/qualyspy/assets/host_list.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/qualyspy/assets/host_list_detection.py` & `qualyspy-0.3.5/qualyspy/assets/host_list_detection.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/qualyspy/certview/certificate.py` & `qualyspy-0.3.5/qualyspy/certview/certificate.py`

 * *Files 6% similar despite different names*

```diff
@@ -423,24 +423,14 @@
 
         raw = self.conn.post(qutils.URLS["List CertView Certificates"], input_data)
 
         if len(raw) > 0:
             certificates: list[Certificate] = []
             for cert in raw:
                 c = Certificate.parse_obj(cert)
-
-                # subject.name somtimes includes null characters "\x00", even though the GUI doesn't
-                # show these.  I've opened a ticket with Qualys about it.  In the meanwhile, this
-                # will replace them with something PostgreSQL is happy with.
-                # Also other fields, apparently...
-                #
-                c.subject.name = c.subject.name.replace("\x00", "\uFFFD")
-                c.subject.locality = c.subject.locality.replace("\x00", "\uFFFD")
-                c.subject.state = c.subject.state.replace("\x00", "\uFFFD")
-
                 certificates.append(c)
             return certificates
         else:
             return None
 
     def __call__(
         self,
```

### Comparing `qualyspy-0.3.3/qualyspy/scan_configuration/knowledgebase.py` & `qualyspy-0.3.5/qualyspy/scan_configuration/knowledgebase.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/.gitignore` & `qualyspy-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/LICENSE` & `qualyspy-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.3/pyproject.toml` & `qualyspy-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "QualysPy"
-version = "0.3.3"
+version = "0.3.5"
 authors = [
   { name="Jordan Barnartt", email="jbarnart@uwaterloo.ca" },
 ]
 description = "A Python wrapper for the Qualys API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `qualyspy-0.3.3/PKG-INFO` & `qualyspy-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QualysPy
-Version: 0.3.3
+Version: 0.3.5
 Summary: A Python wrapper for the Qualys API.
 Project-URL: Homepage, https://github.com/JordanBarnartt/qualyspy
 Project-URL: Bug Tracker, https://github.com/JordanBarnartt/qualyspy/issues
 Author-email: Jordan Barnartt <jbarnart@uwaterloo.ca>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

