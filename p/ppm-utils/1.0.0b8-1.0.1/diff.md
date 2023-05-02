# Comparing `tmp/ppm-utils-1.0.0b8.tar.gz` & `tmp/ppm-utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ppm-utils-1.0.0b8.tar", last modified: Wed Jun 30 10:25:10 2021, max compression
+gzip compressed data, was "ppm-utils-1.0.1.tar", last modified: Tue May  2 15:30:51 2023, max compression
```

## Comparing `ppm-utils-1.0.0b8.tar` & `ppm-utils-1.0.1.tar`

### file list

```diff
@@ -1,54 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 10:25:10.000000 ppm-utils-1.0.0b8/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 10:25:10.000000 ppm-utils-1.0.0b8/ppmutils/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 10:25:10.000000 ppm-utils-1.0.0b8/ppmutils/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 10:25:10.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/user_queued_notification.html
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/admin_contact_notification.html
--rw-r--r--   0 runner    (1001) docker     (121)     2691 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/user_accepted_notification.html
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/user_queued_notification.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/admin_proposed_notification.html
--rw-r--r--   0 runner    (1001) docker     (121)      842 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/user_pending_notification.txt
--rw-r--r--   0 runner    (1001) docker     (121)      812 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/user_proposed_notification.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/admin_contact_notification.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10594 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/_base.html
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/user_accepted_notification.txt
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/admin_proposed_notification.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2220 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/user_proposed_notification.html
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/user_pending_notification.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 10:25:10.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/neer/
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/neer/user_queued_notification.html
--rw-r--r--   0 runner    (1001) docker     (121)     2249 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/templates/ppmutils/neer/user_queued_notification.txt
--rw-r--r--   0 runner    (1001) docker     (121)   259750 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/fhir.py
--rw-r--r--   0 runner    (1001) docker     (121)    74570 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/ppm.py
--rw-r--r--   0 runner    (1001) docker     (121)    28462 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/p2md.py
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/participants.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-06-30 10:25:08.000000 ppm-utils-1.0.0b8/ppmutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18251 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/picnichealth.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 10:25:10.000000 ppm-utils-1.0.0b8/ppmutils/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6185 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/tests/test_ppm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/tests/runtests.py
--rw-r--r--   0 runner    (1001) docker     (121)    59788 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/tests/test_fhir.py
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)    11011 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     9294 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     3904 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 10:25:10.000000 ppm-utils-1.0.0b8/ppmutils/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    53711 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/qualtrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/api.py
--rw-r--r--   0 runner    (1001) docker     (121)   184653 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/ppmutils/sfhir.py
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-06-30 10:24:30.000000 ppm-utils-1.0.0b8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 10:25:10.000000 ppm-utils-1.0.0b8/ppm_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-06-30 10:25:09.000000 ppm-utils-1.0.0b8/ppm_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-30 10:25:09.000000 ppm-utils-1.0.0b8/ppm_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-06-30 10:25:09.000000 ppm-utils-1.0.0b8/ppm_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2021-06-30 10:25:10.000000 ppm-utils-1.0.0b8/ppm_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2021-06-30 10:25:09.000000 ppm-utils-1.0.0b8/ppm_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-06-30 10:25:10.000000 ppm-utils-1.0.0b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2021-06-30 10:25:10.000000 ppm-utils-1.0.0b8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:30:51.566265 ppm-utils-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-02 15:30:51.566265 ppm-utils-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:30:51.566265 ppm-utils-1.0.1/ppm_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-02 15:30:51.000000 ppm-utils-1.0.1/ppm_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-02 15:30:51.000000 ppm-utils-1.0.1/ppm_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:30:51.000000 ppm-utils-1.0.1/ppm_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 15:30:51.000000 ppm-utils-1.0.1/ppm_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 15:30:51.000000 ppm-utils-1.0.1/ppm_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:30:51.566265 ppm-utils-1.0.1/ppmutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-02 15:30:49.000000 ppm-utils-1.0.1/ppmutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/ppmutils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)   284352 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/ppmutils/fhir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34310 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/ppmutils/p2md.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65188 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/ppmutils/ppm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50047 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/ppmutils/qualtrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:30:51.566265 ppm-utils-1.0.1/ppmutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/ppmutils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/ppmutils/tests/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59783 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/ppmutils/tests/test_fhir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/ppmutils/tests/test_ppm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-02 15:30:51.566265 ppm-utils-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-02 15:30:22.000000 ppm-utils-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ppm-utils-1.0.0b8/README.md` & `ppm-utils-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ppm-utils-1.0.0b8/ppmutils/fhir.py` & `ppm-utils-1.0.1/ppmutils/fhir.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,30 +25,24 @@
 from fhirclient.models.researchsubject import ResearchSubject
 from fhirclient.models.fhirreference import FHIRReference
 from fhirclient.models.codeableconcept import CodeableConcept
 from fhirclient.models.coding import Coding
 from fhirclient.models.communication import Communication
 from fhirclient.models.device import Device
 from fhirclient.models.resource import Resource
-from fhirclient.models.questionnaire import Questionnaire
 from fhirclient.models.questionnaireresponse import QuestionnaireResponse
 
 from ppmutils.ppm import PPM
-from ppmutils.settings import ppm_settings
 
-# Get the app logger
 import logging
 
-logger = logging.getLogger(ppm_settings.LOGGER_NAME)
+logger = logging.getLogger(__name__)
 
 
-class FHIR(PPM.Service):
-
-    service = "fhir"
-    ppm_settings_url_name = "FHIR_URL"
+class FHIR:
 
     #
     # CONSTANTS
     #
 
     # This is the system used for Patient identifiers based on email
     patient_email_identifier_system = "http://schema.org/email"
@@ -62,16 +56,18 @@
 
     research_study_identifier_system = "https://peoplepoweredmedicine.org/fhir/study"
     research_study_coding_system = "https://peoplepoweredmedicine.org/study"
 
     research_subject_identifier_system = "https://peoplepoweredmedicine.org/fhir/subject"
     research_subject_coding_system = "https://peoplepoweredmedicine.org/subject"
 
+    device_title_system = "https://peoplepoweredmedicine.org/fhir/device/title"
     device_identifier_system = "https://peoplepoweredmedicine.org/fhir/device"
     device_coding_system = "https://peoplepoweredmedicine.org/device"
+    device_study_extension_url = "https://p2m2.dbmi.hms.harvard.edu/fhir/StructureDefinition/study"
 
     # Type system for PPM data documents
     data_document_reference_identifier_system = "https://peoplepoweredmedicine.org/document-type"
 
     # Type system for PPM documents
     ppm_document_reference_type_system = "https://peoplepoweredmedicine.org/fhir/ppm/document-type"
 
@@ -92,14 +88,15 @@
     twitter_extension_url = "https://p2m2.dbmi.hms.harvard.edu/fhir/StructureDefinition/uses-twitter"
     fitbit_extension_url = "https://p2m2.dbmi.hms.harvard.edu/fhir/StructureDefinition/uses-fitbit"
     picnichealth_extension_url = "https://p2m2.dbmi.hms.harvard.edu/fhir/StructureDefinition/registered-picnichealth"
     facebook_extension_url = "https://p2m2.dbmi.hms.harvard.edu/fhir/StructureDefinition/uses-facebook"
     smart_on_fhir_extension_url = "https://p2m2.dbmi.hms.harvard.edu/fhir/StructureDefinition/uses-smart-on-fhir"
     referral_extension_url = "https://p2m2.dbmi.hms.harvard.edu/fhir/StructureDefinition/how-did-you-hear-about-us"
     admin_notified_extension_url = "https://p2m2.dbmi.hms.harvard.edu/fhir/StructureDefinition/admin-notified"
+    procure_extension_url = "https://p2m2.dbmi.hms.harvard.edu/fhir/StructureDefinition/uses-procure"
 
     # Qualtrics IDs
     qualtrics_survey_identifier_system = "https://peoplepoweredmedicine.org/fhir/qualtrics/survey"
     qualtrics_survey_questionnaire_identifier_system = (
         "https://peoplepoweredmedicine.org/fhir/qualtrics/survey/questionnaire"
     )
     qualtrics_survey_version_identifier_system = "https://peoplepoweredmedicine.org/fhir/qualtrics/survey/version"
@@ -109,28 +106,31 @@
     qualtrics_survey_extension_url = "https://p2m2.dbmi.hms.harvard.edu/fhir/StructureDefinition/qualtrics-survey"
 
     #
     # META
     #
 
     @classmethod
-    def service_url(cls):
-        """
-        FHIR uses a more standard URL for everything so use this one instead of
-        the PPM service stripped down one
-        :return: The FHIR URL
-        :rtype: str
+    def default_url_for_env(cls, environment):
         """
+        Give implementing classes an opportunity to list a default set of URLs
+        based on the DBMI_ENV, if specified. Otherwise, return nothing
+        :param environment: The DBMI_ENV string
+        :return: A URL, if any
+        """
+        if "local" in environment:
+            return "http://fhir:8008"
+        elif "dev" in environment:
+            return "https://fhir.ppm.aws.dbmi-dev.hms.harvard.edu"
+        elif "prod" in environment:
+            return "https://fhir.ppm.aws.dbmi.hms.harvard.edu"
+        else:
+            logger.error(f"Could not return a default URL for environment: {environment}")
 
-        # Get from ppm settings
-        if not hasattr(ppm_settings, cls.ppm_settings_url_name):
-            raise SystemError("FHIR URL not defined in settings".format(cls.service.upper()))
-
-        # Get it
-        return getattr(ppm_settings, cls.ppm_settings_url_name)
+        return None
 
     @staticmethod
     def get_client(fhir_url):
 
         # Create the server
         settings = {"app_id": "hms-dbmi-ppm-p2m2-admin", "api_base": fhir_url}
 
@@ -609,61 +609,14 @@
 
             return {"_id": identifier.id}
 
         else:
             raise ValueError("Unhandled instance of a Patient identifier: {}".format(identifier))
 
     @staticmethod
-    def _patient_id(identifier):
-        """
-        Accepts an identifier and returns the actual Patient ID
-        to 'patient'.
-        :param identifier: object
-        :return: str
-        """
-        # Check types
-        if type(identifier) is str and re.match(r"^\d+$", identifier):
-
-            # Likely a FHIR ID
-            return identifier
-
-        # Check for an email address
-        elif type(identifier) is str and re.match(r"(^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$)", identifier):
-
-            # An email address
-            return FHIR.get_ppm_id(identifier)
-
-        # Check for a resource
-        elif type(identifier) is dict and identifier.get("resourceType") == "Patient":
-
-            return identifier["id"]
-
-        # Check for a bundle entry
-        elif type(identifier) is dict and identifier.get("resource", {}).get("resourceType") == "Patient":
-
-            return identifier["resource"]["id"]
-
-        # Check for a bundle
-        elif (
-            type(identifier) is dict
-            and identifier.get("resource", {}).get("resourceType") == "Bundle"
-            and FHIR._find_resource(identifier, resource_type="Patient")
-        ):
-
-            return FHIR._find_resource(identifier, resource_type="Patient")["id"]
-
-        # Check for a Patient object
-        elif type(identifier) is Patient:
-
-            return identifier.id
-
-        else:
-            raise ValueError("Unhandled instance of a Patient identifier: {}".format(identifier))
-
-    @staticmethod
     def _patient_resource_query(identifier, key="patient"):
         """
         Accepts an identifier and builds the query for resources related to that
          Patient. Identifier can be a FHIR ID, an email address, or a Patient object.
          Optionally specify the parameter key to be used, defaults to 'patient'.
         :param identifier: object
         :param key: str
@@ -709,15 +662,15 @@
         :param response: The raw HTTP response object from FHIR
         :param resource_type: The resource type of the created resource
         :return: str, str
         """
         # Check status
         if not response.ok:
             logger.error(
-                f"FHIR Error: Cannot get resource details from a failed response: "
+                "FHIR Error: Cannot get resource details from a failed response: "
                 f"{response.status_code} : {response.content.decode()}"
             )
             return None, None
 
         try:
             # Get the URL from headers
             url = furl(response.headers.get("Location"))
@@ -746,15 +699,15 @@
         # Try based off the body of the response
         pattern = rf"{resource_type}\/([0-9]+)\/"
         matches = re.findall(pattern, response.content.decode())
         if matches:
             logger.error(f"FHIR ERROR: Could not determine resource ID from response: {response.content.decode()}")
 
             # Build URL
-            url = furl(FHIR.service_url())
+            url = furl(PPM.fhir_url())
             url.path.segments.extend([resource_type, matches[0]])
 
             return matches[0], url.url
 
         # Could not figure it out
         return None, None
 
@@ -824,17 +777,21 @@
         # Add it
         bundle.entry.append(questionnaire_response_entry)
 
         logger.debug(f"PPM/{patient_id}: Saving QuestionnaireResponse for " f"Questionnaire/{questionnaire_id}")
 
         try:
             # Create the organization
-            response = requests.post(FHIR.service_url(), json=bundle.as_json())
+            response = requests.post(PPM.fhir_url(), json=bundle.as_json())
             response.raise_for_status()
 
+            # Log the results of each request
+            for result in [entry["response"] for entry in response.json().get("entry", []) if "response" in entry]:
+                logging.debug(f"FHIR result: {result}")
+
             return response.json()
 
         except Exception as e:
             logger.exception(
                 "Save QuestionnaireResponse error: {}".format(e),
                 exc_info=True,
                 extra={
@@ -846,14 +803,119 @@
         return None
 
     #
     # CREATE
     #
 
     @staticmethod
+    def create(study, patient, resource_type, resource, replace=False, query=None):
+        """
+        A generic method implementation for creating a FHIR resource. This
+        will replace an existing resource if it is found via the optional
+        query.
+
+        :param study: The PPM study for which the resource is related
+        :type study: str
+        :param patient: The PPM participant that owns the resource
+        :type patient: str
+        :param resource_type: The FHIR resource type
+        :type resource_type: str
+        :param resource: The FHIR resource to persist
+        :type resource: dict, defaults to None
+        :param replace: Whether existing resources should be replaced or not
+        :type replace: bool, defaults to False
+        :param query: A query meant to find an existing resource to replace
+        :type query: dict, defaults to None
+        :return: The result of the operation
+        :rtype: Response
+        """
+        logger.debug(f"PPM/{study}/{patient}: Create resource: {resource_type}")
+
+        content = None
+        resource_id = None
+        try:
+            # Check if we need to replace an existing resource
+            if replace:
+
+                # If no query, try on Patient identifier
+                if not query:
+                    query = FHIR._patient_resource_query(identifier=patient)
+
+                # Check if one exsits
+                existing_resources = FHIR._query_resources(resource_type=resource_type, query=query)
+
+                # Check multiple
+                if existing_resources and len(existing_resources) > 1:
+                    logger.error(
+                        f"PPM/{patient}/{study}/FHIR: Multiple resources found, cannot replace",
+                        extra={
+                            "study": study,
+                            "patient": patient,
+                            "resource_type": resource_type,
+                            "query": query,
+                            "existing_resources": existing_resources,
+                        },
+                    )
+
+                # Get ID
+                elif existing_resources:
+                    resource_id = next(iter(existing_resources))["id"]
+                    logger.debug(
+                        f"PPM/{patient}/{study}/FHIR: Will replace {resource_type}/{resource_id}",
+                    )
+
+            # Set the URL
+            url = furl(PPM.fhir_url())
+
+            # Create the questionnaire response
+            action = getattr(requests, "put" if resource_id else "post", None)
+            if resource_id:
+
+                # Add QuestionnaireResponse path
+                url.path.segments.extend([resource_type, resource_id])
+
+            # Make the request
+            logger.debug(f"PPM/{patient}/{study}/FHIR: HTTP {action} to {url.url}")
+            response = action(url.url, json=resource.as_json())
+            content = response.content
+            logger.debug(f"PPM/{patient}/{study}/FHIR: Response {response.status_code}")
+
+            # Check the response
+            response.raise_for_status()
+
+            return response.json()
+
+        except requests.HTTPError as e:
+            logger.debug(f"PPM/{study}/{patient}/FHIR: Create resource response: {content}")
+            logger.exception(
+                f"PPM/{study}/{patient}/FHIR: Create resource request error: {e}",
+                extra={
+                    "study": study,
+                    "patient": patient,
+                    "resource_type": resource_type,
+                    "query": query,
+                    "resource_id": resource_id,
+                    "content": content,
+                },
+            )
+
+        except Exception as e:
+            logger.exception(
+                f"PPM/{study}/{patient}/FHIR: Create resource error: {e}",
+                exc_info=True,
+                extra={
+                    "study": study,
+                    "patient": patient,
+                    "resource_type": resource_type,
+                    "query": query,
+                    "resource_id": resource_id,
+                },
+            )
+
+    @staticmethod
     def create_ppm_research_study(project, title):
         """
         Creates a project list if not already created
         """
         research_study_data = FHIR.Resources.ppm_research_study(project, title)
 
         # Use the FHIR client lib to validate our resource.
@@ -883,21 +945,21 @@
         research_study_entry.request = research_study_request
 
         # Validate it.
         bundle = Bundle()
         bundle.entry = [research_study_entry]
         bundle.type = "transaction"
 
-        logger.debug("Creating...")
-
         # Create the ResearchStudy on the FHIR server.
-        # If we needed the ResearchStudy resource id, we could follow the redirect
-        # returned from a successful POST operation, and get the id out of the
-        # new resource. We don't though, so we can save an HTTP request.
-        response = requests.post(FHIR.service_url(), json=bundle.as_json())
+        logger.debug("Creating ResearchStudy via Transaction")
+        response = requests.post(PPM.fhir_url(), json=bundle.as_json())
+
+        # Parse out created identifiers
+        for result in [entry["response"] for entry in response.json().get("entry", []) if "response" in entry]:
+            logging.debug(f"FHIR result: {result}")
 
         return response.ok
 
     @staticmethod
     def create_ppm_research_subject(project, patient_id):
         """
         Creates a project list if not already created
@@ -922,45 +984,57 @@
         # address, no duplicate records will be created.
         ResearchSubject(research_subject_data)
 
         research_subject_request = BundleEntryRequest(
             {
                 "url": "ResearchSubject",
                 "method": "POST",
+                "ifNoneExist": str(
+                    Query(
+                        {
+                            **FHIR._patient_resource_query(patient_id, key="patient"),
+                            "identifier": f"{FHIR.research_subject_identifier_system}|{PPM.Study.fhir_id(project)}",
+                        }
+                    ),
+                ),
             }
         )
         research_subject_entry = BundleEntry({"resource": research_subject_data, "fullUrl": research_subject_id})
         research_subject_entry.request = research_subject_request
 
         # Validate it.
         bundle = Bundle()
         bundle.entry = [research_subject_entry]
         bundle.type = "transaction"
 
-        logger.debug("Creating...")
-
-        # Create the Patient and Flag on the FHIR server.
-        # If we needed the Patient resource id, we could follow the redirect
-        # returned from a successful POST operation, and get the id out of the
-        # new resource. We don't though, so we can save an HTTP request.
-        response = requests.post(FHIR.service_url(), json=bundle.as_json())
+        # Create the ResearchSubject resource
+        logger.debug("Creating ResearchSubject via Transaction")
+        response = requests.post(PPM.fhir_url(), json=bundle.as_json())
+
+        # Parse out created identifiers
+        for result in [entry["response"] for entry in response.json().get("entry", []) if "response" in entry]:
+            logging.debug(f"FHIR result: {result}")
 
         return response.ok
 
     @staticmethod
