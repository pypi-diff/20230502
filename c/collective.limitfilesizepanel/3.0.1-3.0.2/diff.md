# Comparing `tmp/collective.limitfilesizepanel-3.0.1.tar.gz` & `tmp/collective.limitfilesizepanel-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.limitfilesizepanel-3.0.1.tar", last modified: Tue May  2 14:29:30 2023, max compression
+gzip compressed data, was "collective.limitfilesizepanel-3.0.2.tar", last modified: Tue May  2 14:43:09 2023, max compression
```

## Comparing `collective.limitfilesizepanel-3.0.1.tar` & `collective.limitfilesizepanel-3.0.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.621533 collective.limitfilesizepanel-3.0.1/
--rw-r--r--   0 cekk       (501) staff       (20)      214 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     8371 2023-05-02 14:29:30.621766 collective.limitfilesizepanel-3.0.1/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3425 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)     2059 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/base.cfg
--rw-r--r--   0 cekk       (501) staff       (20)       96 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/buildout.cfg
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.601414 collective.limitfilesizepanel-3.0.1/collective/
--rw-r--r--   0 cekk       (501) staff       (20)      193 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.608067 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.608420 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/Extensions/
--rw-r--r--   0 cekk       (501) staff       (20)      450 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/Extensions/install.py
--rw-r--r--   0 cekk       (501) staff       (20)      221 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.610449 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1321 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1457 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/controlpanel.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.610836 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/images/
--rw-r--r--   0 cekk       (501) staff       (20)      879 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/images/limitfilesize-settings.png
--rw-r--r--   0 cekk       (501) staff       (20)     5492 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/limitfilesizepanel_view.py
--rw-r--r--   0 cekk       (501) staff       (20)     1468 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/tinymce_upload_p5.py
--rw-r--r--   0 cekk       (501) staff       (20)     1827 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     2982 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/dx_validators.py
--rw-r--r--   0 cekk       (501) staff       (20)     2458 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.612216 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      620 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/collective.limitfilesizepanel-manual.pot
--rw-r--r--   0 cekk       (501) staff       (20)     2862 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/collective.limitfilesizepanel.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.593101 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/de/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.612922 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/de/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     1671 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.mo
--rw-r--r--   0 cekk       (501) staff       (20)     3494 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.593668 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.613621 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     2765 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.mo
--rw-r--r--   0 cekk       (501) staff       (20)     4044 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.po
--rwxr-xr-x   0 cekk       (501) staff       (20)      240 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/rebuildPo.sh
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.594562 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.615507 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      159 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      733 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      183 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (501) staff       (20)      112 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      406 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.616655 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      183 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      464 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      561 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/uninstall/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)     2096 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     1282 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.618925 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      592 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/base_dx.py
--rw-r--r--   0 cekk       (501) staff       (20)     1446 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_bypassvalidation.py
--rw-r--r--   0 cekk       (501) staff       (20)     2631 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py
--rw-r--r--   0 cekk       (501) staff       (20)     2534 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_setup.py
--rw-r--r--   0 cekk       (501) staff       (20)     5054 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_validation.py
--rw-r--r--   0 cekk       (501) staff       (20)     1698 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/upgrades.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.605139 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     8371 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2836 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)       90 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      235 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/top_level.txt
--rw-r--r--   0 cekk       (501) staff       (20)       27 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/constraints_plone52.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.621175 collective.limitfilesizepanel-3.0.1/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     2309 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/docs/HISTORY.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1594 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/docs/INSTALL.txt
--rw-r--r--   0 cekk       (501) staff       (20)    17987 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/docs/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      746 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/docs/LICENSE.txt
--rw-r--r--   0 cekk       (501) staff       (20)    30244 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/docs/collective.limitfilesizepanel-1.3-01.png
--rw-r--r--   0 cekk       (501) staff       (20)    21991 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/docs/collective.limitfilesizepanel-1.3-02.png
--rw-r--r--   0 cekk       (501) staff       (20)       42 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      346 2023-05-02 14:29:30.622454 collective.limitfilesizepanel-3.0.1/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     1853 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/setup.py
--rw-r--r--   0 cekk       (501) staff       (20)     1838 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/test_plone52.cfg
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.286267 collective.limitfilesizepanel-3.0.2/
+-rw-r--r--   0 cekk       (501) staff       (20)      214 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     8540 2023-05-02 14:43:09.286535 collective.limitfilesizepanel-3.0.2/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3425 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     2059 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/base.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)       96 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/buildout.cfg
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.268696 collective.limitfilesizepanel-3.0.2/collective/
+-rw-r--r--   0 cekk       (501) staff       (20)      193 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.273923 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.274273 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/Extensions/
+-rw-r--r--   0 cekk       (501) staff       (20)      450 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/Extensions/install.py
+-rw-r--r--   0 cekk       (501) staff       (20)      221 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.275958 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1321 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1457 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/controlpanel.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.276303 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/images/
+-rw-r--r--   0 cekk       (501) staff       (20)      879 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/images/limitfilesize-settings.png
+-rw-r--r--   0 cekk       (501) staff       (20)     5492 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/limitfilesizepanel_view.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1468 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/tinymce_upload_p5.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1827 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     3034 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/dx_validators.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2458 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.277351 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      620 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/collective.limitfilesizepanel-manual.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     2862 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/collective.limitfilesizepanel.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.263635 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/de/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.278051 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/de/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1671 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     3494 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.263969 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.278755 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     2765 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     4044 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.po
+-rwxr-xr-x   0 cekk       (501) staff       (20)      240 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/rebuildPo.sh
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.264507 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.280501 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      159 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      733 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      183 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      112 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      406 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.281550 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      183 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      464 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      561 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/uninstall/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     2096 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1282 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.283752 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      592 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/tests/base_dx.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1446 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/tests/test_bypassvalidation.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2631 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2534 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/tests/test_setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5054 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/tests/test_validation.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1698 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/upgrades.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.271520 collective.limitfilesizepanel-3.0.2/collective.limitfilesizepanel.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     8540 2023-05-02 14:43:09.000000 collective.limitfilesizepanel-3.0.2/collective.limitfilesizepanel.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2836 2023-05-02 14:43:09.000000 collective.limitfilesizepanel-3.0.2/collective.limitfilesizepanel.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-05-02 14:43:09.000000 collective.limitfilesizepanel-3.0.2/collective.limitfilesizepanel.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       90 2023-05-02 14:43:09.000000 collective.limitfilesizepanel-3.0.2/collective.limitfilesizepanel.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2023-05-02 14:43:09.000000 collective.limitfilesizepanel-3.0.2/collective.limitfilesizepanel.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-05-02 14:43:09.000000 collective.limitfilesizepanel-3.0.2/collective.limitfilesizepanel.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      235 2023-05-02 14:43:09.000000 collective.limitfilesizepanel-3.0.2/collective.limitfilesizepanel.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2023-05-02 14:43:09.000000 collective.limitfilesizepanel-3.0.2/collective.limitfilesizepanel.egg-info/top_level.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/constraints_plone52.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:43:09.285921 collective.limitfilesizepanel-3.0.2/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     2422 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/docs/HISTORY.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     1594 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/docs/INSTALL.txt
+-rw-r--r--   0 cekk       (501) staff       (20)    17987 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      746 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/docs/LICENSE.txt
+-rw-r--r--   0 cekk       (501) staff       (20)    30244 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/docs/collective.limitfilesizepanel-1.3-01.png
+-rw-r--r--   0 cekk       (501) staff       (20)    21991 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/docs/collective.limitfilesizepanel-1.3-02.png
+-rw-r--r--   0 cekk       (501) staff       (20)       42 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      346 2023-05-02 14:43:09.287237 collective.limitfilesizepanel-3.0.2/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     1853 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1838 2023-05-02 14:43:08.000000 collective.limitfilesizepanel-3.0.2/test_plone52.cfg
```

### Comparing `collective.limitfilesizepanel-3.0.1/PKG-INFO` & `collective.limitfilesizepanel-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.limitfilesizepanel
-Version: 3.0.1
+Version: 3.0.2
 Summary: Configure files and images size limit through Plone control panel
 Home-page: http://plone.org/products/collective.limitfilesizepanel
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Description: This is an helper package that setup a RedTurtle's Plone site ready to work with Volto.
         
