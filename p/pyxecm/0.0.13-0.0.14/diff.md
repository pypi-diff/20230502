# Comparing `tmp/pyxecm-0.0.13.tar.gz` & `tmp/pyxecm-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-0.0.13.tar", last modified: Tue May  2 08:20:56 2023, max compression
+gzip compressed data, was "pyxecm-0.0.14.tar", last modified: Tue May  2 14:51:12 2023, max compression
```

## Comparing `pyxecm-0.0.13.tar` & `pyxecm-0.0.14.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:20:56.847102 pyxecm-0.0.13/
--rw-rw-rw-   0 root         (0) root         (0)    11360 2023-05-02 08:20:38.000000 pyxecm-0.0.13/LICENSE
--rw-r--r--   0 root         (0) root         (0)      870 2023-05-02 08:20:56.846102 pyxecm-0.0.13/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-02 08:20:38.000000 pyxecm-0.0.13/README.md
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-05-02 08:20:45.000000 pyxecm-0.0.13/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:20:56.844102 pyxecm-0.0.13/pyxecm/
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-02 08:20:38.000000 pyxecm-0.0.13/pyxecm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28270 2023-05-02 08:20:38.000000 pyxecm-0.0.13/pyxecm/k8s.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2023-05-02 08:20:38.000000 pyxecm-0.0.13/pyxecm/otac.py
--rw-rw-rw-   0 root         (0) root         (0)   219758 2023-05-02 08:20:38.000000 pyxecm-0.0.13/pyxecm/otcs.py
--rw-rw-rw-   0 root         (0) root         (0)   115022 2023-05-02 08:20:38.000000 pyxecm-0.0.13/pyxecm/otds.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-05-02 08:20:38.000000 pyxecm-0.0.13/pyxecm/otiv.py
--rw-rw-rw-   0 root         (0) root         (0)    10226 2023-05-02 08:20:38.000000 pyxecm-0.0.13/pyxecm/otpd.py
--rw-rw-rw-   0 root         (0) root         (0)   224230 2023-05-02 08:20:38.000000 pyxecm-0.0.13/pyxecm/payload.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2023-05-02 08:20:38.000000 pyxecm-0.0.13/pyxecm/translate.py
--rw-rw-rw-   0 root         (0) root         (0)     2695 2023-05-02 08:20:38.000000 pyxecm-0.0.13/pyxecm/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:20:56.846102 pyxecm-0.0.13/pyxecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      870 2023-05-02 08:20:56.000000 pyxecm-0.0.13/pyxecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-02 08:20:56.000000 pyxecm-0.0.13/pyxecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 08:20:56.000000 pyxecm-0.0.13/pyxecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-02 08:20:56.000000 pyxecm-0.0.13/pyxecm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-02 08:20:56.000000 pyxecm-0.0.13/pyxecm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 08:20:56.847102 pyxecm-0.0.13/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-02 08:20:38.000000 pyxecm-0.0.13/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:51:12.800557 pyxecm-0.0.14/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-05-02 14:50:53.000000 pyxecm-0.0.14/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      870 2023-05-02 14:51:12.800557 pyxecm-0.0.14/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-02 14:50:53.000000 pyxecm-0.0.14/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-05-02 14:51:02.000000 pyxecm-0.0.14/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:51:12.798557 pyxecm-0.0.14/pyxecm/
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28270 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)    69124 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/m365.py
+-rw-rw-rw-   0 root         (0) root         (0)    49931 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/otac.py
+-rw-rw-rw-   0 root         (0) root         (0)   219914 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)   115012 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/otds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)    10224 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/otpd.py
+-rw-rw-rw-   0 root         (0) root         (0)   226140 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/payload.py
+-rw-rw-rw-   0 root         (0) root         (0)     5987 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/sap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/translate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2695 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:51:12.799557 pyxecm-0.0.14/pyxecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      870 2023-05-02 14:51:12.000000 pyxecm-0.0.14/pyxecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      394 2023-05-02 14:51:12.000000 pyxecm-0.0.14/pyxecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 14:51:12.000000 pyxecm-0.0.14/pyxecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-02 14:51:12.000000 pyxecm-0.0.14/pyxecm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-02 14:51:12.000000 pyxecm-0.0.14/pyxecm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 14:51:12.800557 pyxecm-0.0.14/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-02 14:50:53.000000 pyxecm-0.0.14/setup.py
```

### Comparing `pyxecm-0.0.13/LICENSE` & `pyxecm-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.13/PKG-INFO` & `pyxecm-0.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.13
+Version: 0.0.14
 Summary: A library to connect to Opentext Extended ECM
 Home-page: https://pypi.org/project/pyxecm/
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://github.com/opentext/pyxecm
 Keywords: opentext extendedecm contentserver otds appworks archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyxecm-0.0.13/pyproject.toml` & `pyxecm-0.0.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [project]
   classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
   dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "python-hcl2", "zipfile36"]
   description = "A library to connect to Opentext Extended ECM"
   name = "pyxecm"
   readme = "README.md"
   requires-python = ">=3.10"
