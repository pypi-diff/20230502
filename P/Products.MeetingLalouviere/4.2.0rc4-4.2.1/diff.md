# Comparing `tmp/Products.MeetingLalouviere-4.2.0rc4.tar.gz` & `tmp/Products.MeetingLalouviere-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.MeetingLalouviere-4.2.0rc4.tar", last modified: Wed Apr 19 08:28:03 2023, max compression
+gzip compressed data, was "Products.MeetingLalouviere-4.2.1.tar", last modified: Tue May  2 09:23:30 2023, max compression
```

## Comparing `Products.MeetingLalouviere-4.2.0rc4.tar` & `Products.MeetingLalouviere-4.2.1.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.047814 Products.MeetingLalouviere-4.2.0rc4/
--rw-rw-r--   0 oli       (1000) oli       (1000)     4409 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/CHANGES.rst
--rw-rw-r--   0 oli       (1000) oli       (1000)      354 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/MANIFEST.in
--rw-rw-r--   0 oli       (1000) oli       (1000)     5086 2023-04-19 08:28:03.047814 Products.MeetingLalouviere-4.2.0rc4/PKG-INFO
--rw-rw-r--   0 oli       (1000) oli       (1000)       24 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/README.rst
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.031814 Products.MeetingLalouviere-4.2.0rc4/docs/
--rw-rw-r--   0 oli       (1000) oli       (1000)     2970 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/docs/HISTORY.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)    18092 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/docs/LICENSE.GPL
--rw-rw-r--   0 oli       (1000) oli       (1000)      736 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/docs/LICENSE.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)      534 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/docs/MIGRATION.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)       38 2023-04-19 08:28:03.047814 Products.MeetingLalouviere-4.2.0rc4/setup.cfg
--rw-rw-r--   0 oli       (1000) oli       (1000)     1237 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/setup.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.027814 Products.MeetingLalouviere-4.2.0rc4/src/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.031814 Products.MeetingLalouviere-4.2.0rc4/src/Products/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.031814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/
--rw-rw-r--   0 oli       (1000) oli       (1000)      973 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/README.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)     1803 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)    33265 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/adapters.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.031814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/browser/
--rw-rw-r--   0 oli       (1000) oli       (1000)       21 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/browser/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1229 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/browser/configure.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)     2220 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/browser/overrides.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.031814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/browser/template/
--rw-rw-r--   0 oli       (1000) oli       (1000)    15578 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/browser/template/meeting_before_faceted_infos.pt
--rw-rw-r--   0 oli       (1000) oli       (1000)     4513 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/browser/views.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     7744 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/config.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      782 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/configure.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)      590 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/events.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      482 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/events.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)      164 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/interfaces.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.031814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/
--rw-rw-r--   0 oli       (1000) oli       (1000)    14227 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/PloneMeeting.pot
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.027814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/en/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.031814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/en/LC_MESSAGES/
--rw-rw-r--   0 oli       (1000) oli       (1000)      750 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/en/LC_MESSAGES/plone.po
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.027814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/fr/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.035814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 oli       (1000) oli       (1000)    21979 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 oli       (1000) oli       (1000)     6551 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 oli       (1000) oli       (1000)     2397 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 oli       (1000) oli       (1000)    10461 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 oli       (1000) oli       (1000)     4344 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/imio.actionspanel.pot
--rw-rw-r--   0 oli       (1000) oli       (1000)     1721 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/imio.history.pot
--rw-rw-r--   0 oli       (1000) oli       (1000)     7995 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/plone.pot
--rwxrwxr-x   0 oli       (1000) oli       (1000)      295 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/sync_pos.sh
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.035814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/migrations/
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/migrations/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1208 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/migrations/add_searches.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     5433 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/migrations/migrate_to_4161.py
--rw-rw-r--   0 oli       (1000) oli       (1000)    55239 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/migrations/migrate_to_4200.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     4299 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/migrations/migrate_to_4_1.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.035814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/model/
--rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/model/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     4170 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/model/pm_updates.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1564 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/overrides.zcml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.035814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/
--rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.035814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/MeetingLalouviere_marker.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      208 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/browserlayer.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      743 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/cssregistry.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      807 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/import_steps.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      246 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/metadata.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      831 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/registry.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      950 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/skins.xml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.035814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/workflows/
--rw-rw-r--   0 oli       (1000) oli       (1000)    21914 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_college.odg
--rw-rw-r--   0 oli       (1000) oli       (1000)    21939 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_council.odg
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.035814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/MeetingLalouviere_testing_marker.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.039814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/attach.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/budget.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/budgetAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/cahier.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/decisionAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/financialAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/itemAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/legalAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     3555 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/logo.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)      411 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/negative.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      305 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/nil.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/overheadAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     1147 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/positive.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      355 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/remarks.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      730 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/secretary_remarks.png
--rwxrwxr-x   0 oli       (1000) oli       (1000)     4680 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/import_data.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)      349 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/import_steps.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      176 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/metadata.xml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.039814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/templates/
--rw-rw-r--   0 oli       (1000) oli       (1000)    33545 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/templates/council-oj.odt
--rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/toolset.xml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.039814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/MeetingLalouviere_lalouviere_marker.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      760 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/heldpositions.csv
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.039814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/attach.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/budget.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/budgetAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     1032 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/decisionAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/financialAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/itemAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      761 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/legalAdvice.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/legalAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      885 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/negative.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      305 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/nil.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/overheadAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      583 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/positive.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      705 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/remarks.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      730 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/secretary_remarks.png
--rw-rw-r--   0 oli       (1000) oli       (1000)    11505 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/import_data.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)      632 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/import_steps.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      266 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/organizations.csv
--rw-rw-r--   0 oli       (1000) oli       (1000)      726 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/persons.csv
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.043814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/
--rw-rw-r--   0 oli       (1000) oli       (1000)     9511 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)     9909 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib_recto_verso.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)     9605 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_pv.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12386 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendance-stats.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    17906 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendees.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    18854 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/avis-df.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    22380 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-oj.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    22958 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-pv.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12890 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-rapport.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    13154 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/dashboard.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    32698 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    32449 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation_recto_verso.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)     9652 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/history.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12705 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/meeting_assemblies.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    24785 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-annexes.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    24316 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-table-des-matieres.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    24585 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12170 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/organizations-export.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    16342 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/publications.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    23881 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/pv.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12630 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    11565 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    13706 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/report.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    10369 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles1.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12815 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles2.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    18137 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-avis-df.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    14290 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-df-tb.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    13865 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/users-groups-export.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    14862 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/votes.odt
--rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/toolset.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)     1110 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/refresh.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)     4705 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/setuphandlers.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.027814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.043814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/
--rw-rw-r--   0 oli       (1000) oli       (1000)      636 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToAlderman.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      595 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDg.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      646 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDirector.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      662 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDivisionHead.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      583 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToOfficeManager.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToServiceHead.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     6337 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      699 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_no.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      722 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_provided.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      737 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_yes.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     1082 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/not_printed_in_dashboard.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)     1035 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/printed_in_dashboard.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)      651 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToAlderman.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      737 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToBudgetImpactReviewer.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      575 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDg.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      613 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDirector.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      626 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDivisionHead.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      608 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToOfficeManager.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      638 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToServiceHead.png
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.043814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_styles/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3521 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_styles/meetinglalouviere.css.dtml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.043814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/
--rw-rw-r--   0 oli       (1000) oli       (1000)     8155 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_edit.pt
--rw-rw-r--   0 oli       (1000) oli       (1000)    42603 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_view.pt
--rw-rw-r--   0 oli       (1000) oli       (1000)     1023 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/testing.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      593 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/testing.zcml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.047814 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/
--rwxrwxr-x   0 oli       (1000) oli       (1000)     2161 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/MeetingLalouviereTestCase.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1049 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     6699 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/helpers.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1243 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testAdvices.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1380 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testAnnexes.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1362 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testChangeItemOrderView.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1244 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testColumns.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     3920 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testContacts.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)      551 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1373 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomMeetingConfig.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     7858 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomMeetingItem.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      349 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomSearches.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1360 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomToolPloneMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     3100 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomUtils.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1510 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomViews.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      481 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomWFAdaptations.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1396 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomWorkflows.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1369 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testFaceted.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1300 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1339 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testMeetingCategory.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     6630 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testMeetingConfig.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)     8876 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testMeetingItem.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1290 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testPortlets.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     9778 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testSearches.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1281 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testSetup.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     2279 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testToolPloneMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     2958 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testUtils.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1293 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testValidators.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     2071 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testViews.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1239 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testVotes.py
--rw-rw-r--   0 oli       (1000) oli       (1000)    17680 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testWFAdaptations.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)    20361 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testWorkflows.py
--rw-rw-r--   0 oli       (1000) oli       (1000)        7 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/version.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)     1585 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/vocabularies.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      445 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/vocabularies.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)       56 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-19 08:28:03.031814 Products.MeetingLalouviere-4.2.0rc4/src/Products.MeetingLalouviere.egg-info/
--rw-rw-r--   0 oli       (1000) oli       (1000)     5086 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products.MeetingLalouviere.egg-info/PKG-INFO
--rw-rw-r--   0 oli       (1000) oli       (1000)    12596 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products.MeetingLalouviere.egg-info/SOURCES.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products.MeetingLalouviere.egg-info/dependency_links.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products.MeetingLalouviere.egg-info/namespace_packages.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products.MeetingLalouviere.egg-info/not-zip-safe
--rw-rw-r--   0 oli       (1000) oli       (1000)      139 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products.MeetingLalouviere.egg-info/requires.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-04-19 08:28:02.000000 Products.MeetingLalouviere-4.2.0rc4/src/Products.MeetingLalouviere.egg-info/top_level.txt
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.401727 Products.MeetingLalouviere-4.2.1/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4841 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/CHANGES.rst
+-rw-rw-r--   0 oli       (1000) oli       (1000)      354 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/MANIFEST.in
+-rw-rw-r--   0 oli       (1000) oli       (1000)     5515 2023-05-02 09:23:30.401727 Products.MeetingLalouviere-4.2.1/PKG-INFO
+-rw-rw-r--   0 oli       (1000) oli       (1000)       24 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/README.rst
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.389726 Products.MeetingLalouviere-4.2.1/docs/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2970 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/docs/HISTORY.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    18092 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/docs/LICENSE.GPL
+-rw-rw-r--   0 oli       (1000) oli       (1000)      736 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/docs/LICENSE.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)      534 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/docs/MIGRATION.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)       38 2023-05-02 09:23:30.401727 Products.MeetingLalouviere-4.2.1/setup.cfg
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1234 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/setup.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.389726 Products.MeetingLalouviere-4.2.1/src/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.389726 Products.MeetingLalouviere-4.2.1/src/Products/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.389726 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      973 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/README.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1803 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)    33265 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/adapters.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.389726 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/browser/
+-rw-rw-r--   0 oli       (1000) oli       (1000)       21 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/browser/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1229 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/browser/configure.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2220 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/browser/overrides.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.393727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/browser/template/
+-rw-rw-r--   0 oli       (1000) oli       (1000)    15578 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/browser/template/meeting_before_faceted_infos.pt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4513 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/browser/views.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     7802 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/config.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      782 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/configure.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      590 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/events.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      482 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/events.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      164 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/interfaces.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.393727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/
+-rw-rw-r--   0 oli       (1000) oli       (1000)    14227 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/PloneMeeting.pot
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.389726 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/en/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.393727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      750 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/en/LC_MESSAGES/plone.po
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.389726 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/fr/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.393727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 oli       (1000) oli       (1000)    21979 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 oli       (1000) oli       (1000)     6551 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2397 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 oli       (1000) oli       (1000)    10461 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4344 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/imio.actionspanel.pot
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1721 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/imio.history.pot
+-rw-rw-r--   0 oli       (1000) oli       (1000)     7995 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/plone.pot
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      295 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/sync_pos.sh
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.393727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/migrations/
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/migrations/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1208 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/migrations/add_searches.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     5433 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/migrations/migrate_to_4161.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)    55322 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/migrations/migrate_to_4200.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4299 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/migrations/migrate_to_4_1.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.393727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/model/
+-rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/model/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4099 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/model/pm_updates.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1564 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/overrides.zcml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.393727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/
+-rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/__init__.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.393727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/MeetingLalouviere_marker.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      208 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/browserlayer.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      743 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/cssregistry.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      807 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/import_steps.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      246 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/metadata.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      831 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/registry.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      950 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/skins.xml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.393727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/workflows/
+-rw-rw-r--   0 oli       (1000) oli       (1000)    21914 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_college.odg
+-rw-rw-r--   0 oli       (1000) oli       (1000)    21939 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_council.odg
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.393727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/MeetingLalouviere_testing_marker.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/__init__.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.393727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/attach.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/budget.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/budgetAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/cahier.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/decisionAnnex.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/financialAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/itemAnnex.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/legalAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3555 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/logo.gif
+-rw-rw-r--   0 oli       (1000) oli       (1000)      411 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/negative.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      305 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/nil.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/overheadAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1147 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/positive.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      355 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/remarks.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      730 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/secretary_remarks.png
+-rwxrwxr-x   0 oli       (1000) oli       (1000)     4680 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/import_data.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      349 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/import_steps.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      176 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/metadata.xml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.393727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/templates/
+-rw-rw-r--   0 oli       (1000) oli       (1000)    33545 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/templates/council-oj.odt
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/toolset.xml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.397727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/MeetingLalouviere_lalouviere_marker.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      760 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/heldpositions.csv
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.397727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/attach.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/budget.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/budgetAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1032 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.gif
+-rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/decisionAnnex.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/financialAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/itemAnnex.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      761 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/legalAdvice.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/legalAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      885 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/negative.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      305 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/nil.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/overheadAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      583 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/positive.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      705 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/remarks.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      730 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/secretary_remarks.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)    11505 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/import_data.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      632 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/import_steps.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      266 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/organizations.csv
+-rw-rw-r--   0 oli       (1000) oli       (1000)      726 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/persons.csv
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.397727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9511 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9909 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib_recto_verso.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9605 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_pv.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12386 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendance-stats.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    17906 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendees.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    18854 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/avis-df.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    22380 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-oj.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    22958 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-pv.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12890 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-rapport.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    13154 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/dashboard.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    32698 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    32449 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation_recto_verso.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9652 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/history.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12705 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/meeting_assemblies.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    24785 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-annexes.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    24316 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-table-des-matieres.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    24585 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12170 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/organizations-export.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    16342 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/publications.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    23881 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/pv.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12630 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    11565 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    13706 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/report.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    10369 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles1.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12815 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles2.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    18137 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-avis-df.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    14290 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-df-tb.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    13865 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/users-groups-export.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    14862 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/votes.odt
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/toolset.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1110 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/refresh.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4705 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/setuphandlers.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.389726 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.401727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      636 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToAlderman.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      595 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDg.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      646 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDirector.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      662 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDivisionHead.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      583 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToOfficeManager.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToServiceHead.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     6337 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      699 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_no.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      722 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_provided.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      737 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_yes.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1082 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/not_printed_in_dashboard.gif
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1035 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/printed_in_dashboard.gif
+-rw-rw-r--   0 oli       (1000) oli       (1000)      651 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToAlderman.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      737 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToBudgetImpactReviewer.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      575 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDg.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      613 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDirector.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      626 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDivisionHead.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      608 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToOfficeManager.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      638 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToServiceHead.png
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.401727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_styles/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3521 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_styles/meetinglalouviere.css.dtml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.401727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     8155 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_edit.pt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    42763 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_view.pt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1023 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/testing.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      593 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/testing.zcml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.401727 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/
+-rwxrwxr-x   0 oli       (1000) oli       (1000)     2161 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/MeetingLalouviereTestCase.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1049 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     6699 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/helpers.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1243 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testAdvices.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1380 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testAnnexes.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1362 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testChangeItemOrderView.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1244 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testColumns.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3920 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testContacts.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      551 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomMeeting.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1373 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomMeetingConfig.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     7858 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomMeetingItem.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      349 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomSearches.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1360 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomToolPloneMeeting.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3100 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomUtils.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1510 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomViews.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      481 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomWFAdaptations.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1396 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomWorkflows.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1369 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testFaceted.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1300 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testMeeting.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1339 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testMeetingCategory.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     6630 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testMeetingConfig.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)     8876 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testMeetingItem.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1290 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testPortlets.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9778 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testSearches.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1281 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testSetup.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2279 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testToolPloneMeeting.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2958 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testUtils.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1293 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testValidators.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2071 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testViews.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1239 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testVotes.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)    17680 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testWFAdaptations.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)    20438 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testWorkflows.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)        7 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/version.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1585 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/vocabularies.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      445 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/vocabularies.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)       56 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products/__init__.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-05-02 09:23:30.389726 Products.MeetingLalouviere-4.2.1/src/Products.MeetingLalouviere.egg-info/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     5515 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products.MeetingLalouviere.egg-info/PKG-INFO
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12596 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products.MeetingLalouviere.egg-info/SOURCES.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products.MeetingLalouviere.egg-info/dependency_links.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products.MeetingLalouviere.egg-info/namespace_packages.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products.MeetingLalouviere.egg-info/not-zip-safe
+-rw-rw-r--   0 oli       (1000) oli       (1000)      139 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products.MeetingLalouviere.egg-info/requires.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-05-02 09:23:30.000000 Products.MeetingLalouviere-4.2.1/src/Products.MeetingLalouviere.egg-info/top_level.txt
```

### Comparing `Products.MeetingLalouviere-4.2.0rc4/CHANGES.rst` & `Products.MeetingLalouviere-4.2.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 Products.MeetingLalouviere Changelog
 ====================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
