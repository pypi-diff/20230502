# Comparing `tmp/collective.limitfilesizepanel-3.0.0.tar.gz` & `tmp/collective.limitfilesizepanel-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.limitfilesizepanel-3.0.0.tar", last modified: Thu Apr 27 08:23:18 2023, max compression
+gzip compressed data, was "collective.limitfilesizepanel-3.0.1.tar", last modified: Tue May  2 14:29:30 2023, max compression
```

## Comparing `collective.limitfilesizepanel-3.0.0.tar` & `collective.limitfilesizepanel-3.0.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.970950 collective.limitfilesizepanel-3.0.0/
--rw-r--r--   0 cekk       (501) staff       (20)      214 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     8211 2023-04-27 08:23:18.971144 collective.limitfilesizepanel-3.0.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3425 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)     2059 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/base.cfg
--rw-r--r--   0 cekk       (501) staff       (20)       96 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/buildout.cfg
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.955978 collective.limitfilesizepanel-3.0.0/collective/
--rw-r--r--   0 cekk       (501) staff       (20)      193 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.960694 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.960974 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/Extensions/
--rw-r--r--   0 cekk       (501) staff       (20)      450 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/Extensions/install.py
--rw-r--r--   0 cekk       (501) staff       (20)      221 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.962449 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1321 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1457 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/controlpanel.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.962731 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/images/
--rw-r--r--   0 cekk       (501) staff       (20)      879 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/images/limitfilesize-settings.png
--rw-r--r--   0 cekk       (501) staff       (20)     5492 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/limitfilesizepanel_view.py
--rw-r--r--   0 cekk       (501) staff       (20)     1468 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/tinymce_upload_p5.py
--rw-r--r--   0 cekk       (501) staff       (20)     1827 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     2760 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/dx_validators.py
--rw-r--r--   0 cekk       (501) staff       (20)     2458 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.963589 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      620 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/collective.limitfilesizepanel-manual.pot
--rw-r--r--   0 cekk       (501) staff       (20)     2862 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/collective.limitfilesizepanel.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.951820 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/de/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.964158 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/de/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     1671 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.mo
--rw-r--r--   0 cekk       (501) staff       (20)     3494 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.952096 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.964734 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     2765 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.mo
--rw-r--r--   0 cekk       (501) staff       (20)     4044 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.po
--rwxr-xr-x   0 cekk       (501) staff       (20)      240 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/rebuildPo.sh
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.952633 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.966314 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      159 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      733 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      183 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (501) staff       (20)      112 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      406 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.967201 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      183 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      464 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      561 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/uninstall/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)     2096 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     1282 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.968922 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      592 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/base_dx.py
--rw-r--r--   0 cekk       (501) staff       (20)     1446 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_bypassvalidation.py
--rw-r--r--   0 cekk       (501) staff       (20)     2631 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py
--rw-r--r--   0 cekk       (501) staff       (20)     2534 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_setup.py
--rw-r--r--   0 cekk       (501) staff       (20)     5054 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_validation.py
--rw-r--r--   0 cekk       (501) staff       (20)     1698 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/upgrades.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.958396 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     8211 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2836 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)       90 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      235 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/top_level.txt
--rw-r--r--   0 cekk       (501) staff       (20)       27 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/constraints_plone52.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.970668 collective.limitfilesizepanel-3.0.0/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     2205 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/docs/HISTORY.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1594 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/docs/INSTALL.txt
--rw-r--r--   0 cekk       (501) staff       (20)    17987 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/docs/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      746 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/docs/LICENSE.txt
--rw-r--r--   0 cekk       (501) staff       (20)    30244 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/docs/collective.limitfilesizepanel-1.3-01.png
--rw-r--r--   0 cekk       (501) staff       (20)    21991 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/docs/collective.limitfilesizepanel-1.3-02.png
--rw-r--r--   0 cekk       (501) staff       (20)       42 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      346 2023-04-27 08:23:18.971693 collective.limitfilesizepanel-3.0.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     1853 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/setup.py
--rw-r--r--   0 cekk       (501) staff       (20)     1838 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/test_plone52.cfg
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.621533 collective.limitfilesizepanel-3.0.1/
+-rw-r--r--   0 cekk       (501) staff       (20)      214 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     8371 2023-05-02 14:29:30.621766 collective.limitfilesizepanel-3.0.1/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3425 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     2059 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/base.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)       96 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/buildout.cfg
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.601414 collective.limitfilesizepanel-3.0.1/collective/
+-rw-r--r--   0 cekk       (501) staff       (20)      193 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.608067 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.608420 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/Extensions/
+-rw-r--r--   0 cekk       (501) staff       (20)      450 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/Extensions/install.py
+-rw-r--r--   0 cekk       (501) staff       (20)      221 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.610449 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1321 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1457 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/controlpanel.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.610836 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/images/
+-rw-r--r--   0 cekk       (501) staff       (20)      879 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/images/limitfilesize-settings.png
+-rw-r--r--   0 cekk       (501) staff       (20)     5492 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/limitfilesizepanel_view.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1468 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/tinymce_upload_p5.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1827 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2982 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/dx_validators.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2458 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.612216 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      620 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/collective.limitfilesizepanel-manual.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     2862 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/collective.limitfilesizepanel.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.593101 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/de/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.612922 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/de/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1671 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     3494 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.593668 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.613621 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     2765 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     4044 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.po
+-rwxr-xr-x   0 cekk       (501) staff       (20)      240 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/rebuildPo.sh
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.594562 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.615507 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      159 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      733 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      183 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      112 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      406 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.616655 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      183 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      464 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      561 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/uninstall/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     2096 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1282 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.618925 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      592 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/base_dx.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1446 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_bypassvalidation.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2631 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2534 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5054 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_validation.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1698 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/upgrades.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.605139 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     8371 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2836 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       90 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      235 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2023-05-02 14:29:30.000000 collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/top_level.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/constraints_plone52.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-05-02 14:29:30.621175 collective.limitfilesizepanel-3.0.1/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     2309 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/docs/HISTORY.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     1594 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/docs/INSTALL.txt
+-rw-r--r--   0 cekk       (501) staff       (20)    17987 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      746 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/docs/LICENSE.txt
+-rw-r--r--   0 cekk       (501) staff       (20)    30244 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/docs/collective.limitfilesizepanel-1.3-01.png
+-rw-r--r--   0 cekk       (501) staff       (20)    21991 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/docs/collective.limitfilesizepanel-1.3-02.png
+-rw-r--r--   0 cekk       (501) staff       (20)       42 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      346 2023-05-02 14:29:30.622454 collective.limitfilesizepanel-3.0.1/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     1853 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1838 2023-05-02 14:29:29.000000 collective.limitfilesizepanel-3.0.1/test_plone52.cfg
```

### Comparing `collective.limitfilesizepanel-3.0.0/PKG-INFO` & `collective.limitfilesizepanel-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.limitfilesizepanel
-Version: 3.0.0
+Version: 3.0.1
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
         