-    def create_ppm_device(patient_id, item, identifier=None, shipped=None, returned=None):
+    def create_ppm_device(patient_id, study, code, display, title, identifier, shipped=None, returned=None, note=None):
         """
         Creates a project list if not already created
         """
         device_data = FHIR.Resources.ppm_device(
-            item=item,
             patient_ref="Patient/{}".format(patient_id),
+            study=study,
+            code=code,
+            display=display,
+            title=title,
             identifier=identifier,
             shipped=shipped,
             returned=returned,
+            note=note,
         )
 
         # Use the FHIR client lib to validate our resource.
         Device(device_data)
 
         device_request = BundleEntryRequest(
             {
@@ -976,36 +1050,110 @@
         device_entry.request = device_request
 
         # Validate it.
         bundle = Bundle()
         bundle.entry = [device_entry]
         bundle.type = "transaction"
 
-        logger.debug("Creating...")
-
         # Create the Device on the FHIR server.
-        # If we needed the Patient resource id, we could follow the redirect
-        # returned from a successful POST operation, and get the id out of the
-        # new resource. We don't though, so we can save an HTTP request.
-        response = requests.post(FHIR.service_url(), json=bundle.as_json())
+        logger.debug("Creating Device via Transaction")
+        response = requests.post(PPM.fhir_url(), json=bundle.as_json())
+
+        # Parse out created identifiers
+        for result in [entry["response"] for entry in response.json().get("entry", []) if "response" in entry]:
+            logging.debug(f"FHIR result: {result}")
 
         return response.ok
 
     @staticmethod
+    def query_ppm_study_and_patient(study, patient):
+        """
+        Performs a query for a Patient as well as a ResearchStudy matching
+        the passed study identifier.
+
+        :param study: The study identifier
+        :type study: str
+        :param patient: The patient identifier, either ID or email
+        :type patient: str
+        :return: A tuple of the research study and the patient objects, if they exist
+        :rtype: object, object
+        """
+        patient_request = BundleEntryRequest(
+            {
+                "method": "GET",
+                "url": f"Patient?{str(Query(FHIR._patient_query(patient)))}",
+            }
+        )
+        patient_entry = BundleEntry()
+        patient_entry.request = patient_request
+
+        research_study_request = BundleEntryRequest(
+            {
+                "method": "GET",
+                "url": "ResearchStudy?"
+                + str(
+                    Query(
+                        {
+                            "identifier": f"{FHIR.research_study_identifier_system}|{PPM.Study.fhir_id(study)}",
+                        }
+                    )
+                ),
+            }
+        )
+        research_study_entry = BundleEntry()
+        research_study_entry.request = research_study_request
+
+        # Validate it.
+        bundle = Bundle()
+        bundle.entry = [patient_entry, research_study_entry]
+        bundle.type = "transaction"
+
+        logger.debug(f"Querying FHIR for Patient:{str(patient)} and Study:{study}")
+
+        # Execute transaction
+        response = requests.post(PPM.fhir_url(), json=bundle.as_json())
+
+        # Get resources
+        patient = research_study = None
+        for entry in [e for entry in response.json().get("entry", []) for e in entry["resource"].get("entry", [])]:
+
+            # Check for resources
+            if entry["resource"]["resourceType"] == "Patient":
+                patient = entry["resource"]
+                logger.debug(f"Found Patient/{patient['id']}")
+            if entry["resource"]["resourceType"] == "ResearchStudy":
+                research_study = entry["resource"]
+                logger.debug(f"Found ResearchStudy/{research_study['id']}")
+
+        return research_study, patient
+
+    @staticmethod
     def create_patient(form, project):
         """
-        Create a Patient resource in the FHIR server.
+        Creates the core resources necessary for a participant in PPM. Resources
+        include a Patient, a Flag and a ResearchSubject. The flag tracks
+        enrollment state for the specific study and the research subject
+        resource includes a participant in a specific PPM study.add()
+
+        :param form: The registration form filled out by the participant
+        :type form: dict
+        :param project: The name of the study for which the enrollment was for
+        :type project: str
+        :return: A tuple of the created resource IDs
+        :rtype: str, str, str
         """
         try:
-            # Get the study, or create it
-            study = FHIR._query_resources(
-                "ResearchStudy",
-                query={"identifier": "{}|{}".format(FHIR.research_study_identifier_system, PPM.Study.fhir_id(project))},
-            )
-            if not study:
+            # Check for existing study and patient
+            research_study, patient = FHIR.query_ppm_study_and_patient(project, form["email"])
+            if patient:
+                logger.warning(f"Patient already exists for {form['email']}, nothing to do")
+                return
+
+            # Create study if it doesn't exist
+            if not research_study:
                 FHIR.create_ppm_research_study(project, PPM.Study.title(project))
 
             # Build out patient JSON
             patient_data = FHIR.Resources.patient(form)
 
             # Create a placeholder ID for the patient the flag can reference.
             patient_uuid = uuid.uuid1()
@@ -1021,95 +1169,161 @@
                 {"system": FHIR.patient_identifier_system, "value": str(patient_uuid)}
             )
 
             patient_request = BundleEntryRequest(
                 {
                     "url": "Patient",
                     "method": "POST",
-                    "ifNoneExist": str(
-                        Query(
-                            {
-                                "identifier": "http://schema.org/email|" + form.get("email"),
-                            }
-                        )
-                    ),
+                    "ifNoneExist": str(Query({**FHIR._patient_query(form["email"])})),
                 }
             )
             patient_entry = BundleEntry({"resource": patient_data, "fullUrl": patient_uuid.urn})
             patient_entry.request = patient_request
 
             # Build enrollment flag.
             flag = Flag(FHIR.Resources.enrollment_flag(patient_uuid.urn, "registered"))
-            flag_request = BundleEntryRequest({"url": "Flag", "method": "POST"})
+            # TODO: Include the study in this resource once PPM needs
+            # to support participants with multiple studies
+            # flag = Flag(project, FHIR.Resources.enrollment_flag(patient_uuid.urn, "registered"))
+            flag_request = BundleEntryRequest(
+                {
+                    "url": "Flag",
+                    "method": "POST",
+                    "ifNoneExist": str(
+                        Query(
+                            {
+                                # TODO: Include the study in this conditional once PPM needs
+                                # to support participants with multiple studies
+                                # "encounter": f"ResearchStudy/{PPM.Study.fhir_id(study)}"
+                                **FHIR._patient_resource_query(form["email"], key="patient"),
+                            }
+                        ),
+                    ),
+                }
+            )
             flag_entry = BundleEntry({"resource": flag.as_json()})
             flag_entry.request = flag_request
 
             # Build research subject
             research_subject_data = FHIR.Resources.ppm_research_subject(project, patient_uuid.urn, "candidate")
-            research_subject_request = BundleEntryRequest({"url": "ResearchSubject", "method": "POST"})
+            research_subject_request = BundleEntryRequest(
+                {
+                    "url": "ResearchSubject",
+                    "method": "POST",
+                    "ifNoneExist": str(
+                        Query(
+                            {
+                                "identifier": f"{FHIR.research_subject_identifier_system}|{PPM.Study.fhir_id(project)}",
+                                **FHIR._patient_resource_query(form["email"], key="patient"),
+                            }
+                        ),
+                    ),
+                }
+            )
             research_subject_entry = BundleEntry({"resource": research_subject_data})
             research_subject_entry.request = research_subject_request
 
             # Validate it.
             bundle = Bundle()
             bundle.entry = [patient_entry, flag_entry, research_subject_entry]
             bundle.type = "transaction"
 
-            logger.debug("Creating...")
-
-            # Create the Patient and Flag on the FHIR server.
-            # If we needed the Patient resource id, we could follow the redirect
-            # returned from a successful POST operation, and get the id out of the
-            # new resource. We don't though, so we can save an HTTP request.
-            response = requests.post(FHIR.service_url(), json=bundle.as_json())
+            # Create the resources on the FHIR server.
+            logger.debug("Creating Patient/ResearchSubject/Flag via Transaction")
+            response = requests.post(PPM.fhir_url(), json=bundle.as_json())
 
             # Parse out created identifiers
-            for result in response.json():
+            patient_id = None
+            flag_id = None
+            research_subject_id = None
+
+            # Iterate results
+            for result in [entry["response"] for entry in response.json().get("entry", []) if "response" in entry]:
+                logging.debug(f"FHIR result: {result}")
+
+                # Get the location
+                location = result.get("location")
+                if not location:
+                    continue
 
-                # Do something
-                logging.debug("Created: {}".format(result))
+                # Get the ID
+                resource_id = re.search(r"^[A-Za-z-_]+\/([0-9]+)\/_history\/[0-9]+$", location, re.IGNORECASE).group(1)
 
-                pass
+                # Get resource ID
+                if location.startswith("Patient/"):
+                    patient_id = resource_id
+                elif location.startswith("Flag/"):
+                    flag_id = resource_id
+                elif location.startswith("ResearchSubject/"):
+                    research_subject_id = resource_id
 
-            return response.ok
+            return patient_id, flag_id, research_subject_id
 
         except Exception as e:
             logger.exception(e)
             raise
 
     @staticmethod
     def create_patient_enrollment(patient_id, status="registered"):
         """
         Create a Flag resource in the FHIR server to indicate a user's enrollment.
-        :param patient_id:
-        :param status:
-        :return:
+        :param patient_id: The patient identifier
+        :type patient_id: str or object
+        :param status: The enrollment status to set for the flag
+        :type status: str
+        :return: Whether the request was successful or not
+        :rtype: bool
         """
         logger.debug("Patient: {}".format(patient_id))
 
         # Use the FHIR client lib to validate our resource.
         flag = Flag(FHIR.Resources.enrollment_flag("Patient/{}".format(patient_id), status))
 
         # Set a date if enrolled.
         if status == "accepted":
             now = FHIRDate(datetime.now().isoformat())
             period = Period()
             period.start = now
             flag.period = period
 
-        # Build the FHIR Flag destination URL.
-        url = furl(FHIR.service_url())
-        url.path.segments.append("Flag")
+        # Build enrollment flag.
+        flag_request = BundleEntryRequest(
+            {
+                "url": "Flag",
+                "method": "POST",
+                "ifNoneExist": str(
+                    Query(
+                        {
+                            # TODO: Include the study in this conditional once PPM needs
+                            # to support participants with multiple studies
+                            # "encounter": f"ResearchStudy/{PPM.Study.fhir_id(study)}"
+                            **FHIR._patient_resource_query(patient_id, key="patient"),
+                        }
+                    ),
+                ),
+            }
+        )
+        flag_entry = BundleEntry({"resource": flag.as_json()})
+        flag_entry.request = flag_request
+
+        # Validate it.
+        bundle = Bundle()
+        bundle.entry = [flag_entry]
+        bundle.type = "transaction"
 
-        logger.debug("Creating flag at: {}".format(url.url))
+        logger.debug("Creating Flag via Transaction")
 
-        response = requests.post(url.url, json=flag.as_json())
-        logger.debug("Response: {}".format(response.status_code))
+        # Create the Flag resource
+        response = requests.post(PPM.fhir_url(), json=bundle.as_json())
 
-        return response
+        # Parse out created identifiers
+        for result in [entry["response"] for entry in response.json().get("entry", []) if "response" in entry]:
+            logging.debug(f"FHIR result: {result}")
+
+        return response.ok
 
     @staticmethod
     def create_communication(patient_id, content, identifier):
         """
         Create a record of a communication to a participant
         :param patient_id:
         :param content: The content of the email
@@ -1125,99 +1339,25 @@
                 identifier=identifier,
                 content=content,
                 sent=datetime.now().isoformat(),
             )
         )
 
         # Build the FHIR Communication destination URL.
-        url = furl(FHIR.service_url())
+        url = furl(PPM.fhir_url())
         url.path.segments.append("Communication")
 
         logger.debug("Creating communication at: {}".format(url.url))
 
         response = requests.post(url.url, json=communication.as_json())
         logger.debug("Response: {}".format(response.status_code))
 
         return response
 
     @staticmethod
-    def create_qualtrics_questionnaire(study, questionnaire_id, survey_id, survey, replace=False):
-        """
-        Create a Questionnaire resource created from the Qualtrics
-        survey.
-        :param study: The PPM study for which the survey/questionnaire is related
-        :type study: str
-        :param questionnaire_id: The questionnaire ID to use in FHIR
-        :type questionnaire_id: str
-        :param survey_id: The Qualtrics survey ID
-        :type survey_id: str
-        :param survey: The Qualtrics survey object from the Qualtrics API
-        :type survey: dict
-        :param replace: Whether existing resources should be replaced or not
-        :type replace: bool, defaults to False
-        :return: The result of the operation
-        :rtype: Response
-        """
-        logger.debug("Qualtrics survey: {}".format(survey["id"]))
-
-        # Use the FHIR client lib to validate our resource.
-        questionnaire = Questionnaire(
-            FHIR.Resources.ppm_qualtrics_survey_questionnaire(
-                study=study, questionnaire_id=questionnaire_id, survey_id=survey_id, survey=survey
-            )
-        )
-
-        # Check if exists if not replacing
-        if not replace:
-            questionnaires = FHIR._query_resources(
-                "Questionnaire",
-                query={
-                    "version": questionnaire.version,
-                },
-            )
-            if questionnaires:
-                return next(iter(questionnaires))
-
-        questionnaire_request = BundleEntryRequest(
-            {
-                "url": f"Questionnaire/{questionnaire_id}",
-                "method": "PUT",
-                "ifNoneExist": str(Query({"version:exact": questionnaire.version})),
-            }
-        )
-        questionnaire_entry = BundleEntry()
-        questionnaire_entry.resource = questionnaire
-        questionnaire_entry.request = questionnaire_request
-
-        # Validate it.
-        bundle = Bundle()
-        bundle.entry = [questionnaire_entry]
-        bundle.type = "transaction"
-
-        logger.debug("Creating Questionnaire for Qualtrics: {}".format(survey["id"]))
-
-        try:
-            # Create the organization
-            response = requests.post(FHIR.service_url(), json=bundle.as_json())
-            logger.debug("Response: {}".format(response.status_code))
-            response.raise_for_status()
-
-            return response.json()
-
-        except Exception as e:
-            logger.exception(
-                "PPM/FHIR: Create Questionnaire error: {}".format(e),
-                exc_info=True,
-                extra={
-                    "survey_id": survey["id"],
-                    "questionnaire_version": questionnaire.version,
-                },
-            )
-
-    @staticmethod
     def create_research_study(patient_id, research_study_title):
         logger.debug("Create ResearchStudy: {}".format(research_study_title))
 
         # Create temp identifier for the study
         research_study_id = uuid.uuid1().urn
 
         # Create the organization
@@ -1263,17 +1403,22 @@
         bundle.entry = [research_study_entry, research_subject_entry]
         bundle.type = "transaction"
 
         logger.debug("Creating: {}".format(research_study_title))
 
         try:
             # Create the organization
-            response = requests.post(FHIR.service_url(), json=bundle.as_json())
+            response = requests.post(PPM.fhir_url(), json=bundle.as_json())
+            logger.debug("Response: {}".format(response.status_code))
             response.raise_for_status()
 
+            # Parse out created identifiers
+            for result in [entry["response"] for entry in response.json().get("entry", []) if "response" in entry]:
+                logging.debug(f"FHIR result: {result}")
+
             return response.json()
 
         except Exception as e:
             logger.exception(
                 "Create ResearchStudy error: {}".format(e),
                 exc_info=True,
                 extra={
@@ -1375,15 +1520,19 @@
         bundle_entries.append(bundle_item_list)
 
         # Create and send the full bundle.
         full_bundle = Bundle()
         full_bundle.entry = bundle_entries
         full_bundle.type = "transaction"
 
-        response = requests.post(url=FHIR.service_url(), json=full_bundle.as_json())
+        response = requests.post(url=PPM.fhir_url(), json=full_bundle.as_json())
+
+        # Parse out created identifiers
+        for result in [entry["response"] for entry in response.json().get("entry", []) if "response" in entry]:
+            logging.debug(f"FHIR result: {result}")
 
         return response.ok
 
     @staticmethod
     def create_consent_document_reference(study, ppm_id, filename, url, hash, size, composition, identifiers=None):
         """
         Accepts details and rendering of a signed PPM consent and saves that data as a
@@ -1503,17 +1652,21 @@
             composition_entry = BundleEntry({"resource": composition})
             composition_entry.request = composition_request
 
             # Add it
             bundle.entry.append(composition_entry)
 
             # Post the transaction
-            response = requests.post(FHIR.service_url(), json=bundle.as_json())
+            response = requests.post(PPM.fhir_url(), json=bundle.as_json())
             response.raise_for_status()
 
+            # Parse out created identifiers
+            for result in [entry["response"] for entry in response.json().get("entry", []) if "response" in entry]:
+                logging.debug(f"FHIR result: {result}")
+
             # Check response
             return response.ok
 
         except (requests.HTTPError, TypeError, ValueError):
             logger.error(
                 "Create consent DocumentReference failed",
                 exc_info=True,
@@ -1536,15 +1689,15 @@
         :type query: dict
         :return: A list of FHIR resource dicts
         :rtype: list
         """
         logger.debug("Query resource: {}".format(resource_type))
 
         # Build the URL.
-        url_builder = furl(FHIR.service_url())
+        url_builder = furl(PPM.fhir_url())
         url_builder.path.add(resource_type)
 
         # Add query if passed and set a return count to a high number,
         # despite the server
         # probably ignoring it.
         url_builder.query.params.add("_count", 1000)
         if query is not None:
@@ -1593,15 +1746,15 @@
         :type resource_type: str
         :param query: A dict of key value pairs for searching resources
         :type query: dict
         :return: A Bundle of FHIR resources
         :rtype: Bundle
         """
         # Build the URL.
-        url_builder = furl(FHIR.service_url())
+        url_builder = furl(PPM.fhir_url())
         url_builder.path.add(resource_type)
 
         # Add query if passed and set a return count to a high number,
         # despite the server
         # probably ignoring it.
         url_builder.query.params.add("_count", 1000)
         if query is not None:
@@ -1652,15 +1805,15 @@
         :type _id: str
         :return: A FHIR resource
         :rtype: dict
         """
         logger.debug('Query resource "{}": {}'.format(resource_type, _id))
 
         # Build the URL.
-        url_builder = furl(FHIR.service_url())
+        url_builder = furl(PPM.fhir_url())
         url_builder.path.add(resource_type)
         url_builder.path.add(_id)
 
         # Make the request.
         response = requests.get(url_builder.url)
         response.raise_for_status()
 
@@ -1800,153 +1953,121 @@
         enrollments = enrollment.split(",") if enrollment else None
         studies = study.split(",") if study else None
 
         # Call the query_participants method
         return FHIR.query_participants(studies, enrollments, active, testing)
 
     @staticmethod
-    def query_participant(patient, flatten_return=False):
-
-        # Build the FHIR Consent URL.
-        url = furl(FHIR.service_url())
-        url.path.segments.append("Patient")
-        url.query.params.add("_include", "*")
-        url.query.params.add("_revinclude", "*")
-
-        # Add patient query
-        for key, value in FHIR._patient_query(patient).items():
-            url.query.params.add(key, value)
-
-        # Make the call
-        content = None
-        try:
-            # Make the FHIR request.
-            response = requests.get(url.url)
-            content = response.content
-
-            if flatten_return:
-                return FHIR.flatten_participant(response.json())
-            else:
-                return response.json()
-
-        except requests.HTTPError as e:
-            logger.exception(
-                "FHIR Connection Error: {}".format(e),
-                exc_info=True,
-                extra={"response": content},
-            )
-
-        except KeyError as e:
-            logger.exception("FHIR Error: {}".format(e), exc_info=True, extra={"response": content})
-
-        return None
-
-    # TODO: Remove this method
-    @staticmethod
-    def query_patient(patient, flatten_return=False):
-
-        # Build the FHIR Consent URL.
-        url = furl(FHIR.service_url())
-        url.path.segments.append("Patient")
-
-        # Get flags for current user
-        query = FHIR._patient_query(patient)
-
-        # Make the call
-        content = None
-        try:
-            # Make the FHIR request.
-            response = requests.get(url.url, params=query)
-            content = response.content
-
-            # Ensure we have a resource
-            bundle = response.json()
-
-            if flatten_return:
-                return FHIR.flatten_patient(bundle)
-            else:
-                return [entry["resource"] for entry in bundle.get("entry", [])]
-
-        except requests.HTTPError as e:
-            logger.exception(
-                "FHIR Connection Error: {}".format(e),
-                exc_info=True,
-                extra={"response": content},
-            )
-
-        except KeyError as e:
-            logger.exception("FHIR Error: {}".format(e), exc_info=True, extra={"response": content})
-
-        return None
-
-    @staticmethod
-    def get_participant(patient, flatten_return=False, questionnaire_ids=None):
+    def get_participant(patient, questionnaires=None, flatten_return=False):
         """
         This method fetches a participant's entire FHIR record and returns it.
         If specified, the record will be flattened into a dictionary. Otherwise,
         a list of all resources belonging to the participant are returned.
+        Optional values include questionnaire IDs
+        to be flattened. If these are not specified, hard-coded values from the
+        PPM module will be used, althought this is deprecated behavior.
 
         :param patient: The participant identifier, PPM ID or email
         :type patient: str
+        :param questionnaires: The list of survey/questionnaires for this study
+        :type questionnaires: list, defaults to None
         :param flatten_return: Whether to flatten the resources or not
         :type flatten_return: bool, defaults to False
-        :param questionnaire_ids: The list of Questionnaire IDs to include
-        :type questionnaire_ids: list, defaults to None
         :returns: A dictionary comprising the user's record
         :rtype: dict
         """
-
         # Build the FHIR Consent URL.
-        url = furl(FHIR.service_url())
+        url = furl(PPM.fhir_url())
         url.path.segments.append("Patient")
         url.query.params.add("_include", "*")
         url.query.params.add("_revinclude", "*")
 
         # Add patient query
         for key, value in FHIR._patient_query(patient).items():
             url.query.params.add(key, value)
 
         # Make the call
-        content = None
+        content = response = None
         try:
             # Make the FHIR request.
             response = requests.get(url.url)
             content = response.content
             response.raise_for_status()
 
             # Check for entries
             bundle = response.json()
             if not bundle.get("entry") or not FHIR._find_resources(bundle, "Patient"):
+                logger.debug(f"PPM/FHIR: Empty and/or no Patient for {patient}")
                 return {}
 
             if flatten_return:
-                return FHIR.flatten_participant(response.json(), questionnaire_ids)
+                return FHIR.flatten_participant(
+                    bundle=response.json(),
+                    questionnaires=questionnaires,
+                )
             else:
                 return [entry["resource"] for entry in bundle.get("entry")]
 
         except requests.HTTPError as e:
+            logger.debug(f"PPM/FHIR: Patient request response: {content}")
             logger.exception(
-                "FHIR Connection Error: {}".format(e),
-                exc_info=True,
-                extra={"response": content},
+                f"PPM/FHIR: Patient request error: {e}",
+                extra={
+                    "patient": patient,
+                    "url": url,
+                    "response": response,
+                    "content": content,
+                },
             )
 
         except KeyError as e:
             logger.exception("FHIR Error: {}".format(e), exc_info=True, extra={"response": content})
 
         return None
 
     @staticmethod
+    def query_participant(patient, questionnaires=None, flatten_return=False):
+        """
+        This method queries a participant's entire FHIR record and returns it
+        if available. If specified, the record will be flattened into a
+        dictionary. Otherwise, a list of all resources belonging to the
+        participant are returned. Optional values include questionnaire IDs
+        to be flattened. If these are not specified, hard-coded values from the
+        PPM module will be used, althought this is deprecated behavior.
+
+        :param patient: The participant identifier, PPM ID or email
+        :type patient: str
+        :param questionnaires: The list of survey/questionnaires for this study
+        :type questionnaires: list, defaults to None
+        :param flatten_return: Whether to flatten the resources or not
+        :type flatten_return: bool, defaults to False
+        :returns: A dictionary comprising the user's record
+        :rtype: dict
+        """
+        logger.warning('PPM/FHIR: Method "query_participant" is deprecated')
+        warnings.warn('PPM/FHIR: "query_participant" is deprecated, use "get_participant" instead', DeprecationWarning)
+        return FHIR.get_participant(patient, questionnaires, flatten_return)
+
+    @staticmethod
     def get_patient(patient, flatten_return=False):
+        """
+        This method queries a participant's FHIR Patient record and returns it
+        if available. If specified, the record will be flattened into a
+        dictionary. Otherwise, a list of relevant resources will be returned.
 
+        :param patient: The participant identifier, PPM ID or email
+        :type patient: str
+        :param flatten_return: Whether to flatten the resources or not
+        :type flatten_return: bool, defaults to False
+        :returns: A dictionary comprising the user's Patient record
+        :rtype: dict
+        """
         # Build the FHIR Consent URL.
-        url = furl(FHIR.service_url())
+        url = furl(PPM.fhir_url())
         url.path.segments.append("Patient")
-        url.query.params.add("_include", "*")
-        url.query.params.add("_revinclude", "*")
 
         # Add query for patient
         for key, value in FHIR._patient_query(patient).items():
             url.query.params.add(key, value)
 
         # Make the call
         content = None
@@ -1960,37 +2081,72 @@
             else:
                 return next(
                     (entry["resource"] for entry in response.json().get("entry", [])),
                     None,
                 )
 
         except requests.HTTPError as e:
+            logger.debug(f"PPM/FHIR: Patient request response: {content}")
             logger.exception(
-                "FHIR Connection Error: {}".format(e),
-                exc_info=True,
-                extra={"response": content},
+                f"PPM/FHIR: Patient request error: {e}",
+                extra={
+                    "patient": patient,
+                    "url": url,
+                    "response": response,
+                    "content": content,
+                },
             )
 
         except KeyError as e:
-            logger.exception("FHIR Error: {}".format(e), exc_info=True, extra={"response": content})
+            logger.exception(
+                f"PPM/FHIR Error: {e}",
+                exc_info=True,
+                extra={
+                    "patient": patient,
+                    "url": url,
+                    "response": response,
+                    "content": content,
+                },
+            )
 
         return None
 
+    @staticmethod
+    def query_patient(patient, flatten_return=False):
+        """
+        This method queries a participant's FHIR Patient record and returns it
+        if available. If specified, the record will be flattened into a
+        dictionary. Otherwise, a list of relevant resources will be returned.
+
+        :param patient: The participant identifier, PPM ID or email
+        :type patient: str
+        :param flatten_return: Whether to flatten the resources or not
+        :type flatten_return: bool, defaults to False
+        :returns: A dictionary comprising the user's Patient record
+        :rtype: dict
+        """
+        logger.warning('PPM/FHIR: Method "query_patient" is deprecated')
+        warnings.warn('PPM/FHIR: "query_patient" is deprecated, use "get_patient" instead', DeprecationWarning)
+        return FHIR.get_patient(patient, flatten_return)
+
     # TODO: This method is deprecated
     @staticmethod
     def get_composition(patient, flatten_return=False):
         """
         Gets and returns the Composition storing the user's signed consent resources
         :param patient: The Patient object who owns the consent
         :type patient: str
         :param flatten_return: Whether to return FHIR JSON or a flattened dict
         :type flatten_return: bool
         :return: The Composition object
         """
-        logger.warning("DEPRECATED: This method should not be used for fetching consent composition resources")
+        logger.warning('PPM/FHIR: Method "get_composition" is deprecated')
+        warnings.warn(
+            'PPM/FHIR: "get_composition" is deprecated, use "query_consent_compositions" instead', DeprecationWarning
+        )
 
         # Just return the first from querying
         compositions = FHIR.query_consent_compositions(patient=patient, flatten_return=flatten_return)
         if compositions:
             return compositions[0]
 
         return None
@@ -2164,15 +2320,15 @@
             return resources
 
     @staticmethod
     def query_patient_id(email):
 
         try:
             # Get the client
-            client = FHIR.get_client(FHIR.service_url())
+            client = FHIR.get_client(PPM.fhir_url())
 
             # Query the Patient
             search = Patient.where(struct={"identifier": "http://schema.org/email|{}".format(email)})
             resources = search.perform_resources(client.server)
             for resource in resources:
 
                 # Return the ID of the first Patient
@@ -2184,14 +2340,36 @@
                 exc_info=True,
                 extra={"email": email},
             )
 
         return None
 
     @staticmethod
+    def get_ppm_device(id, flatten_return=False):
+        """
+        Queries FHIR for PPM devices and returns the device, if any, matching
+        the passed ID. Note: This is the numeric FHIR ID of the resource.
+
+        :param id: The item's FHIR ID
+        :type id: str
+        :param flatten_return: Whether to flatten the resource or not
+        :type flatten_return: bool
+        :return: The matching device resource, if any
+        :rtype: dict, defaults to None
+        """
+        # Get the devices
+        device = next(iter(FHIR._query_resources("Device", query={"_id": id})), None)
+
+        # Check if the resource should be flattened
+        if device and flatten_return:
+            return FHIR.flatten_ppm_device(device)
+
+        return device
+
+    @staticmethod
     def query_ppm_devices(patient=None, item=None, identifier=None, flatten_return=False):
         """
         Queries the participants FHIR record for any PPM-related Device
         resources. These are used to track kits, etc that
         are sent to participants for collecting samples and other information/data.
         :param patient: The patient identifier/ID/object
         :type patient: object
@@ -2200,14 +2378,15 @@
         :param identifier: The device identifier
         :type identifier: str
         :param flatten_return: Whether to flatten the resource or not
         :type flatten_return: bool
         :return: A list of resources
         :rtype: list
         """
+
         # Check item type
         if item:
             query = {
                 "type": "{}|{}".format(FHIR.device_coding_system, item),
             }
         else:
 
@@ -2274,15 +2453,15 @@
         else:
             return research_subjects
 
     @staticmethod
     def query_enrollment_flag(patient, flatten_return=False):
 
         # Build the FHIR Consent URL.
-        url = furl(FHIR.service_url())
+        url = furl(PPM.fhir_url())
         url.path.segments.append("Flag")
 
         # Get flags for current user
         query = FHIR._patient_resource_query(patient, "subject")
 
         # Make the call
         content = None
@@ -2413,40 +2592,60 @@
         :return: The FHIR Questionnaire object
         :rtype: object
         """
         return FHIR._query_resource("Questionnaire", questionnaire_id)
 
     @staticmethod
     def get_questionnaire_response(patient, questionnaire_id, flatten_return=False):
+        """
+        Returns the QuestionnaireResponse for the given patient and
+        questionnaire. If specified to do so, the response object will be
+        flattened to an easier to parse dictionary object. Returns None if
+        not QuestionnaireResponse is found.add()
+
+        :param patient: The PPM participant to find the response for
+        :type patient: str
+        :param questionnaire_id: The ID of the Questionnaire the response was for
+        :type questionnaire_id: str
+        :param flatten_return: Whether to flatten the resource or not, defaults to False
+        :type flatten_return: bool, optional
+        :return: The QuestionnaireResponse object
+        :rtype: dict, or None
+        """
 
         # Build the query
         query = {
             "questionnaire": "Questionnaire/{}".format(questionnaire_id),
             "_include": "*",
             "_revinclude": "*",
         }
 
         # Check patient
         query.update(FHIR._patient_resource_query(identifier=patient, key="source"))
 
         # Query resources
         bundle = FHIR._query_bundle("QuestionnaireResponse", query=query)
 
-        if flatten_return:
+        # Ensure we've got resources
+        if bundle.entry:
 
-            # We need the whole bundle to flatten it
-            return FHIR.flatten_questionnaire_response(bundle, questionnaire_id)
-        else:
+            if flatten_return:
 
-            # Fetch the questionnaire response from the bundle
-            questionnaire_response = next(
-                (r.resource for r in bundle.entry if r.resource.resource_type == "QuestionnaireResponse"),
-                None,
-            )
-            return questionnaire_response.as_json()
+                # We need the whole bundle to flatten it
+                return FHIR.flatten_questionnaire_response(bundle, questionnaire_id)
+            else:
+
+                # Fetch the questionnaire response from the bundle
+                questionnaire_response = next(
+                    (r.resource.as_json() for r in bundle.entry if r.resource.resource_type == "QuestionnaireResponse"),
+                    None,
+                )
+                return questionnaire_response
+        else:
+            logger.warning(f"PPM/FHIR: No QuestionnaireResponse for query: {query}")
 
     @staticmethod
     def get_qualtrics_questionnaire_response(patient, survey_id, flatten_return=False):
         """
         Queries FHIR for a QuestionnaireResponse for the passed patient and
         Qualtrics survey. If specified, FHIR resource is flattened for output.
 
@@ -2743,15 +2942,15 @@
 
         # Find matching resource(s)
         bundle = FHIR._query_bundle("List", query=query)
 
         if flatten_return:
             return FHIR.flatten_list(bundle, "Organization")
         else:
-            return next((entry["resource"] for entry in bundle.as_json().get("entry", [])), None)
+            return [entry["resource"] for entry in bundle.as_json().get("entry", [])]
 
     @staticmethod
     def query_ppm_communications(patient=None, identifier=None, flatten_return=False):
         """
         Find all Communications filtered by patient, study and/or identifier
         :param patient: The patient to query on (FHIR ID, email, Patient object)
         :type patient: str
@@ -2873,15 +3072,15 @@
                         break
 
             active = form.get("active")
             if active is not None:
                 patient["active"] = False if active in ["false", False] else True
 
             # Build the URL
-            url = furl(FHIR.service_url())
+            url = furl(PPM.fhir_url())
             url.path.segments.append("Patient")
             url.path.segments.append(fhir_id)
 
             # Put it
             response = requests.put(url.url, json=patient)
             content = response.content
             response.raise_for_status()
@@ -2906,15 +3105,15 @@
         # Make the updates
         content = None
         try:
             # Build the update
             patch = [{"op": "replace", "path": "/active", "value": True if active else False}]
 
             # Build the URL
-            url = furl(FHIR.service_url())
+            url = furl(PPM.fhir_url())
             url.path.segments.append("Patient")
             url.path.segments.append(patient_id)
 
             # Put it
             response = requests.patch(
                 url.url,
                 json=patch,
@@ -2934,84 +3133,173 @@
 
         except Exception as e:
             logger.error("FHIR Error: {}".format(e), exc_info=True, extra={"ppm_id": patient_id})
 
         return False
 
     @staticmethod
-    def update_ppm_device(patient_id, item, identifier=None, shipped=None, returned=None):
-
+    def update_ppm_device(
+        id, patient_id, study, code, display, title, identifier, shipped=None, returned=None, note=None
+    ):
+        """
+        Updates the Device for the given ID. Optional fields will be updated
+        if a value is passed or deleted if None is passed.
+
+        :param id: The ID of the Device resource
+        :type id: str
+        :param patient_id: The ID of the participant
+        :type patient_id: str
+        :param study: The study for which the device pertains, defaults to None
+        :type study: str
+        :param code: The code of the device type, defaults to None
+        :type code: str
+        :param display: The name of the device type, defaults to None
+        :type display: str
+        :param title: The admin-assigned title of the device, defaults to None
+        :type title: str
+        :param identifier: The identifier of the device, defaults to None
+        :type identifier: str, optional
+        :param shipped: The date the item was shipped to the participant, defaults to None
+        :type shipped: datetime, optional
+        :param returned: The date the item was returned to PPM, defaults to None
+        :type returned: datetime, optional
+        :param note: Any admin-assigned note for this device, defaults to None
+        :type note: str, optional
+        :return: Whether the operation succeeded or not
+        :rtype: boolean
+        """
         # Make the updates
-        content = None
+        url = response = content = None
         try:
             # Get the device
-            device = next(iter(FHIR.query_ppm_devices(patient=patient_id, item=item)), None)
+            device = FHIR.get_ppm_device(id=id, flatten_return=False)
             if not device:
-                logger.debug(f"No PPM device could be found for {patient_id}/{item}/{identifier}")
+                logger.debug(f"No PPM device could be found for {patient_id}/{id}/{identifier}")
                 return False
 
             # Update the resource identifier
-            if identifier:
+            ppm_identifier = next(
+                (i for i in device.get("identifier", []) if i.get("system") == FHIR.device_identifier_system),
+                None,
+            )
+            if ppm_identifier and ppm_identifier.get("value") != identifier:
+                ppm_identifier["value"] = identifier
 
-                # Get the PPM identifier dictionary
-                identifiers = device.get("identifier", [])
-                ppm_identifier = next(
-                    (_id for _id in identifiers if _id.get("system") == FHIR.device_identifier_system),
-                    None,
+            elif not ppm_identifier:
+                device.setdefault("identifier", []).append(
+                    {
+                        "system": FHIR.device_identifier_system,
+                        "value": identifier,
+                    }
                 )
-                if ppm_identifier:
 
-                    # Update it
-                    ppm_identifier["value"] = identifier.lower()
-
-                else:
+            # Set the study
+            extension = next(
+                (e for e in device.get("extension", []) if e.get("url") == FHIR.device_study_extension_url), None
+            )
+            if extension:
+                extension["valueString"] = study
+            else:
+                device.setdefault("extension", []).append(
+                    {
+                        "url": FHIR.device_study_extension_url,
+                        "valueString": study,
+                    }
+                )
 
-                    # Add a new one
-                    identifiers.append(
-                        {
-                            "system": FHIR.device_identifier_system,
-                            "value": identifier.lower(),
-                        }
-                    )
+            # Set the title
+            title_identifier = next(
+                (i for i in device.get("identifier", []) if i.get("system") == FHIR.device_title_system), None
+            )
+            if title_identifier and title_identifier.get("value") != title:
+                title_identifier["value"] = title
+            elif not title_identifier:
+                device.setdefault("identifier", []).append(
+                    {
+                        "system": FHIR.device_title_system,
+                        "value": title,
+                    }
+                )
 
-                # Set it
-                device["identifier"] = identifiers
+            # Update type
+            type_code = next(
+                (c for c in device.get("type", {}).get("coding", []) if c.get("system") == FHIR.device_coding_system),
+                None,
+            )
+            if type_code and type_code.get("code") != code or type_code.get("display") != display:
+                type_code["code"] = code
+                type_code["display"] = display
+                device["type"]["text"] = display
+            elif not type_code:
+                device.setdefault("type", {}).setdefault("coding", []).append(
+                    {
+                        "system": FHIR.device_coding_system,
+                        "code": code,
+                        "display": display,
+                    }
+                )
+                device["type"]["text"] = display
 
             # Check dates
             if shipped:
                 device["manufactureDate"] = shipped.isoformat()
             elif device.get("manufactureDate"):
                 del device["manufactureDate"]
 
             if returned:
                 device["expirationDate"] = returned.isoformat()
             elif device.get("expirationDate"):
                 del device["expirationDate"]
 
+            # Get the first note
+            annotation = next((n for n in device.get("note", [])), None)
+            if annotation and not note:
+                del device["note"]
+            elif annotation and annotation.get("text") != note:
+                annotation["text"] = note
+            elif not annotation and note:
+                device["note"] = [
+                    {
+                        "time": datetime.now().isoformat(),
+                        "text": note,
+                    }
+                ]
+
             # Build the URL
-            url = furl(FHIR.service_url())
+            url = furl(PPM.fhir_url())
             url.path.segments.append("Device")
             url.path.segments.append(device["id"])
 
             # Put it
             response = requests.put(url.url, json=device)
             content = response.content
             response.raise_for_status()
 
             return response.ok
 
         except requests.HTTPError as e:
+            logger.debug(f"PPM/FHIR: Device request error: {content}")
             logger.error(
-                "FHIR Request Error: {}".format(e),
-                exc_info=True,
-                extra={"ppm_id": patient_id, "response": content},
+                "PPM/FHIR: Device request Error: {}".format(e),
+                extra={"ppm_id": patient_id, "id": id, "url": url, "response": response},
             )
 
         except Exception as e:
-            logger.error("FHIR Error: {}".format(e), exc_info=True, extra={"ppm_id": patient_id})
+            logger.error(
+                f"PPM/FHIR: Device update error: {e}",
+                exc_info=True,
+                extra={
+                    "ppm_id": patient_id,
+                    "id": id,
+                    "study": study,
+                    "code": code,
+                    "url": url,
+                    "response": response,
+                },
+            )
 
         return False
 
     @staticmethod
     def update_patient_deceased(patient_id, date=None, active=None):
         """
         Updates a participant as deceased. If a date is passed, they are marked
@@ -3038,15 +3326,15 @@
                 patch = [{"op": "remove", "path": "/deceasedDateTime"}]
 
             # Update active if needed
             if active is not None:
                 patch.append({"op": "replace", "path": "/active", "value": active})
 
             # Build the URL
-            url = furl(FHIR.service_url())
+            url = furl(PPM.fhir_url())
             url.path.segments.append("Patient")
             url.path.segments.append(patient_id)
 
             # Put it
             response = requests.patch(
                 url.url,
                 json=patch,
@@ -3070,19 +3358,20 @@
         return False
 
     @staticmethod
     def update_patient_enrollment(patient_id, status):
         logger.debug("Patient: {}, Status: {}".format(patient_id, status))
 
         # Fetch the flag.
-        url = furl(FHIR.service_url())
+        url = furl(PPM.fhir_url())
         url.path.segments.append("Flag")
 
-        # Build the query
-        query = FHIR._patient_resource_query(patient_id, key="subject")
+        query = {
+            "subject": "Patient/{}".format(patient_id),
+        }
 
         content = None
         try:
             # Fetch the flag.
             response = requests.get(url.url, params=query)
             flag_entries = Bundle(response.json())
 
@@ -3169,15 +3458,15 @@
 
                 # Set the code.
                 code.code = status
                 code.display = status.title()
                 flag.code.text = status.title()
 
                 # Build the URL
-                flag_url = furl(FHIR.service_url())
+                flag_url = furl(PPM.fhir_url())
                 flag_url.path.segments.extend(["Flag", flag.id])
 
                 logger.debug('Updating Flag "{}" with code: "{}"'.format(flag_url.url, status))
 
                 # Post it.
                 response = requests.put(flag_url.url, json=flag.as_json())
                 content = response.content
@@ -3268,15 +3557,15 @@
                 if "ResearchStudy" in reference:
                     break
             else:
                 # Add it
                 composition["section"].append({"reference": f"ResearchStudy/{PPM.Study.fhir_id(study)}"})
 
             # Build the URL
-            url = furl(FHIR.service_url())
+            url = furl(PPM.fhir_url())
             url.path.segments.append("Composition")
             url.path.segments.append(composition["id"])
 
             # Put it
             response = requests.put(url.url, json=composition)
             content = response.content
             response.raise_for_status()
@@ -3325,15 +3614,15 @@
                         "op": "update",
                         "path": "/period/start",
                         "value": start.isoformat(),
                     }
                 ]
 
             # Build the URL
-            url = furl(FHIR.service_url())
+            url = furl(PPM.fhir_url())
             url.path.segments.append("ResearchSubject")
             url.path.segments.append(research_subject_id)
 
             # Put it
             response = requests.patch(
                 url.url,
                 json=patch,
@@ -3368,15 +3657,15 @@
         return False
 
     @staticmethod
     def update_ppm_research_subject(patient_id, study=None, start=None, end=None):
         logger.debug("Patient: {}, Study: {}, Start: {}, End: {}".format(patient_id, study, start, end))
 
         # Fetch the flag.
-        url = furl(FHIR.service_url())
+        url = furl(PPM.fhir_url())
         url.path.segments.append("ResearchSubject")
 
         # Build the query
         query = FHIR._patient_resource_query(patient_id)
 
         # Build study identifier
         study_query = "{}|".format(FHIR.research_subject_identifier_system)
@@ -3427,99 +3716,113 @@
     @staticmethod
     def update_point_of_care_list(patient, point_of_care):
         """
         Adds a point of care to a Participant's existing list and returns the flattened
         updated list of points of care (just a list with the name of the Organization).
         Will return the existing list if the point of care is already in the list. Will
         look for an existing Organization before creating.
+
         :param patient: The participant's email address
+        :type patient: str
         :param point_of_care: The name of the point of care
-        :return: [str]
+        :type point_of_care: str
+        :returns: A list of the current points of care for the participant
+        :rtype: list
+        """
+        return FHIR.update_points_of_care_list(patient, [point_of_care])
+
+    @staticmethod
+    def update_points_of_care_list(patient, points_of_care):
+        """
+        Adds a point of care to a Participant's existing list and returns the flattened
+        updated list of points of care (just a list with the name of the Organization).
+        Will return the existing list if the point of care is already in the list. Will
+        look for an existing Organization before creating.
+
+        :param patient: The participant's email address
+        :type patient: str
+        :param point_of_care: The name of the point of care
+        :type point_of_care: str
+        :returns: A list of the current points of care for the participant
+        :rtype: list
         """
-        logger.debug("Add point of care: {}".format(point_of_care))
+        logger.debug("Add points of care: {}".format(points_of_care))
 
-        # Get the flattened list
-        points_of_care = FHIR.get_point_of_care_list(patient, flatten_return=True)
+        # Get the list and related organizations
+        resources = FHIR.get_point_of_care_list(patient, flatten_return=False)
+
+        # Extract resources
+        organizations = [r for r in resources if r["resourceType"] == "Organization"]
+        points_of_care_list = next((r for r in resources if r["resourceType"] == "List"), None)
+
+        # Create if it doesn't exist
+        if not points_of_care_list:
+            # Set the list to persist
+            points_of_care = [points_of_care]
+            logger.debug("PPM/FHIR: POC list doesn't exist, will create")
+            FHIR.create_point_of_care_list(patient, points_of_care)
+            return points_of_care
 
         # Check if the name exists in the list already
-        for organization in points_of_care:
-            if organization == point_of_care:
-                logger.debug("Organization is already in List!")
-
-                # Just return the list as is
-                return points_of_care
-
-        # Look for it
-        organization_url = furl(FHIR.service_url())
-        organization_url.path.add("Organization")
-        organization_url.query.params.add("name", point_of_care)
+        for organization in [o["name"] for o in organizations]:
+            if organization in points_of_care:
+                logger.debug(f'PPM/FHIR: Organization "{organization}" is already in List')
 
-        response = requests.get(organization_url.url)
-        response.raise_for_status()
+                # Pop it
+                points_of_care.remove(organization)
 
         # Start a bundle request
         bundle = Bundle()
         bundle.entry = []
         bundle.type = "transaction"
 
-        results = response.json()
-        if results["total"] >= 1:
-            logger.debug("Found existing organization!")
-
-            # Get the ID
-            organization_id = "Organization/{}".format(results["entry"][0]["resource"]["id"])
-            logger.debug("Existing organization: {}".format(organization_id))
+        list_request = BundleEntryRequest()
+        list_request.method = "PUT"
+        list_request.url = "List/{}".format(points_of_care_list["id"])
 
-        else:
-            logger.debug("No existing organization, creating...")
+        # Add Organization objects to bundle.
+        for point_of_care in points_of_care:
 
             # Create the organization
             organization = Organization()
             organization.name = point_of_care
-
-            # Create placeholder ID
             organization_id = uuid.uuid1().urn
 
-            # Add Organization objects to bundle.
             organization_request = BundleEntryRequest()
             organization_request.method = "POST"
             organization_request.url = "Organization"
 
-            # Create the organization entry
-            organization_entry = BundleEntry({"resource": organization.as_json()})
-            organization_entry.request = organization_request
+            # Don't recreate Organizations if we can find them by the exact name.
+            # No fuzzy matching.
+            organization_request.ifNoneExist = str(Query({"name:exact": organization.name}))
+
+            organization_entry = BundleEntry()
+            organization_entry.resource = organization
             organization_entry.fullUrl = organization_id
+            organization_entry.request = organization_request
 
-            # Add it
+            # Add it to the transaction
             bundle.entry.append(organization_entry)
 
-        # Add it to the list
-        point_of_care_list = FHIR.get_point_of_care_list(patient, flatten_return=False)
-        point_of_care_list["entry"].append({"item": {"reference": organization_id}})
-
-        # Add List objects to bundle.
-        list_request = BundleEntryRequest()
-        list_request.method = "PUT"
-        list_request.url = "List/{}".format(point_of_care_list["id"])
+            # Add it
+            points_of_care_list["entry"].append({"item": {"reference": f"Organization/{organization_id}"}})
 
-        # Create the organization entry
-        list_entry = BundleEntry({"resource": point_of_care_list})
+        # Add List object to bundle.
+        list_entry = BundleEntry()
+        list_entry.resource = List(points_of_care_list)
         list_entry.request = list_request
 
-        # Add it
+        # Add the updated List to the transaction
         bundle.entry.append(list_entry)
 
         # Post the transaction
-        response = requests.post(FHIR.service_url(), json=bundle.as_json())
+        response = requests.post(PPM.fhir_url(), json=bundle.as_json())
         response.raise_for_status()
 
-        # Return the flattened list with the new organization
-        points_of_care.append(point_of_care)
-
-        return points_of_care
+        return [o["name"] for o in organizations] + points_of_care
 
     @staticmethod
     def update_twitter(patient_id, handle=None, uses_twitter=None):
         """
         Accepts details of a Twitter integration and updates the Patient record.
         A handle automatically sets the 'uses-twitter' extension as true, whereas
         no handle and no value for 'uses-twitter' deletes the extension and the
@@ -3530,15 +3833,15 @@
         out of the integration
         :return: bool
         """
         logger.debug("Twitter handle: {}, Uses Twitter: {}".format(handle, uses_twitter))
 
         try:
             # Fetch the Patient.
-            url = furl(FHIR.service_url())
+            url = furl(PPM.fhir_url())
             url.path.segments.extend(["Patient"])
 
             # Add patient query
             url.query.params.update(FHIR._patient_query(patient_id))
 
             # Make the request
             response = requests.get(url.url)
@@ -3619,15 +3922,15 @@
         :param value: The value to set: str, bool, int or None
         :return: bool
         """
         logger.debug('Patient extension: "{}" -> "{}"'.format(extension_url, value))
 
         try:
             # Fetch the Patient.
-            url = furl(FHIR.service_url())
+            url = furl(PPM.fhir_url())
             url.path.segments.extend(["Patient"])
 
             # Add patient query
             url.query.params.update(FHIR._patient_query(patient_id))
 
             # Get the data
             response = requests.get(url.url)
@@ -3691,15 +3994,15 @@
 
     @staticmethod
     def update_picnichealth(patient_id, registered=True):
         logger.debug("Picnichealth registration: {} -> {}".format(patient_id, registered))
 
         try:
             # Fetch the Patient.
-            url = furl(FHIR.service_url())
+            url = furl(PPM.fhir_url())
             url.path.segments.extend(["Patient"])
             url.query.params.update(FHIR._patient_query(patient_id))
             response = requests.get(url.url)
             response.raise_for_status()
             patient = response.json().get("entry")[0]["resource"]
 
             # Check for an existing Twitter status extension
@@ -3742,15 +4045,15 @@
     @staticmethod
     def update_document_reference(document_reference, status="current"):
         logger.debug("Supersede DocumentReference: {}".format(document_reference["id"]))
 
         patient_ref = None
         try:
             # Build the URL
-            url = furl(FHIR.service_url())
+            url = furl(PPM.fhir_url())
             url.path.segments.extend(["DocumentReference", document_reference["id"]])
 
             # Get the patient reference
             patient_ref = document_reference["subject"]["reference"]
 
             # Set headers for patch operation
             headers = {"Content-Type": "application/json-patch+json"}
@@ -3774,14 +4077,140 @@
                     "document_reference": document_reference,
                     "patient": patient_ref,
                 },
             )
 
         return False
 
+    @staticmethod
+    def update_questionnaire_response(patient, questionnaire_id, questionnaire_response_id, questionnaire_response):
+        """
+        Updates a participant's questionnaire response.
+
+        :param patient: The patient's identifier
+        :type patient: str
+        :param questionnaire_id: The ID of the Questionnaire the response was for
+        :type questionnaire_id: str
+        :param questionnaire_response_id: The ID of the QuestionnaireResponse to update
+        :type questionnaire_response_id: str
+        :param questionnaire_response: The update QuestionnaireResponse object to persist
+        :type questionnaire_response: dict
+        :return: True if the resource was updated, False if failed
+        :rtype: boolean
+        """
+        logger.debug(
+            f"PPM/{patient}/Questionnaire/{questionnaire_id}: "
+            f"Updating QuestionnaireResponse/{questionnaire_response_id}"
+        )
+
+        try:
+            # Ensure the ID is set on the resource
+            questionnaire_response["id"] = questionnaire_response_id
+
+            # Build the URL
+            url = furl(PPM.fhir_url())
+            url.path.segments.append("QuestionnaireResponse")
+            url.path.segments.append(questionnaire_response_id)
+
+            # Put it
+            response = requests.put(url.url, json=questionnaire_response)
+            response.raise_for_status()
+
+            return response.ok
+
+        except requests.HTTPError as e:
+            logger.debug(f"PPM/{patient}: FHIR response: {e.response}")
+            logger.error(
+                f"PPM/{patient}: FHIR Request Error: {e}",
+                extra={
+                    "patient": patient,
+                    "response": e.response.content,
+                    "questionnaire_id": questionnaire_id,
+                    "questionnaire_response_id": questionnaire_response_id,
+                },
+            )
+
+        except Exception as e:
+            logger.error(
+                f"PPM/{patient}: FHIR Error: {e}",
+                exc_info=True,
+                extra={
+                    "patient": patient,
+                    "questionnaire_id": questionnaire_id,
+                    "questionnaire_response_id": questionnaire_response_id,
+                },
+            )
+
+        return False
+
+    @staticmethod
+    def update_or_create_questionnaire_response(patient, questionnaire_id, questionnaire_response):
+        """
+        Updates or creates (if none exist for the given Questionnaire)
+        a participant's questionnaire response.
+
+        :param patient: The patient's identifier
+        :type patient: str
+        :param questionnaire_id: The ID of the Questionnaire the response was for
+        :type questionnaire_id: str
+        :param questionnaire_response: The update QuestionnaireResponse object to persist
+        :type questionnaire_response: dict
+        :return: True if the resource was created/updated, False if failed
+        :rtype: boolean
+        """
+        logger.debug(f"PPM/{patient}: Update/create response for Questionnaire/{questionnaire_id}")
+
+        questionnaire_response_id = None
+        try:
+            # Get the existing questionnaire response
+            questionnaire_responses = FHIR.query_questionnaire_responses(
+                patient=patient,
+                questionnaire_id=questionnaire_id,
+            )
+
+            # Ensure only one, else raise exception
+            if len(questionnaire_responses) > 1:
+                raise RuntimeError(
+                    "Found multiple QuestionnaireResponse resources for " f"{patient}/Questionnaire/{questionnaire_id}"
+                )
+
+            # Check if it exists and create if necessary
+            if not questionnaire_responses:
+                logger.debug(f"PPM/{patient}: Create QuestionnaireResponse")
+                return FHIR.save_questionnaire_response(
+                    patient_id=patient,
+                    questionnaire_id=questionnaire_id,
+                    questionnaire_response=questionnaire_response,
+                )
+
+            # Get the ID
+            questionnaire_response_id = next(entry.resource.id for entry in questionnaire_responses.entry)
+
+            # Do the update
+            logger.debug(f"PPM/{patient}: Update QuestionnaireResponse/{questionnaire_response_id}")
+            return FHIR.update_questionnaire_response(
+                patient=patient,
+                questionnaire_id=questionnaire_id,
+                questionnaire_response_id=questionnaire_response_id,
+                questionnaire_response=questionnaire_response,
+            )
+
+        except Exception as e:
+            logger.error(
+                f"PPM/{patient}: FHIR Error: {e}",
+                exc_info=True,
+                extra={
+                    "patient": patient,
+                    "questionnaire_id": questionnaire_id,
+                    "questionnaire_response_id": questionnaire_response_id,
+                },
+            )
+
+        return False
+
     #
     # DELETE
     #
 
     @staticmethod
     def _delete_resources(source_resource_type, source_resource_id, target_resource_types=[]):
         """
@@ -3802,15 +4231,15 @@
         :rtype: Bool
         """
         content = None
         try:
             logger.debug("Target resource: {}/{}".format(source_resource_type, source_resource_id))
             logger.debug("Target related resources: {}".format(target_resource_types))
 
-            source_url = furl(FHIR.service_url())
+            source_url = furl(PPM.fhir_url())
             source_url.path.add(source_resource_type)
             source_url.query.params.add("_id", source_resource_id)
             source_url.query.params.add("_include", "*")
             source_url.query.params.add("_revinclude", "*")
 
             # Make the request.
             source_response = requests.get(source_url.url)
@@ -3837,15 +4266,17 @@
                 logger.debug("Add: {}".format(resource_id))
                 transaction["entry"].append({"request": {"url": resource_id, "method": "DELETE"}})
 
             logger.debug("Delete request: {}".format(json.dumps(transaction)))
 
             # Do the delete.
             response = requests.post(
-                FHIR.service_url(), headers={"content-type": "application/json"}, data=json.dumps(transaction)
+                PPM.fhir_url(),
+                headers={"content-type": "application/json"},
+                data=json.dumps(transaction),
             )
             response.raise_for_status()
 
             # Log it.
             logger.debug("Delete response: {}".format(response.content))
             logger.debug(
                 "Successfully deleted all for resource: {}/{}".format(source_resource_type, source_resource_id)
@@ -3870,15 +4301,15 @@
     def _delete_resource(resource_type, resource_id):
         logger.debug("Delete request: {}/{}".format(resource_type, resource_id))
 
         content = None
         url = None
         try:
             # Build the URL
-            url = furl(FHIR.service_url())
+            url = furl(PPM.fhir_url())
             url.path.segments.append(resource_type)
             url.path.segments.append(resource_id)
 
             # Do the delete.
             response = requests.delete(url.url)
             response.raise_for_status()
 
@@ -4087,15 +4518,15 @@
                     }
                 }
             )
 
         elif PPM.Study.get(project) is PPM.Study.NEER:
 
             # Delete questionnaire responses
