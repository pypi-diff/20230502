# Comparing `tmp/drafthorse-2.2.1.tar.gz` & `tmp/drafthorse-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drafthorse-2.2.1.tar", last modified: Wed Feb  1 15:38:40 2023, max compression
+gzip compressed data, was "drafthorse-2.3.0.tar", last modified: Tue May  2 08:09:03 2023, max compression
```

## Comparing `drafthorse-2.2.1.tar` & `drafthorse-2.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-02-01 15:38:40.830325 drafthorse-2.2.1/
--rw-r--r--   0 raphael   (1000) raphael   (1000)    11358 2022-02-19 19:40:43.000000 drafthorse-2.2.1/LICENSE
--rw-r--r--   0 raphael   (1000) raphael   (1000)       73 2022-02-19 19:40:43.000000 drafthorse-2.2.1/MANIFEST.in
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6156 2023-02-01 15:38:40.830325 drafthorse-2.2.1/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5502 2022-08-05 08:44:32.000000 drafthorse-2.2.1/README.rst
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-02-01 15:38:40.826991 drafthorse-2.2.1/drafthorse/
--rw-r--r--   0 raphael   (1000) raphael   (1000)       18 2023-02-01 15:38:05.000000 drafthorse-2.2.1/drafthorse/__init__.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-02-01 15:38:40.830325 drafthorse-2.2.1/drafthorse/models/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      438 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7885 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/accounting.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2584 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/container.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1903 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/delivery.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3108 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/document.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    12927 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/elements.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    10420 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/fields.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      487 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/note.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     4534 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/party.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5363 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/payment.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2973 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/product.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     4690 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/references.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6764 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/trade.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5755 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/models/tradelines.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    12570 2023-02-01 15:37:23.000000 drafthorse-2.2.1/drafthorse/pdf.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-02-01 15:38:40.830325 drafthorse-2.2.1/drafthorse/schema/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1628 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC-WL.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)    29033 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC-WL_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)    10995 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC-WL_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1831 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC-WL_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1619 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)    29030 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)    13692 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2076 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1625 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EN16931.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)    64030 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EN16931_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)    18030 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EN16931_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2988 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EN16931_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1628 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EXTENDED.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)    94568 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EXTENDED_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)    28365 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EXTENDED_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3529 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EXTENDED_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1625 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_MINIMUM.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)    18809 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_MINIMUM_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)     4434 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_MINIMUM_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1383 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/FACTUR-X_MINIMUM_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2995 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/schema/ZUGFeRD2p2_extension_schema.xmp
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1364 2022-08-05 08:44:32.000000 drafthorse-2.2.1/drafthorse/utils.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-02-01 15:38:40.826991 drafthorse-2.2.1/drafthorse.egg-info/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6156 2023-02-01 15:38:40.000000 drafthorse-2.2.1/drafthorse.egg-info/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2527 2023-02-01 15:38:40.000000 drafthorse-2.2.1/drafthorse.egg-info/SOURCES.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2023-02-01 15:38:40.000000 drafthorse-2.2.1/drafthorse.egg-info/dependency_links.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       12 2023-02-01 15:38:40.000000 drafthorse-2.2.1/drafthorse.egg-info/requires.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       11 2023-02-01 15:38:40.000000 drafthorse-2.2.1/drafthorse.egg-info/top_level.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)      287 2023-02-01 15:38:40.830325 drafthorse-2.2.1/setup.cfg
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1225 2022-08-05 08:44:32.000000 drafthorse-2.2.1/setup.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-05-02 08:09:03.233327 drafthorse-2.3.0/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    11358 2022-02-19 19:40:43.000000 drafthorse-2.3.0/LICENSE
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       73 2022-02-19 19:40:43.000000 drafthorse-2.3.0/MANIFEST.in
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     6156 2023-05-02 08:09:03.233327 drafthorse-2.3.0/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5502 2022-08-05 08:44:32.000000 drafthorse-2.3.0/README.rst
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-05-02 08:09:03.233327 drafthorse-2.3.0/drafthorse/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       18 2023-05-02 08:08:40.000000 drafthorse-2.3.0/drafthorse/__init__.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-05-02 08:09:03.233327 drafthorse-2.3.0/drafthorse/models/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      438 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7885 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/accounting.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2584 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/container.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1903 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/delivery.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3108 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/document.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    12927 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/elements.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    10420 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/fields.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      487 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/note.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     4534 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/party.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5363 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/payment.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2973 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/product.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     4690 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/references.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     6764 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/trade.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5755 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/models/tradelines.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    12666 2023-05-02 08:08:23.000000 drafthorse-2.3.0/drafthorse/pdf.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-05-02 08:09:03.233327 drafthorse-2.3.0/drafthorse/schema/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1628 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC-WL.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    29033 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC-WL_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    10995 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC-WL_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1831 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC-WL_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1619 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    29030 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    13692 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2076 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1625 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EN16931.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    64030 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EN16931_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    18030 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EN16931_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2988 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EN16931_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1628 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EXTENDED.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    94568 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EXTENDED_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    28365 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EXTENDED_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3529 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EXTENDED_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1625 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_MINIMUM.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    18809 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_MINIMUM_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     4434 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_MINIMUM_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1383 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/FACTUR-X_MINIMUM_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2995 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/schema/ZUGFeRD2p2_extension_schema.xmp
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1364 2022-08-05 08:44:32.000000 drafthorse-2.3.0/drafthorse/utils.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-05-02 08:09:03.233327 drafthorse-2.3.0/drafthorse.egg-info/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     6156 2023-05-02 08:09:03.000000 drafthorse-2.3.0/drafthorse.egg-info/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2527 2023-05-02 08:09:03.000000 drafthorse-2.3.0/drafthorse.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2023-05-02 08:09:03.000000 drafthorse-2.3.0/drafthorse.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       11 2023-05-02 08:09:03.000000 drafthorse-2.3.0/drafthorse.egg-info/requires.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       11 2023-05-02 08:09:03.000000 drafthorse-2.3.0/drafthorse.egg-info/top_level.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      287 2023-05-02 08:09:03.233327 drafthorse-2.3.0/setup.cfg
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1224 2023-05-02 08:08:23.000000 drafthorse-2.3.0/setup.py
```

### Comparing `drafthorse-2.2.1/LICENSE` & `drafthorse-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/PKG-INFO` & `drafthorse-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drafthorse
-Version: 2.2.1
+Version: 2.3.0
 Summary: Python ZUGFeRD XML implementation
 Home-page: https://github.com/pretix/python-drafthorse
 Author: Raphael Michel
 Author-email: michel@rami.io
 License: Apache License
 Keywords: xml banking sepa
 Platform: UNKNOWN