@@ -104,14 +104,21 @@
         .. image:: http://www.redturtle.it/redturtle_banner.png
            :alt: RedTurtle Technology Site
            :target: http://www.redturtle.it/
         
         Changelog
         =========
         
+        3.0.2 (2023-05-02)
+        ------------------
+        
+        - Raise custom ValidationError to have a 400 on restapi calls.
+          [cekk]
+        
+        
         3.0.1 (2023-05-02)
         ------------------
         
         - Raise ValueError instead Invalid for restapi calls.
           [cekk]
```

### Comparing `collective.limitfilesizepanel-3.0.1/README.rst` & `collective.limitfilesizepanel-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/base.cfg` & `collective.limitfilesizepanel-3.0.2/base.cfg`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/configure.zcml` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/controlpanel.py` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/images/limitfilesize-settings.png` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/images/limitfilesize-settings.png`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/limitfilesizepanel_view.py` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/limitfilesizepanel_view.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/tinymce_upload_p5.py` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/browser/tinymce_upload_p5.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/configure.zcml` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/dx_validators.py` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/dx_validators.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,28 @@
 from plone.namedfile.interfaces import INamedFileField
 from plone.namedfile.interfaces import IPluggableFileFieldValidation
 from plone.namedfile.interfaces import IPluggableImageFieldValidation
 from plone.namedfile.interfaces import INamedImageField
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
-from zope.interface import Invalid
 from zope.globalrequest import getRequest
+from zope.schema import ValidationError
+
+
+class InvalidSize(ValidationError):
+    """Exception for invalid size"""
+
+    __doc__ = "Invalid size"
+
+    def doc(self):
+        if len(self.args) > 1:
+            return self.args[0]
+        else:
+            return self.__class__.__doc__
 
 
 class BaseFileSizeValidator:
     """ """
 
     def __init__(self, field, value):
         self.field = field
@@ -47,18 +59,15 @@
 
         size_check = self.helper_view.check_size(
             maxsize=maxsize,
             uploadfile=self.value,
         )
 
         if size_check and not size_check.get("valid", False):
-            if self.is_restapi():
-                raise ValueError(size_check.get("error", ""))
-            else:
-                raise Invalid(size_check.get("error", ""))
+            raise InvalidSize(size_check.get("error", ""), self.field.__name__)
         return True
 
     def skip(self):
         """
         Skip only if we are in edit mode and newDataOnly is set
         """
         if not self.helper_view.newDataOnly():
@@ -75,17 +84,14 @@
         if self.request.steps:
             if self.request.steps[-1].startswith("++add++"):
                 return self.request.steps[-1].replace("++add++", "")
             if "@type" in self.request.form:
                 return self.request.form["@type"]
         return self.field.context.portal_type
 
-    def is_restapi(self):
-        return self.request.get_header("content-type") == "application/json"
-
 
 @implementer(IPluggableFileFieldValidation)
 @adapter(INamedFileField, Interface)
 class FileSizeValidator(BaseFileSizeValidator):
     """plone.namedfiled validator for filetype"""
```

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/interfaces.py` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/collective.limitfilesizepanel-manual.pot` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/collective.limitfilesizepanel-manual.pot`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/collective.limitfilesizepanel.pot` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/collective.limitfilesizepanel.pot`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.mo` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.mo`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.po` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.po`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.mo` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.mo`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.po` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.po`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/controlpanel.xml` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/uninstall/registry.xml` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/profiles/uninstall/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/setuphandlers.py` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/testing.py` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/testing.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/base_dx.py` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/tests/base_dx.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_bypassvalidation.py` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/tests/test_bypassvalidation.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_setup.py` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_validation.py` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/upgrades.zcml` & `collective.limitfilesizepanel-3.0.2/collective/limitfilesizepanel/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/PKG-INFO` & `collective.limitfilesizepanel-3.0.2/collective.limitfilesizepanel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.limitfilesizepanel
-Version: 3.0.1
+Version: 3.0.2
 Summary: Configure files and images size limit through Plone control panel
 Home-page: http://plone.org/products/collective.limitfilesizepanel
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Description: This is an helper package that setup a RedTurtle's Plone site ready to work with Volto.
         
@@ -104,14 +104,21 @@
         .. image:: http://www.redturtle.it/redturtle_banner.png
            :alt: RedTurtle Technology Site
            :target: http://www.redturtle.it/
         
         Changelog
         =========
         
+        3.0.2 (2023-05-02)
+        ------------------
+        
+        - Raise custom ValidationError to have a 400 on restapi calls.
+          [cekk]
+        
+        
         3.0.1 (2023-05-02)
         ------------------
         
         - Raise ValueError instead Invalid for restapi calls.
           [cekk]
```