-            questionnaire_ids = ["neer-signature", "neer-signature-v2"]
+            questionnaire_ids = ["neer-signature", "neer-signature-v2", "neer-signature-v3"]
             for questionnaire_id in questionnaire_ids:
                 transaction["entry"].append(
                     {
                         "request": {
                             "url": "QuestionnaireResponse?"
                             "questionnaire=Questionnaire/{}&source=Patient/{}".format(questionnaire_id, patient_id),
                             "method": "DELETE",
@@ -4138,15 +4569,17 @@
                 )
 
         else:
             logger.error("Unsupported project: {}".format(project), extra={"ppm_id": patient_id})
 
         # Make the FHIR request.
         response = requests.post(
-            FHIR.service_url(), headers={"content-type": "application/json"}, data=json.dumps(transaction)
+            PPM.fhir_url(),
+            headers={"content-type": "application/json"},
+            data=json.dumps(transaction),
         )
         response.raise_for_status()
 
     #
     # BUNDLES
     #
 
@@ -4159,15 +4592,15 @@
             logger.debug("No Research Subjects, no Research Studies")
             return None
 
         # Get study IDs
         research_study_ids = [subject["study"]["reference"].split("/")[1] for subject in subjects]
 
         # Make the query
-        research_study_url = furl(FHIR.service_url())
+        research_study_url = furl(PPM.fhir_url())
         research_study_url.path.add("ResearchStudy")
         research_study_url.query.params.add("_id", ",".join(research_study_ids))
 
         # Fetch them
         research_study_response = requests.get(research_study_url.url)
 
         # Get the IDs
@@ -4188,15 +4621,15 @@
             logger.debug("No Research Subjects, no Research Studies")
             return None
 
         # Get study IDs
         research_study_ids = [subject["study"]["reference"].split("/")[1] for subject in subjects]
 
         # Make the query
-        research_study_url = furl(FHIR.service_url())
+        research_study_url = furl(PPM.fhir_url())
         research_study_url.path.add("ResearchStudy")
         research_study_url.query.params.add("_id", ",".join(research_study_ids))
 
         # Fetch them
         research_study_response = requests.get(research_study_url.url)
 
         # Get the IDs
@@ -4250,15 +4683,15 @@
     #
 
     @staticmethod
     def get_ppm_id(email):
 
         try:
             # Get the client
-            client = FHIR.get_client(FHIR.service_url())
+            client = FHIR.get_client(PPM.fhir_url())
 
             # Query the Patient
             search = Patient.where(struct={"identifier": "http://schema.org/email|{}".format(email)})
             resources = search.perform_resources(client.server)
             for resource in resources:
 
                 # Return the ID of the first Patient
@@ -4305,22 +4738,24 @@
 
         if not names:
             names = ["Participant"]
 
         return " ".join(names)
 
     @staticmethod
-    def flatten_participant(bundle, questionnaire_ids=None):
+    def flatten_participant(bundle, study=None, questionnaires=None):
         """
         Accepts a Bundle containing everything related to a Patient resource
         and flattens the data into something easier to build templates/views with.
         :param bundle: The Patient resource bundle as JSON/dict
         :type bundle: dict
-        :param questionnaire_ids: A dictionary of Questionnaires to include if available
-        :type questionnaire_ids: dict, defaults to None
+        :param study: The study for which this participant's record should be constructed
+        :type study: str, defaults to None
+        :param questionnaires: The survey/questionnaires for the study
+        :type questionnaires: str, defaults to None
         :return: A flattened dictionary of the Participant/Patient's entire FHIR data record
         :rtype: dict
         """
 
         # Build a dictionary
         participant = {}
 
@@ -4335,21 +4770,52 @@
                 logger.debug("No Patient in bundle")
                 return {}
 
             # Get props
             ppm_id = participant["fhir_id"]
             email = participant["email"]
 
+            ####################################################################
+            # Study
+            ####################################################################
+
             # Get the PPM study/project resources
             studies = FHIR.flatten_ppm_studies(bundle)
-            if len(studies) > 1:
-                logger.warning("Patient/{} has more than one PPM study: {}".format(ppm_id, studies))
+
+            # Ensure they are in this study
+            if study and not next((s for s in studies if s["study"] == study), None):
+                logger.error(
+                    f"PPM/{ppm_id}: Participant no in study: {study}",
+                    extra={"study": study, "ppm_id": ppm_id, "studies": studies},
+                )
+                raise ValueError(f"Participant does not exist in study {study}")
+
+            # If they're in multiple studies, ensure the specific study is defined
+            elif not study and len(studies) > 1:
+                logger.error(
+                    f"PPM/{ppm_id}: Multiple PPM studies: {studies}",
+                    extra={"study": study, "ppm_id": ppm_id, "studies": studies},
+                )
+                raise ValueError("Participant has multiple studies but requested study has not been defined")
+
+            # If study wasn't passed, get it from the single entry list
+            elif not study:
+
+                # Get the study from the bundle
+                study = studies[0]["study"]
+
+            # Validate it
+            study = PPM.Study.enum(study).value
+
+            ####################################################################
+            # Enrollment
+            ####################################################################
 
             # Check for accepted and a start date
-            participant["project"] = participant["study"] = studies[0]["study"]
+            participant["project"] = participant["study"] = study
             participant["date_registered"] = FHIR._format_date(studies[0]["start"], "%m/%d/%Y")
             participant["datetime_registered"] = studies[0]["start"]
 
             # Get the enrollment properties
             enrollment = FHIR.flatten_enrollment(bundle)
 
             # Set status and dates
@@ -4369,136 +4835,174 @@
 
                 # Convert time zone to assumed ET
                 participant["enrollment_terminated_date"] = FHIR._format_date(enrollment["end"], "%m/%d/%Y")
             #
             # else:
             #     participant['enrollment_terminated_date'] = ''
 
+            ####################################################################
+            # Consent
+            ####################################################################
+
             # Flatten consent composition
             participant["composition"] = FHIR.flatten_consent_composition(bundle)
 
-            # Get the project
-            _questionnaire_id = PPM.Questionnaire.questionnaire_for_study(study=participant["project"])
+            ####################################################################
+            # Questionnaires
+            ####################################################################
+
+            # Collect flattened questionnaires
+            participant["questionnaires"] = {}
+
+            # If not specified, use the value hard-coded in the PPM module
+            if not questionnaires:
+                eligibility_questionnaire_id = PPM.Questionnaire.questionnaire_for_study(study=study)
+                logger.warning(
+                    f"PPM/{study}/{ppm_id}: Using deprecated PPM.Questionnaire eligibility questionnaires: "
+                    f" {eligibility_questionnaire_id}"
+                )
+            else:
+                # Get needed questionnaire IDs
+                eligibility_questionnaire_id = next(
+                    (q["questionnaire_id"] for q in questionnaires if q.get("eligibility_for") == study),
+                    PPM.Questionnaire.questionnaire_for_study(study=study),
+                )
 
-            # Parse out the responses
-            questionnaire_response = FHIR.flatten_questionnaire_response(bundle, _questionnaire_id)
+            # Handle eligibility questionnaire
+            logger.debug(f"PPM/{study}/{ppm_id}: Eligibility questionnaire: {eligibility_questionnaire_id}")
+            questionnaire = FHIR.flatten_questionnaire_response(bundle, eligibility_questionnaire_id)
+            participant["questionnaire"] = participant["questionnaires"][eligibility_questionnaire_id] = questionnaire
+
+            # If not specified, use hard-coded questionnaire IDs from PPM module
+            if not questionnaires:
+                questionnaire_ids = [q.value for q in PPM.Questionnaire.extra_questionnaires_for_study(study=study)]
+                logger.warning(
+                    f"PPM/{study}/{ppm_id}: Using deprecated PPM.Questionnaire questionnaires: " f" {questionnaire_ids}"
+                )
+            else:
+                questionnaire_ids = [q["questionnaire_id"] for q in questionnaires if q.get("questionnaire_id")]
+
+            # Parse remaining questionnaires
+            logger.debug(f"PPM/{study}/{ppm_id}: Study questionnaires: {questionnaire_ids}")
+            for questionnaire_id in questionnaire_ids:
 
-            # Add primary questionnaire and all questionnaires
-            participant["questionnaire"] = questionnaire_response
-            participant["questionnaires"] = {_questionnaire_id: questionnaire_response}
-
-            # Add additional questionnaires
-            for questionnaire in PPM.Questionnaire.extra_questionnaires_for_study(participant["project"]):
-
-                # Attempt to parse it
-                participant["questionnaires"][questionnaire.value] = FHIR.flatten_questionnaire_response(
-                    bundle, questionnaire.value
+                # Parse it and add it
+                participant["questionnaires"][questionnaire_id] = FHIR.flatten_questionnaire_response(
+                    bundle, questionnaire_id
                 )
 
-            # Add additional questionnaires
-            if questionnaire_ids:
-                for questionnaire_id in questionnaire_ids:
-
-                    # Attempt to parse it
-                    participant["questionnaires"][questionnaire_id] = FHIR.flatten_questionnaire_response(
-                        bundle, questionnaire_id
-                    )
+            ####################################################################
+            # Points of care
+            ####################################################################
 
             # Flatten points of care
             participant["points_of_care"] = FHIR.flatten_list(bundle, "Organization")
 
+            ####################################################################
+            # Devices
+            ####################################################################
+
             # Flatten consent composition
             participant["devices"] = FHIR.flatten_ppm_devices(bundle)
 
+            ####################################################################
+            # Research Studies
+            ####################################################################
+
             # Check for research studies
             research_studies = FHIR.get_research_studies(bundle)
             if research_studies:
                 participant["research_studies"] = research_studies
 
-            # Autism has a special consent with a quiz, get that content and add it
-            if participant["project"] == PPM.Study.ASD.value:
-
-                # Initially none
-                participant["consent_quiz"] = None
-                participant["consent_quiz_answers"] = None
-
-                # Check if they've even consented
-                if participant.get("composition"):
-
-                    # Get the Questionnaire ID used for the quiz portion of the consent
-                    quiz_id = PPM.Questionnaire.questionnaire_for_consent(participant.get("composition"))
-
-                    # Flatten the Q's and A's for output
-                    quiz = FHIR.flatten_questionnaire_response(bundle, quiz_id)
-                    if quiz:
-
-                        # Add it
-                        participant["consent_quiz"] = quiz
-                        participant["consent_quiz_answers"] = FHIR.questionnaire_answers(bundle, quiz_id)
+            ####################################################################
+            # Study-sepcific Resources
+            ####################################################################
 
             # Get study specific resources
-            if hasattr(FHIR, f"_flatten_{PPM.Study.enum(participant['study']).value}_participant"):
+            if hasattr(FHIR, f"_flatten_{study}_participant"):
 
                 # Run it
-                values, study_values = getattr(
-                    FHIR, f"_flatten_{PPM.Study.enum(participant['study']).value}_participant"
-                )(bundle=bundle, ppm_id=ppm_id)
+                values, study_values = getattr(FHIR, f"_flatten_{study}_participant")(
+                    bundle=bundle,
+                    ppm_id=ppm_id,
+                    questionnaires=questionnaires,
+                )
 
                 # Set them
                 participant.update(values)
-                participant[PPM.Study.enum(participant["study"]).value] = study_values
+                participant[study] = study_values
 
         except Exception as e:
             logger.exception(
                 "FHIR error: {}".format(e),
                 exc_info=True,
-                extra={"ppm_id": ppm_id, "email": email},
+                extra={"study": study, "ppm_id": ppm_id, "email": email},
             )
 
         return participant
 
     @staticmethod
-    def _flatten_asd_participant(bundle, ppm_id):
+    def _flatten_asd_participant(bundle, ppm_id, questionnaires=None):
         """
         Continues flattening a participant by adding any study specific data to
         their record. This will include answers in questionnaires, etc. Returns
         a dictionary to merge into the root participant dictionary as well as
         a dictionary that will be keyed by the study value.
 
         :param bundle: The participant's entire FHIR record
         :type bundle: dict
         :param ppm_id: The PPM ID of the participant
         :type ppm_id: str
+        :param questionnaires: The survey/questionnaires for the study
+        :type questionnaires: str, defaults to None
         :returns: A tuple of properties for the root participant object, and for
         the study sub-object
         :rtype: dict, dict
         """
         logger.debug(f"PPM/{ppm_id}/FHIR: Flattening ASD participant")
 
         # Put values and study values in dictionaries
         values = {}
         study_values = {}
 
-        # TODO: Implement this
-        logger.warning(f"PPM/ASD/{ppm_id}/FHIR: Flattening ASD participant needs to be fully implemented")
+        # Initially none
+        values["consent_quiz"] = None
+        values["consent_quiz_answers"] = None
+
+        # Check if they've even consented
+        composition = FHIR.flatten_consent_composition(bundle)
+        if composition:
+
+            # Get the Questionnaire ID used for the quiz portion of the consent
+            quiz_id = PPM.Questionnaire.questionnaire_for_consent(composition)
+
+            # Flatten the Q's and A's for output
+            quiz = FHIR.flatten_questionnaire_response(bundle, quiz_id)
+            if quiz:
+
+                # Add it
+                values["consent_quiz"] = quiz
+                values["consent_quiz_answers"] = FHIR.questionnaire_answers(bundle, quiz_id)
 
         return values, study_values
 
     @staticmethod
-    def _flatten_neer_participant(bundle, ppm_id):
+    def _flatten_neer_participant(bundle, ppm_id, questionnaires=None):
         """
         Continues flattening a participant by adding any study specific data to
         their record. This will include answers in questionnaires, etc. Returns
         a dictionary to merge into the root participant dictionary as well as
         a dictionary that will be keyed by the study value.
 
         :param bundle: The participant's entire FHIR record
         :type bundle: dict
         :param ppm_id: The PPM ID of the participant
         :type ppm_id: str
+        :param questionnaires: The survey/questionnaires for the study
+        :type questionnaires: str, defaults to None
         :returns: A tuple of properties for the root participant object, and for
         the study sub-object
         :rtype: dict, dict
         """
         logger.debug(f"PPM/{ppm_id}/FHIR: Flattening NEER participant")
 
         # Put values and study values in dictionaries
@@ -4606,296 +5110,334 @@
 
                     # Assign default value
                     study_values[key] = "---"
 
         return values, study_values
 
     @staticmethod
-    def _flatten_rant_participant(bundle, ppm_id):
+    def _flatten_rant_participant(bundle, ppm_id, questionnaires=None):
         """
         Continues flattening a participant by adding any study specific data to
         their record. This will include answers in questionnaires, etc. Returns
         a dictionary to merge into the root participant dictionary as well as
         a dictionary that will be keyed by the study value.
 
         :param bundle: The participant's entire FHIR record
         :type bundle: dict
         :param ppm_id: The PPM ID of the participant
         :type ppm_id: str
+        :param questionnaires: The survey/questionnaires for the study
+        :type questionnaires: str, defaults to None
         :returns: A tuple of properties for the root participant object, and for
         the study sub-object
         :rtype: dict, dict
         """
         logger.debug(f"PPM/{ppm_id}/FHIR: Flattening RANT participant")
 
         # Put values and study values in dictionaries
         values = {}
         study_values = {}
 
-        # Check for points of care questionnaire
-        questionnaire_response = next(
-            (
-                q
-                for q in FHIR._find_resources(bundle, "QuestionnaireResponse")
-                if q["questionnaire"]["reference"]
-                == f"Questionnaire/{PPM.Questionnaire.RANTPointsOfCareQuestionnaire.value}"
-            ),
-            None,
-        )
-        if questionnaire_response:
-
-            # Set a list
-            values["points_of_care"] = []
+        # Check for questionnaires
+        if questionnaires:
 
-            # Parse answers
-            diagnosing_name = next(
-                (
-                    next(a["valueString"] for a in i["answer"])
-                    for i in questionnaire_response["item"]
-                    if i["linkId"] == "question-1"
-                ),
-                None,
-            )
-            diagnosing_address = next(
-                (
-                    next(a["valueString"] for a in i["answer"])
-                    for i in questionnaire_response["item"]
-                    if i["linkId"] == "question-2"
-                ),
+            # Get needed questionnaire IDs
+            points_of_care_questionnaire_id = next(
+                (q["questionnaire_id"] for q in questionnaires if q.get("points_of_care_for") == PPM.Study.RANT.value),
                 None,
             )
-            diagnosing_phone = next(
-                (
-                    next(a["valueString"] for a in i["answer"])
-                    for i in questionnaire_response["item"]
-                    if i["linkId"] == "question-3"
-                ),
-                None,
+
+            # Add them
+            study_values["points_of_care"] = FHIR._flatten_rant_points_of_care(
+                bundle=bundle,
+                ppm_id=ppm_id,
+                questionnaire_id=points_of_care_questionnaire_id,
             )
 
-            # Add it.
-            values["points_of_care"].append(f"{diagnosing_name}, {diagnosing_phone}, {diagnosing_address}")
+        return values, study_values
 
-            # Check for another
-            if (
-                next(
-                    (
-                        next(a["valueString"] for a in i["answer"])
-                        for i in questionnaire_response["item"]
-                        if i["linkId"] == "question-4"
-                    ),
-                    "",
-                )
-                == "No"
-            ):
+    @staticmethod
+    def _flatten_example_participant(bundle, ppm_id, questionnaires=None):
+        """
+        Continues flattening a participant by adding any study specific data to
+        their record. This will include answers in questionnaires, etc. Returns
+        a dictionary to merge into the root participant dictionary as well as
+        a dictionary that will be keyed by the study value.
 
-                # Parse answers
-                current_name = next(
-                    (
-                        next(a["valueString"] for a in i["answer"])
-                        for i in questionnaire_response["item"]
-                        if i["linkId"] == "question-5"
-                    ),
-                    None,
-                )
-                current_address = next(
-                    (
-                        next(a["valueString"] for a in i["answer"])
-                        for i in questionnaire_response["item"]
-                        if i["linkId"] == "question-6"
-                    ),
-                    None,
-                )
-                current_phone = next(
-                    (
-                        next(a["valueString"] for a in i["answer"])
-                        for i in questionnaire_response["item"]
-                        if i["linkId"] == "question-7"
-                    ),
-                    None,
-                )
+        :param bundle: The participant's entire FHIR record
+        :type bundle: dict
+        :param ppm_id: The PPM ID of the participant
+        :type ppm_id: str
+        :param questionnaires: The survey/questionnaires for the study
+        :type questionnaires: str, defaults to None
+        :returns: A tuple of properties for the root participant object, and for
+        the study sub-object
+        :rtype: dict, dict
+        """
+        logger.debug(f"PPM/{ppm_id}/FHIR: Flattening EXAMPLE participant")
 
-                # Add it.
-                values["points_of_care"].append(f"{current_name}, {current_phone}, {current_address}")
+        # Put values and study values in dictionaries
+        values = {}
+        study_values = {}
 
-            # Get remaining RA places
-            additional_ra_points_of_care = next(
+        # Check for passed questionnaires
+        if questionnaires:
+
+            # Get needed questionnaire IDs
+            points_of_care_questionnaire_id = next(
                 (
-                    next(a["valueString"] for a in i["answer"])
-                    for i in questionnaire_response["item"]
-                    if i["linkId"] == "question-8"
+                    q["questionnaire_id"]
+                    for q in questionnaires
+                    if q.get("points_of_care_for") == PPM.Study.EXAMPLE.value
                 ),
                 None,
             )
-            if additional_ra_points_of_care:
-                values["points_of_care"].append(additional_ra_points_of_care)
 
-            # Check for another
-            if (
-                next(
-                    (
-                        next(a["valueString"] for a in i["answer"])
-                        for i in questionnaire_response["item"]
-                        if i["linkId"] == "question-9"
-                    ),
-                    "",
-                )
-                == "Yes"
-            ):
-
-                # Get remaining places
-                additional_points_of_care = next(
-                    (
-                        next(a["valueString"] for a in i["answer"])
-                        for i in questionnaire_response["item"]
-                        if i["linkId"] == "question-10"
-                    ),
-                    None,
-                )
-                if additional_points_of_care:
-                    values["points_of_care"].append(additional_points_of_care)
+            # Add them
+            study_values["points_of_care"] = FHIR._flatten_rant_points_of_care(
+                bundle=bundle,
+                ppm_id=ppm_id,
+                questionnaire_id=points_of_care_questionnaire_id,
+            )
 
         return values, study_values
 
     @staticmethod
-    def _flatten_example_participant(bundle, ppm_id):
+    def _flatten_rant_points_of_care(bundle, ppm_id, questionnaire_id):
         """
         Continues flattening a participant by adding any study specific data to
         their record. This will include answers in questionnaires, etc. Returns
         a dictionary to merge into the root participant dictionary as well as
         a dictionary that will be keyed by the study value.
 
         :param bundle: The participant's entire FHIR record
         :type bundle: dict
         :param ppm_id: The PPM ID of the participant
         :type ppm_id: str
-        :returns: A tuple of properties for the root participant object, and for
-        the study sub-object
-        :rtype: dict, dict
+        :param questionnaire_id: The questionnaire ID containing points of care
+        :type questionnaire_id: str, defaults to None
+        :returns: A list of points of care parsed from questionnaire
+        :rtype: list
         """
-        logger.debug(f"PPM/{ppm_id}/FHIR: Flattening EXAMPLE participant")
-
-        # Put values and study values in dictionaries
-        values = {}
-        study_values = {}
+        # Set a list
+        points_of_care = []
 
         # Get questionnaire answers
         questionnaire_response = next(
             (
                 q
                 for q in FHIR._find_resources(bundle, "QuestionnaireResponse")
-                if q["questionnaire"]["reference"] == f"Questionnaire/{PPM.Questionnaire.EXAMPLEQuestionnaire.value}"
+                if q["questionnaire"]["reference"] == f"Questionnaire/{questionnaire_id}"
             ),
             None,
         )
-        if questionnaire_response:
-            logger.debug(f"PPM/{ppm_id}/FHIR: Flattening QuestionnaireResponse/" f'{questionnaire_response["id"]}')
-
-            # Map linkIds to keys
-            text_answers = {
-                "question-12": "diagnosis",
-                "question-24": "pcp",
-                "question-25": "oncologist",
-            }
+        if not questionnaire_response or not questionnaire_response.get("item"):
+            logger.debug(f"PPM/FHIR/{questionnaire_id}/{ppm_id}: No response items")
+            return None
 
-            date_answers = {
-                "question-5": "birthdate",
-                "question-14": "date_diagnosis",
-            }
+        # Parse answers
+        diagnosing_name = FHIR.get_questionnaire_response_item_value(
+            questionnaire_response=questionnaire_response,
+            link_id="question-1",
+        )
+        diagnosing_address = FHIR.get_questionnaire_response_item_value(
+            questionnaire_response=questionnaire_response,
+            link_id="question-2",
+        )
+        diagnosing_phone = FHIR.get_questionnaire_response_item_value(
+            questionnaire_response=questionnaire_response,
+            link_id="question-3",
+        )
 
-            # Iterate items
-            for link_id, key in text_answers.items():
-                try:
-                    # Get the answer
-                    answer = next(
-                        i["answer"][0]["valueString"] for i in questionnaire_response["item"] if i["linkId"] == link_id
-                    )
+        # Add it.
+        points_of_care.append(f"{diagnosing_name}, {diagnosing_phone}, {diagnosing_address}")
 
-                    # Assign it
-                    study_values[key] = answer
-                except Exception as e:
-                    logger.exception(
-                        f"PPM/{ppm_id}/Questionnaire/{link_id}: {e}",
-                        exc_info=True,
-                        extra={
-                            "ppm_id": ppm_id,
-                            "link_id": link_id,
-                            "key": key,
-                            "questionnaire_response": f"QuestionnaireResponse/" f'{questionnaire_response["id"]}',
-                            "item": next(
-                                (i for i in questionnaire_response["item"] if i["linkId"] == link_id),
-                                "",
-                            ),
-                        },
-                    )
+        # Check for another
+        if (
+            FHIR.get_questionnaire_response_item_value(
+                questionnaire_response=questionnaire_response, link_id="question-4"
+            )
+            == "No"
+        ):
 
-                    # Assign default value
-                    study_values[key] = "---"
+            # Parse answers
+            current_name = FHIR.get_questionnaire_response_item_value(
+                questionnaire_response=questionnaire_response,
+                link_id="question-5",
+            )
+            current_address = FHIR.get_questionnaire_response_item_value(
+                questionnaire_response=questionnaire_response,
+                link_id="question-6",
+            )
+            current_phone = FHIR.get_questionnaire_response_item_value(
+                questionnaire_response=questionnaire_response,
+                link_id="question-7",
+            )
 
-            # Iterate date items and attempt to parse dates, otherwise treat as text
-            for link_id, key in date_answers.items():
+            # Add it.
+            points_of_care.append(f"{current_name}, {current_phone}, {current_address}")
 
-                try:
-                    # Get the answer
-                    answer = next(i["answer"][0] for i in questionnaire_response["item"] if i["linkId"] == link_id)
+        # Get remaining RA places
+        additional_ra_points_of_care = FHIR.get_questionnaire_response_item_value(
+            questionnaire_response=questionnaire_response,
+            link_id="question-8",
+        )
+        if additional_ra_points_of_care:
+            points_of_care.append(additional_ra_points_of_care)
 
-                    try:
-                        # Check type
-                        if answer.get("valueDate") or answer.get("valueDateTime"):
-                            # Date is already a date object, assign it
-                            study_values[key] = answer.get("valueDate", answer.get("valueDateTime"))
+        # Check for another
+        if (
+            FHIR.get_questionnaire_response_item_value(
+                questionnaire_response=questionnaire_response, link_id="question-9"
+            )
+            == "Yes"
+        ):
 
-                        elif answer.get("valueString"):
+            # Get remaining places
+            additional_points_of_care = FHIR.get_questionnaire_response_item_value(
+                questionnaire_response=questionnaire_response,
+                link_id="question-10",
+            )
+            if additional_points_of_care:
+                points_of_care.append(additional_points_of_care)
 
-                            # Attempt to parse it
-                            answer_date = parse(answer.get("valueString"))
+        return points_of_care
 
-                            # Assign it
-                            study_values[key] = answer_date.isoformat()
+    @staticmethod
+    def get_questionnaire_response_item_value(questionnaire_response, link_id):
+        """
+        Returns the value for the given questionnaire response and link ID.
 
-                        else:
-                            logger.error(f"PPM/{ppm_id}/Questionnaire/{link_id}: Unhandled answer type: {answer}")
+        :param questionnaire_response: The QuestionnaireResponse resource to check
+        :type questionnaire_response: dict
+        :param link_id: The link ID of the item's value to return
+        :type link_id: str
+        :param first: Return the first found answer value
+        :type first: boolean
+        :return: The value object, if it exists
+        :rtype: object, defaults to None
+        """
+        # Get answer value(s)
+        values = FHIR.get_questionnaire_response_item_values(
+            questionnaire_response=questionnaire_response, link_id=link_id
+        )
+        if values and len(values) > 1:
+            # Get IDs
+            questionnaire_id = questionnaire_response["questionnaire"]["reference"].replace("Questionnaire/", "")
+            questionnaire_response_id = questionnaire_response["id"]
+            logger.debug(
+                f"PPM/FHIR/{questionnaire_id}/{questionnaire_response_id}/{link_id}: Ignoring other answer values"
+            )
+        return next(iter(values)) if values else None
 
-                    except ValueError:
-                        logger.debug(f"PPM/{ppm_id}/Questionnaire/{link_id}: Invalid date: {answer}")
+    @staticmethod
+    def get_questionnaire_response_item_values(questionnaire_response, link_id):
+        """
+        Returns the value(s) for the given questionnaire response and link ID.
 
-                        # Assign the raw value
-                        study_values[key] = answer
+        :param questionnaire_response: The QuestionnaireResponse resource to check
+        :type questionnaire_response: dict
+        :param link_id: The link ID of the item's value to return
+        :type link_id: str
+        :param first: Return the first found answer value
+        :type first: boolean
+        :return: A list of value objects
+        :rtype: list
+        """
+        # Collect values
+        values = []
+        questionnaire_id = questionnaire_response_id = answer = None
+        try:
+            # Get IDs
+            questionnaire_id = questionnaire_response["questionnaire"]["reference"].replace("Questionnaire/", "")
+            questionnaire_response_id = questionnaire_response["id"]
+            logger.debug(f"PPM/FHIR/{questionnaire_id}/{questionnaire_response_id}/{link_id}: Getting answer value(s)")
+
+            # Get the item
+            answers = next(
+                (i.get("answer") for i in questionnaire_response["item"] if i["linkId"] == link_id),
+                None,
+            )
 
-                except Exception as e:
-                    logger.exception(
-                        f"PPM/{ppm_id}/Questionnaire/{link_id}: Missing response: {e}",
-                        exc_info=True,
-                        extra={
-                            "ppm_id": ppm_id,
-                            "link_id": link_id,
-                            "key": key,
-                            "questionnaire_response": f"QuestionnaireResponse/" f'{questionnaire_response["id"]}',
-                            "item": next(
-                                (i for i in questionnaire_response["item"] if i["linkId"] == link_id),
-                                "",
-                            ),
-                        },
+            # If answer, parse answer
+            if not answers:
+                logger.debug(f"PPM/FHIR/{questionnaire_id}/{questionnaire_response_id}/{link_id}: No answer for item")
+                return None
+
+            # Iterate values
+            for answer in answers:
+                # Check types
+                if answer.get("valueString"):
+                    values.append(answer["valueString"])
+                elif answer.get("valueBoolean"):
+                    values.append(answer["valueBoolean"])
+                elif answer.get("valueInteger"):
+                    values.append(answer["valueInteger"])
+                elif answer.get("valueDecimal"):
+                    values.append(answer["valueDecimal"])
+                elif answer.get("valueDate"):
+                    try:
+                        values.append(parse(answer["valueDate"]))
+                    except ValueError as e:
+                        logger.exception(
+                            f"PPM/FHIR: Date error: {e}",
+                            exc_info=True,
+                            extra={
+                                "questionnaire_id": questionnaire_id,
+                                "questionnaire_response": questionnaire_response_id,
+                                "link_id": link_id,
+                                "answer": answer,
+                            },
+                        )
+                elif answer.get("valueDateTime"):
+                    try:
+                        values.append(parse(answer["valueDateTime"]))
+                    except ValueError as e:
+                        logger.exception(
+                            f"PPM/FHIR: Date error: {e}",
+                            exc_info=True,
+                            extra={
+                                "questionnaire_id": questionnaire_id,
+                                "questionnaire_response": questionnaire_response_id,
+                                "link_id": link_id,
+                                "answer": answer,
+                            },
+                        )
+                else:
+                    logger.debug(
+                        f"PPM/FHIR/{questionnaire_id}/{questionnaire_response_id}/{link_id}: "
+                        f"Unhandled FHIR answer type: {answer}"
                     )
+                    raise ValueError(f"Unhandled FHIR answer type: {answer}")
 
-                    # Assign default value
-                    study_values[key] = "---"
+            return values
 
-        return values, study_values
+        except Exception as e:
+            logger.exception(
+                f"PPM/FHIR: Error getting item value: {e}",
+                exc_info=True,
+                extra={
+                    "questionnaire_id": questionnaire_id,
+                    "questionnaire_response": questionnaire_response_id,
+                    "link_id": link_id,
+                    "answer": answer,
+                },
+            )
 
     @staticmethod
     def flatten_questionnaire_response(bundle_dict, questionnaire_id):
         """
         Picks out the relevant Questionnaire and QuestionnaireResponse resources and
         returns a dict mapping the text of each question to a list of answer texts.
         To handle duplicate question texts, each question is prepended with an index.
         :param bundle_dict: The parsed JSON response from a FHIR query
         :param questionnaire_id: The ID of the Questionnaire to parse for
         :return: dict
         """
+        logger.debug(f"PPM/FHIR: Flattening {questionnaire_id}")
 
         # Build the bundle
         bundle = Bundle(bundle_dict)
 
         # Pick out the questionnaire and its response
         questionnaire = next(
             (entry.resource for entry in bundle.entry if entry.resource.id == questionnaire_id),
@@ -4909,175 +5451,190 @@
                 and entry.resource.questionnaire.reference == "Questionnaire/{}".format(questionnaire_id)
             ),
             None,
         )
 
         # Ensure resources exist
         if not questionnaire or not questionnaire_response:
-            logger.debug("User has no responses for Questionnaire/{}, returning".format(questionnaire_id))
+            logger.debug(f"PPM/FHIR: No response for Questionnaire/{questionnaire_id}")
             return None
 
-        # Get questions and answers
-        questions = FHIR._questions(questionnaire.item)
-        answers = FHIR._answers(questionnaire_response.item)
-
-        # Process sub-questions first
-        for linkId, condition in {
-            linkId: condition for linkId, condition in questions.items() if type(condition) is dict
-        }.items():
-            try:
-                # Assume only one condition, fetch the parent question linkId
-                parent = next(iter(condition))
-                if not parent:
-                    logger.warning(
-                        "FHIR Error: Subquestion not properly specified: {}:{}".format(linkId, condition),
-                        extra={
-                            "questionnaire": questionnaire_id,
-                            "ppm_id": questionnaire_response.source,
-                            "questionnaire_response": questionnaire_response.id,
-                        },
+        # If no items, return empty
+        if questionnaire_response.item:
+
+            # Get questions and answers
+            questions = FHIR.questionnaire_questions(questionnaire, questionnaire.item)
+            answers = FHIR.questionnaire_response_answers(
+                questionnaire, questionnaire_response, questionnaire_response.item
+            )
+
+            # Process sub-questions first
+            for linkId, condition in {
+                linkId: condition for linkId, condition in questions.items() if type(condition) is dict
+            }.items():
+                try:
+                    # Assume only one condition, fetch the parent question linkId
+                    parent = next(iter(condition))
+                    if not parent:
+                        logger.warning(
+                            "FHIR Error: Subquestion not properly specified: {}:{}".format(linkId, condition),
+                            extra={
+                                "questionnaire": questionnaire_id,
+                                "ppm_id": questionnaire_response.source,
+                                "questionnaire_response": questionnaire_response.id,
+                            },
+                        )
+                        continue
+
+                    if len(condition) > 1:
+                        logger.warning(
+                            "FHIR Error: Subquestion has multiple conditions: {}:{}".format(linkId, condition),
+                            extra={
+                                "questionnaire": questionnaire_id,
+                                "ppm_id": questionnaire_response.source,
+                                "questionnaire_response": questionnaire_response.id,
+                            },
+                        )
+
+                    # Ensure they've answered this one
+                    if not answers.get(parent) or condition[parent] not in answers.get(parent):
+                        continue
+
+                    # Get the question and answer item
+                    answer = answers[parent]
+                    index = answer.index(condition[parent])
+
+                    # Check for commas
+                    sub_answers = answers[linkId]
+                    if "," in next(iter(sub_answers)):
+
+                        # Split it
+                        sub_answers = [sub.strip() for sub in next(iter(sub_answers)).split(",")]
+
+                    # Format them
+                    value = '{} <span class="label label-primary">{}</span>'.format(
+                        answer[index],
+                        '</span>&nbsp;<span class="label label-primary">'.join(sub_answers),
                     )
-                    continue
 
-                if len(condition) > 1:
-                    logger.warning(
-                        "FHIR Error: Subquestion has multiple conditions: {}:{}".format(linkId, condition),
+                    # Append the value
+                    answer[index] = mark_safe(value)
+
+                except Exception as e:
+                    logger.exception(
+                        "FHIR error: {}".format(e),
+                        exc_info=True,
                         extra={
                             "questionnaire": questionnaire_id,
+                            "link_id": linkId,
                             "ppm_id": questionnaire_response.source,
-                            "questionnaire_response": questionnaire_response.id,
                         },
                     )
 
-                # Ensure they've answered this one
-                if not answers.get(parent) or condition[parent] not in answers.get(parent):
-                    continue
+            # Build the response
+            response = collections.OrderedDict()
 
-                # Get the question and answer item
-                answer = answers[parent]
-                index = answer.index(condition[parent])
-
-                # Check for commas
-                sub_answers = answers[linkId]
-                if "," in next(iter(sub_answers)):
-
-                    # Split it
-                    sub_answers = [sub.strip() for sub in next(iter(sub_answers)).split(",")]
-
-                # Format them
-                value = '{} <span class="label label-primary">{}</span>'.format(
-                    answer[index],
-                    '</span>&nbsp;<span class="label label-primary">'.join(sub_answers),
-                )
-
-                # Append the value
-                answer[index] = mark_safe(value)
-
-            except Exception as e:
-                logger.exception(
-                    "FHIR error: {}".format(e),
-                    exc_info=True,
-                    extra={
-                        "questionnaire": questionnaire_id,
-                        "link_id": linkId,
-                        "ppm_id": questionnaire_response.source,
-                    },
-                )
-
-        # Build the response
-        response = collections.OrderedDict()
+            # Determine index
+            indices = FHIR.get_answer_indices(questionnaire, questions)
+            for linkId, question in questions.items():
+
+                # Check for the answer
+                answer = answers.get(linkId)
+                if not answer:
+
+                    # Check if group or in a repeating group
+                    item = FHIR.find_questionnaire_item(questionnaire.item, linkId)
+
+                    # Skip repeating groups, those are handled below
+                    if FHIR.get_questionnaire_repeating_group(questionnaire, linkId):
+                        # If it's in a repeating group with no answer, then the
+                        # group should be hidden
+                        continue
 
-        # Determine index
-        indices = FHIR.get_answer_indices(questionnaire, questions)
-        for linkId, question in questions.items():
-
-            # Check for the answer
-            answer = answers.get(linkId)
-            if not answer:
-
-                # Check if group or in a repeating group
-                item = FHIR.find_questionnaire_item(questionnaire.item, linkId)
-
-                # Skip repeating groups, those are handled below
-                if FHIR.get_questionnaire_repeating_group(questionnaire, linkId):
-                    # If it's in a repeating group with no answer, then the
-                    # group should be hidden
-                    continue
+                    elif item.type == "group" and item.item:
 
-                elif item.type == "group" and item.item:
+                        # This is a header
+                        answer = []
 
-                    # This is a header
-                    answer = []
+                    # Check if dependent and enabled
+                    elif FHIR.question_is_conditionally_enabled(
+                        questionnaire, linkId
+                    ) and not FHIR.questionnaire_response_is_enabled(questionnaire, questionnaire_response, linkId):
 
-                # Check if dependent and enabled
-                elif FHIR.question_is_conditionally_enabled(
-                    questionnaire, linkId
-                ) and not FHIR.questionnaire_response_is_enabled(questionnaire, questionnaire_response, linkId):
+                        # If it's a sub-question, hide it
+                        if re.match(r"question\-[\d]+\-[\d]+", linkId):
+                            continue
 
-                    # If it's a sub-question, hide it
-                    if re.match(r"question\-[\d]+\-[\d]+", linkId):
-                        continue
+                        # Else, show it as unanswered
+                        else:
+                            answer = [mark_safe('<span class="label label-info">N/A</span>')]
 
-                    # Else, show it as unanswered
                     else:
-                        answer = [mark_safe('<span class="label label-info">N/A</span>')]
+                        # Set a default answer
+                        answer = [mark_safe('<span class="label label-warning">N/A</span>')]
 
-                else:
-                    # Set a default answer
-                    answer = [mark_safe('<span class="label label-warning">N/A</span>')]
-
-                    # Check if dependent and was enabled (or should have an answer but doesn't)
-                    if FHIR.questionnaire_response_is_required(questionnaire, questionnaire_response, linkId):
-                        logger.error(
-                            f"FHIR Questionnaire: No answer found for {linkId}",
-                            extra={
-                                "questionnaire": questionnaire_id,
-                                "link_id": linkId,
-                                "ppm_id": questionnaire_response.source,
-                            },
-                        )
-
-            # Format the question text
-            text = "{} {}".format(indices.get(linkId), question)
+                        # Check if dependent and was enabled (or should have an answer but doesn't)
+                        if FHIR.questionnaire_response_is_required(questionnaire, questionnaire_response, linkId):
+                            logger.error(
+                                f"FHIR Questionnaire: No answer found for {linkId}",
+                                extra={
+                                    "questionnaire": questionnaire_id,
+                                    "link_id": linkId,
+                                    "ppm_id": questionnaire_response.source,
+                                },
+                            )
 
-            # Add the answer
-            response[text] = answer
+                # Format the question text
+                text = "{} {}".format(indices.get(linkId), question)
 
-        # Get repeating groups
-        groups = [i for i in questionnaire_response.item if i.answer and next(iter(i.answer)).item]
-        for group in groups:
+                # Add the answer
+                response[text] = answer
 
-            # Parse answers
-            for group_answer in group.answer:
+            # Get repeating groups
+            groups = [i for i in questionnaire_response.item if i.answer and next(iter(i.answer)).item]
+            for group in groups:
 
                 # Parse answers
-                group_answers = FHIR._answers(group_answer.item)
+                for group_answer in group.answer:
+
+                    # Parse answers
+                    group_answers = FHIR.questionnaire_response_answers(
+                        questionnaire, questionnaire_response, group_answer.item
+                    )
 
-                # Set a header
-                response[f"Response #{group_answer.valueInteger}"] = []
+                    # Set a header
+                    response[f"Response #{group_answer.valueInteger}"] = []
 
-                for linkId, question in questions.items():
+                    for linkId, question in questions.items():
 
-                    # Check for the answer
-                    answer = group_answers.get(linkId)
-                    if not answer:
+                        # Check for the answer
+                        answer = group_answers.get(linkId)
+                        if not answer:
+
+                            # Skip if not in this group
+                            if not FHIR.get_questionnaire_repeating_group(questionnaire, linkId):
+                                continue
 
-                        # Skip if not in this group
-                        if not FHIR.get_questionnaire_repeating_group(questionnaire, linkId):
-                            continue
+                            else:
+                                # Set as unanswered
+                                answer = [mark_safe('<span class="label label-info">N/A</span>')]
 
-                        else:
-                            # Set as unanswered
-                            answer = [mark_safe('<span class="label label-info">N/A</span>')]
+                        # Format the question text
+                        text = "{}| {} {}".format(group_answer.valueInteger, indices.get(linkId), question)
 
-                    # Format the question text
-                    text = "{}| {} {}".format(group_answer.valueInteger, indices.get(linkId), question)
+                        # Add the answer
+                        response[text] = answer
 
-                    # Add the answer
-                    response[text] = answer
+        else:
+            # Set an empty response
+            response = {}
+            logger.warning(
+                f"PPM/FHIR: Empty QuestionnaireResponse/"
+                f"{questionnaire_response.id} for Questionnaire/{questionnaire_id}"
+            )
 
         # Add the date that the questionnaire was completed
         authored_date = questionnaire_response.authored.origval
         formatted_authored_date = FHIR._format_date(authored_date, "%m/%d/%Y")
 
         return {
             "ppm_id": FHIR._get_referenced_id(questionnaire_response.as_json(), "Patient"),
@@ -5185,15 +5742,15 @@
                 letter_multiplier = int((letter_index - 1) / len(string.ascii_lowercase)) + 1
                 letter = string.ascii_lowercase[(letter_index - 1) % len(string.ascii_lowercase)] * letter_multiplier
                 indices[linkId] = f"{indices[linkId]}{letter}. "
 
             if len(parts) == 3:
 
                 # Ensure we have siblings
-                if len([l for l in questions.keys() if linkId.rsplit(parts[2], 1)[0] in l]) == 1:
+                if len([link_id for link_id in questions.keys() if linkId.rsplit(parts[2], 1)[0] in link_id]) == 1:
                     continue
 
                 i_count = int(parts[2])
                 indices[linkId] = f"{indices[linkId]}{FHIR.int_to_roman(i_count).lower()}. "
 
         return indices
 
@@ -5401,14 +5958,17 @@
                         return False
                 elif enable_when.answerDateTime is not None:
                     if enable_when.answerDateTime.isostring not in answer:
                         return False
                 elif enable_when.answerInteger is not None:
                     if enable_when.answerInteger not in answer:
                         return False
+                elif enable_when.answerDecimal is not None:
+                    if enable_when.answerDecimal not in answer:
+                        return False
                 else:
                     logger.error(f"PPM/FHIR: Unhandled enableWhen answer type: {enable_when.as_json()}")
                     return False
 
             else:
                 logger.error(f"PPM/FHIR: Unhandled enableWhen operation type: {enable_when.as_json()}")
                 return False
@@ -5446,28 +6006,44 @@
         if not FHIR.questionnaire_response_is_enabled(questionnaire, questionnaire_response, linkId):
             return False
 
         # If we are here, this item is required and all dependencies are satisfied (if any)
         return True
 
     @staticmethod
-    def _questions(items):
+    def questionnaire_questions(questionnaire, items):
+        """
+        This accepts a questionnaire resource and a specific
+        item from the questionnaire and returns a dictionary of
+        question linkIds mapped to parsed question texts from the
+        questionnaire. will recurse into subitems and add them to the
+        mapping, although the mapping will be flat.
+
+        :param questionnaire: The FHIR Questionnaire resource
+        :type questionnaire: Questionnaire
+        :param questionnaire_response: The FHIR QuestionnaireResponse resource
+        :type questionnaire_response: QuestionnaireResponse
+        :param items: The FHIR QuestionnaireResponseItem items list
+        :type items: list
+        :return: [description]
+        :rtype: [type]
+        """
 
         # Iterate items
         questions = {}
         for item in items:
 
             # Leave out display or ...
             if item.type == "display":
                 continue
 
             elif item.type == "group" and item.item:
 
                 # Get answers
-                sub_questions = FHIR._questions(item.item)
+                sub_questions = FHIR.questionnaire_questions(questionnaire, item.item)
 
                 # Check for text
                 if item.text:
                     questions[item.linkId] = item.text
 
                 # Add them
                 questions.update(sub_questions)
@@ -5492,38 +6068,65 @@
                 else:
                     # Indicate a blank question text, presumably a sub-question
                     questions[item.linkId] = "-"
 
                 # Check for subtypes
                 if item.item:
                     # Get answers
-                    sub_questions = FHIR._questions(item.item)
+                    sub_questions = FHIR.questionnaire_questions(questionnaire, item.item)
 
                     # Add them
                     questions.update(sub_questions)
 
         return questions
 
     @staticmethod
-    def _answers(items):
+    def questionnaire_response_answers(questionnaire, questionnaire_response, items):
+        """
+        This accepts a questionnaire, a questionnaire response and a specific
+        item from the questionnaire response and returns a dictionary of
+        question linkIds mapped to parsed answers from the response. This
+        will recurse into subitems and add them to the mapping, although the
+        mapping will be flat.
 
+        :param questionnaire: The FHIR Questionnaire resource
+        :type questionnaire: Questionnaire
+        :param questionnaire_response: The FHIR QuestionnaireResponse resource
+        :type questionnaire_response: QuestionnaireResponse
+        :param items: The FHIR QuestionnaireResponseItem items list
+        :type items: list
+        :return: [description]
+        :rtype: [type]
+        """
         # Iterate items
         responses = {}
         for item in items:
 
             # List them out
             responses[item.linkId] = []
 
             # Ensure we've got answers
             if not item.answer:
-                logger.error(
-                    f"FHIR questionnaire error: Missing items for question {item.linkId}",
-                    extra={"link_id": item.linkId},
-                )
-                responses[item.linkId] = ["------"]
+
+                # Check if omitted due to error
+                if FHIR.questionnaire_response_is_required(questionnaire, questionnaire_response, item.linkId):
+                    logger.error(
+                        f"FHIR/QuestionnaireResponse/{item.linkId}: Missing answer item(s) for question item",
+                        extra={
+                            "questionnaire": questionnaire.id,
+                            "questionnaire_response": questionnaire_response.id,
+                            "link_id": item.linkId,
+                        },
+                    )
+
+                    # Set an N/A value
+                    responses[item.linkId] = [mark_safe('<span class="label label-warning">N/A</span>')]
+                else:
+                    # Set an N/A value
+                    responses[item.linkId] = [mark_safe('<span class="label label-info">N/A</span>')]
 
             else:
 
                 # Iterate answers
                 for answer in item.answer:
 
                     # Get the value
@@ -5537,23 +6140,29 @@
                         responses[item.linkId].append(answer.valueDecimal)
                     elif answer.valueDate is not None:
                         responses[item.linkId].append(answer.valueDate.isostring)
                     elif answer.valueDateTime is not None:
                         responses[item.linkId].append(answer.valueDateTime.isostring)
 
                     else:
-                        logger.warning(
-                            "Unhandled answer value type: {}".format(answer.as_json()),
-                            extra={"link_id": item.linkId},
+                        logger.error(
+                            f"FHIR/QuestionnaireResponse/{item.linkId}: Unhandled answer value "
+                            f"type: {answer.as_json()}",
+                            extra={
+                                "questionnaire": questionnaire.id,
+                                "questionnaire_response": questionnaire_response.id,
+                                "link_id": item.linkId,
+                                "answer": answer.as_json(),
+                            },
                         )
 
             # Check for subtypes
             if item.item:
                 # Get answers
-                sub_answers = FHIR._answers(item.item)
+                sub_answers = FHIR.questionnaire_response_answers(questionnaire, questionnaire_response, item.item)
 
                 # Add them
                 responses[item.linkId].extend(sub_answers)
 
         return responses
 
     @staticmethod
@@ -5691,14 +6300,24 @@
                 extension["valueBoolean"]
                 for extension in resource.get("extension", [])
                 if "uses-smart-on-fhir" in extension.get("url")
             ),
             True,
         )
 
+        # Get if they are not using Fitbit
+        patient["uses_procure"] = next(
+            (
+                extension["valueBoolean"]
+                for extension in resource.get("extension", [])
+                if FHIR.procure_extension_url in extension.get("url")
+            ),
+            True,
+        )
+
         # Get if they are registered with Picnichealth
         patient["picnichealth"] = next(
             (
                 extension["valueBoolean"]
                 for extension in resource.get("extension", [])
                 if FHIR.picnichealth_extension_url in extension.get("url")
             ),
@@ -5786,49 +6405,74 @@
                     # Flatten it
                     devices.append(FHIR.flatten_ppm_device(device))
 
         return devices
 
     @staticmethod
     def flatten_ppm_device(resource):
+        """
+        Parses and flattens a Device resource into a more manageable object.
+
+        :param resource: The Device FHIR resource as JSON
+        :type resource: dict
+        :return: A condensed dictionary describing the device
+        :rtype: dict
+        """
 
         # Get the actual resource in case we were handed a BundleEntry
         resource = FHIR._get_or(resource, ["resource"], resource)
 
         # Get the resource.
         record = dict()
 
         # Try and get the values
+        record["id"] = resource["id"]
         record["status"] = FHIR._get_or(resource, ["status"])
-        record["shipped"] = FHIR._get_or(resource, ["manufactureDate"])
-        record["returned"] = FHIR._get_or(resource, ["expirationDate"])
+
+        # Try to get dates
+        if resource.get("manufactureDate"):
+            record["shipped"] = parse(resource["manufactureDate"])
+        if resource.get("expirationDate"):
+            record["returned"] = parse(resource["expirationDate"])
+
+        # Get the study
+        record["study"] = ""
+        for e in resource.get("extension", []):
+            if e.get("url") == FHIR.device_study_extension_url:
+                record["study"] = e["valueString"]
 
         # Get the proper identifier
+        record["identifier"] = ""
+        record["title"] = ""
         for identifier in resource.get("identifier", []):
             if identifier.get("system") == FHIR.device_identifier_system:
 
                 # Set properties
                 record["identifier"] = identifier["value"]
-                break
 
-        else:
-            record["identifier"] = ""
+            if identifier.get("system") == FHIR.device_title_system:
+
+                # Set properties
+                record["title"] = identifier["value"]
+
+        # Get notes
+        record["note"] = ""
+        for note in resource.get("note", []):
+            if note.get("text"):
+                record["note"] = note["text"]
 
         # Get the proper coding
+        record["type"] = ""
+        record["name"] = ""
         for coding in FHIR._get_or(resource, ["type", "coding"], []):
             if coding.get("system") == FHIR.device_coding_system:
 
                 # Set properties
                 record["type"] = coding["code"]
                 record["name"] = coding["display"]
-                break
-
-        else:
-            record["type"] = ""
-            record["name"] = ""
 
         # Link back to participant
         record["ppm_id"] = FHIR._get_referenced_id(resource, "Patient", key="patient")
 
         return record
 
     @staticmethod
@@ -6305,14 +6949,17 @@
                             "code": status,
                             "display": status.title(),
                         }
                     ],
                     "text": status.title(),
                 },
                 "subject": {"reference": patient_ref},
+                # TODO: Include the study in this conditional once PPM needs
+                # to support participants with multiple studies
+                # "encounter": {"reference": f"ResearchStudy/{PPM.Study.fhir_id(study)}"}
             }
 
             # Set dates if specified.
             if start:
                 data["period"] = {"start": start.isoformat()}
                 if end:
                     data["period"]["end"] = end.isoformat()
@@ -6390,59 +7037,73 @@
             if consent:
                 data["consent"] = {"reference": "Consent/{}".format(consent)}
 
             return data
 
         @staticmethod
         def ppm_device(
-            item,
             patient_ref,
-            identifier=None,
+            study,
+            code,
+            display,
+            title,
+            identifier,
             shipped=None,
             returned=None,
             status="active",
+            note=None,
         ):
 
             data = {
                 "resourceType": "Device",
+                "identifier": [
+                    {
+                        "system": FHIR.device_identifier_system,
+                        "value": identifier,
+                    },
+                    {
+                        "system": FHIR.device_title_system,
+                        "value": title,
+                    },
+                ],
                 "type": {
                     "coding": [
                         {
                             "system": FHIR.device_coding_system,
-                            "code": item,
-                            "display": dict(PPM.TrackedItem.choices())[item],
+                            "code": code,
+                            "display": display,
                         }
                     ],
-                    "text": dict(PPM.TrackedItem.choices())[item],
+                    "text": display,
                 },
                 "status": status,
                 "patient": {"reference": patient_ref},
+                "extension": [
+                    {
+                        "url": FHIR.device_study_extension_url,
+                        "valueString": study,
+                    }
+                ],
             }
 
-            # Prefill some details based on the item type
-            if item is PPM.TrackedItem.BloodSampleKit:
-                pass
-            elif item is PPM.TrackedItem.SalivaSampleKit:
-                pass
-            elif item is PPM.TrackedItem.uBiomeFecalSampleKit:
-                pass
-            elif item is PPM.TrackedItem.Fitbit:
-                pass
-
-            # Add identifier
-            if identifier:
-                data["identifier"] = [{"system": FHIR.device_identifier_system, "value": identifier}]
-
             # Check dates
             if shipped:
                 data["manufactureDate"] = shipped.isoformat()
 
             if returned:
                 data["expirationDate"] = returned.isoformat()
 
+            if note:
+                data["note"] = [
+                    {
+                        "time": datetime.now().isoformat(),
+                        "text": note,
+                    }
+                ]
+
             return data
 
         @staticmethod
         def communication(
             patient_ref,
             identifier,
             content=None,
@@ -6514,15 +7175,15 @@
                     {
                         "system": FHIR.patient_email_telecom_system,
                         "value": form.get("contact_email"),
                     }
                 )
 
             if form.get("how_did_you_hear_about_us"):
-                logger.debug('Adding "How did you hear about is"')
+                logger.debug('Adding "How did you hear about us"')
                 patient_data["extension"] = [
                     {
                         "url": FHIR.referral_extension_url,
                         "valueString": form.get("how_did_you_hear_about_us"),
                     }
                 ]
 
@@ -6541,155 +7202,14 @@
         @staticmethod
         def coding(system, code):
             """
             Returns a coding resource
             """
             return {"coding": [{"system": system, "code": code}]}
 
-        @staticmethod
-        def ppm_qualtrics_survey_questionnaire(study, questionnaire_id, survey_id, survey):
-            """
-            Returns QuestionnaireResponse resource for a survey taken through
-            Qualtrics. This method requires that Qualtrics question names are
-            matched to the FHIR Questionnaire linkIds.
-
-            :param study: The study for which the questionnaire was given
-            :type study: PPM.Study
-            :param questionnaire_id: The ID for the related FHIR Questionnaire
-            :type questionnaire_id: str
-            :param survey_id: The ID of the Qualtrics survey
-            :type survey_id: str
-            :param survey: The survey object from Qualtrics
-            :type survey: dict
-            :return: The QuestionnaireResponse resource
-            :rtype: dict
-            """
-            from ppmutils.qualtrics import Qualtrics
-
-            warnings.warn(f"This method has moved to ppmutils.qualtrics.Qualtrics", DeprecationWarning)
-            return Qualtrics.ppm_qualtrics_survey_questionnaire(study, questionnaire_id, survey_id, survey)
-
-        def ppm_qualtrics_survey_questionnaire_items(survey, blocks):
-            """
-            Accepts the survey object as well as the list of blocks and their
-            respective questions and yields a set of QuestionnareItem
-            resources to be set for the Questionnaire.
-
-            :param survey: The Qualtrics survey object
-            :type survey: object
-            :param blocks: The dictionary of blocks comprising the survey
-            :type blocks: dict
-            :raises Exception: Raises exception if value is an unhandled type
-            :returns A generator of QuestionnaireItem resources
-            :rtype generator
-            """
-            from ppmutils.qualtrics import Qualtrics
-
-            warnings.warn(f"This method has moved to ppmutils.qualtrics.Qualtrics", DeprecationWarning)
-            return Qualtrics.ppm_qualtrics_survey_questionnaire_items(survey, blocks)
-
-        def ppm_qualtrics_survey_questionnaire_item(survey, qid, question):
-            """
-            Returns a FHIR resource for a QuestionnaireItem parsed from
-            the Qualtrics survey's question
-
-            :param survey: The Qualtrics survey object
-            :type survey: dict
-            :param qid: The Qualtrics survey question identifier
-            :type qid: str
-            :param question: The Qualtrics survey question object
-            :type question: dict
-            :raises Exception: Raises exception if question is an unhandled type
-            :return: The FHIR QuestionnaireItem resource
-            :rtype: dict
-            """
-            from ppmutils.qualtrics import Qualtrics
-
-            warnings.warn(f"This method has moved to ppmutils.qualtrics.Qualtrics", DeprecationWarning)
-            return Qualtrics.ppm_qualtrics_survey_questionnaire_item(survey, qid, question)
-
-        @staticmethod
-        def ppm_qualtrics_survey_questionnaire_response(
-            study, ppm_id, questionnaire_id, survey_id, survey, response_id, response
-        ):
-            """
-            Returns QuestionnaireResponse resource for a survey taken through
-            Qualtrics. This method requires that Qualtrics question names are
-            matched to the FHIR Questionnaire linkIds.
-
-            :param study: The study for which the questionnaire was given
-            :type study: PPM.Study
-            :param ppm_id: The PPM ID for the participant who took the survey
-            :type ppm_id: str
-            :param questionnaire_id: The ID for the related FHIR Questionnaire
-            :type questionnaire_id: str
-            :param survey_id: The ID of the Qualtrics survey
-            :type survey_id: str
-            :param survey: The Qualtrics survey object
-            :type survey: dict
-            :param response_id: The ID of the Qualtrics survey response
-            :type response_id: str
-            :param response: The Qualtrics survey response object
-            :type response: dict
-            :return: The QuestionnaireResponse resource
-            :rtype: dict
-            """
-            from ppmutils.qualtrics import Qualtrics
-
-            warnings.warn(f"This method has moved to ppmutils.qualtrics.Qualtrics", DeprecationWarning)
-            return Qualtrics.questionnaire_response(
-                study, ppm_id, questionnaire_id, survey_id, survey, response_id, response
-            )
-
-        def ppm_qualtrics_survey_questionnaire_response_items(survey, response, blocks):
-            """
-            Accepts the survey, response objects as well as the list of blocks add their
-            respective questions and yields a set of QuestionnareResponseItem
-            resources to be set for the QuestionnaireResponse.
-
-            :param survey: The Qualtrics survey object
-            :type survey: object
-            :param response: The Qualtrics survey response item
-            :type response: object
-            :param blocks: The dictionary of blocks comprising the survey
-            :type blocks: dict
-            :param blocks: The ID of the specific block to process
-            :type blocks: str
-            :raises Exception: Raises exception if value is an unhandled type
-            :returns A generator of QuestionnaireResponseItem resources
-            :rtype generator
-            """
-            from ppmutils.qualtrics import Qualtrics
-
-            warnings.warn(f"This method has moved to ppmutils.qualtrics.Qualtrics", DeprecationWarning)
-            return Qualtrics.questionnaire_response_item_generator(survey, response, blocks)
-
-        def ppm_qualtrics_survey_questionnaire_response_item(survey, response, key, loop=None):
-            """
-            Returns a FHIR QuestionnaireResponse.Item resource for the passed
-            Qualtrics survey question response key and loop (if applicable).
-
-            :param survey: The Qualtrics survey object
-            :type survey: object
-            :param response: The Qualtrics survey response item
-            :type response: object
-            :type survey: object
-            :param key: The Qualtrics question ID to process
-            :type key: str
-            :param loop: The Qualtrics loop ID to process
-            :type loop: str
-            :raises Exception: Raises exception if value is an unhandled type
-            :return: A FHIR QuestionnaireResponse.Item resource
-            :rtype: dict
-            """
-            from ppmutils.qualtrics import Qualtrics
-
-            warnings.warn(f"This method has moved to ppmutils.qualtrics.Qualtrics", DeprecationWarning)
-            return Qualtrics.questionnaire_response_item(survey, response, key, loop)
-
         def _questionnaire_response_answer(value):
             """
             Returns a FHIR resource for a QuestionnaireResponse answer
 
             :param value: The value object
             :type value: object
             :raises Exception: Raises exception if value is an unhandled type
@@ -6773,15 +7293,15 @@
                 logger.info("----- FHIR/Ops: Starting '{}' -----".format(op.__name__))
                 success, message = op(*args, **kwargs)
                 if success:
                     logger.info("----- FHIR/Ops: Completed '{}' ----".format(op.__name__))
                 else:
                     logger.error("----- FHIR/Ops: Failed '{}' ----".format(op.__name__))
                     logger.error("----- FHIR/Ops: '{}' Message: ----\n{}\n".format(op.__name__, message))
-                    logger.info("----- FHIR/Ops: Operation failed, halting operations ----".format(op.__name__))
+                    logger.info("----- FHIR/Ops: Operation failed, halting operations ----")
                     break
 
         def _op_fix_asd_researchstudy_20201031(*args, **kwargs):
             """
             This operation fixes the study identifier of ASD from 'autism' to
             'asd'. This updates the actual ResearchStudy instance as well
             as all ResearchSubject and other referencing resources as
@@ -6846,25 +7366,25 @@
                 research_study_delete_entry = BundleEntry()
                 research_study_delete_entry.request = research_study_delete_request
 
                 # Add it
                 bundle.entry.append(research_study_delete_entry)
 
             else:
-                logger.debug(f"PPM/FHIR/Ops/fix_asd_research_study: No ResearchStudy for 'ppm-autism' found")
+                logger.debug("PPM/FHIR/Ops/fix_asd_research_study: No ResearchStudy for 'ppm-autism' found")
 
             # Else, get all referencing ResearchSubjects
             research_subjects = FHIR.query_ppm_research_subjects()
             research_subjects = [
                 r for r in research_subjects if r["study"]["reference"].replace("ResearchStudy/", "") == "ppm-autism"
             ]
             logger.debug(
-                f"PPM/FHIR/Ops/fix_asd_research_study: Found "
+                "PPM/FHIR/Ops/fix_asd_research_study: Found "
                 f"{len(research_subjects)} ResearchSubject resources"
-                f"for 'ppm-autism'"
+                "for 'ppm-autism'"
             )
 
             # Filter for those referencing 'ppm-autism'
             for research_subject in research_subjects:
                 logger.debug(f"PPM/FHIR/Ops/fix_asd_research_study: Fixing ResearchSubject/{research_subject['id']}")
                 logger.warning(research_subject)
 
@@ -6905,17 +7425,17 @@
             document_references = [
                 d
                 for d in document_references
                 if "ppm-autism"
                 in [r["ref"]["reference"].replace("ResearchStudy/", "") for r in d["context"]["related"]]
             ]
             logger.debug(
-                f"PPM/FHIR/Ops/fix_asd_research_study: Found "
+                "PPM/FHIR/Ops/fix_asd_research_study: Found "
                 f"{len(document_references)} DocumentReference resources "
-                f"for 'ppm-autism'"
+                "for 'ppm-autism'"
             )
 
             # Filter for those referencing 'ppm-autism'
             for document_reference in document_references:
                 logger.debug(
                     f"PPM/FHIR/Ops/fix_asd_research_study: Fixing DocumentReference/{document_reference['id']}"
                 )
@@ -6944,22 +7464,22 @@
 
             # Get all referencing Compositions
 
             # Build the query
             query = {"type": f"{FHIR.ppm_consent_type_system}|{FHIR.ppm_consent_type_value}"}
 
             # Check for ppm-autism study
-            query["entry"] = f"ResearchStudy/ppm-autism"
+            query["entry"] = "ResearchStudy/ppm-autism"
 
             # Get resources
             compositions = FHIR._query_resources("Composition", query=query)
             logger.debug(
-                f"PPM/FHIR/Ops/fix_asd_research_study: Found "
+                "PPM/FHIR/Ops/fix_asd_research_study: Found "
                 f"{len(compositions)} Composition resources with ref "
-                f"to 'ppm-autism'"
+                "to 'ppm-autism'"
             )
 
             # Filter for those referencing 'ppm-autism'
             for composition in compositions:
                 logger.debug(f"PPM/FHIR/Ops/fix_asd_research_study: Fixing Composition/{composition['id']}")
 
                 # Iterate sections
@@ -6982,9 +7502,9 @@
                 )
                 composition_entry.request = composition_request
 
                 # Add it
                 bundle.entry.append(composition_entry)
 
             # Run the operation
-            response = requests.post(FHIR.service_url(), json=bundle.as_json())
+            response = requests.post(PPM.fhir_url(), json=bundle.as_json())
             return response.ok, response.content
```

### Comparing `ppm-utils-1.0.0b8/ppmutils/ppm.py` & `ppm-utils-1.0.1/ppmutils/ppm.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,23 +2,19 @@
 import requests
 from furl import furl
 import json
 import re
 import os
 from functools import total_ordering
 
-from django.template.loader import render_to_string
-from django.core.mail import EmailMultiAlternatives
 from django.conf import settings
-from ppmutils.settings import ppm_settings
 
-# Get the app logger
 import logging
 
-logger = logging.getLogger(ppm_settings.LOGGER_NAME)
+logger = logging.getLogger(__name__)
 
 
 # Adding this decorator to an Enum allows it to
 # be passed into a Django context and its members
 # accessed via name and value as well as being iterated (untested)
 def django_enum(cls):
     cls.do_not_call_in_templates = True
@@ -159,14 +155,31 @@
             # See if it's valid
             elif not cls.check(env.lower()):
                 raise ValueError(f"Configured environment '{env}' is invalid")
 
             return cls.get(env.lower())
 
     @staticmethod
+    def fhir_url():
+        if hasattr(settings, "FHIR_URL"):
+            return settings.FHIR_URL
+
+        elif os.environ.get("FHIR_URL"):
+            return os.environ.get("FHIR_URL")
+
+        # Search environment
+        for key, value in os.environ.items():
+            if "_FHIR_URL" in key:
+                logger.debug("Found FHIR_URL in key: {}".format(key))
+
+                return value
+
+        raise ValueError("FHIR_URL not defined in settings or in environment")
+
+    @staticmethod
     def is_tester(email):
         """
         Checks test user email patterns and returns True if a user's email
         matches.
         :param email: The user's email address
         :return: bool
         """
@@ -188,29 +201,14 @@
     class Study(PPMEnum):
         NEER = "neer"
         ASD = "asd"
         EXAMPLE = "example"
         RANT = "rant"
 
         @staticmethod
-        def equals(this, that):
-            """
-            Compares a reference to a study and returns whether it is the second
-            passed PPM.Study enum
-            :param this: The study object to be compared
-            :type this: object
-            :param that: What we are comparing against
-            :type that: object
-            :return: Whether they are one and the same
-            :rtype: boolean
-            """
-            # Compare
-            return PPM.Study.get(this) is PPM.Study.get(that)
-
-        @staticmethod
         def fhir_id(study):
             """
             Return the FHIR identifier for the passed study
             :return: A PPM study identifier
             :rtype: str
             """
             return "ppm-{}".format(PPM.Study.get(study).value)
@@ -267,25 +265,14 @@
             :type enum: Object
             :return: The instance of PPM Study enum
             :rtype: PPM.Study
             """
             return cls.enum(enum)
 
         @staticmethod
-        def dashboard_url(study):
-            """
-            Returns the defined dashboard for the passed study
-            :param study: The study we want the dashboard URL for
-            :type study: PPM.Study
-            :return: The dashboard URL
-            :rtype: str
-            """
-            return ppm_settings.dashboard_url(PPM.Study.get(study).value)
-
-        @staticmethod
         def from_value(study):
             """
             Returns an instance of the Study enum for the given study value
             :param study: The study value string
             :type study: str
             :return: The instance of PPM Study enum
             :rtype: PPM.Study
@@ -448,20 +435,14 @@
                     {
                         "step": "research-studies",
                         "blocking": False,
                         "required": False,
                         "enabled": True,
                     },
                     {
-                        "step": "survey",
-                        "blocking": False,
-                        "required": False,
-                        "enabled": True,
-                    },
-                    {
                         "step": "twitter",
                         "blocking": False,
                         "required": False,
                         "enabled": True,
                     },
                     {
                         "step": "fitbit",
@@ -542,15 +523,21 @@
                     {
                         "step": "research-studies",
                         "blocking": False,
                         "required": False,
                         "enabled": True,
                     },
                     {
-                        "step": "survey",
+                        "step": "twitter",
+                        "blocking": False,
+                        "required": False,
+                        "enabled": True,
+                    },
+                    {
+                        "step": "fitbit",
                         "blocking": False,
                         "required": False,
                         "enabled": True,
                     },
                     {
                         "step": "picnichealth",
                         "blocking": False,
@@ -592,21 +579,21 @@
                     {
                         "step": "approval",
                         "blocking": True,
                         "required": True,
                         "enabled": True,
                     },
                     {
-                        "step": "qualtrics-SV_6YHOgpujEr8uDaZ",
-                        "blocking": False,
-                        "required": False,
+                        "step": "poc",
+                        "blocking": True,
+                        "required": True,
                         "enabled": True,
                     },
                     {
-                        "step": "qualtrics-SV_74G8i7ukzojD88J",
+                        "step": "research-studies",
                         "blocking": False,
                         "required": False,
                         "enabled": True,
                     },
                     {
                         "step": "procure",
                         "blocking": False,
@@ -640,85 +627,14 @@
             if step_dict and step_dict.get("enabled"):
                 return True
             elif not step_dict:
                 logger.warning('Step "{}" does not exist in dashboard spec for study "{}"'.format(step, study))
 
             return False
 
-        @staticmethod
-        def providers(study, environment):
-            """
-            Returns a list of enabled providers for the given study and environment
-            """
-            # Get the enum
-            _study = PPM.Study.get(study)
-
-            providers = None
-            if _study is PPM.Study.ASD:
-                providers = [
-                    PPM.Provider.PPM,
-                    PPM.Provider.Fitbit,
-                    PPM.Provider.Twitter,
-                    PPM.Provider.Facebook,
-                    PPM.Provider.PicnicHealth,
-                    PPM.Provider.Broad,
-                    PPM.Provider.File,
-                    PPM.Provider.Qualtrics,
-                    PPM.Provider.ImmunoSEQ,
-                ]
-            elif _study is PPM.Study.NEER:
-                providers = [
-                    PPM.Provider.PPM,
-                    PPM.Provider.Twitter,
-                    PPM.Provider.PicnicHealth,
-                    PPM.Provider.Broad,
-                    PPM.Provider.File,
-                    PPM.Provider.Qualtrics,
-                    PPM.Provider.ImmunoSEQ,
-                ]
-            elif _study is PPM.Study.RANT:
-                providers = [
-                    PPM.Provider.PPM,
-                    PPM.Provider.PicnicHealth,
-                    PPM.Provider.Broad,
-                    PPM.Provider.File,
-                    PPM.Provider.Qualtrics,
-                    PPM.Provider.ImmunoSEQ,
-                    PPM.Provider.Procure,
-                ]
-            elif _study is PPM.Study.EXAMPLE:
-                providers = [
-                    PPM.Provider.PPM,
-                    PPM.Provider.Fitbit,
-                    PPM.Provider.Twitter,
-                    PPM.Provider.Facebook,
-                    PPM.Provider.PicnicHealth,
-                    PPM.Provider.Broad,
-                    PPM.Provider.File,
-                    PPM.Provider.SMART,
-                    PPM.Provider.Qualtrics,
-                    PPM.Provider.ImmunoSEQ,
-                    PPM.Provider.Procure,
-                ]
-
-            return providers
-
-        @staticmethod
-        def is_provider_enabled(provider, study, environment):
-            """
-            Returns whether the given provider for the current study and environment
-            should be enabled or not.
-            :param provider: The code for the provider to check
-            :param study: The current PPM study
-            :param environment: The current PPM environment
-            :return: bool
-            """
-            _provider = PPM.Provider.get(provider)
-            return _provider in PPM.Study.providers(study, environment)
-
     # Alias Project as Study until we migrate all usages to Study
     Project = Study
 
     # Set the appropriate participant statuses
     @total_ordering
     @django_enum
     class Enrollment(PPMEnum):
@@ -875,30 +791,39 @@
         participants are expected to take during the course of the study
 
         NOTE: When adding a new questionnaire, ensure it is set as a class
         variable and the title is also set in `choices()`
         """
 
         # Pre-approval survey/Questionnaires
-        EXAMPLEQuestionnaire = "ppm-example-registration-questionnaire"
+        EXAMPLEQuestionnaire = "ppm-example-eligibility-questionnaire"
         NEERQuestionnaire = "ppm-neer-registration-questionnaire"
-        RANTQuestionnaire = "ppm-rant-registration-questionnaire"
+        RANTQuestionnaire = "ppm-rant-eligibility-questionnaire"
 
         # Post-approval surveys/questionnaires
         ASDQuestionnaire = "ppm-asd-questionnaire"
+
+        # NEER
         NEERRISCQuestionnaire = "ppm-neer-risc-questionnaire"
         NEERDietQuestionnaire = "ppm-neer-diet-questionnaire"
         NEERCAMQuestionnaire = "ppm-neer-cam-questionnaire"
+
+        # RANT
         RANTPointsOfCareQuestionnaire = "ppm-rant-points-of-care-questionnaire"
         RANTRASymptomQuestionnaire = "ppm-rant-ra-symptom-questionnaire"
         RANTCOVIDQuestionnaire = "ppm-rant-covid-questionnaire"
 
+        # Example
+        EXAMPLEPointsOfCareQuestionnaire = "ppm-example-points-of-care-questionnaire"
+        EXAMPLERASymptomQuestionnaire = "ppm-example-ra-symptom-questionnaire"
+        EXAMPLECOVIDQuestionnaire = "ppm-example-covid-questionnaire"
+
         # Consents (Current)
         EXAMPLEConsent = "example-signature"
-        NEERConsent = "neer-signature-v2"
+        NEERConsent = "neer-signature-v3"
         ASDGuardianConsentQuestionnaire = "ppm-asd-consent-guardian-quiz"
         ASDIndividualConsentQuestionnaire = "ppm-asd-consent-individual-quiz"
         ASDConsentIndividualSignatureQuestionnaire = "individual-signature-part-1"
         ASDConsentGuardianSignature1Questionnaire = "guardian-signature-part-1"
         ASDConsentGuardianSignature2Questionnaire = "guardian-signature-part-2"
         ASDConsentGuardianSignature3Questionnaire = "guardian-signature-part-3"
 
@@ -910,29 +835,32 @@
             return (
                 (PPM.Questionnaire.EXAMPLEQuestionnaire.value, "Example Registration Questionnaire"),
                 (PPM.Questionnaire.NEERQuestionnaire.value, "NEER Registration Questionnaire"),
                 (PPM.Questionnaire.NEERRISCQuestionnaire.value, "NEER CD-RISC Resilience Scale Questionnaire"),
                 (PPM.Questionnaire.NEERDietQuestionnaire.value, "NEER Diet Questionnaire"),
                 (PPM.Questionnaire.NEERCAMQuestionnaire.value, "NEER CAM Questionnaire"),
                 (PPM.Questionnaire.ASDQuestionnaire.value, "ASD Registration Questionnaire"),
-                (PPM.Questionnaire.RANTQuestionnaire.value, "RANT Registration Questionnaire"),
                 (PPM.Questionnaire.RANTPointsOfCareQuestionnaire.value, "RANT Points of Care Questionnaire"),
                 (PPM.Questionnaire.RANTRASymptomQuestionnaire.value, "RANT RA Symptom Questionnaire"),
                 (PPM.Questionnaire.RANTCOVIDQuestionnaire.value, "RANT COVID Questionnaire"),
                 (PPM.Questionnaire.EXAMPLEConsent.value, "Example Consent Signature"),
                 (PPM.Questionnaire.NEERConsent.value, "NEER Consent Signature"),
                 (PPM.Questionnaire.ASDGuardianConsentQuestionnaire.value, "ASD Guardian Consent Questionnaire"),
                 (PPM.Questionnaire.ASDIndividualConsentQuestionnaire.value, "ASD Individual ConsentQuestionnaire"),
                 (
                     PPM.Questionnaire.ASDConsentIndividualSignatureQuestionnaire.value,
                     "ASD Individual Consent Signature",
                 ),
                 (PPM.Questionnaire.ASDConsentGuardianSignature1Questionnaire.value, "ASD Guardian Consent Signature"),
                 (PPM.Questionnaire.ASDConsentGuardianSignature2Questionnaire.value, "ASD Guardian Consent Signature"),
                 (PPM.Questionnaire.ASDConsentGuardianSignature3Questionnaire.value, "ASD Guardian Assent Signature"),
+                (PPM.Questionnaire.RANTQuestionnaire.value, "RANT Registration Questionnaire"),
+                (PPM.Questionnaire.EXAMPLEPointsOfCareQuestionnaire.value, "Example Points of Care Questionnaire"),
+                (PPM.Questionnaire.EXAMPLERASymptomQuestionnaire.value, "Example RA Symptom Questionnaire"),
+                (PPM.Questionnaire.EXAMPLECOVIDQuestionnaire.value, "Example COVID Questionnaire"),
             )
 
         @classmethod
         def questionnaires_for_study(cls, study):
             """
             Returns a list of Questionnaires for the passed study. This includes
             both mandatory and optional questionnaires.
@@ -1202,17 +1130,18 @@
             to use for the exclusion item
             :param questionnaire_id: The Questionnaire ID
             :return: dict
             """
             if questionnaire_id == PPM.Questionnaire.NEERConsent.value:
                 return {
                     "question-1": "82078001",
-                    "question-2": "258435002",
-                    "question-3": "284036006",
-                    "question-4": "702475000",
+                    "question-2": "165334004",
+                    "question-3": "258435002",
+                    "question-4": "284036006",
+                    "question-5": "702475000",
                 }
 
             elif questionnaire_id == PPM.Questionnaire.EXAMPLEConsent.value:
                 return {
                     "question-1": "82078001",
                     "question-2": "165334004",
                     "question-3": "258435002",
@@ -1373,250 +1302,77 @@
             }
 
             return devices[study] if study else devices
 
     # Alias Device to TrackedItem
     Device = TrackedItem
 
-    class Email(Enum):
-        AdminProposedNotification = "admin_proposed_notification"
-        AdminContactNotification = "admin_contact_notification"
-        UserProposedNotification = "user_proposed_notification"
-        UserAcceptedNotification = "user_accepted_notification"
-        UserPendingNotification = "user_pending_notification"
-        UserQueuedNotification = "user_queued_notification"
-
-        @staticmethod
-        def send(email, study, recipients, subject=None, sender=None, context=None, reply_to=None):
-            """
-            Sends an email for the corresponding email identifier.
-            :param email: The email identifier
-            :param study: The study for which the email concerns
-            :param recipients: A list of recipients
-            :param subject: The subject for the email
-            :param sender: The sender
-            :param context: Context for the email
-            :param reply_to: A list of reply to addresses, if any
-            :return:
-            """
-            try:
-                # Add subject
-                if not subject:
-                    subject = PPM.Email.subject(email=email, study=study)
-
-                for recipient in recipients:
-                    logger.debug(f'Email: Sending "{email.value}" for study "{study}" -> "{recipient}"')
-
-                    # Check if test
-                    test_admin = PPM.Email.is_test(recipient)
-                    if test_admin:
-                        recipient = test_admin
-
-                    # Check reply to
-                    if not reply_to:
-                        reply_to = []
-
-                    # Render templates
-                    html, plain = PPM.Email.render(email=email, study=study, context=context, subject=subject)
-
-                    # Perform send
-                    msg = EmailMultiAlternatives(
-                        subject, plain, ppm_settings.EMAIL_DEFAULT_FROM, [recipient], reply_to=reply_to
-                    )
-                    msg.attach_alternative(html, "text/html")
-                    msg.send()
-
-                    logger.debug(f'Email: Sent email "{email.value}" for study "{study}" -> "{recipient}"')
-
-                return True
-
-            except Exception as e:
-                logger.exception(
-                    "Email error: {}".format(e),
-                    exc_info=True,
-                    extra={
-                        "email": email.value,
-                        "study": study,
-                        "subject": subject,
-                        "sender": sender,
-                        "context": context,
-                    },
-                )
-
-            return False
-
-        @staticmethod
-        def is_test(recipient):
-            """
-            Tests the given user account for matching that of a test account.
-            Test accounts are specified as [regex 1]:[admin email],[regex 2]:[admin email],...
-            If the given user is a test account, return the specific admin for which notifications
-            should be limited to sending to.
-            :param recipient: The recipient email
-            :return: Admin email address if test account, None if not
-            """
-
-            # Check for test accounts
-            try:
-                if hasattr(ppm_settings, "EMAIL_TEST_ACCOUNTS"):
-                    test_accounts = ppm_settings.EMAIL_TEST_ACCOUNTS
-                elif hasattr(settings, "TEST_EMAIL_ACCOUNTS"):
-                    test_accounts = settings.TEST_EMAIL_ACCOUNTS.split(",")
-                else:
-                    return None
-
-                if test_accounts is not None and len(test_accounts) > 0:
-                    logger.info("Test accounts found, checking now...")
-
-                    for test_account in test_accounts:
-
-                        # Split the test account email from the destination admin email
-                        test_account_parts = test_account.split(":")
-                        regex = re.compile(test_account_parts[0])
-                        matches = regex.match(recipient)
-                        if matches is not None and matches.group():
-                            logger.info(
-                                "Email: Test account found: {}, sending to {}".format(recipient, test_account_parts[1])
-                            )
-
-                            # Return the test admin email
-                            return test_account_parts[1]
-
-            except Exception as e:
-                logger.warning("Test email lookup failed: {}".format(e), exc_info=True)
-
-            return None
-
-        @staticmethod
-        def render(email, study, context, subject=None):
-            """
-            Accepts an email identifier and context and returns the rendered content as a string
-            :param email: The email identifier
-            :param study: The study for which the email concerns
-            :param context: The context for the email's content
-            :param subject: The optional subject line
-            :return: str
-            """
-            # Get the study
-            _study = PPM.Study.get(study)
-
-            # Add study
-            context["ppm_study"] = _study.value
-            context["ppm_study_title"] = PPM.Study.title(study)
-
-            # Add subject
-            context["ppm_subject"] = subject if subject is not None else PPM.Email.subject(email=email, study=study)
-
-            # Add signature bits
-            context["ppm_signature"] = ppm_settings.EMAIL_SIGNATURE
-
-            try:
-                # Check for study specific templates
-                if os.path.exists(f"ppmutils/{_study.value}/{email.value}.html"):
-
-                    # These templates are specific to this study
-                    template_paths = (
-                        f"ppmutils/{_study.value}/{email.value}.html",
-                        f"ppmutils/{_study.value}/{email.value}.txt",
-                    )
-
-                else:
-
-                    # These are generic templates and can be rendered across all studies
-                    template_paths = f"ppmutils/{email.value}.html", f"ppmutils/{email.value}.txt"
-
-                # Render templates
-                html = render_to_string(template_paths[0], context)
-                plain = render_to_string(template_paths[1], context)
-
-                return html, plain
-
-            except Exception as e:
-                logger.exception(
-                    f"Email error: {e}",
-                    exc_info=True,
-                    extra={
-                        "email": email.value,
-                        "study": study,
-                    },
-                )
-
-        @staticmethod
-        def subject(email, study):
-            """
-            Returns the default subject time for the email and study combination
-            :param email: The email identifier
-            :param study: The study for which the email concerned
-            :return: str
-            """
-            # Set email subject lines
-            subjects = {
-                "admin_contact_notification": f"People-Powered Medicine - {PPM.Study.title(study)} - Support",
-                "admin_proposed_notification": f"People-Powered Medicine - {PPM.Study.title(study)} - New User Signup",
-                "user_proposed_notification": f"People-Powered Medicine - {PPM.Study.title(study)} - Registration",
-                "user_accepted_notification": f"People-Powered Medicine - {PPM.Study.title(study)} - Approved",
-                "user_queued_notification": f"People-Powered Medicine - {PPM.Study.title(study)} - Update",
-                "user_pending_notification": f"People-Powered Medicine - {PPM.Study.title(study)} - Update",
-            }
-
-            return subjects[email.value]
-
     class Service(object):
 
         # Subclasses set this to direct requests
         service = None
 
-        # If enabled, all requests are routed through PPM-API
-        proxied = False
-
         # Set some auth header properties
         jwt_cookie_name = "DBMI_JWT"
         jwt_authorization_prefix = "JWT"
         token_authorization_prefix = "Token"
-        ppm_settings_url_name = None
 
         @classmethod
         def _build_url(cls, path):
 
             # Build the url, chancing on doubling up a slash or two.
-            scheme, domain = tuple(cls.service_url().strip("/").split("://"))
-            url = furl("{}://{}/{}".format(scheme, domain, path.lstrip("/").replace("//", "/")))
+            url = furl(cls.service_url().rstrip("/") + "/" + path.lstrip("/"))
+
+            # Filter empty segments (double slashes in path)
+            segments = [
+                segment
+                for index, segment in enumerate(url.path.segments)
+                if segment != "" or index == len(url.path.segments) - 1
+            ]
+
+            # Set it
+            url.path.segments = segments
 
             return url.url
 
         @classmethod
         def service_url(cls):
 
-            # Check if this service should be proxied through PPM-API
-            if cls.proxied:
+            # Check variations of names
+            names = ["###_URL", "DBMI_###_URL", "###_API_URL", "###_BASE_URL"]
+            for name in names:
+                if hasattr(settings, name.replace("###", cls.service.upper())):
+                    service_url = getattr(settings, name.replace("###", cls.service.upper()))
 
-                # We want only the domain and no paths, as those should be specified in the calls
-                # so strip any included paths and queries and return
-                url = furl(ppm_settings.API_URL)
-                url.path.segments.clear()
-                url.query.params.clear()
+                    # We want only the domain and no paths, as those should be
+                    # specified in the calls so strip any included paths and queries
+                    # and return
+                    url = furl(service_url)
+                    url.path.segments.clear()
+                    url.query.params.clear()
 
-                # Add API base path
-                url.path.segments.extend(["api", "v1", cls.service])
+                    return url.url
 
-            else:
-                # Get from ppm settings
-                if not hasattr(ppm_settings, cls.ppm_settings_url_name):
-                    raise SystemError("Service URL not defined in settings".format(cls.service.upper()))
-
-                # Get it
-                service_url = getattr(ppm_settings, cls.ppm_settings_url_name)
-
-                # We want only the domain and no paths, as those should be specified in the calls
-                # so strip any included paths and queries and return
-                url = furl(service_url)
-                url.path.segments.clear()
-                url.query.params.clear()
+            # Check for a default
+            environment = os.environ.get("DBMI_ENV")
+            if environment and cls.default_url_for_env(environment):
+                return cls.default_url_for_env(environment)
 
-            return url.url
+            raise ValueError("Service URL not defined in settings")
+
+        @classmethod
+        def default_url_for_env(cls, environment):
+            """
+            Give implementing classes an opportunity to list a default set of URLs
+            based on the DBMI_ENV, if specified. Otherwise, return nothing
+            :param environment: The DBMI_ENV string
+            :return: A URL, if any
+            """
+            logger.warning("Class PPM does not return a default URL for " "environment: {}".format(environment))
+            return None
 
         @classmethod
         def headers(cls, request=None, content_type="application/json"):
             """
             Builds request headers. If no request is passed, service is assumed to
             use a pre-defined token in settings as `[SERVICE_NAME]_AUTH_TOKEN`
             :param request: The current request, if any
@@ -1758,35 +1514,54 @@
             :param raw: How the response should be returned
             :return: object
             """
             # Check for params
             if not data:
                 data = {}
 
+            # Set placeholders for debugging
+            content = status_code = None
             try:
                 # Prepare the request.
                 response = requests.post(
                     cls._build_url(path),
                     headers=cls.headers(request),
                     data=json.dumps(data),
                 )
+                content = response.content
+                status_code = response.status_code
 
                 # Check response type
                 if raw:
                     return response
                 else:
                     return response.json()
 
+            except requests.HTTPError as e:
+                logger.debug(f"{cls.service} request error: {data}/{path} -> [{status_code}] {content}")
+                logger.exception(
+                    "{} request error: {}".format(cls.service, e),
+                    extra={
+                        "data": data,
+                        "path": path,
+                        "content": content,
+                        "status_code": status_code,
+                    },
+                )
+
             except Exception as e:
+                logger.debug(f"{cls.service} error: {data}/{path} -> [{status_code}] {content}")
                 logger.exception(
                     "{} error: {}".format(cls.service, e),
                     exc_info=True,
                     extra={
                         "data": data,
                         "path": path,
+                        "content": content,
+                        "status_code": status_code,
                     },
                 )
 
             return None
 
         @classmethod
         def put(cls, request=None, path="/", data=None, raw=False):
@@ -1907,42 +1682,35 @@
                         "path": path,
                     },
                 )
 
             return False
 
         @classmethod
-        def request(cls, verb, headers=None, request=None, path="/", data=None, check=True):
+        def request(cls, verb, request=None, path="/", data=None, check=True):
             """
             Runs the appropriate REST operation. Request is required for JWT auth,
             not required for token auth.
             :param verb: The RESTful operation to be performed
-            :param headers: Any additional headers to include
             :param request: The current Django request
             :param path: The path of the request
             :param data: Request data or params
             :param check: Check the response and raise exception if faulty
             :return: object
             """
             # Check for params
             if not data:
                 data = {}
 
-            # Compile headers
-            if headers:
-                cls.headers(request).update(headers)
-            else:
-                headers = cls.headers(request)
-
             # Track response for error reporting
             response = None
             try:
                 # Build arguments
                 args = [cls._build_url(path)]
-                kwargs = {"headers": headers}
+                kwargs = {"headers": cls.headers(request)}
 
                 # Check how data should be passed
                 if verb.lower() in ["get", "head"]:
                     # Pass dict along
                     kwargs["params"] = data
                 else:
                     # Format as JSON string
```

### Comparing `ppm-utils-1.0.0b8/ppmutils/p2md.py` & `ppm-utils-1.0.1/ppmutils/p2md.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from enum import Enum
 from furl import furl
 
 from ppmutils.ppm import PPM
 from ppmutils.fhir import FHIR
-from ppmutils.settings import ppm_settings
 
-# Get the app logger
 import logging
 
-logger = logging.getLogger(ppm_settings.LOGGER_NAME)
+logger = logging.getLogger(__name__)
 
 
 class P2MD(PPM.Service):
 
-    service = "data"
-    ppm_settings_url_name = "DATA_URL"
+    service = "P2MD"
 
     # This is the system prefix used for coding DocumentReferences created by P2MD
     system = FHIR.data_document_reference_identifier_system
 
     # Set identifier systems
     p2md_identifier_system = "https://peoplepoweredmedicine.org/fhir/p2md/operation"
     fileservice_identifier_system = "https://peoplepoweredmedicine.org/fhir/fileservice/file"
@@ -26,14 +23,33 @@
     class ExportProviders(Enum):
         Participant = "ppm-participant"
         i2b2 = "ppm-i2b2"
         JSON = "ppm-json"
         FHIR = "ppm-fhir"
 
     @classmethod
+    def default_url_for_env(cls, environment):
+        """
+        Give implementing classes an opportunity to list a default set of URLs based
+        on the DBMI_ENV, if specified. Otherwise, return nothing
+        :param environment: The DBMI_ENV string
+        :return: A URL, if any
+        """
+        if "local" in environment:
+            return "https://data.ppm.aws.dbmi-loc.hms.harvard.edu"
+        elif "dev" in environment:
+            return "https://p2m2.aws.dbmi-dev.hms.harvard.edu"
+        elif "prod" in environment:
+            return "https://p2m2.dbmi.hms.harvard.edu"
+        else:
+            logger.error(f"Could not return a default URL for environment: {environment}")
+
+        return None
+
+    @classmethod
     def get_auth_link(cls, request, provider, ppm_id, return_url):
         """
         Builds and returns the link that should be followed for the user to authorize
         PPM with the provided data source.
         :param request: The original Django request
         :param provider: The desired data provider (eg Fitbit, Facebook, etc)
         :param ppm_id: The PPM ID of the current user
@@ -138,14 +154,36 @@
 
         if approvals:
             params["support_for"] = PPM.Study.get(study).value
 
         return cls.get(request, "/ppm/api/administrator/", params)
 
     @classmethod
+    def get_tracked_items(cls, request, study):
+        """
+        Make a request to P2MD to get the current list of tracked items. List
+        contains description and metadata for all items to be tracked for a
+        participant in the given study.
+
+        :param request: The current HTTP request
+        :type request: HttpRequest
+        :param study: The study to query on
+        :type study: str
+        :return: The study object
+        :rtype: dict
+        """
+        # Set query parameters
+        params = {}
+        if study:
+            params.update({"studies": PPM.Study.get(study).value})
+
+        # Ensure it's a valid study
+        return cls.get(request, "/ppm/api/trackeditem/", params)
+
+    @classmethod
     def get_authorizations(cls, request, ppm_ids):
         """
         Make a request to P2MD to determine what providers all participants
         have authorized.
         """
         return cls.get(request, "/sources/api/auths", {"ppm_ids": ",".join(ppm_ids)})
 
@@ -426,25 +464,113 @@
         # Set data
         data = {"study": study, "document_reference_id": document_reference_id}
 
         # Return True if no errors
         return cls.delete(request, f"/sources/api/consent/{study}/{ppm_id}", data)
 
     @classmethod
+    def get_study_surveys(cls, request, study):
+        """
+        Make a request to P2MD to get the current study's survey objects.
+        Objects contain details of the survey as well as the FHIR resources
+        used in PPM to track their responses.
+
+        :param request: The current HTTP request
+        :type request: HttpRequest
+        :param study: The study to query on
+        :type study: str
+        :return: The list of survey objects
+        :rtype: list
+        """
+        # Ensure it's a valid study
+        if not study or not PPM.Study.get(study) in PPM.Study:
+            raise ValueError(f"'{study}' is not a valid PPM study identifier")
+
+        return cls.get(request, "/ppm/api/survey/", {"study": PPM.Study.get(study).value})
+
+    @classmethod
+    def get_study_questionnaires(cls, request, study):
+        """
+        Make a request to P2MD to get questionnaires for the current study.
+        This returns a tuple of eligibility questionnaire ID, if any, and a
+        list of questionnaire IDs, if any.
+
+        :param request: The current request
+        :type request: HttpRequest
+        :param study: The study for which the surveys should be returned
+        :type study: str
+        :returns: A tuple of eligibility questionnaire ID and other questionnaire IDs
+        :rtype: str, list
+        """
+        # Get surveys
+        surveys = P2MD.get_qualtrics_surveys(request, study=study)
+        questionnaire_ids = [s["questionnaire_id"] for s in surveys if s.get("questionnaire_id")]
+        eligibility_questionnaire_id = next((s["questionnaire_id"] for s in surveys if s.get("eligibility_for")), None)
+
+        # Ensure the eligibility does not appear twice
+        if eligibility_questionnaire_id and eligibility_questionnaire_id in questionnaire_ids:
+            questionnaire_ids.remove(eligibility_questionnaire_id)
+
+        return eligibility_questionnaire_id, questionnaire_ids
+
+    @classmethod
     def get_qualtrics_surveys(cls, request, study):
         """
-        Make a request to P2MD to get available Qualtrics surveys
+        Make a request to P2MD to get available Qualtrics surveys that
+        are active for the passed study.
         :param request: The current request
         :param study: The study for which the surveys should be returned
         :return: list
         """
         # Return response
         return cls.get(request, f"/sources/api/qualtrics/surveys/{study}/")
 
     @classmethod
+    def get_eligibility_survey(cls, request, study):
+        """
+        Make a request to P2MD to get the eligibility survey for this study
+
+        :param request: The current request
+        :type request: HttpRequest
+        :param study: The study for which the surveys should be returned
+        :type study: str
+        :returns: The survey object, if it exists
+        :rtype: dict
+        """
+        # Set query for request
+        data = {
+            "eligibility_for": study,
+            "is_enabled": True,
+        }
+
+        # Return response
+        return next(iter(cls.get(request, "/ppm/api/survey/", data=data)), None)
+
+    @classmethod
+    def get_points_of_care_survey(cls, request, study):
+        """
+        Make a request to P2MD to get the points of care survey for this study
+
+        :param request: The current request
+        :type request: HttpRequest
+        :param study: The study for which the surveys should be returned
+        :type study: str
+        :returns: The survey object, if it exists
+        :rtype: dict
+        """
+        # Set query for request
+        data = {
+            "points_of_care_for": study,
+            "is_enabled": True,
+        }
+
+        # Return response
+        return next(iter(cls.get(request, "/ppm/api/survey/", data=data)), None)
+
+    @classmethod
     def check_qualtrics_survey(cls, request, study, ppm_id, survey_id):
         """
         Checks the passed survey to see if it has been completed by the
         passed participant or not.
         :param request: The current request
         :param study: The study for which the survey is being used
         :param ppm_id: The participant
@@ -479,28 +605,61 @@
         """
         # Return True if no errors
         url = cls._build_url(path=f"/sources/api/qualtrics/{study}/{ppm_id}/{survey_id}/")
 
         return url
 
     @classmethod
-    def get_qualtrics_survey_data(cls, request, study, ppm_id, survey_id, response_id=None, older_than=None):
+    def check_qualtrics_contact(cls, request, study, ppm_id):
+        """
+        Checks if the contact exists in P2MD and Qualtrics or not.
+        :param request: The current request
+        :param study: The study for which the contact will be taking surveys
+        :param study: The PPM identifier for the contact to add
+        :return: bool
+        """
+        # Return response
+        response = cls.head(request, f"/sources/api/qualtrics/contact/{study}/{ppm_id}/", raw=True)
+        if response:
+            return response.ok
+
+        return False
+
+    @classmethod
+    def create_qualtrics_contact(cls, request, study, ppm_id):
+        """
+        Make a request to P2MD to get available Qualtrics surveys
+        :param request: The current request
+        :param study: The study for which the contact will be taking surveys
+        :param study: The PPM identifier for the contact to add
+        :return: bool
+        """
+        # Return response
+        return cls.post(request, f"/sources/api/qualtrics/contact/{study}/{ppm_id}/")
+
+    @classmethod
+    def get_qualtrics_survey_data(
+        cls, request, study, ppm_id, survey_id, response_id=None, older_than=None, force=False
+    ):
         """
         Make a call to P2MD to look for a survey response
         """
         # Return True if no errors
         url = furl(cls.get_qualtrics_survey_data_url(study=study, ppm_id=ppm_id, survey_id=survey_id))
 
         data = {}
         if response_id:
             data["response_id"] = response_id
 
         if older_than:
             data["older_than"] = older_than
 
+        if force:
+            data["force"] = force
+
         # Make the request
         response = cls.post(request, url.pathstr, data, raw=True)
         if response:
             return response.ok
 
         return False
 
@@ -558,25 +717,27 @@
         cls,
         request,
         study,
         ppm_id,
         document_type,
         uuid,
         location,
+        hash,
         content_type="application/octect-stream",
     ):
         """
         Make a request to P2MD to create a file upload
         """
         # Set data
         data = {
             "study": study,
             "uuid": uuid,
             "location": location,
             "type": document_type,
+            "hash": hash,
             "content_type": content_type,
         }
 
         # Return True if no errors
         return cls.patch(request, f"/sources/api/file/{ppm_id}", data)
 
     @classmethod
@@ -624,24 +785,24 @@
     @classmethod
     def get_providers(cls, request=None):
         """
         Return a list of all registered data providers' codes and titles
         :param request: The current HttpRequest
         :return: list
         """
-        return cls.get(request, f"/sources/api/provider")
+        return cls.get(request, "/sources/api/provider")
 
     @classmethod
     def get_file_types(cls, request=None):
         """
         Return a list of all registered data providers' codes and titles
         :param request: The current HttpRequest
         :return: list
         """
-        return cls.get(request, f"/sources/api/file/type")
+        return cls.get(request, "/sources/api/file/type")
 
     @classmethod
     def get_participant_data_url(cls, ppm_id, filename=None, providers=None):
         """
         Downloads the PPM dataset for the passed user
         :param ppm_id: The PPM ID of the requesting user
         :param filename: What the resulting archive should be called
```

### Comparing `ppm-utils-1.0.0b8/ppmutils/tests/test_ppm.py` & `ppm-utils-1.0.1/ppmutils/tests/test_ppm.py`

 * *Files identical despite different names*

### Comparing `ppm-utils-1.0.0b8/ppmutils/tests/runtests.py` & `ppm-utils-1.0.1/ppmutils/tests/runtests.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 #!/usr/bin/env python
 """
 This script is a trick to setup a fake Django environment, since this reusable
-app will be developed and tested outside any specific Django project.
+app will be developed and tested outside any specifiv Django project.
 Via ``settings.configure`` you will be able to set all necessary settings
 for your app and run the tests as if you were calling ``./manage.py test``.
 """
 import sys
-from django_nose import NoseTestSuiteRunner
+import pytest
 from django.conf import settings
 
 EXTERNAL_APPS = [
+    "django.contrib.admin",
     "django.contrib.admindocs",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.messages",
     "django.contrib.sessions",
     "django.contrib.staticfiles",
     "django.contrib.sitemaps",
     "django.contrib.sites",
 ]
-INTERNAL_APPS = [
-    "django_nose",
-    "ppmutils",
-]
+INTERNAL_APPS = []
 INSTALLED_APPS = EXTERNAL_APPS + INTERNAL_APPS
 
 if not settings.configured:
     settings.configure(
+        SECRET_KEY="*4n1!z0%@w-e&u9c-kpyqof=-nxvx^v2m000#gf9vewm3s+_v)",
         DATABASES={
             "default": {
                 "ENGINE": "django.db.backends.sqlite3",
                 "NAME": ":memory:",
             }
         },
         INSTALLED_APPS=INSTALLED_APPS,
-        PPM_CONFIG={"FHIR_URL": "https://fhir.ppm.dbmi.hms.harvard.edu/baseDstu3"},
     )
 
 
 def main(*test_args):
-    sys.exit(NoseTestSuiteRunner(verbosity=2, interactive=True).run_tests(test_args))
+    sys.exit(pytest.main(["-x"]))
 
 
 if __name__ == "__main__":
     main(*sys.argv[1:])
```

### Comparing `ppm-utils-1.0.0b8/ppmutils/tests/test_fhir.py` & `ppm-utils-1.0.1/ppmutils/tests/test_fhir.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def setUpClass(cls):
 
         # Set the FHIR URL
         cls.fhir_url = "https://fhir.ppm.aws.dbmi-test.hms.harvard.edu"
         cls.fhir_url_pattern = r"{}/.*".format(cls.fhir_url)
 
         # Patch PPM FHIR URL
-        cls.ppm_fhir_url_patcher = mock.patch("ppmutils.fhir.FHIR.service_url")
+        cls.ppm_fhir_url_patcher = mock.patch("ppmutils.ppm.PPM.fhir_url")
         cls.mock_ppm_fhir_url = cls.ppm_fhir_url_patcher.start()
         cls.mock_ppm_fhir_url.return_value = cls.fhir_url
 
     @classmethod
     def tearDownClass(cls):
 
         # Disable patcher
```

### Comparing `ppm-utils-1.0.0b8/ppmutils/auth.py` & `ppm-utils-1.0.1/ppmutils/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,19 @@
         :returns: Whether the user has the permissions or not
         :rtype: bool
         """
         if not studies:
             # Get participant details
             patient, studies = FHIR.query_ppm_participant_details(participant)
 
+            # Ensure patient exists
+            if not studies:
+                logger.error(f'PPM/Auths: Invalid check on non-existent participant "{participant}"')
+                return False
+
         # Check for study permissions on at least one
         for study in studies:
 
             # Run the check
             item, permission = Auth.get_permission(permissions, method, study)
             if item is not None and permission is not None:
                 return True
@@ -242,14 +247,19 @@
         :returns: Whether the user has the permissions or not
         :rtype: bool
         """
         # Get participant details
         if not patient:
             patient, studies = FHIR.query_ppm_participant_details(participant)
 
+            # Ensure patient exists
+            if not patient:
+                logger.error(f'PPM/Auths: Invalid check on non-existent participant "{participant}"')
+                return False
+
         # Compare details
         if email.lower() == patient.get("email").lower() and participant == patient.get("ppm_id"):
 
             # Ensure method is not DELETE
             return method is None or method != "DELETE"
 
         return False
```

### Comparing `ppm-utils-1.0.0b8/ppmutils/qualtrics.py` & `ppm-utils-1.0.1/ppmutils/qualtrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from datetime import datetime
 from dateutil.parser import parse
 import hashlib
 import json
 import re
 import sys
 import collections
-import warnings
 from furl import furl
 import requests
 from fhirclient.models.bundle import Bundle, BundleEntry, BundleEntryRequest
 from fhirclient.models.questionnaire import Questionnaire
 
 from ppmutils.fhir import FHIR
 from ppmutils.ppm import PPM
@@ -20,14 +19,89 @@
 
 
 class Qualtrics:
     class ConversionError(Exception):
         pass
 
     @classmethod
+    def is_survey_export(cls, survey):
+        """
+        Inspects a survey export object and confirms that's what it is.
+        Qualtrics surveys can be described by three separate formats:
+        survey object from API, survey definition from API, and survey
+        export from GUI.
+
+        :param survey: The survey object in questions
+        :type survey: dict
+        :returns: Whether the passed survey object is an export or not
+        :rtype: boolean
+        """
+        return survey.get("SurveyElements") is not None
+
+    @classmethod
+    def is_survey_definition(cls, survey):
+        """
+        Inspects a survey definition object and confirms that's what it is.
+        Qualtrics surveys can be described by three separate formats:
+        survey object from API, survey definition from API, and survey
+        export from GUI.
+
+        :param survey: The survey object in questions
+        :type survey: dict
+        :returns: Whether the passed survey object is an definition or not
+        :rtype: boolean
+        """
+        return survey.get("SurveyOptions") is not None and survey.get("Questions") is not None
+
+    @classmethod
+    def is_survey_object(cls, survey):
+        """
+        Inspects a survey object and confirms that's what it is.
+        Qualtrics surveys can be described by three separate formats:
+        survey object from API, survey definition from API, and survey
+        export from GUI.
+
+        :param survey: The survey object in questions
+        :type survey: dict
+        :returns: Whether the passed survey object is an object or not
+        :rtype: boolean
+        """
+        return survey.get("name") is not None and survey.get("questions") is not None
+
+    @classmethod
+    def get_survey_response_metadata(cls, response):
+        """
+        Given a Qualtrics survey response object from the API, this returns
+        a dictionary of metadata for the response relating to the study
+        and the participant who created the response.
+
+        :param response: A Qualtrics API response object
+        :type response: dict
+        :return: A dictionary of metadata
+        :rtype: dict
+        """
+        # Set basic details
+        metadata = {"response_id": response.get("responseId")}
+
+        # Get values dictionary
+        values = response.get("values")
+        if values:
+
+            # Set data
+            metadata.update(
+                {
+                    "study": values.get("ppm_study", ""),
+                    "ppm_id": values.get("ppm_id", values.get("externalDataReference", "")),
+                    "survey_id": values.get("SurveyID", ""),
+                }
+            )
+
+        return metadata
+
+    @classmethod
     def questionnaire(cls, survey, survey_id, questionnaire_id=None):
         """
         Accepts a Qualtrics survey definition (QSF) and creates a FHIR
         Questionnaire resource from it. Does not support all of Qualtrics
         functionality and will fail where question-types or other unsupported
         features are encountered.add()
 
@@ -134,15 +208,15 @@
             }
         elif type(_blocks) is dict:
             blocks = {
                 f: next(b for b in _blocks.values() if b["Type"] in ["Default", "Standard"] and b["ID"] == f)
                 for f in flows
             }
         else:
-            logger.error(f"PPM/Qualtrics: Invalid Qualtrics block spec")
+            logger.error("PPM/Qualtrics: Invalid Qualtrics block spec")
 
         questions = {f: [e["QuestionID"] for e in blocks[f]["BlockElements"] if e["Type"] == "Question"] for f in flows}
 
         # Walk through elements
         for block_id, block in blocks.items():
 
             # Check if we need this grouped
@@ -255,15 +329,15 @@
         :return: The FHIR QuestionnaireItem resource
         :rtype: dict
         """
         # Set root link ID
         link_id = cls._qid_to_linkid(question_id)
 
         # Strip text of HTML and other characters
-        text = re.sub("<[^<]+?>", "", question["QuestionText"]).strip().replace("\n", "").replace("\r", "")
+        text = re.sub("<[^<]+?>", "", question["QuestionText"]).strip().replace("\n", " ").replace("\r", "")
 
         # Determine if required
         required = question["Validation"].get("Settings", {}).get("ForceResponse", False) == "ON"
 
         # Get question text
         item = {
             "linkId": link_id,
@@ -514,15 +588,15 @@
                             }
                         )
 
                     item["item"].append(sub_item)
 
             else:
                 logger.error(
-                    "PPM/Questionnaire: Unhandled survey question" f" type {survey_id}/{question_id}: {question_type}"
+                    "PPM/Questionnaire: Unhandled survey question type {survey_id}/{question_id}: {question_type}"
                 )
                 raise ValueError(f"Failed to process survey {survey_id}")
         except Exception as e:
             logger.exception(
                 f"PPM/FHIR: Error processing questionnaire item: {e}",
                 exc_info=True,
                 extra={
@@ -532,49 +606,51 @@
                 },
             )
             raise e
 
         return item
 
     @classmethod
-    def questionnaire_response(cls, study, ppm_id, questionnaire_id, survey_id, survey, response_id, response):
+    def questionnaire_response(
+        cls, study, ppm_id, questionnaire_id, survey_id, response_id, survey_definition=None, survey=None, response=None
+    ):
         """
         Returns QuestionnaireResponse resource for a survey taken through
         Qualtrics. This method requires that Qualtrics question names are
-        matched to the FHIR Questionnaire linkIds.
+        matched to the FHIR Questionnaire linkIds. If the response data is not
+        available, an empty QuestionnaireResponse is created to be updated
+        at a later time.
 
         :param study: The study for which the questionnaire was given
         :type study: PPM.Study
         :param ppm_id: The PPM ID for the participant who took the survey
         :type ppm_id: str
         :param questionnaire_id: The ID for the related FHIR Questionnaire
         :type questionnaire_id: str
         :param survey_id: The ID of the Qualtrics survey
         :type survey_id: str
-        :param survey: The Qualtrics survey object
-        :type survey: dict
         :param response_id: The ID of the Qualtrics survey response
         :type response_id: str
+        :param survey_definition: The Qualtrics survey definition object
+        :type survey_definition: dict, defaults to None
+        :param survey: The Qualtrics survey object
+        :type survey: dict, defaults to None
         :param response: The Qualtrics survey response object
-        :type response: dict
+        :type response: dict, defaults to None
         :return: The QuestionnaireResponse resource
         :rtype: dict
         """
-        # Build a dictionary describing block and question order
-        blocks = {
-            f["id"]: [
-                e["questionId"] for e in survey["blocks"][f["id"]].get("elements", []) if e.get("type") == "Question"
-            ]
-            for f in survey["flow"]
-            if f.get("type") == "Block"
-        }
+        # Run checks
+        if survey and not Qualtrics.is_survey_object(survey):
+            raise ValueError("PPM/Qualtrics: survey is not a valid Qualtrics API survey object")
 
-        # Build response groups
-        items = list(cls.questionnaire_response_item_generator(survey, response, blocks))
+        if survey_definition and not Qualtrics.is_survey_definition(survey_definition):
+            raise ValueError("PPM/Qualtrics: survey_definition is not a valid Qualtrics API survey definition object")
 
+        # Prepare resource properties
         data = {
             "resourceType": "QuestionnaireResponse",
             "meta": {"lastUpdated": datetime.now().isoformat()},
             "identifier": {
                 "system": FHIR.qualtrics_response_identifier_system,
                 "value": response_id,
             },
@@ -586,42 +662,59 @@
             "authored": datetime.now().isoformat(),
             "extension": [
                 {
                     "url": FHIR.qualtrics_survey_extension_url,
                     "valueString": survey_id,
                 }
             ],
-            "item": items,
         }
 
-        # Set dates if specified.
-        if response.get("endDate"):
-            data["authored"] = response["endDate"]
+        # If response, parse answers
+        if response and survey:
+
+            # Build a dictionary describing block and question order
+            blocks = {
+                f["id"]: [
+                    e["questionId"]
+                    for e in survey["blocks"][f["id"]].get("elements", [])
+                    if e.get("type") == "Question"
+                ]
+                for f in survey["flow"]
+                if f.get("type") == "Block"
+            }
+
+            # Build response groups and add it to the questionnair response
+            data["item"] = list(cls.questionnaire_response_item_generator(survey_definition, survey, response, blocks))
+
+            # Set dates if specified.
+            if response.get("endDate"):
+                data["authored"] = response["endDate"]
 
         return data
 
     @classmethod
-    def questionnaire_response_item_generator(cls, survey, response, blocks):
+    def questionnaire_response_item_generator(cls, survey_definition, survey, response, blocks):
         """
         Accepts the survey, response objects as well as the list of blocks add their
         respective questions and yields a set of QuestionnareResponseItem
         resources to be set for the QuestionnaireResponse.
 
+        :param survey_definition: The Qualtrics survey definition object
+        :type survey_definition: dict, defaults to None
         :param survey: The Qualtrics survey object
         :type survey: object
         :param response: The Qualtrics survey response item
         :type response: object
         :param blocks: The dictionary of blocks comprising the survey
         :type blocks: dict
-        :param blocks: The ID of the specific block to process
-        :type blocks: str
         :raises Exception: Raises exception if value is an unhandled type
         :returns A generator of QuestionnaireResponseItem resources
         :rtype generator
         """
+        question_id = None
         for block_id, question_ids in blocks.items():
             try:
                 # Get the block
                 block = survey["blocks"][block_id]
 
                 # Set root link ID
                 link_id = f"group-{block_id.replace('BL_', '')}"
@@ -661,46 +754,245 @@
                     if answers:
                         yield {
                             "linkId": link_id,
                             "answer": answers,
                         }
 
                 else:
-                    # Filter values to those for this block/group
-                    values = {
-                        k: v
-                        for k, v in response["values"].items()
-                        if re.match(rf"^({'|'.join(question_ids)}[^\d]?)", k)
-                    }
-                    if not values:
-                        logger.warning(f"PPM/FHIR/Qualtrics: Cannot find values for '{block_id}/{question_ids}'")
-                        continue
-
-                    # Get items
-                    items = [cls.questionnaire_response_item(survey, response, key) for key in values.keys()]
-
-                    # Weed out duplicates
-                    filtered_items = [i for n, i in enumerate(items) if i not in items[n + 1 :] and i is not None]
-
-                    # We don't want to group un-repeated items, so just return them
-                    for item in filtered_items:
-                        yield item
+                    # Iterate questions
+                    for question_id in question_ids:
+
+                        # Filter values to those for this block/group
+                        pattern = rf"^({question_id})(?![S\d])"
+                        values = {k: v for k, v in response["values"].items() if re.match(pattern, k)}
+                        if not values:
+
+                            # Check each question
+                            if Qualtrics.survey_response_is_required(
+                                survey_definition=survey_definition, survey=survey, response=response, key=question_id
+                            ):
+                                logger.error(
+                                    f'PPM/Qualtrics: No value(s) for required "{question_id}"',
+                                    extra={
+                                        **Qualtrics.get_survey_response_metadata(response),
+                                        "block_id": block_id,
+                                        "question_id": question_id,
+                                    },
+                                )
+
+                            # Nothing else to do
+                            continue
+
+                        # Get items
+                        items = [cls.questionnaire_response_item(survey, response, key) for key in values.keys()]
+
+                        # Weed out duplicates
+                        filtered_items = [i for n, i in enumerate(items) if i not in items[n + 1 :] and i is not None]
+
+                        # We don't want to group un-repeated items, so just return them
+                        for item in filtered_items:
+                            yield item
 
             except Exception as e:
                 logger.exception(
-                    f"PPM/FHIR: Error processing block {block_id}: {e}",
+                    f"PPM/Qualtrics: Error processing block/question {block_id}/{question_id}: {e}",
                     exc_info=True,
                     extra={
-                        "survey_id": survey["id"],
+                        **Qualtrics.get_survey_response_metadata(response),
                         "block_id": block_id,
+                        "question_id": question_id,
                     },
                 )
                 raise e
 
     @classmethod
+    def survey_response_is_required(cls, survey_definition, survey, response, key):
+        """
+        Returns whether a response to the question is required or not according
+        to the Qualtrics survey object. This inspects not only properties of
+        the question but also ensures it's enabled via conditional logic. If
+        not enabled, will not be returned as required.
+
+        :param survey_definition: The Qualtrics survey definition object
+        :type survey_definition: dict, defaults to None
+        :param survey: The Qualtrics survey object
+        :type survey: object
+        :param response: The response object
+        :type response: dict
+        :param key: The Qualtrics question ID to process
+        :type key: str
+        :raises Exception: Raises exception if value is an unhandled type
+        :return: Whether the question is required or not
+        :rtype: boolean
+        """
+        try:
+            # Get ID
+            survey_id = survey["id"]
+
+            # Get questions
+            question = survey["questions"].get(key)
+            if not question:
+                logger.error(
+                    f"PPM/Qualtrics/{key}: Question not found",
+                    extra={
+                        "key": key,
+                    },
+                )
+
+            question_definition = survey_definition["Questions"].get(key)
+            if not question:
+                logger.error(
+                    f"PPM/Qualtrics/{key}: Question definition not found",
+                    extra={
+                        "key": key,
+                    },
+                )
+
+            # Check if required
+            if not question.get("validation", {}).get("doesForceResponse", False):
+                return False
+
+            # It's required, but check if it is conditionally enabled
+            display_logic = question_definition.get("DisplayLogic", False)
+            enabled = False
+            if display_logic:
+                logger.debug(f"PPM/Qualtrics/{survey_id}/{key}: Is required but also conditionally enabled")
+
+                # We are only processing BooleanExpressions
+                if display_logic["Type"] != "BooleanExpression":
+                    logger.error(
+                        f"PPM/Qualtrics/{survey_id}/{key}: Unhandled DisplayLogic type: {display_logic.get('Type')}",
+                        extra={
+                            "survey_id": survey_id,
+                            "qid": key,
+                            "question": question,
+                            "question_definition": question_definition,
+                            "display_logic": display_logic,
+                        },
+                    )
+                    return False
+
+                # Iterate conditions for display of this question
+                # INFO: Currently only selected choice conditions are supported
+                for expression in [v for k, v in display_logic.items() if type(v) is dict]:
+
+                    # Check type
+                    if expression["Type"] == "If":
+
+                        # TODO: Not implemented to handle multiple logical statements
+                        if len([v for k, v in expression.items() if type(v) is dict]) > 1:
+                            logger.error(
+                                f"PPM/Qualtrics/{survey_id}/{key}: Multiple DisplayLogic statements found",
+                                extra={
+                                    "survey_id": survey_id,
+                                    "qid": key,
+                                    "question": question,
+                                    "question_definition": question_definition,
+                                    "display_logic": display_logic,
+                                },
+                            )
+
+                        # Iterate statements
+                        for statement in [v for k, v in expression.items() if type(v) is dict]:
+
+                            # Fetch the value of the answer
+                            components = furl(statement["LeftOperand"]).path.segments
+
+                            # Check type
+                            if components[0] == "SelectableChoice":
+
+                                # Get answer index and value
+                                index = components[1]
+
+                                # Find question
+                                condition_qid = statement["QuestionID"]
+                                conditional_question = survey_definition["Questions"][condition_qid]
+
+                                # Get answer value
+                                conditional_value = next(
+                                    c["Display"] for i, c in conditional_question["Choices"].items() if i == index
+                                )
+                                logger.debug(
+                                    f"PPM/Qualtrics/{survey_id}/{key}: Depends on {condition_qid} = "
+                                    f"{conditional_value}"
+                                )
+
+                                # Get the actual response
+                                responded_answer_items = Qualtrics.get_survey_response_values(
+                                    survey=survey, response=response, qid=condition_qid
+                                )
+                                responded_values = [v for a in responded_answer_items for k, v in a.items()]
+
+                                # Check if matches
+                                if responded_values and conditional_value in responded_values:
+                                    logger.debug(
+                                        f"PPM/Qualtrics/{survey_id}/{key}: Condition {condition_qid} = "
+                                        f"{responded_values} is satisfied"
+                                    )
+
+                                    # Set enabled
+                                    enabled = True
+                                else:
+                                    logger.debug(
+                                        f"PPM/Qualtrics/{survey_id}/{key}: Condition {condition_qid} = "
+                                        f"{responded_values} is NOT satisfied"
+                                    )
+
+                                    # Set disabled
+                                    enabled = False
+
+            logger.debug(f"PPM/Qualtrics/{survey_id}/{key}: Conditional question is {'' if enabled else 'NOT '}enabled")
+            return enabled
+
+        except Exception as e:
+            logger.exception(
+                f"PPM/Qualtrics: Error checking requirement: {e}",
+                exc_info=True,
+                extra={
+                    "survey_id": survey.get("id"),
+                    "response_id": response.get("responseId"),
+                    "question_id": key,
+                },
+            )
+
+        # Assume required
+        return True
+
+    @classmethod
+    def get_survey_response_values(cls, survey, response, qid):
+        """
+        This method parses a survey response and returns the value of the
+        response for the given question, if any at all.
+
+        :param survey: The survey object the response was for
+        :type survey: dict
+        :param response: The response object
+        :type response: dict
+        :param qid: The question ID to get the response value for
+        :type qid: str
+        :return: The response value(s), if any
+        :rtype: list, defaults to None
+        """
+        # Filter values to those for this block/group
+        pattern = rf"^({qid})(?![S\d])"
+        values = {k: v for k, v in response["values"].items() if re.match(pattern, k)}
+        if not values:
+            return None
+
+        # Get items
+        items = [cls.questionnaire_response_item(survey, response, key) for key in values.keys()]
+
+        # Get the first valid item
+        item = next((i for i in items if i and i.get("answer")), None)
+        if not item:
+            return None
+
+        return item.get("answer")
+
+    @classmethod
     def questionnaire_response_item(cls, survey, response, key, loop=None):
         """
         Returns a FHIR QuestionnaireResponse.Item resource for the passed
         Qualtrics survey question response key and loop (if applicable).
 
         :param survey: The Qualtrics survey object
         :type survey: object
@@ -799,15 +1091,16 @@
                             _q_subid = key_regex.match(k).groupdict()["subid"]
 
                             # Add the label
                             answer.append(survey["questions"][_q_id]["subQuestions"][_q_subid]["choiceText"])
 
                 else:
                     logger.error(
-                        f"PPM/Questionnaire: Unhandled singular hot spot Qualtrics " f"answer item: {key} = {value}"
+                        f"PPM/QuestionnaireResponse/{key}: Unhandled "
+                        f"singular hot spot Qualtrics answer item: {value}"
                     )
                     return None
 
             # This is a matrix, single answer question
             elif question_type == "Matrix" and type(value) is int:
 
                 # Just set label
@@ -835,15 +1128,15 @@
                         _responses = collections.OrderedDict(sorted(_responses.items()))
 
                         # Join them together
                         answer = " ".join([response["labels"][k] for k, v in _responses.items()])
 
                     else:
                         logger.error(
-                            f"PPM/Questionnaire: Unhandled drill down Qualtrics " f"answer item: {key} = {value}"
+                            f"PPM/QuestionnaireResponse/{key}: Unhandled drill down Qualtrics answer item: {value}"
                         )
                         return None
 
             # This is a multiple-choice, single answer question (radio)
             elif question_type == "MC" and type(value) is int:
 
                 # Add it
@@ -858,16 +1151,28 @@
                 # Set link ID for sub question
                 if q_subid:
                     link_id = f"{link_id}-{q_columnid}-{q_subid}"
 
             # This is a multiple-choice scale, multiple answer question (matrix)
             elif question_type == "MC" and type(value) is list:
 
-                # Index to a list of options
-                value_list = response["labels"].get(key)
+                # If the answer is empty but this is a forced response, it's likely that this question has
+                # a "None of the above" option and that's what was selected. Qualtrics just returns an empty
+                # response in this instance.
+                none_of_the_above = next(
+                    (v["choiceText"] for k, v in question["choices"].items() if v.get("analyze") is False), None
+                )
+                if len(value) == 0 and question.get("validation", {}).get("doesForceResponse") and none_of_the_above:
+
+                    # Use that answer
+                    value_list = [none_of_the_above]
+
+                else:
+                    # Index to a list of options
+                    value_list = response["labels"].get(key)
 
                 # Set link ID for sub question
                 if q_subid:
                     link_id = link_id + "-" + q_subid
 
                 # Set the answer
                 answer = value_list
@@ -885,27 +1190,39 @@
                 value_list = response["labels"].get(key)
 
                 # Add it
                 answer = value_list
 
             else:
                 logger.error(
-                    f"PPM/Questionnaire: Unhandled Qualtrics "
-                    f"answer item: {key} = {value} ({q_id}/"
+                    f"PPM/QuestionnaireResponse/{key}: Unhandled Qualtrics "
+                    f"answer item: {value} ({q_id}/"
                     f"{q_subid}/{q_type})"
                 )
 
         except (IndexError, ValueError, KeyError, TypeError) as e:
             logger.exception(
-                f"PPM/Questionnaire: Unhandled Qualtrics " f"answer item: {key}: {e}",
+                f"PPM/QuestionnaireResponse/{key}: Unhandled  Qualtrics answer item: {key}: {e}",
                 exc_info=True,
             )
 
         # Check
-        if not link_id or not answer:
+        if not link_id:
+            logger.debug(
+                f"PPM/Qualtrics/QuestionnaireResponse/{key}:Ignoring Qualtrics response answer item due to no link ID"
+            )
+            return None
+
+        # Check answer
+        if answer is None:
+            logger.debug(
+                f"PPM/Qualtrics/QuestionnaireResponse/{key}:"
+                f"Ignoring Qualtrics response due to no answer: "
+                f"{value} = {answer}"
+            )
             return None
 
         # Return response after formatting answer
         return {"linkId": link_id, "answer": FHIR.Resources._questionnaire_response_answer(answer)}
 
     @classmethod
     def questionnaire_transaction(cls, questionnaire, questionnaire_id=None):
@@ -929,15 +1246,15 @@
         if questionnaire_id:
             query["_id"] = questionnaire_id
 
         questionnaires = FHIR._query_resources("Questionnaire", query)
         if questionnaires:
 
             # No need to recreate it
-            logger.debug(f"API/Qualtrics: Questionnaire already exists for survey version {version}")
+            logger.debug(f"PPM/Qualtrics: Questionnaire already exists for survey version {version}")
             return None
 
         # Use the FHIR client lib to validate our resource.
         questionnaire = Questionnaire(questionnaire)
         questionnaire_request = BundleEntryRequest(
             {
                 "url": f"Questionnaire/{questionnaire_id}" if questionnaire_id else "Questionnaire",
@@ -951,472 +1268,11 @@
         # Validate it.
         bundle = Bundle()
         bundle.entry = [questionnaire_entry]
         bundle.type = "transaction"
 
         # Create the organization
         response = requests.post(PPM.fhir_url(), json=bundle.as_json())
-        logger.debug("Response: {}".format(response.status_code))
+        logger.debug("PPM/Qualtrics: FHIR Response: {}".format(response.status_code))
         response.raise_for_status()
 
         return response.json()
-
-    @classmethod
-    def ppm_qualtrics_survey_questionnaire(cls, study, questionnaire_id, survey_id, survey):
-        """
-        Returns QuestionnaireResponse resource for a survey taken through
-        Qualtrics. This method requires that Qualtrics question names are
-        matched to the FHIR Questionnaire linkIds.
-
-        :param study: The study for which the questionnaire was given
-        :type study: PPM.Study
-        :param questionnaire_id: The ID for the related FHIR Questionnaire
-        :type questionnaire_id: str
-        :param survey_id: The ID of the Qualtrics survey
-        :type survey_id: str
-        :param survey: The survey object from Qualtrics
-        :type survey: dict
-        :return: The QuestionnaireResponse resource
-        :rtype: dict
-        """
-        warnings.warn(f"This method should not be used. Instead use Qualtrics.questionnaire()", DeprecationWarning)
-
-        # Hash the questions of the survey to track version of the survey
-        version = hashlib.md5(json.dumps(survey["questions"], sort_keys=True).encode()).hexdigest()
-
-        # Build a dictionary describing block and question order
-        blocks = {
-            f["id"]: [
-                e["questionId"] for e in survey["blocks"][f["id"]].get("elements", []) if e.get("type") == "Question"
-            ]
-            for f in survey["flow"]
-            if f.get("type") == "Block"
-        }
-
-        # Build list of items
-        items = []
-        for _, question_ids in blocks.items():
-
-            # Create them
-            items.extend(
-                [
-                    cls.ppm_qualtrics_survey_questionnaire_item(survey, qid, survey["questions"][qid])
-                    for qid in question_ids
-                ]
-            )
-
-        # Build the resource
-        data = {
-            "id": questionnaire_id,
-            "resourceType": "Questionnaire",
-            "meta": {"lastUpdated": datetime.now().isoformat()},
-            "identifier": [
-                {
-                    "system": FHIR.qualtrics_survey_identifier_system,
-                    "value": survey_id,
-                },
-                {
-                    "system": FHIR.qualtrics_survey_version_identifier_system,
-                    "value": version,
-                },
-            ],
-            "version": version,
-            "name": survey_id,
-            "title": survey["name"],
-            "status": "active" if survey["isActive"] else "draft",
-            "approvalDate": survey["creationDate"],
-            "date": survey["lastModifiedDate"],
-            "extension": [
-                {
-                    "url": FHIR.qualtrics_survey_extension_url,
-                    "valueString": survey_id,
-                }
-            ],
-            "item": items,
-        }
-
-        # If expiration, add it
-        if survey.get("expiration", {}).get("startDate"):
-
-            data["effectivePeriod"] = {
-                "start": survey["expiration"]["startDate"],
-                "end": survey["expiration"]["endDate"],
-            }
-
-            # If after expiration, set status
-            if survey["expiration"].get("endDate"):
-                if parse(survey["expiration"]["endDate"]) < datetime.now():
-                    data["status"] = "retired"
-
-        return data
-
-    @classmethod
-    def ppm_qualtrics_survey_questionnaire_items(cls, survey, blocks):
-        """
-        Accepts the survey object as well as the list of blocks and their
-        respective questions and yields a set of QuestionnareItem
-        resources to be set for the Questionnaire.
-
-        :param survey: The Qualtrics survey object
-        :type survey: object
-        :param blocks: The dictionary of blocks comprising the survey
-        :type blocks: dict
-        :raises Exception: Raises exception if value is an unhandled type
-        :returns A generator of QuestionnaireItem resources
-        :rtype generator
-        """
-        warnings.warn(
-            f"This method should not be used. Instead use Qualtrics.questionnaire_item_generator()", DeprecationWarning
-        )
-        for block_id, question_ids in blocks.items():
-            try:
-                # Get the block
-                block = survey["blocks"][block_id]
-
-                # Set root link ID
-                link_id = f"group-{block_id.replace('BL_', '')}"
-
-                # Get all questions in this block
-                question_ids = [e["questionId"] for e in block["elements"] if e["type"] == "Question"]
-
-                # Check if repeating
-                if survey.get("loopAndMerge").get(block_id, None):
-
-                    # Create this
-                    pass
-
-                else:
-
-                    # Process each question
-                    for question_id in question_ids:
-
-                        # Set root link ID
-                        link_id = cls._qid_to_linkid(question_id)
-
-                        # Fetch the question
-                        question = survey["questions"][question_id]
-
-                        # Strip text of HTML and other characters
-                        text = (
-                            re.sub("<[^<]+?>", "", question["QuestionText"]).strip().replace("\n", "").replace("\r", "")
-                        )
-                        text = text.replace("&nbsp;", " ")
-
-                        # Determine if required
-                        required = question["validation"].get("doesForceResponse", False)
-
-                        # Get question text
-                        item = {
-                            "linkId": link_id,
-                            "text": text,
-                            "required": required,
-                        }
-
-                        yield item
-
-            except Exception as e:
-                logger.exception(
-                    f"PPM/FHIR: Error processing block {block_id}: {e}",
-                    exc_info=True,
-                    extra={
-                        "survey_id": survey["id"],
-                        "block_id": block_id,
-                    },
-                )
-                raise e
-
-    @classmethod
-    def ppm_qualtrics_survey_questionnaire_item(cls, survey, qid, question):
-        """
-        Returns a FHIR resource for a QuestionnaireItem parsed from
-        the Qualtrics survey's question
-
-        :param survey: The Qualtrics survey object
-        :type survey: dict
-        :param qid: The Qualtrics survey question identifier
-        :type qid: str
-        :param question: The Qualtrics survey question object
-        :type question: dict
-        :raises Exception: Raises exception if question is an unhandled type
-        :return: The FHIR QuestionnaireItem resource
-        :rtype: dict
-        """
-        warnings.warn(
-            f"This method should not be used. Instead use Qualtrics.questionnaire_item()",
-            DeprecationWarning,
-        )
-        # Get common survey info
-        survey_id = survey["id"]
-
-        # Set root link ID
-        link_id = cls._qid_to_linkid(qid)
-
-        # Strip text of HTML and other characters
-        text = re.sub("<[^<]+?>", "", question["questionText"]).strip().replace("\n", "").replace("\r", "")
-
-        # Remove nbsp;'s
-        text.replace("&nbsp;", "")
-
-        # Get question text
-        item = {"linkId": link_id, "text": text, "required": question["validation"].get("doesForceResponse", False)}
-
-        # Check for conditional enabling
-        if question.get("DisplayLogic", False):
-
-            # Intialize enableWhen item
-            enable_whens = []
-
-            # We are only processing BooleanExpressions
-            if question["DisplayLogic"]["Type"] != "BooleanExpression":
-                logger.error(
-                    f"PPM/Questionnaire: Unhandled DisplayLogic " f"type {survey_id}/{qid}: {question['DisplayLogic']}"
-                )
-                raise ValueError(f"Failed to process survey {survey['id']}")
-
-            # Iterate conditions for display of this question
-            # INFO: Currently only selected choice conditions are supported
-            for k, expression in question["DisplayLogic"].items():
-
-                # Check type
-                if expression["Type"] == "If":
-
-                    # Iterate statements
-                    for j, statement in expression.items():
-
-                        # Fetch the value of the answer
-                        components = furl(statement["LeftOperand"]).path.segments
-
-                        # Check type
-                        if components[0] == "SelectableChoice":
-
-                            # Get answer index and value
-                            index = components[1]
-
-                            # Find question
-                            conditional_question = next(
-                                e for e in survey["SurveyElements"] if e["PrimaryAttribute"] == qid
-                            )
-
-                            # Get answer value
-                            conditional_value = next(
-                                c["Display"] for i, c in conditional_question["Payload"]["Choices"] if i == index
-                            )
-
-                            # Add it
-                            enable_whens.append(
-                                {
-                                    "question": cls._qid_to_linkid(qid),
-                                    "answerString": conditional_value,
-                                }
-                            )
-
-                        else:
-                            logger.error(
-                                f"PPM/Questionnaire: Unhandled DisplayLogic expression"
-                                f"type {survey_id}/{qid}: {expression}"
-                            )
-                            raise ValueError(f"Failed to process survey {survey['id']}")
-
-                else:
-                    logger.error(f"PPM/Questionnaire: Unhandled DisplayLogic " f"type {survey_id}/{qid}: {expression}")
-                    raise ValueError(f"Failed to process survey {survey['id']}")
-
-            # Add enableWhen's if we've got them
-            if enable_whens:
-                item["enableWhen"] = enable_whens
-
-        # Check type
-        question_type = question["questionType"]
-
-        try:
-            # Text (single line)
-            if question_type["type"] == "TE" and question_type["selector"] == "SL":
-
-                # Set type
-                item["type"] = "string"
-
-            # Text (multiple line)
-            elif question_type["type"] == "TE" and question_type["selector"] == "ESTB":
-
-                # Set type
-                item["type"] = "text"
-
-            # Text (multiple line)
-            elif question_type["type"] == "TE" and question_type["selector"] == "ML":
-
-                # Set type
-                item["type"] = "text"
-
-            # Multiple choice (single answer)
-            elif question_type["type"] == "MC" and question_type["selector"] == "SAVR":
-
-                # Set type
-                item["type"] = "choice"
-
-                # Set choices
-                item["option"] = [{"valueString": c["choiceText"]} for k, c in question["choices"].items()]
-
-            # Multiple choice (multiple answer)
-            elif question_type["type"] == "MC" and question_type["selector"] == "MAVR":
-
-                # Set type
-                item["type"] = "choice"
-                item["repeats"] = True
-
-                # Set choices
-                item["option"] = [{"valueString": c["choiceText"]} for k, c in question["choices"].items()]
-
-            # Matrix (single answer)
-            elif (
-                question_type["type"] == "Matrix"
-                and question_type["selector"] == "Likert"
-                and question_type["subSelector"] == "SingleAnswer"
-            ):
-
-                # Add this as a grouped set of multiple choice, single answer questions
-                item["type"] = "group"
-
-                # Preselect choices
-                choices = [{"valueString": c["choiceText"]} for k, c in question["choices"].items()]
-
-                # Set subitems
-                item["item"] = [
-                    {
-                        "linkId": f"{link_id}-{k}",
-                        "text": s["choiceText"],
-                        "type": "choice",
-                        "option": choices,
-                        "required": question["validation"].get("doesForceResponse", False),
-                    }
-                    for k, s in question["subQuestions"].items()
-                ]
-
-            # Matrix (multiple answer)
-            elif (
-                question_type["type"] == "Matrix"
-                and question_type["selector"] == "Likert"
-                and question_type["subSelector"] == "MultipleAnswer"
-            ):
-
-                # Add this as a grouped set of multiple choice, single answer questions
-                item["type"] = "group"
-                item["repeats"] = True
-
-                # Preselect choices
-                choices = [{"valueString": c["choiceText"]} for k, c in question["choices"].items()]
-
-                # Set subitems
-                item["item"] = [
-                    {
-                        "linkId": f"{link_id}-{k}",
-                        "text": s["choiceText"],
-                        "type": "choice",
-                        "option": choices,
-                        "required": question["validation"].get("doesForceResponse", False),
-                    }
-                    for k, s in question["subQuestions"].items()
-                ]
-
-            # Multiple Matrix (multiple answer)
-            elif question_type["type"] == "SBS" and question_type["selector"] == "SBSMatrix":
-
-                item["type"] = "group"
-                item["text"] = question["questionText"]
-                item["item"] = []
-
-                # Get choices
-                questions = {k: c["choiceText"] for k, c in question["subQuestions"].items()}
-
-                # Add this as multiple grouped sets of multiple choice, single answer questions
-                for k, additional_question in question["columns"].items():
-
-                    # Add another display for the subquestion
-                    sub_item = {
-                        "linkId": f"{link_id}-{k}",
-                        "type": "group",
-                        "text": additional_question["questionText"],
-                        "item": [],
-                    }
-
-                    # Preselect choices
-                    answers = [{"valueString": c["choiceText"]} for k, c in additional_question["choices"].items()]
-
-                    # Add a question per choice
-                    for sub_k, sub_question in questions.items():
-
-                        # Remove prefixes, if set
-                        sub_question = re.sub(r"^[\d]{1,4}\.\s", "", sub_question)
-
-                        # Set subitems
-                        sub_item["item"].append(
-                            {
-                                "linkId": f"{link_id}-{k}-{sub_k}",
-                                "text": sub_question,
-                                "type": "choice",
-                                "option": answers,
-                                "required": question["validation"].get("doesForceResponse", False),
-                            }
-                        )
-
-                    # Add it
-                    item["item"].append(sub_item)
-
-            # Slider (integer answer)
-            elif question_type["type"] == "Slider" and question_type["selector"] == "HBAR":
-
-                # Set type
-                item["type"] = "integer"
-
-            # Slider (integer answer)
-            elif question_type["type"] == "Slider" and question_type["selector"] == "HSLIDER":
-
-                # Set type
-                item["type"] = "decimal"
-
-            # Hot spot (multiple choice, multiple answer)
-            elif question_type["type"] == "HotSpot" and question_type["selector"] == "OnOff":
-
-                # Set type
-                item["type"] = "choice"
-                item["repeats"] = True
-
-                # Set choices
-                item["option"] = [{"valueString": c["choiceText"]} for k, c in question["subQuestions"].items()]
-
-            # Drill down
-            elif question_type["type"] == "DD" and question_type["selector"] == "DL":
-
-                # Set type
-                item["type"] = "choice"
-                item["repeats"] = False
-
-                # Set choices
-                item["option"] = [{"valueString": c["Display"]} for k, c in question["Answers"].items()]
-
-            # Descriptive text
-            elif question_type["type"] == "DB":
-
-                # Set type
-                item["type"] = "display"
-
-            # Descriptive graphics
-            elif question_type["type"] == "GB":
-
-                # Set type
-                item["type"] = "display"
-
-            else:
-                logger.error("PPM/Questionnaire: Unhandled survey question" f" type {survey_id}/{qid}: {question_type}")
-                raise ValueError(f"Failed to process survey {survey['id']}")
-        except Exception as e:
-            logger.exception(
-                f"PPM/FHIR: Error processing question" f" {survey_id}/{qid}: {e}",
-                exc_info=True,
-                extra={
-                    "survey_id": survey["id"],
-                    "qid": qid,
-                    "question": question,
-                },
-            )
-            raise e
-
-        return item
```