+        3.0.1 (2023-05-02)
+        ------------------
+        
+        - Raise ValueError instead Invalid for restapi calls.
+          [cekk]
+        
+        
         3.0.0 (2023-04-27)
         ------------------
         
         - Python3 support.
           [cekk]
         - Drop usage of persistent fields in registry. Now we use collective.z3cform.jsonwidget.
           [cekk]
```

### Comparing `collective.limitfilesizepanel-3.0.0/README.rst` & `collective.limitfilesizepanel-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/base.cfg` & `collective.limitfilesizepanel-3.0.1/base.cfg`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/configure.zcml` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/controlpanel.py` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/images/limitfilesize-settings.png` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/images/limitfilesize-settings.png`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/limitfilesizepanel_view.py` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/limitfilesizepanel_view.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/tinymce_upload_p5.py` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/browser/tinymce_upload_p5.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/configure.zcml` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/dx_validators.py` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/dx_validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,18 @@
 
         size_check = self.helper_view.check_size(
             maxsize=maxsize,
             uploadfile=self.value,
         )
 
         if size_check and not size_check.get("valid", False):
-            raise Invalid(size_check.get("error", ""))
+            if self.is_restapi():
+                raise ValueError(size_check.get("error", ""))
+            else:
+                raise Invalid(size_check.get("error", ""))
         return True
 
     def skip(self):
         """
         Skip only if we are in edit mode and newDataOnly is set
         """
         if not self.helper_view.newDataOnly():
@@ -72,14 +75,17 @@
         if self.request.steps:
             if self.request.steps[-1].startswith("++add++"):
                 return self.request.steps[-1].replace("++add++", "")
             if "@type" in self.request.form:
                 return self.request.form["@type"]
         return self.field.context.portal_type
 
+    def is_restapi(self):
+        return self.request.get_header("content-type") == "application/json"
+
 
 @implementer(IPluggableFileFieldValidation)
 @adapter(INamedFileField, Interface)
 class FileSizeValidator(BaseFileSizeValidator):
     """plone.namedfiled validator for filetype"""
```

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/interfaces.py` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/collective.limitfilesizepanel-manual.pot` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/collective.limitfilesizepanel-manual.pot`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/collective.limitfilesizepanel.pot` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/collective.limitfilesizepanel.pot`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.mo` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.mo`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.po` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.po`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.mo` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.mo`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.po` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.po`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/controlpanel.xml` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/uninstall/registry.xml` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/profiles/uninstall/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/setuphandlers.py` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/testing.py` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/testing.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/base_dx.py` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/base_dx.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_bypassvalidation.py` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_bypassvalidation.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_setup.py` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_validation.py` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/upgrades.zcml` & `collective.limitfilesizepanel-3.0.1/collective/limitfilesizepanel/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/PKG-INFO` & `collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.limitfilesizepanel
-Version: 3.0.0
+Version: 3.0.1
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
         
+        3.0.1 (2023-05-02)
+        ------------------
+        
+        - Raise ValueError instead Invalid for restapi calls.
+          [cekk]
+        
+        
         3.0.0 (2023-04-27)
         ------------------
         
         - Python3 support.
           [cekk]
         - Drop usage of persistent fields in registry. Now we use collective.z3cform.jsonwidget.
           [cekk]
```