```

### Comparing `drafthorse-2.2.1/README.rst` & `drafthorse-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/models/accounting.py` & `drafthorse-2.3.0/drafthorse/models/accounting.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/models/container.py` & `drafthorse-2.3.0/drafthorse/models/container.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/models/delivery.py` & `drafthorse-2.3.0/drafthorse/models/delivery.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/models/document.py` & `drafthorse-2.3.0/drafthorse/models/document.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/models/elements.py` & `drafthorse-2.3.0/drafthorse/models/elements.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/models/fields.py` & `drafthorse-2.3.0/drafthorse/models/fields.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/models/party.py` & `drafthorse-2.3.0/drafthorse/models/party.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/models/payment.py` & `drafthorse-2.3.0/drafthorse/models/payment.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/models/product.py` & `drafthorse-2.3.0/drafthorse/models/product.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/models/references.py` & `drafthorse-2.3.0/drafthorse/models/references.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/models/trade.py` & `drafthorse-2.3.0/drafthorse/models/trade.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/models/tradelines.py` & `drafthorse-2.3.0/drafthorse/models/tradelines.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/pdf.py` & `drafthorse-2.3.0/drafthorse/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,29 @@
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 # LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 # DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 # THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 import datetime
+import logging
 import os
 from io import BytesIO
 from lxml import etree