+4.2.1 (2023-05-02)
+------------------
+
+- Revert `set correct migration profile_name`.
+  [odelaere]
+
+
+4.2.0 (2023-05-02)
+------------------
+
+- Revert access rights of field "observations" to default from MeetingCommunes.
+  [odelaere]
+- set correct migration profile_name.
+  [odelaere]
+- adapt vote config in migration.
+  [odelaere]
+- Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
+  [gbastien]
+
+
 4.2.0rc4 (2023-04-19)
 ---------------------
 
 - Apply todos after migration.
   [odelaere]
```

### Comparing `Products.MeetingLalouviere-4.2.0rc4/PKG-INFO` & `Products.MeetingLalouviere-4.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingLalouviere
-Version: 4.2.0rc4
+Version: 4.2.1
 Summary: Official meetings management for college and council custom profile for La Louvière
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Olivier Delaere
 Author-email: olivier.delaere@imio.be
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -19,14 +19,34 @@
 Check 'docs/README.txt'
 
 Products.MeetingLalouviere Changelog
 ====================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
+4.2.1 (2023-05-02)
+------------------
+
+- Revert `set correct migration profile_name`.
+  [odelaere]
+
+
+4.2.0 (2023-05-02)
+------------------
+
+- Revert access rights of field "observations" to default from MeetingCommunes.
+  [odelaere]
+- set correct migration profile_name.
+  [odelaere]
+- adapt vote config in migration.
+  [odelaere]
+- Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
+  [gbastien]
+
+
 4.2.0rc4 (2023-04-19)
 ---------------------
 
 - Apply todos after migration.
   [odelaere]