### Comparing `collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/SOURCES.txt` & `collective.limitfilesizepanel-3.0.1/collective.limitfilesizepanel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/docs/HISTORY.rst` & `collective.limitfilesizepanel-3.0.1/docs/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+3.0.1 (2023-05-02)
+------------------
+
+- Raise ValueError instead Invalid for restapi calls.
+  [cekk]
+
+
 3.0.0 (2023-04-27)
 ------------------
 
 - Python3 support.
   [cekk]
 - Drop usage of persistent fields in registry. Now we use collective.z3cform.jsonwidget.
   [cekk]
```

### Comparing `collective.limitfilesizepanel-3.0.0/docs/INSTALL.txt` & `collective.limitfilesizepanel-3.0.1/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/docs/LICENSE.GPL` & `collective.limitfilesizepanel-3.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/docs/LICENSE.txt` & `collective.limitfilesizepanel-3.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/docs/collective.limitfilesizepanel-1.3-01.png` & `collective.limitfilesizepanel-3.0.1/docs/collective.limitfilesizepanel-1.3-01.png`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/docs/collective.limitfilesizepanel-1.3-02.png` & `collective.limitfilesizepanel-3.0.1/docs/collective.limitfilesizepanel-1.3-02.png`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-3.0.0/setup.py` & `collective.limitfilesizepanel-3.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-version = "3.0.0"
+version = "3.0.1"
 
 tests_require = [
     "plone.app.testing",
     "plone.testing>=5.0.0",
     "plone.app.contenttypes",
     "plone.app.robotframework[debug]",
 ]
```

### Comparing `collective.limitfilesizepanel-3.0.0/test_plone52.cfg` & `collective.limitfilesizepanel-3.0.1/test_plone52.cfg`

 * *Files identical despite different names*