-from PyPDF2 import PdfReader, PdfWriter
-from PyPDF2.generic import (
+from pypdf import PdfReader, PdfWriter
+from pypdf.generic import (
     ArrayObject,
     DecodedStreamObject,
     DictionaryObject,
     NameObject,
-    createStringObject,
+    create_string_object,
 )
 
+logger = logging.getLogger("drafthorse")
+
 
 def attach_xml(original_pdf, xml_data, level="BASIC"):
     if not isinstance(original_pdf, bytes):
         raise TypeError("Please supply original PDF as bytes.")
     if not isinstance(xml_data, bytes):
         raise TypeError("Please supply XML data as bytes.")
 
@@ -67,21 +70,21 @@
 
 def _get_original_output_intents(original_pdf):
     output_intents = []
     try:
         pdf_root = original_pdf.trailer["/Root"]
         ori_output_intents = pdf_root["/OutputIntents"]
         for ori_output_intent in ori_output_intents:
-            ori_output_intent_dict = ori_output_intent.getObject()
+            ori_output_intent_dict = ori_output_intent.get_object()
             dest_output_profile_dict = ori_output_intent_dict[
                 "/DestOutputProfile"
-            ].getObject()
+            ].get_object()
             output_intents.append((ori_output_intent_dict, dest_output_profile_dict))