```

### Comparing `Products.MeetingLalouviere-4.2.0rc4/docs/HISTORY.txt` & `Products.MeetingLalouviere-4.2.1/docs/HISTORY.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/docs/LICENSE.GPL` & `Products.MeetingLalouviere-4.2.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/docs/LICENSE.txt` & `Products.MeetingLalouviere-4.2.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/docs/MIGRATION.txt` & `Products.MeetingLalouviere-4.2.1/docs/MIGRATION.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/setup.py` & `Products.MeetingLalouviere-4.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding=utf-8
 from setuptools import setup, find_packages
 
-version = "4.2.0rc4"
+version = "4.2.1"
 
 setup(
     name="Products.MeetingLalouviere",
     version=version,
     description="Official meetings management for college and council custom profile for La Louvière",
     long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
     classifiers=[
```

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/README.txt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/README.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/__init__.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/adapters.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/adapters.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/browser/configure.zcml` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/browser/overrides.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/browser/overrides.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/browser/template/meeting_before_faceted_infos.pt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/browser/template/meeting_before_faceted_infos.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/browser/views.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/browser/views.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/config.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,22 +226,24 @@
     "removed",
     "return_to_proposing_group",
     "no_publication",
     'propose_to_budget_reviewer',
     'waiting_advices',
     'waiting_advices_proposing_group_send_back',
     'item_validation_shortcuts',
+    'postpone_next_meeting',
 )
 
 LLO_APPLYED_COUNCIL_WFA = (
     "accepted_but_modified",
     "pre_accepted",
     "refused",
     "delayed",
     "removed",
     "return_to_proposing_group",
     'apply_council_state_label',
     'propose_to_budget_reviewer',
     'waiting_advices',
     'waiting_advices_proposing_group_send_back',
     'item_validation_shortcuts',
+    'postpone_next_meeting',
 )
```

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/configure.zcml` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/events.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/events.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/PloneMeeting.pot` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/PloneMeeting.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/en/LC_MESSAGES/plone.po` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.history.po` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/plone.po` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/imio.actionspanel.pot` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/imio.actionspanel.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/imio.history.pot` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/locales/plone.pot` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/migrations/add_searches.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/migrations/add_searches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/migrations/migrate_to_4161.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/migrations/migrate_to_4161.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/migrations/migrate_to_4200.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/migrations/migrate_to_4200.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,15 +426,14 @@
                     self.replace_in_list("c24", "c31", cfg.getDashboardItemsListingsFilters()))
                 cfg.setDashboardMeetingAvailableItemsFilters(
                     self.replace_in_list("c24", "c31", cfg.getDashboardMeetingAvailableItemsFilters()))
                 cfg.setDashboardMeetingLinkedItemsFilters(
                     self.replace_in_list("c24", "c31", cfg.getDashboardMeetingLinkedItemsFilters()))
             else:
                 cfg.setWorkflowAdaptations(LLO_APPLYED_COLLEGE_WFA)
-                cfg.setMeetingColumns(cfg.getMeetingColumns() + ('static_meeting_number',))
             # replace action and review_state column by async actions
             self.updateColumns(to_replace={'actions': 'async_actions',
                                            'review_state': 'review_state_title',
                                            'getRawClassifier': 'committees_index'})
             # remove old attrs
             old_attrs = ('preMeetingAssembly_default', 'preMeetingAssembly_2_default', 'preMeetingAssembly_3_default',
                          'preMeetingAssembly_4_default', 'preMeetingAssembly_5_default', 'preMeetingAssembly_6_default',
@@ -455,16 +454,18 @@
                                                              u'proposed_to_budget_reviewer',
                                                              cfg.getItemAdviceViewStates())
                                         )
             cfg.setItemAdviceEditStates(self.replace_in_list(u'proposed_to_budgetimpact_reviewer',
                                                              u'proposed_to_budget_reviewer',
                                                              cfg.getItemAdviceEditStates())
                                         )
-            cfg.setUseVotes(True)
-            cfg.setVotesResultTALExpr("python: pm_utils.print_votes(item)")
+            cfg.setUseVotes('council' in cfg.getId())
+            cfg.setVotesResultTALExpr(
+                "python: item.getPollType() == 'no_vote' and '' or '<p>&nbsp;</p>' + pm_utils.print_votes(item)")
+            cfg.setEnabledAnnexesBatchActions(('delete', 'download-annexes'))
 
     def replace_in_list(self, to_replace, new_value, list):
         result = set()
         for value in list:
             if value == to_replace:
                 result.add(new_value)
             else:
```

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/migrations/migrate_to_4_1.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/migrations/migrate_to_4_1.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/model/pm_updates.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/model/pm_updates.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,16 +78,14 @@
     ),)
 
     # Don't forget the label override in skins/meetinglalouviere_templates/meetingitem_view.pt
     baseSchema['description'].widget.label_method = "getLabelDescription"
 
     baseSchema['privacy'].widget.condition = "python: here.showMeetingManagerReservedField('privacy')"
 