-  version = "0.0.13"
+  version = "0.0.14"
 
   [[project.authors]]
     email = "kgatzweiler@opentext.com"
     name = "Kai Gatzweiler"
 
   [[project.authors]]
     email = "mdiefenb@opentext.com"
```

### Comparing `pyxecm-0.0.13/pyxecm/k8s.py` & `pyxecm-0.0.14/pyxecm/k8s.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.13/pyxecm/otac.py` & `pyxecm-0.0.14/pyxecm/otac.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.13/pyxecm/otcs.py` & `pyxecm-0.0.14/pyxecm/otcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,14 +377,17 @@
 
             Content Server may produce corrupt response when it gets restarted
             or hitting resource limits. So we try to avoid a fatal error and bail
             out more gracefully.
 
         Args:
             response_object (object): this is reponse object delivered by the request call
+            additional_error_message (string): print a custom error message
+            show_error (boolean): if True log an error, if False log a warning
+
         Return: a python dict object or null in case of an error
         """
 
         if not response_object:
             return None
 
         try:
```

### Comparing `pyxecm-0.0.13/pyxecm/otds.py` & `pyxecm-0.0.14/pyxecm/otds.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,20 +232,19 @@
         response_object: object,
         additional_error_message: str = "",
         show_error: bool = True,
     ) -> dict:
         """Converts the request response to a Python dict in a safe way
            that also handles exceptions.
 
-            Content Server may produce corrupt response when it gets restarted
-            or hitting resource limits. So we try to avoid a fatal error and bail
-            out more gracefully.
-
         Args:
             response_object (object): this is reponse object delivered by the request call
+            additional_error_message (string): print a custom error message
+            show_error (boolean): if True log an error, if False log a warning
+
         Return: a python dict object or null in case of an error
         """
 
         if not response_object:
             return None
 
         try:
@@ -261,14 +260,16 @@
                 logger.error(message)
             else:
                 logger.warning(message)
             return None
         else:
             return dict_object
 
+    # end method definition
+
     def authenticate(self, revalidate: bool = False):
         """Authenticate at Directory Services and retrieve OTCS Ticket.
 
         Args:
             revalidate (bool): determine if a re-athentication is enforced
                                (e.g. if session has timed out with 401 error)
         Return: Cookie information. Also stores cookie information in self._cookie
```

### Comparing `pyxecm-0.0.13/pyxecm/otiv.py` & `pyxecm-0.0.14/pyxecm/otiv.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.13/pyxecm/otpd.py` & `pyxecm-0.0.14/pyxecm/otpd.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,49 +125,50 @@
 
     def restUrl(self):
         return self.config()["restUrl"]
 
     def parseRequestResponse(
         self,
         response_object: object,
-        additionalErrorMessage: str = "",
-        showError: bool = True,
+        additional_error_message: str = "",
+        show_error: bool = True,
     ) -> dict:
         """Converts the request response to a Python dict in a safe way
            that also handles exceptions.
 
-            Content Server may produce corrupt response when it gets restarted
-            or hitting resource limits. So we try to avoid a fatal error and bail
-            out more gracefully.
-
         Args:
             response_object (object): this is reponse object delivered by the request call
+            additional_error_message (string): print a custom error message
+            show_error (boolean): if True log an error, if False log a warning
+
         Return: a python dict object or null in case of an error
         """
 
         if not response_object:
             return None
 
         try:
             dict_object = json.loads(response_object.text)
         except json.JSONDecodeError as e:
-            if additionalErrorMessage:
+            if additional_error_message:
                 message = "Cannot decode response as JSon. {}; error -> {}".format(
-                    additionalErrorMessage, e
+                    additional_error_message, e
                 )
             else:
                 message = "Cannot decode response as JSon; error -> {}".format(e)
-            if showError:
+            if show_error:
                 logger.error(message)
             else:
                 logger.warning(message)
             return None
         else:
             return dict_object
 
+    # end method definition
+
     def importDatabase(self, filename):
         """Import PowerDocs database backup from a zip file"""
 
         file = filename.split("/")[-1]
         file_tup = (file, open(filename, "rb"), "application/zip")
 
         # fields attribute is set according to the other party's interface description
