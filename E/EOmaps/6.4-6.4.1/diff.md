# Comparing `tmp/EOmaps-6.4.tar.gz` & `tmp/EOmaps-6.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/EOmaps-6.4.tar", last modified: Mon Apr 24 13:10:45 2023, max compression
+gzip compressed data, was "dist/EOmaps-6.4.1.tar", last modified: Tue May  2 11:41:34 2023, max compression
```

## Comparing `EOmaps-6.4.tar` & `EOmaps-6.4.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:45.000000 EOmaps-6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:45.000000 EOmaps-6.4/EOmaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-04-24 13:10:44.000000 EOmaps-6.4/EOmaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-24 13:10:45.000000 EOmaps-6.4/EOmaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:10:44.000000 EOmaps-6.4/EOmaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-24 13:10:44.000000 EOmaps-6.4/EOmaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 13:10:44.000000 EOmaps-6.4/EOmaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 13:10:33.000000 EOmaps-6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-04-24 13:10:45.000000 EOmaps-6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-04-24 13:10:33.000000 EOmaps-6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:45.000000 EOmaps-6.4/eomaps/
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/NE_features.json
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68730 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_cb_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27548 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    62949 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    46463 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_webmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    81704 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_webmap_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    40682 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    44442 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    19138 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/compass.py
--rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)   176295 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/eomaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    82397 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/mapsgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/ne_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/projections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:45.000000 EOmaps-6.4/eomaps/qtcompanion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:45.000000 EOmaps-6.4/eomaps/qtcompanion/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/close.png
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/eye_closed.png
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/eye_open.png
--rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/maximize.png
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_bottom_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_circle.png
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_circle_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_ellipse.png
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_ellipse_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_left_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_rectangle.png
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_rectangle_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_right_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_square.png
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_square_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_top.png
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_top_active.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:45.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18878 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/click_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)    47567 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/extent.py
--rw-r--r--   0 runner    (1001) docker     (123)    36930 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/peek.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/save.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/wms.py
--rw-r--r--   0 runner    (1001) docker     (123)    46756 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/scalebar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:10:45.000000 EOmaps-6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-24 13:10:34.000000 EOmaps-6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:34.000000 EOmaps-6.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:34.000000 EOmaps-6.4.1/EOmaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-05-02 11:41:33.000000 EOmaps-6.4.1/EOmaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-02 11:41:34.000000 EOmaps-6.4.1/EOmaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:41:33.000000 EOmaps-6.4.1/EOmaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-02 11:41:33.000000 EOmaps-6.4.1/EOmaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 11:41:33.000000 EOmaps-6.4.1/EOmaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 11:41:21.000000 EOmaps-6.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-05-02 11:41:34.000000 EOmaps-6.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-05-02 11:41:21.000000 EOmaps-6.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:34.000000 EOmaps-6.4.1/eomaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/NE_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68730 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_cb_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27548 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62949 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46463 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_webmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81704 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_webmap_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40682 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44442 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19138 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176338 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/eomaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82477 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/mapsgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/ne_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/projections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:34.000000 EOmaps-6.4.1/eomaps/qtcompanion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:34.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/close.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/eye_closed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/eye_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/maximize.png
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_bottom_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_circle.png
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_circle_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_ellipse.png
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_ellipse_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_left_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_rectangle.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_rectangle_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_right_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_square_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_top.png
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_top_active.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:34.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18878 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/click_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47567 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36930 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/peek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/wms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46756 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/scalebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:41:34.000000 EOmaps-6.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-02 11:41:21.000000 EOmaps-6.4.1/setup.py
```

### Comparing `EOmaps-6.4/EOmaps.egg-info/PKG-INFO` & `EOmaps-6.4.1/EOmaps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EOmaps
-Version: 6.4
+Version: 6.4.1
 Summary: A library to create interactive maps of geographical datasets.
 Home-page: https://github.com/raphaelquast/maps
 Author: Raphael Quast
 Author-email: raphael.quast@geo.tuwien.ac.at
 Maintainer: Raphael Quast
 Maintainer-email: raphael.quast@geo.tuwien.ac.at
 License: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EOmaps Version: 6.4 Summary: A library to create