-    baseSchema['observations'].write_permission = ModifyPortalContent
-
     completeItemSchema = baseSchema + specificSchema.copy()
     return completeItemSchema
 
 
 MeetingItem.schema = update_item_schema(MeetingItem.schema)
```

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/overrides.zcml` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/overrides.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/cssregistry.xml` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/import_steps.xml` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/registry.xml` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/skins.xml` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_college.odg` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_college.odg`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_council.odg` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_council.odg`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/attach.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/budget.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/cahier.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/financialAnalysis.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/logo.gif` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/logo.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/overheadAnalysis.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/positive.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/images/secretary_remarks.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/images/secretary_remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/import_data.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/testing/templates/council-oj.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/testing/templates/council-oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/heldpositions.csv` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/heldpositions.csv`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/attach.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/budget.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.gif` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/financialAnalysis.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/legalAdvice.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/negative.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/overheadAnalysis.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/positive.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/remarks.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/images/secretary_remarks.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/secretary_remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/import_data.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/import_steps.xml` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/persons.csv` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/persons.csv`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib_recto_verso.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib_recto_verso.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_pv.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendance-stats.ods` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendance-stats.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendees.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendees.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/avis-df.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/avis-df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-oj.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-pv.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-rapport.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-rapport.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/dashboard.ods` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/dashboard.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation_recto_verso.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation_recto_verso.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/history.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/history.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/meeting_assemblies.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/meeting_assemblies.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-annexes.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-annexes.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-table-des-matieres.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-table-des-matieres.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/organizations-export.ods` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/organizations-export.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/publications.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/publications.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/pv.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.ods` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/report.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/report.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles1.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles1.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles2.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles2.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-avis-df.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-avis-df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-df-tb.ods` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-df-tb.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/users-groups-export.ods` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/users-groups-export.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/votes.odt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/votes.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/profiles.zcml` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/setuphandlers.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToAlderman.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToAlderman.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDg.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDg.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDirector.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDirector.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDivisionHead.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDivisionHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToOfficeManager.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToOfficeManager.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToServiceHead.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToServiceHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_no.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_no.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_provided.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_provided.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_yes.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_yes.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/not_printed_in_dashboard.gif` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/not_printed_in_dashboard.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/printed_in_dashboard.gif` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/printed_in_dashboard.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToAlderman.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToAlderman.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToBudgetImpactReviewer.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToBudgetImpactReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDg.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDg.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDirector.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDirector.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDivisionHead.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDivisionHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToOfficeManager.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToOfficeManager.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToServiceHead.png` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToServiceHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_styles/meetinglalouviere.css.dtml` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_styles/meetinglalouviere.css.dtml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_edit.pt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_view.pt` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_view.pt`

 * *Files 0% similar despite different names*