```

### Comparing `pyxecm-0.0.13/pyxecm/payload.py` & `pyxecm-0.0.14/pyxecm/payload.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,25 +90,19 @@
 import logging
 import yaml
 import hcl2
 import re
 
 from urllib.parse import urlparse
 
-
-logger = logging.getLogger(os.path.basename(__file__))
-
 # OpenText specific modules:
-from pyxecm import web
-
-try:
-  from pyxecm import sap
-except ImportError as e:
-  logger.error(f"Loading SAP failed -> {e}")  
+import pyxecm.web as web
+import pyxecm.sap as sap
 
+logger = logging.getLogger(os.path.basename(__file__))
 
 
 class Payload(object):
     """Used to process Terrarium payload."""
 
     # _debug controls whether or not transport processing is
     # stopped if one transport fails:
@@ -1086,46 +1080,46 @@
                 continue
 
             # Check if the group does already exist (e.g. if job is restarted)
             # as this is a pattern search it could return multiple groups:
             existing_groups = self._m365.getGroup(group_name)
             if existing_groups and existing_groups["value"]:
                 logger.debug(
-                    "Found existing Azure AD groups -> {}".format(existing_groups["value"]))
+                    "Found existing Microsoft 365 groups -> {}".format(existing_groups["value"]))
                 # Get list of all matching groups:
                 existing_groups_list = existing_groups["value"]
                 # Find the group with the exact match of the name:
                 existing_group = next(
                     (item for item in existing_groups_list if item["displayName"] == group_name),
                     None,
                 )
                 # Have we found an exact match?
                 if existing_group is not None:
                     logger.info(
-                        "Found existing Azure AD group -> {} ({}) - skip creation of group...".format(
+                        "Found existing Microsoft 365 group -> {} ({}) - skip creation of group...".format(
                             existing_group["displayName"], existing_group["id"]
                         )
                     )
                     group["m365_id"] = existing_group["id"]
                     continue
                 else:
                     logger.info(
-                        "Did not find an exact match for the group - creating a new Azure AD group..."
+                        "Did not find an exact match for the group - creating a new Microsoft 365 group..."
                     )
             else:
                 logger.info(
-                    "Did not find any matching group - creating a new Azure AD group...")
+                    "Did not find any matching group - creating a new Microsoft 365 group...")
 
             # Now we know it is a new group...
             new_group = self._m365.addGroup(group_name)
             if new_group is not None:
                 # Store the Microsoft 365 group ID in payload:
                 group["m365_id"] = new_group["id"]
                 logger.info(
-                    "New Azure AD group -> {} with ID -> {} has been created".format(
+                    "New Microsoft 365 group -> {} with ID -> {} has been created".format(
                         group_name, group["m365_id"]
                     )
                 )
 
         # end method definition
 
     def processUsers(self):
@@ -1346,72 +1340,97 @@
                 )
                 continue
             user_password = user["password"]
             # be careful with the following fields - they could be empty
             user_department = user.get("base_group", "")
             user_first_name = user.get("firstname", "")
             user_last_name = user.get("lastname", "")
+            user_location = user.get("location", "US")
 
             # Check if the user does already exist (e.g. if job is restarted)
             # As this is a pattern search it could return multiple users:
             user_name = user_name + "@" + self._m365.config()["domain"]
             existing_user = self._m365.getUser(user_name)
             if existing_user:
                 logger.info(
-                    "Found existing Azure AD user -> {} ({}) with ID -> {}".format(
+                    "Found existing Microsoft 365 user -> {} ({}) with ID -> {}".format(
                         existing_user["displayName"], existing_user["userPrincipalName"], existing_user["id"]
                     )
                 )
                 user["m365_id"] = existing_user["id"]
             else:
                 logger.info(
-                    "Did not find existing user - creating a new Azure AD user...")
+                    "Did not find existing user - creating a new Microsoft 365 user...")
 
                 # Now we know it is a new user...
                 new_user = self._m365.addUser(email=user_name,
                                               password=user_password,
                                               first_name=user_first_name,
                                               last_name=user_last_name,
-                                              location="US",
+                                              location=user_location,
                                               department=user_department)
                 if new_user is not None:
                     # Store the Microsoft 365 user ID in payload:
                     user["m365_id"] = new_user["id"]
                     logger.info(
-                        "New Azure AD user -> {} with ID -> {} has been created".format(
+                        "New Microsoft 365 user -> {} with ID -> {} has been created".format(
                             user_name, user["m365_id"]
                         )
                     )
                 else:
                     logger.error(
-                        "Failed to create new Azure AD user -> {}".format(user_name))
+                        "Failed to create new Microsoft 365 user -> {}".format(user_name))
                     continue
 