### Comparing `collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/SOURCES.txt` & `collective.limitfilesizepanel-3.0.2/collective.limitfilesizepanel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/docs/HISTORY.rst` & `collective.limitfilesizepanel-3.0.2/docs/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+3.0.2 (2023-05-02)
+------------------
+
+- Raise custom ValidationError to have a 400 on restapi calls.
+  [cekk]
+
+
 3.0.1 (2023-05-02)
 ------------------
 
 - Raise ValueError instead Invalid for restapi calls.
   [cekk]
```

### Comparing `collective.limitfilesizepanel-3.0.1/docs/INSTALL.txt` & `collective.limitfilesizepanel-3.0.2/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/docs/LICENSE.GPL` & `collective.limitfilesizepanel-3.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/docs/LICENSE.txt` & `collective.limitfilesizepanel-3.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/docs/collective.limitfilesizepanel-1.3-01.png` & `collective.limitfilesizepanel-3.0.2/docs/collective.limitfilesizepanel-1.3-01.png`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/docs/collective.limitfilesizepanel-1.3-02.png` & `collective.limitfilesizepanel-3.0.2/docs/collective.limitfilesizepanel-1.3-02.png`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.1/setup.py` & `collective.limitfilesizepanel-3.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-version = "3.0.1"
+version = "3.0.2"
 
 tests_require = [
     "plone.app.testing",
     "plone.testing>=5.0.0",
     "plone.app.contenttypes",
     "plone.app.robotframework[debug]",
 ]
```

### Comparing `collective.limitfilesizepanel-3.0.1/test_plone52.cfg` & `collective.limitfilesizepanel-3.0.2/test_plone52.cfg`

 * *Files identical despite different names*