```diff
@@ -523,15 +523,18 @@
       <div id="clonable_to_other_mcs_content">
         <tal:displayOtherMeetingConfigsClonableTo tal:condition="otherMCs">
             <span tal:replace="structure python: context.displayOtherMeetingConfigsClonableTo()">Other mc clonable to (Emergency, privacy)</span>
         </tal:displayOtherMeetingConfigsClonableTo>
         <span tal:condition="not: otherMCs">-</span>
         <div tal:condition="otherMCs">
           <fieldset>
-            <legend i18n:translate="">Data that will be used on new item</legend>
+            <legend i18n:translate="">
+              Data that will be used on new item to
+              <span i18n:name="cfg_titles" tal:content="python: context.displayOtherMeetingConfigsClonableToPossibleValues()" />
+            </legend>
             <tal:otherMeetingConfigsClonableToFieldTitle condition="python: 'otherMeetingConfigsClonableToFieldTitle' in usedAttrs">
               <span class="item_attribute_label"
                     i18n:translate="PloneMeeting_label_itemTitle"></span>:&nbsp;&nbsp;
               <span metal:use-macro="python: here.widget('otherMeetingConfigsClonableToFieldTitle', mode='view')" />
             </tal:otherMeetingConfigsClonableToFieldTitle>
             <tal:loop tal:repeat="other_mc_field_name python: context.get_enable_clone_to_other_mc_fields(cfg, ignored_field_names=['otherMeetingConfigsClonableToFieldTitle'])">
                 <tal:field define="fieldName python: other_mc_field_name; ajaxEdit python:True">
```