-            # Now we assign a license to the new Azure AD user:
-            sku_id = self._m365.config()["skuId"]
-            if sku_id and not "m365_sku" in user:
-                response = self._m365.assignLicenseToUser(
-                    user["m365_id"], sku_id)
-                if not response:
-                    logger.error(
-                        "Failed to assign license -> {} to Azure AD user -> {}".format(sku_id, user_name))
+            # Now we assign a license to the new M365 user.
+            # First we see if there's a specific M365 SKU in user
+            # payload - if not we use the default SKU configured
+            # for the m365 object:
+            sku_id = user.get("m365_sku", self._m365.config()["skuId"])
+            if sku_id:
+                # Check if the M365 user already has this license:
+                existing_user_licenses = self._m365.getUserLicenses(user["m365_id"])
+                if not self._m365.existResultItem(existing_user_licenses, "skuId", sku_id):
+                    response = self._m365.assignLicenseToUser(
+                        user["m365_id"], sku_id)
+                    if not response:
+                        logger.error(
+                            "Failed to assign license -> {} to Microsoft 365 user -> {}".format(sku_id, user_name))
+                    else:
+                        user["m365_sku"] = sku_id
+                        logger.info(
+                            "License -> {} has been assigned to Microsoft 365 user -> {}".format(sku_id, user_name))
                 else:
-                    user["m365_sku"] = sku_id
                     logger.info(
-                        "License -> {} has been assigned to Azure AD user -> {}".format(sku_id, user_name))
+                        "Microsoft 365 user -> {} already has the license -> {}".format(user_name, sku_id))
+
+            # Now we assign the Extended ECM Teams App to the new M365 user.
+            # First we check if the app is already assigned to the user.
+            # If not we install / assign the app. If the user already has
+            # the Extended ECM app we try to uprade it:
+            app_name = self._m365.config()["teamsAppName"]
+            response = self._m365.getTeamsAppsOfUser(user["m365_id"], "contains(teamsAppDefinition/displayName, '{}')".format(app_name))
+            if self._m365.existResultItem(response, "displayName", app_name, sub_dict_name="teamsAppDefinition"):
+                logger.info(
+                    "Upgrade MS Teams app -> {} for user -> {}".format(app_name, user_name))
+                response = self._m365.upgradeTeamsAppOfUser(user["m365_id"], app_name)
+            else:
+                logger.info(
+                    "Install MS Teams app -> {} for user -> {}".format(app_name, user_name))
+                response = self._m365.assignTeamsAppToUser(user["m365_id"], app_name)
 
             # Process Microsoft 365 group memberships of new user:
             if "m365_id" in user:
                 user_id = user["m365_id"]
                 # don't forget the base group (department) !
                 group_names = user["groups"]
                 if user_department:
                     group_names.append(user_department)
                 logger.info(
-                    "User -> {} has these groups in payload -> {} (including base group -> {}). Checking if they are Azure AD Groups...".format(user_name, group_names, user_department))
+                    "User -> {} has these groups in payload -> {} (including base group -> {}). Checking if they are Microsoft 365 Groups...".format(user_name, group_names, user_department))
                 for group_name in group_names:
 
                     # Find the group dictionary item to the parent group name:
                     group = next(
                         (item for item in self._groups if item["name"]
                          == group_name), None
                     )
