# Comparing `tmp/maisaedu-utilities-prefect-1.0.8.tar.gz` & `tmp/maisaedu-utilities-prefect-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maisaedu-utilities-prefect-1.0.8.tar", last modified: Wed Nov 16 19:23:50 2022, max compression
+gzip compressed data, was "maisaedu-utilities-prefect-1.0.9.tar", last modified: Wed Nov 16 19:30:50 2022, max compression
```

## Comparing `maisaedu-utilities-prefect-1.0.8.tar` & `maisaedu-utilities-prefect-1.0.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:50.235916 maisaedu-utilities-prefect-1.0.8/
--rw-r--r--   0 vsts      (1001) docker     (122)     1081 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      286 2022-11-16 19:23:50.235916 maisaedu-utilities-prefect-1.0.8/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:50.231916 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/
--rw-r--r--   0 vsts      (1001) docker     (122)      551 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:50.231916 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/constants/
--rw-r--r--   0 vsts      (1001) docker     (122)       81 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/constants/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       41 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/constants/environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)       31 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/constants/notification.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:50.231916 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/database/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/database/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2819 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/database/postgres.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11374 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/deploy.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3955 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/dw.py
--rw-r--r--   0 vsts      (1001) docker     (122)      349 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/environment.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:50.231916 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/googlesheet/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/googlesheet/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1044 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/googlesheet/gspread.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:50.235916 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1406 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/associations.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1748 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/company.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5247 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/contacts.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1653 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/contacts_lists.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3970 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/deals.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2222 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/email_events.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1631 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/forms.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2023 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/forms_submissions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3833 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/landing_pages.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1627 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/lineItems.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2060 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/marketing_emails.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2864 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/objects.py
--rw-r--r--   0 vsts      (1001) docker     (122)      693 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/owners.py
--rw-r--r--   0 vsts      (1001) docker     (122)      916 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/pipelines.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7425 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/tickets.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2325 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/notification.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:50.235916 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:50.235916 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1955 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:50.235916 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/services/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/services/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4921 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2778 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2605 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/services/client.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:50.235916 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/scripts/
--rw-r--r--   0 vsts      (1001) docker     (122)     1771 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/scripts/flow-mem-limit
--rw-r--r--   0 vsts      (1001) docker     (122)      140 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/scripts/refresh-secrets
--rw-r--r--   0 vsts      (1001) docker     (122)     4465 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/secrets.py
--rw-r--r--   0 vsts      (1001) docker     (122)      506 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:50.231916 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)      286 2022-11-16 19:23:49.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     2190 2022-11-16 19:23:49.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2022-11-16 19:23:49.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       84 2022-11-16 19:23:49.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       27 2022-11-16 19:23:49.000000 maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2022-11-16 19:23:50.235916 maisaedu-utilities-prefect-1.0.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      724 2022-11-16 19:23:37.000000 maisaedu-utilities-prefect-1.0.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1081 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      286 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/
+-rw-r--r--   0 vsts      (1001) docker     (122)      551 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/constants/
+-rw-r--r--   0 vsts      (1001) docker     (122)       81 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/constants/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       41 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/constants/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       31 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/constants/notification.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/database/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/database/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2819 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/database/postgres.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11374 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/deploy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3955 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/dw.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      349 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/environment.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/googlesheet/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/googlesheet/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1044 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/googlesheet/gspread.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1406 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/associations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1748 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/company.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5247 2022-11-16 19:30:31.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/contacts.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1653 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/contacts_lists.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3970 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/deals.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2222 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/email_events.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1631 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/forms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2023 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/forms_submissions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3833 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/landing_pages.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1627 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/lineItems.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2060 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/marketing_emails.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2864 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/objects.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      693 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/owners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      916 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/pipelines.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7425 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/tickets.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2341 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/notification.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1955 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4921 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2778 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2605 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/client.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/scripts/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1771 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/scripts/flow-mem-limit
+-rw-r--r--   0 vsts      (1001) docker     (122)      140 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/scripts/refresh-secrets
+-rw-r--r--   0 vsts      (1001) docker     (122)     4465 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/secrets.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      506 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)      286 2022-11-16 19:30:50.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2190 2022-11-16 19:30:50.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2022-11-16 19:30:50.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       84 2022-11-16 19:30:50.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       27 2022-11-16 19:30:50.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      724 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/setup.py
```

### Comparing `maisaedu-utilities-prefect-1.0.8/LICENSE` & `maisaedu-utilities-prefect-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/__init__.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/__init__.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/database/postgres.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/database/postgres.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/deploy.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/deploy.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/dw.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/dw.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/googlesheet/gspread.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/googlesheet/gspread.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/associations.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/associations.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/company.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/company.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/contacts.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/contacts.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/contacts_lists.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/contacts_lists.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/deals.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/deals.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/email_events.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/email_events.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/forms.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/forms.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/forms_submissions.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/forms_submissions.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/landing_pages.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/landing_pages.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/lineItems.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/lineItems.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/marketing_emails.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/marketing_emails.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/objects.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/objects.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/owners.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/owners.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/pipelines.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/pipelines.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/hubspot/tickets.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/tickets.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/notification.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import requests
 
 try:
     from prefect.engine.state import Failed
 
     prefect_2 = False
 except Exception as e:
     prefect_2 = True
```

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/powerbi_api/services/client.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/client.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/scripts/flow-mem-limit` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/scripts/flow-mem-limit`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect/secrets.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/secrets.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/maisaedu_utilities_prefect.egg-info/SOURCES.txt` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.8/setup.py` & `maisaedu-utilities-prefect-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="maisaedu-utilities-prefect",
-    version="1.0.8",
+    version="1.0.9",
     description="Utilities for interaction with Prefect, for +A Education",
     license="MIT License",
     author="A+ Educação",
     author_email="dataeng@maisaedu.com.br",
     packages=find_packages(),
     scripts=[
         "maisaedu_utilities_prefect/scripts/refresh-secrets",
```