#### html2text {}

```diff
@@ -44,15 +44,15 @@
 budgetRelated and budgetInfos
 Budget
 
   Motivation
  Decision    DecisionSuite    DecisionEnd
  Other meetingConfigs clonable to
  Other mc clonable to (Emergency, privacy)  -
- Data that will be used on new item  :  
+  Data that will be used on new item to    :  
   Annexes and advices
    Advices
  Text check list
 Text check list Nothing to display.
  In and out moves    Notes    Committee observations    Committee transcript
 Votes observations    Meeting managers notes    Meeting managers notes suite
 Meeting managers notes end    Poll type observations    Observations
```

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/testing.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/testing.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/testing.zcml` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/MeetingLalouviereTestCase.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/MeetingLalouviereTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/__init__.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/helpers.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testAdvices.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testAnnexes.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testChangeItemOrderView.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testColumns.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testContacts.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testContacts.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomMeeting.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomMeetingConfig.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomMeetingItem.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomToolPloneMeeting.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomUtils.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomViews.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testCustomWorkflows.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testCustomWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testFaceted.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testMeeting.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testMeetingCategory.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testMeetingConfig.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testMeetingItem.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testPortlets.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testSearches.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testSetup.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testToolPloneMeeting.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testUtils.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testValidators.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testViews.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testVotes.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testVotes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testWFAdaptations.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testWFAdaptations.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/tests/testWorkflows.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/tests/testWorkflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,46 +19,50 @@
        account the write_permission and read_permission tags that are defined
        on some attributes of the Archetypes model. So when we need to check
        that a user is not authorized to set the value of a field protected
        in this way, we do not try to use the accessor to trigger an exception
        (self.assertRaise). Instead, we check that the user has the permission
        to do so (getSecurityManager().checkPermission)."""
 
-    def _check_users_can_modify(self, item, users, annex):
+    def _check_users_can_modify(self, item, users=None, annex=None):
+        if users is None:
+            users = [self.member.id]
         for user_id in users:
             self.changeUser(user_id)
-            self.assertTrue(item.mayQuickEdit("observations"))
-            self.failUnless(self.hasPermission(ModifyPortalContent, (item, annex)))
+            if annex is None:
+                self.failUnless(self.hasPermission(ModifyPortalContent, item))
+            else:
+                self.failUnless(self.hasPermission(ModifyPortalContent, (item, annex)))
 
     def _testWholeDecisionProcessCollege(self):
         """This test covers the whole decision workflow. It begins with the
            creation of some items, and ends by closing a meeting."""
         # pmCreator1 creates an item with 1 annex and proposes it
         self._enableField("observations")
         self._activate_wfas(('waiting_advices',
                              # 'waiting_advices_adviser_send_back',
                              'waiting_advices_proposing_group_send_back',
                              'propose_to_budget_reviewer'),
                             keep_existing=True)
         self.meetingConfig.setItemAdviceStates(("itemcreated_waiting_advices", ))
         self.changeUser("pmCreator1")
         item1 = self.create("MeetingItem", title="The first item", optionalAdvisers=(self.vendors_uid, ))
-        self.assertTrue(item1.mayQuickEdit("observations"))
+        self._check_users_can_modify(item1)
         annex1 = self.addAnnex(item1)
         self.addAnnex(item1, relatedTo="item_decision")
         item1.setOptionalAdvisers((self.vendors_uid, ))
         self.do(item1, "wait_advices_from_itemcreated")
         self.assertEqual("itemcreated_waiting_advices", item1.query_state())
         self.do(item1, "backTo_itemcreated_from_waiting_advices")
         self.do(item1, "proposeToBudgetImpactReviewer")
         self.assertEqual("proposed_to_budget_reviewer", item1.query_state())
         self.failIf(self.transitions(item1))  # He may trigger no more action
         self.failIf(self.hasPermission("PloneMeeting: Add annex", item1))
         self.changeUser("pmBudgetReviewer1")
-        self.assertTrue(item1.mayQuickEdit("observations"))
+        self._check_users_can_modify(item1)
         self.do(item1, "backTo_itemcreated_from_proposed_to_budget_reviewer")
         self.assertEqual("itemcreated", item1.query_state())
         self.changeUser("pmCreator1")
         self.do(item1, "proposeToServiceHead")
         self.assertRaises(Unauthorized, self.addAnnex, item1)
         self.failIf(self.transitions(item1))  # He may trigger no more action
         self.failIf(self.hasPermission(AddAnnex, item1))
@@ -120,15 +124,15 @@
                                      annex1)
         self.do(item1, "validate")
         self.assertRaises(Unauthorized, self.addAnnex, item1, relatedTo="item_decision")
         self.failIf(self.transitions(item1))  # He may trigger no more action
         self.failIf(self.hasPermission("PloneMeeting: Add annex", item1))
         # pmManager creates a meeting
         self.changeUser("pmManager")
-        self.assertTrue(item1.mayQuickEdit("observations"))
+        self._check_users_can_modify(item1)
         meeting = self.create("Meeting", date=datetime(2007, 12, 11, 9))
         self.addAnnex(item1, relatedTo="item_decision")
         # pmCreator2 creates and proposes an item
         self.changeUser("pmCreator2")
         item2 = self.create(
             "MeetingItem", title="The second item", preferredMeeting=meeting.UID()
         )
@@ -249,15 +253,15 @@
         self.addAnnex(item1, relatedTo="item_decision")
         self.do(item1, "validate")
         self.failIf(self.hasPermission(ModifyPortalContent, item1))
         # The reviewer cannot add a decision annex on validated item
         self.assertRaises(Unauthorized, self.addAnnex, item1, relatedTo="item_decision")
         # pmManager creates a meeting
         self.changeUser("pmManager")
-        self.assertTrue(item1.mayQuickEdit("observations"))
+        self._check_users_can_modify(item1)
         meeting = self.create("Meeting", date=datetime(2007, 12, 11, 9, 0, 0))
         # The meetingManager can add a decision annex
         self.addAnnex(item1, relatedTo="item_decision")
         # pmCreator2 creates and proposes an item
         self.changeUser("pmCreator2")
         item2 = self.create(
             "MeetingItem",
```

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products/MeetingLalouviere/vocabularies.py` & `Products.MeetingLalouviere-4.2.1/src/Products/MeetingLalouviere/vocabularies.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products.MeetingLalouviere.egg-info/PKG-INFO` & `Products.MeetingLalouviere-4.2.1/src/Products.MeetingLalouviere.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingLalouviere
-Version: 4.2.0rc4
+Version: 4.2.1
 Summary: Official meetings management for college and council custom profile for La Louvière
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Olivier Delaere
 Author-email: olivier.delaere@imio.be
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -19,14 +19,34 @@
 Check 'docs/README.txt'
 
 Products.MeetingLalouviere Changelog
 ====================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
+4.2.1 (2023-05-02)
+------------------
+
+- Revert `set correct migration profile_name`.
+  [odelaere]
+
+
+4.2.0 (2023-05-02)
+------------------
+
+- Revert access rights of field "observations" to default from MeetingCommunes.
+  [odelaere]
+- set correct migration profile_name.
+  [odelaere]
+- adapt vote config in migration.
+  [odelaere]
+- Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
+  [gbastien]
+
+
 4.2.0rc4 (2023-04-19)
 ---------------------
 
 - Apply todos after migration.
   [odelaere]
```

### Comparing `Products.MeetingLalouviere-4.2.0rc4/src/Products.MeetingLalouviere.egg-info/SOURCES.txt` & `Products.MeetingLalouviere-4.2.1/src/Products.MeetingLalouviere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