@@ -1424,39 +1443,39 @@
                             "Payload Group -> {} is not enabled for M365. Skipping...".format(
                                 group_name)
                         )
                     else:
                         response = self._m365.getGroup(group_name)
                         if response is None or not "value" in response or not response["value"]:
                             logger.error(
-                                "Azure AD Group -> {} not found. Skipping...".format(
+                                "Microsoft 365 Group -> {} not found. Skipping...".format(
                                     group_name)
                             )
                         else:
                             group_id = response["value"][0]["id"]
 
                             # Check if user is already a member. We don't want
                             # to throw an error if the user is not found as a member:
                             if self._m365.isMember(group_id, user_id, show_error=False):
                                 logger.info(
-                                    "Azure AD user -> {} ({}) is already in Azure AD group -> {} ({})".format(
+                                    "Microsoft 365 user -> {} ({}) is already in Microsoft 365 group -> {} ({})".format(
                                         user["name"], user_id, group_name, group_id
                                     ))
                             else:
                                 logger.info(
-                                    "Add Azure AD user -> {} ({}) to Azure AD group -> {} ({})".format(
+                                    "Add Microsoft 365 user -> {} ({}) to Microsoft 365 group -> {} ({})".format(
                                         user["name"], user_id, group_name, group_id
                                     )
                                 )
                                 self._m365.addGroupMember(group_id, user_id)
                                 # As each group should have at least one owner in M365
                                 # we set all users also as owners for now. Later we
                                 # may want to configure this via payload:
                                 logger.info(
-                                    "Make Azure AD user -> {} ({}) owner of Azure AD group -> {} ({})".format(
+                                    "Make Microsoft 365 user -> {} ({}) owner of Microsoft 365 group -> {} ({})".format(
                                         user["name"], user_id, group_name, group_id
                                     )
                                 )
                                 self._m365.addGroupOwner(group_id, user_id)
 
                     # As M365 groups are flat (not nested) we also add the
                     # user as member to the parent groups of the current group:
@@ -1478,31 +1497,31 @@
                                     group_name)
                             )
                             continue
 
                         response = self._m365.getGroup(parent_group_name)
                         if response is None or not "value" in response or not response["value"]:
                             logger.error(
-                                "Azure AD Group -> {} not found. Skipping...".format(
+                                "Microsoft 365 Group -> {} not found. Skipping...".format(
                                     group_name)
                             )
                             continue
                         parent_group_id = response["value"][0]["id"]
 
                         # Check if user is already a member. We don't want
                         # to throw an error if the user is not found as a member:
                         if self._m365.isMember(parent_group_id, user_id, show_error=False):
                             logger.info(
-                                "Azure AD user -> {} ({}) is already in Azure AD group -> {} ({})".format(
+                                "Microsoft 365 user -> {} ({}) is already in Microsoft 365 group -> {} ({})".format(
                                     user["name"], user_id, parent_group_name, parent_group_id
                                 ))
                             continue
 
                         logger.info(
-                            "Add Azure AD user -> {} ({}) to Azure AD group -> {} ({})".format(
+                            "Add Microsoft 365 user -> {} ({}) to Microsoft 365 group -> {} ({})".format(
                                 user["name"], user_id, parent_group_name, parent_group_id
                             )
                         )
                         self._m365.addGroupMember(parent_group_id, user_id)
 
         # end method definition
 
@@ -2063,15 +2082,15 @@
         else:
             logger.info(
                 "Successfully added photo for admin")
 
         # end method definition
 
     def processUserPhotosM365(self):
-        """Process user photos in payload and assign them to Azure AD users.
+        """Process user photos in payload and assign them to Microsoft 365 users.
 
         Args: None
         Return: None
         """
 
         # we assume the nickname of the photo item equals the login name of the user
         # we also assume that the photos have been uploaded / transported into the target system
@@ -2080,15 +2099,14 @@
             if not "id" in user:
                 logger.error(
                     "User -> {} does not have an ID. The user creation may have failed before. Skipping...".format(
                         user_name
                     )
                 )
                 continue
-            user_id = user["id"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
                 logger.info(
                     "Payload for User -> {} is disabled. Skipping...".format(
                         user_name)
@@ -2105,14 +2123,18 @@
                     "Office 365 user -> {} has not been created. Skipping...".format(
                         user_name)
                 )
                 continue
 
             user_m365_id = user["m365_id"]
 
+            if self._m365.getUserPhoto(user_m365_id):
+                logger.info("User -> {} ({}) has already a photo in Microsoft 365. Skipping...".format(user_name, user_m365_id))
+                continue
+
             response = self._otcs.getNodeFromNickname(user_name)
             if response == None:
                 logger.warning(
                     "Missing photo for user -> {} - nickname not found. Skipping...".format(
                         user_name
                     )
                 )
@@ -5034,10 +5056,8 @@
     def getOTDS(self) -> object:
         return self._otds
 
     def getK8S(self) -> object:
         return self._k8s
 
     def getM365(self) -> object:
-        return self._m365
-
-
+        return self._m365
```

### Comparing `pyxecm-0.0.13/pyxecm/translate.py` & `pyxecm-0.0.14/pyxecm/translate.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.13/pyxecm/web.py` & `pyxecm-0.0.14/pyxecm/web.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.13/pyxecm.egg-info/PKG-INFO` & `pyxecm-0.0.14/pyxecm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.13
+Version: 0.0.14
 Summary: A library to connect to Opentext Extended ECM
 Home-page: https://pypi.org/project/pyxecm/
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://github.com/opentext/pyxecm
 Keywords: opentext extendedecm contentserver otds appworks archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