+Metadata-Version: 2.1 Name: EOmaps Version: 6.4.1 Summary: A library to create
 interactive maps of geographical datasets. Home-page: https://github.com/
 raphaelquast/maps Author: Raphael Quast Author-email:
 raphael.quast@geo.tuwien.ac.at Maintainer: Raphael Quast Maintainer-email:
 raphael.quast@geo.tuwien.ac.at License: GNU General Public License v3 or later
 (GPLv3+) Description:
                                  [EOmaps_logo]
 [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/
```

### Comparing `EOmaps-6.4/EOmaps.egg-info/SOURCES.txt` & `EOmaps-6.4.1/EOmaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/LICENSE` & `EOmaps-6.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/PKG-INFO` & `EOmaps-6.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EOmaps
-Version: 6.4
+Version: 6.4.1
 Summary: A library to create interactive maps of geographical datasets.
 Home-page: https://github.com/raphaelquast/maps
 Author: Raphael Quast
 Author-email: raphael.quast@geo.tuwien.ac.at
 Maintainer: Raphael Quast
 Maintainer-email: raphael.quast@geo.tuwien.ac.at
 License: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EOmaps Version: 6.4 Summary: A library to create
+Metadata-Version: 2.1 Name: EOmaps Version: 6.4.1 Summary: A library to create
 interactive maps of geographical datasets. Home-page: https://github.com/
 raphaelquast/maps Author: Raphael Quast Author-email:
 raphael.quast@geo.tuwien.ac.at Maintainer: Raphael Quast Maintainer-email:
 raphael.quast@geo.tuwien.ac.at License: GNU General Public License v3 or later
 (GPLv3+) Description:
                                  [EOmaps_logo]
 [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/
```

### Comparing `EOmaps-6.4/README.md` & `EOmaps-6.4.1/README.md`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/NE_features.json` & `EOmaps-6.4.1/eomaps/NE_features.json`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/__init__.py` & `EOmaps-6.4.1/eomaps/__init__.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/_cb_container.py` & `EOmaps-6.4.1/eomaps/_cb_container.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/_containers.py` & `EOmaps-6.4.1/eomaps/_containers.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/_data_manager.py` & `EOmaps-6.4.1/eomaps/_data_manager.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/_shapes.py` & `EOmaps-6.4.1/eomaps/_shapes.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/_webmap.py` & `EOmaps-6.4.1/eomaps/_webmap.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/_webmap_containers.py` & `EOmaps-6.4.1/eomaps/_webmap_containers.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/callbacks.py` & `EOmaps-6.4.1/eomaps/callbacks.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/colorbar.py` & `EOmaps-6.4.1/eomaps/colorbar.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/compass.py` & `EOmaps-6.4.1/eomaps/compass.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/draw.py` & `EOmaps-6.4.1/eomaps/draw.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/eomaps.py` & `EOmaps-6.4.1/eomaps/eomaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -2355,16 +2355,16 @@
             crs = self._get_cartopy_crs(crs)
         else:
             crs = Maps.CRS.PlateCarree()
 
         return self.ax.get_extent(crs=crs)
 
     def _set_vmin_vmax(self, vmin=None, vmax=None):
-        self._vmin = vmin
-        self._vmax = vmax
+        self._vmin = self._encode_values(vmin)
+        self._vmax = self._encode_values(vmax)
 
         if self._inherit_classification is not None:
             if not (vmin is None and vmax is None):
                 raise TypeError(
                     "EOmaps: 'vmin' and 'vmax' cannot be set explicitly "
                     "if the classification is inherited!"
                 )
@@ -2376,30 +2376,26 @@
 
             self._vmin = self._inherit_classification._vmin
             self._vmax = self._inherit_classification._vmax
             return
 
         if not self.shape.name.startswith("shade_"):
             if vmin is None and self.data is not None:
-                self._vmin = self._encode_values(np.nanmin(self._data_manager.z_data))
+                self._vmin = np.nanmin(self._data_manager.z_data)
             if vmax is None and self.data is not None:
-                self._vmax = self._encode_values(np.nanmax(self._data_manager.z_data))
+                self._vmax = np.nanmax(self._data_manager.z_data)
         else:
             # get the name of the used aggretation reduction
             aggname = self.shape.aggregator.__class__.__name__
             if aggname in ["first", "last", "max", "min", "mean", "mode"]:
                 # set vmin/vmax in case the aggregation still represents data-values
                 if vmin is None:
-                    self._vmin = self._encode_values(
-                        np.nanmin(self._data_manager.z_data)
-                    )
+                    self._vmin = np.nanmin(self._data_manager.z_data)
                 if vmax is None:
-                    self._vmax = self._encode_values(
-                        np.nanmax(self._data_manager.z_data)
-                    )
+                    self._vmax = np.nanmax(self._data_manager.z_data)
             else:
                 # set vmin/vmax for aggregations that do NOT represent data values
 
                 # allow vmin/vmax = None (e.g. autoscaling)
                 if "count" in aggname:
                     # if the reduction represents a count, don't count empty pixels
                     if vmin and vmin <= 0:
@@ -4373,27 +4369,34 @@
 
         Returns
         -------
         encoded_values
             The encoded data values
         """
         encoding = self.data_specs.encoding
+
         if encoding is not None:
             try:
                 scale_factor = encoding.get("scale_factor", None)
                 add_offset = encoding.get("add_offset", None)
+                fill_value = encoding.get("_FillValue", None)
+
+                if val is None:
+                    return fill_value
 
                 if add_offset:
                     val = val - add_offset
                 if scale_factor:
                     val = val / scale_factor
 
                 return val
             except:
-                print("EOmaps: There was an error while trying to encode the data.")
+                print(
+                    "EOmaps: There was an error while trying to encode the data:", val
+                )
                 return val
         else:
             return val
 
     def _decode_values(self, val):
         """
         Decode data-values with respect to the provided "scale_factor" and "add_offset".
```

### Comparing `EOmaps-6.4/eomaps/grid.py` & `EOmaps-6.4.1/eomaps/grid.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/helpers.py` & `EOmaps-6.4.1/eomaps/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
             if getattr(self._m.shape, "radius_crs", None) != "out":
                 try:
                     radius = self._m.set_shape._estimate_radius(self._m, "out", np.max)
                 except AssertionError:
                     print(
                         "EOmaps: Unable to estimate search-radius based on data."
                         "Defaulting to `np.inf`. "
-                        "See `m.tree.set_search_radius` for more details!"
+                        "See `m.cb.pick.set_props(search_radius=...)` for more details!"
                     )
                     radius = [np.inf]
             else:
                 radius = self._m.shape.radius
 
             self._d = np.max(radius) * float(self._search_radius)
         elif isinstance(r, (int, float, np.number)):
@@ -1943,14 +1943,16 @@
 
         # tag all relevant layers for refetch
         self._refetch_layer(layer)
 
         for f in self._on_add_bg_artist:
             f()
 
+        self.canvas.draw_idle()
+
     def remove_bg_artist(self, art, layer=None):
         # handle the "__inset_" prefix of inset-map artists
         if (
             layer is not None
             and getattr(art, "axes", None) is not None
             and art.axes.get_label() == "inset_map"
             and not layer.startswith("__inset_")
@@ -1988,14 +1990,16 @@
         if removed:
             for f in self._on_remove_bg_artist:
                 f()
 
             # tag all relevant layers for refetch
             self._refetch_layer(layer)
 
+        self.canvas.draw_idle()
+
     def remove_artist(self, art, layer=None):
         # this only removes the artist from the blit-manager,
         # it does not clear it from the plot!
 
         if layer is None:
             for key, layerartists in self._artists.items():
                 if art in layerartists:
```

### Comparing `EOmaps-6.4/eomaps/logo.png` & `EOmaps-6.4.1/eomaps/logo.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/mapsgrid.py` & `EOmaps-6.4.1/eomaps/mapsgrid.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/ne_features.py` & `EOmaps-6.4.1/eomaps/ne_features.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/projections.py` & `EOmaps-6.4.1/eomaps/projections.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/app.py` & `EOmaps-6.4.1/eomaps/qtcompanion/app.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/base.py` & `EOmaps-6.4.1/eomaps/qtcompanion/base.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/icons/eye_closed.png` & `EOmaps-6.4.1/eomaps/qtcompanion/icons/eye_closed.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/icons/eye_open.png` & `EOmaps-6.4.1/eomaps/qtcompanion/icons/eye_open.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/icons/logo.png` & `EOmaps-6.4.1/eomaps/qtcompanion/icons/logo.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/icons/peek_circle.png` & `EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_circle.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/icons/peek_circle_active.png` & `EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_circle_active.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/icons/peek_ellipse.png` & `EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_ellipse.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/icons/peek_ellipse_active.png` & `EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_ellipse_active.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/widgets/annotate.py` & `EOmaps-6.4.1/eomaps/qtcompanion/widgets/annotate.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/widgets/click_callbacks.py` & `EOmaps-6.4.1/eomaps/qtcompanion/widgets/click_callbacks.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/widgets/draw.py` & `EOmaps-6.4.1/eomaps/qtcompanion/widgets/draw.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/widgets/editor.py` & `EOmaps-6.4.1/eomaps/qtcompanion/widgets/editor.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/widgets/extent.py` & `EOmaps-6.4.1/eomaps/qtcompanion/widgets/extent.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/widgets/files.py` & `EOmaps-6.4.1/eomaps/qtcompanion/widgets/files.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/widgets/layer.py` & `EOmaps-6.4.1/eomaps/qtcompanion/widgets/layer.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/widgets/peek.py` & `EOmaps-6.4.1/eomaps/qtcompanion/widgets/peek.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/widgets/save.py` & `EOmaps-6.4.1/eomaps/qtcompanion/widgets/save.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/widgets/utils.py` & `EOmaps-6.4.1/eomaps/qtcompanion/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/qtcompanion/widgets/wms.py` & `EOmaps-6.4.1/eomaps/qtcompanion/widgets/wms.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/reader.py` & `EOmaps-6.4.1/eomaps/reader.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/scalebar.py` & `EOmaps-6.4.1/eomaps/scalebar.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/eomaps/utilities.py` & `EOmaps-6.4.1/eomaps/utilities.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4/setup.py` & `EOmaps-6.4.1/setup.py`

 * *Files identical despite different names*