-    except:  # noqa
-        pass
+    except Exception as ex:
+        logger.error(ex)
     return output_intents
 
 
 def _prepare_pdf_metadata_txt(pdf_metadata):
     pdf_date = datetime.datetime.utcnow().strftime("D:%Y%m%d%H%M%SZ")
     info_dict = {
         "/Author": pdf_metadata.get("author", ""),
@@ -134,15 +137,15 @@
     dc_desc_alt = etree.SubElement(dc_desc, ns_rdf + "Alt")
     dc_desc_alt_li = etree.SubElement(dc_desc_alt, ns_rdf + "li")
     dc_desc_alt_li.text = pdf_metadata.get("subject", "")
     dc_desc_alt_li.set(ns_xml + "lang", "x-default")
     desc_adobe = etree.SubElement(rdf, ns_rdf + "Description", nsmap=nsmap_pdf)
     desc_adobe.set(ns_rdf + "about", "")
     producer = etree.SubElement(desc_adobe, ns_pdf + "Producer")
-    producer.text = "PyPDF2"
+    producer.text = "pypdf"
     desc_xmp = etree.SubElement(rdf, ns_rdf + "Description", nsmap=nsmap_xmp)
     desc_xmp.set(ns_rdf + "about", "")
     creator = etree.SubElement(desc_xmp, ns_xmp + "CreatorTool")
     creator.text = "python-drafthorse"
     xmp_date = datetime.datetime.utcnow().replace(microsecond=0).isoformat() + "+00:00"
     etree.SubElement(desc_xmp, ns_xmp + "CreateDate").text = xmp_date
     etree.SubElement(desc_xmp, ns_xmp + "ModifyDate").text = xmp_date
@@ -188,22 +191,22 @@
     return xml_final_str
 
 
 def _facturx_update_metadata_add_attachment(
     pdf_filestream, facturx_xml_str, pdf_metadata, facturx_level, output_intents
 ):
     # md5sum = hashlib.md5(facturx_xml_str).hexdigest()
-    # md5sum_obj = createStringObject(md5sum)
+    # md5sum_obj = create_string_object(md5sum)
     pdf_date = datetime.datetime.utcnow().strftime("D:%Y%m%d%H%M%SZ")
     params_dict = DictionaryObject(
         {
             # NameObject('/CheckSum'): md5sum_obj,
-            NameObject("/ModDate"): createStringObject(pdf_date),
-            NameObject("/CreationDate"): createStringObject(pdf_date),
-            NameObject("/Size"): NameObject(str(len(facturx_xml_str))),
+            NameObject("/ModDate"): create_string_object(pdf_date),
+            NameObject("/CreationDate"): create_string_object(pdf_date),
+            NameObject("/Size"): create_string_object(str(len(facturx_xml_str))),
         }
     )
     file_entry = DecodedStreamObject()
     file_entry.set_data(facturx_xml_str)  # here we integrate the file itself
     file_entry.update(
         {
             NameObject("/Type"): NameObject("/EmbeddedFile"),
@@ -214,21 +217,21 @@
     )
     file_entry_obj = pdf_filestream._add_object(file_entry)
     # The Filespec entry
     ef_dict = DictionaryObject(
         {NameObject("/F"): file_entry_obj, NameObject("/UF"): file_entry_obj}
     )
 
-    fname_obj = createStringObject("factur-x.xml")
+    fname_obj = create_string_object("factur-x.xml")
     filespec_dict = DictionaryObject(
         {
             NameObject("/AFRelationship"): NameObject(
                 "/Data" if facturx_level in ("BASIC-WL", "MINIMUM") else "/Alternative"
             ),
-            NameObject("/Desc"): createStringObject(
+            NameObject("/Desc"): create_string_object(
                 "Invoice metadata conforming to ZUGFeRD standard (http://www.ferd-net.de/front_content.php?idcat=231&lang=4)"
             ),
             NameObject("/Type"): NameObject("/Filespec"),
             NameObject("/F"): fname_obj,
             NameObject("/EF"): ef_dict,
             NameObject("/UF"): fname_obj,
         }
@@ -236,15 +239,15 @@
     filespec_obj = pdf_filestream._add_object(filespec_dict)
     name_arrayobj_cdict = {fname_obj: filespec_obj}
     name_arrayobj_content_sort = list(
         sorted(name_arrayobj_cdict.items(), key=lambda x: x[0])
     )
     name_arrayobj_content_final = []
     af_list = []
-    for (fname_obj, filespec_obj) in name_arrayobj_content_sort:
+    for fname_obj, filespec_obj in name_arrayobj_content_sort:
         name_arrayobj_content_final += [fname_obj, filespec_obj]
         af_list.append(filespec_obj)
     embedded_files_names_dict = DictionaryObject(
         {NameObject("/Names"): ArrayObject(name_arrayobj_content_final)}
     )
     # Then create the entry for the root, as it needs a
     # reference to the Filespec
```

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC-WL.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC-WL.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC-WL_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC-WL_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC-WL_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC-WL_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC-WL_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC-WL_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_BASIC_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_BASIC_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EN16931.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EN16931.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EN16931_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EN16931_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EN16931_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EN16931_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EN16931_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EN16931_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EXTENDED.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EXTENDED.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EXTENDED_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EXTENDED_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EXTENDED_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EXTENDED_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_EXTENDED_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_EXTENDED_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_MINIMUM.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_MINIMUM.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_MINIMUM_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_MINIMUM_urn_un_unece_uncefact_data_standard_QualifiedDataType_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_MINIMUM_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_MINIMUM_urn_un_unece_uncefact_data_standard_ReusableAggregateBusinessInformationEntity_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/FACTUR-X_MINIMUM_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd` & `drafthorse-2.3.0/drafthorse/schema/FACTUR-X_MINIMUM_urn_un_unece_uncefact_data_standard_UnqualifiedDataType_100.xsd`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/schema/ZUGFeRD2p2_extension_schema.xmp` & `drafthorse-2.3.0/drafthorse/schema/ZUGFeRD2p2_extension_schema.xmp`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse/utils.py` & `drafthorse-2.3.0/drafthorse/utils.py`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/drafthorse.egg-info/PKG-INFO` & `drafthorse-2.3.0/drafthorse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drafthorse
-Version: 2.2.1
+Version: 2.3.0
 Summary: Python ZUGFeRD XML implementation
 Home-page: https://github.com/pretix/python-drafthorse
 Author: Raphael Michel
 Author-email: michel@rami.io
 License: Apache License
 Keywords: xml banking sepa
 Platform: UNKNOWN
```

### Comparing `drafthorse-2.2.1/drafthorse.egg-info/SOURCES.txt` & `drafthorse-2.3.0/drafthorse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drafthorse-2.2.1/setup.py` & `drafthorse-2.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,11 +29,11 @@
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     keywords="xml banking sepa",
-    install_requires=["lxml", "PyPDF2"],
+    install_requires=["lxml", "pypdf"],
     packages=find_packages(include=["drafthorse", "drafthorse.*"]),
     include_package_data=True,
 )
```

