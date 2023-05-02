# Comparing `tmp/xicsrt-0.8.7.tar.gz` & `tmp/xicsrt-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xicsrt-0.8.7.tar", last modified: Wed Mar  8 14:39:10 2023, max compression
+gzip compressed data, was "xicsrt-0.8.8.tar", last modified: Tue May  2 19:46:28 2023, max compression
```

## Comparing `xicsrt-0.8.7.tar` & `xicsrt-0.8.8.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.286899 xicsrt-0.8.7/
--rw-r--r--   0 npablant (149941814) 1832971548      495 2021-08-03 19:49:51.000000 xicsrt-0.8.7/AUTHORS
--rw-r--r--   0 npablant (149941814) 1832971548     1120 2021-10-28 17:18:05.000000 xicsrt-0.8.7/LICENSE
--rw-r--r--   0 npablant (149941814) 1832971548     2583 2023-03-08 14:39:10.286748 xicsrt-0.8.7/PKG-INFO
--rw-r--r--   0 npablant (149941814) 1832971548     1961 2021-07-13 18:33:20.000000 xicsrt-0.8.7/README.md
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.262923 xicsrt-0.8.7/examples/
--rw-r--r--   0 npablant (149941814) 1832971548      180 2020-10-14 18:03:43.000000 xicsrt-0.8.7/examples/__init__.py
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.263349 xicsrt-0.8.7/examples/example_00/
--rw-r--r--   0 npablant (149941814) 1832971548        0 2020-10-14 18:03:43.000000 xicsrt-0.8.7/examples/example_00/__init__.py
--rw-r--r--   0 npablant (149941814) 1832971548     2745 2021-10-28 16:30:58.000000 xicsrt-0.8.7/examples/example_00/example_00.py
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.263754 xicsrt-0.8.7/examples/example_01/
--rw-r--r--   0 npablant (149941814) 1832971548        0 2020-10-14 18:03:43.000000 xicsrt-0.8.7/examples/example_01/__init__.py
--rw-r--r--   0 npablant (149941814) 1832971548     2032 2021-10-28 16:30:58.000000 xicsrt-0.8.7/examples/example_01/example_01.py
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.264037 xicsrt-0.8.7/examples/example_02/
--rw-r--r--   0 npablant (149941814) 1832971548        0 2021-10-28 16:30:58.000000 xicsrt-0.8.7/examples/example_02/__init__.py
--rw-r--r--   0 npablant (149941814) 1832971548     1869 2021-10-28 16:30:58.000000 xicsrt-0.8.7/examples/example_02/example_02.py
--rw-r--r--   0 npablant (149941814) 1832971548       38 2023-03-08 14:39:10.286944 xicsrt-0.8.7/setup.cfg
--rw-r--r--   0 npablant (149941814) 1832971548     1568 2021-08-03 19:49:51.000000 xicsrt-0.8.7/setup.py
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.265963 xicsrt-0.8.7/xicsrt/
--rw-r--r--   0 npablant (149941814) 1832971548      376 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/__init__.py
--rw-r--r--   0 npablant (149941814) 1832971548     4230 2021-08-10 19:43:11.000000 xicsrt-0.8.7/xicsrt/__main__.py
--rw-r--r--   0 npablant (149941814) 1832971548      956 2023-03-08 14:37:28.000000 xicsrt-0.8.7/xicsrt/_version.py
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.267378 xicsrt-0.8.7/xicsrt/filters/
--rw-r--r--   0 npablant (149941814) 1832971548      672 2021-07-10 01:56:10.000000 xicsrt-0.8.7/xicsrt/filters/_XicsrtBundleFilter.py
--rw-r--r--   0 npablant (149941814) 1832971548     1529 2021-07-10 01:56:11.000000 xicsrt-0.8.7/xicsrt/filters/_XicsrtBundleFilterSightline.py
--rw-r--r--   0 npablant (149941814) 1832971548      119 2021-06-22 02:32:10.000000 xicsrt-0.8.7/xicsrt/filters/__init__.py
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.268426 xicsrt-0.8.7/xicsrt/objects/
--rw-r--r--   0 npablant (149941814) 1832971548     2325 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/objects/_ConfigObject.py
--rw-r--r--   0 npablant (149941814) 1832971548     6957 2021-08-03 19:49:51.000000 xicsrt-0.8.7/xicsrt/objects/_Dispatcher.py
--rw-r--r--   0 npablant (149941814) 1832971548     5747 2021-10-28 17:18:05.000000 xicsrt-0.8.7/xicsrt/objects/_GeometryObject.py
--rw-r--r--   0 npablant (149941814) 1832971548     2957 2021-07-13 18:33:20.000000 xicsrt-0.8.7/xicsrt/objects/_RayArray.py
--rw-r--r--   0 npablant (149941814) 1832971548       54 2020-10-14 18:03:43.000000 xicsrt-0.8.7/xicsrt/objects/__init__.py
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.273460 xicsrt-0.8.7/xicsrt/optics/
--rw-r--r--   0 npablant (149941814) 1832971548     6844 2023-03-08 14:00:09.000000 xicsrt-0.8.7/xicsrt/optics/_InteractCrystal.py
--rw-r--r--   0 npablant (149941814) 1832971548     1085 2022-03-15 19:31:44.000000 xicsrt-0.8.7/xicsrt/optics/_InteractMirror.py
--rw-r--r--   0 npablant (149941814) 1832971548     5512 2023-03-08 14:34:28.000000 xicsrt-0.8.7/xicsrt/optics/_InteractMosaicCrystal.py
--rw-r--r--   0 npablant (149941814) 1832971548      474 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_InteractNone.py
--rw-r--r--   0 npablant (149941814) 1832971548     1060 2021-11-24 00:54:59.000000 xicsrt-0.8.7/xicsrt/optics/_InteractObject.py
--rw-r--r--   0 npablant (149941814) 1832971548    16320 2023-02-09 18:54:05.000000 xicsrt-0.8.7/xicsrt/optics/_ShapeMesh.py
--rw-r--r--   0 npablant (149941814) 1832971548     3065 2022-03-15 19:31:44.000000 xicsrt-0.8.7/xicsrt/optics/_ShapeMeshSphere.py
--rw-r--r--   0 npablant (149941814) 1832971548     6524 2021-10-28 17:18:05.000000 xicsrt-0.8.7/xicsrt/optics/_ShapeMeshTorus.py
--rw-r--r--   0 npablant (149941814) 1832971548     2493 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_ShapeObject.py
--rw-r--r--   0 npablant (149941814) 1832971548     1755 2022-01-13 02:02:40.000000 xicsrt-0.8.7/xicsrt/optics/_ShapePlane.py
--rw-r--r--   0 npablant (149941814) 1832971548     3655 2023-02-27 22:56:39.000000 xicsrt-0.8.7/xicsrt/optics/_ShapeSphere.py
--rw-r--r--   0 npablant (149941814) 1832971548    11512 2022-03-15 19:31:44.000000 xicsrt-0.8.7/xicsrt/optics/_TraceObject.py
--rw-r--r--   0 npablant (149941814) 1832971548      615 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticAperture.py
--rw-r--r--   0 npablant (149941814) 1832971548      661 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticDetector.py
--rw-r--r--   0 npablant (149941814) 1832971548      434 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticMeshCrystal.py
--rw-r--r--   0 npablant (149941814) 1832971548      436 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticMeshMirror.py
--rw-r--r--   0 npablant (149941814) 1832971548      471 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticMeshMosaicCrystal.py
--rw-r--r--   0 npablant (149941814) 1832971548     1154 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticMeshSphericalCrystal.py
--rw-r--r--   0 npablant (149941814) 1832971548     1145 2021-10-28 17:18:05.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticMeshToroidalCrystal.py
--rw-r--r--   0 npablant (149941814) 1832971548      444 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticPlanarCrystal.py
--rw-r--r--   0 npablant (149941814) 1832971548      441 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticPlanarMirror.py
--rw-r--r--   0 npablant (149941814) 1832971548      476 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticPlanarMosaicCrystal.py
--rw-r--r--   0 npablant (149941814) 1832971548      451 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticSphericalCrystal.py
--rw-r--r--   0 npablant (149941814) 1832971548      453 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticSphericalMirror.py
--rw-r--r--   0 npablant (149941814) 1832971548      485 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticSphericalMosaicCrystal.py
--rw-r--r--   0 npablant (149941814) 1832971548      118 2021-06-22 02:32:10.000000 xicsrt-0.8.7/xicsrt/optics/__init__.py
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.275411 xicsrt-0.8.7/xicsrt/sources/
--rw-r--r--   0 npablant (149941814) 1832971548      927 2021-07-13 18:33:20.000000 xicsrt-0.8.7/xicsrt/sources/_XicsrtPlasmaCubic.py
--rw-r--r--   0 npablant (149941814) 1832971548     2094 2021-07-13 18:33:20.000000 xicsrt-0.8.7/xicsrt/sources/_XicsrtPlasmaCylindrical.py
--rw-r--r--   0 npablant (149941814) 1832971548    16917 2023-02-09 18:54:05.000000 xicsrt-0.8.7/xicsrt/sources/_XicsrtPlasmaGeneric.py
--rw-r--r--   0 npablant (149941814) 1832971548     2807 2021-10-22 18:46:14.000000 xicsrt-0.8.7/xicsrt/sources/_XicsrtPlasmaToroidal.py
--rw-r--r--   0 npablant (149941814) 1832971548     1338 2021-07-10 01:56:11.000000 xicsrt-0.8.7/xicsrt/sources/_XicsrtPlasmaToroidalDatafile.py
--rw-r--r--   0 npablant (149941814) 1832971548     1588 2021-07-10 01:56:11.000000 xicsrt-0.8.7/xicsrt/sources/_XicsrtSourceDirected.py
--rw-r--r--   0 npablant (149941814) 1832971548     1434 2021-08-03 19:49:51.000000 xicsrt-0.8.7/xicsrt/sources/_XicsrtSourceFocused.py
--rw-r--r--   0 npablant (149941814) 1832971548    16222 2023-02-09 18:54:05.000000 xicsrt-0.8.7/xicsrt/sources/_XicsrtSourceGeneric.py
--rw-r--r--   0 npablant (149941814) 1832971548      119 2021-06-22 02:32:10.000000 xicsrt-0.8.7/xicsrt/sources/__init__.py
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.283336 xicsrt-0.8.7/xicsrt/tools/
--rw-r--r--   0 npablant (149941814) 1832971548      126 2020-10-14 18:03:43.000000 xicsrt-0.8.7/xicsrt/tools/__init__.py
--rw-r--r--   0 npablant (149941814) 1832971548     5179 2021-07-13 18:33:20.000000 xicsrt-0.8.7/xicsrt/tools/xicsrt_aperture.py
--rw-r--r--   0 npablant (149941814) 1832971548     3221 2021-08-03 19:49:51.000000 xicsrt-0.8.7/xicsrt/tools/xicsrt_bragg.py
--rw-r--r--   0 npablant (149941814) 1832971548     3943 2022-03-15 19:31:44.000000 xicsrt-0.8.7/xicsrt/tools/xicsrt_doc.py
--rw-r--r--   0 npablant (149941814) 1832971548    59887 2022-03-11 17:48:45.000000 xicsrt-0.8.7/xicsrt/tools/xicsrt_fb8.py
--rw-r--r--   0 npablant (149941814) 1832971548     9352 2023-02-09 18:54:05.000000 xicsrt-0.8.7/xicsrt/tools/xicsrt_math.py
--rw-r--r--   0 npablant (149941814) 1832971548     3251 2021-07-13 18:33:20.000000 xicsrt-0.8.7/xicsrt/tools/xicsrt_math_jax.py
--rw-r--r--   0 npablant (149941814) 1832971548     3592 2021-07-21 02:18:26.000000 xicsrt-0.8.7/xicsrt/tools/xicsrt_misc.py
--rw-r--r--   0 npablant (149941814) 1832971548      525 2023-02-09 18:54:05.000000 xicsrt-0.8.7/xicsrt/tools/xicsrt_physics.py
--rw-r--r--   0 npablant (149941814) 1832971548    11674 2022-05-20 19:28:21.000000 xicsrt-0.8.7/xicsrt/tools/xicsrt_spread.py
--rw-r--r--   0 npablant (149941814) 1832971548      781 2021-01-22 22:24:45.000000 xicsrt-0.8.7/xicsrt/tools/xicsrt_string.py
--rw-r--r--   0 npablant (149941814) 1832971548     4330 2022-03-15 19:31:44.000000 xicsrt-0.8.7/xicsrt/tools/xicsrt_voigt.py
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.284987 xicsrt-0.8.7/xicsrt/util/
--rw-r--r--   0 npablant (149941814) 1832971548      419 2021-01-22 22:24:45.000000 xicsrt-0.8.7/xicsrt/util/__init__.py
--rw-r--r--   0 npablant (149941814) 1832971548     6582 2020-10-01 01:19:06.000000 xicsrt-0.8.7/xicsrt/util/mircolor.py
--rw-r--r--   0 npablant (149941814) 1832971548    10815 2021-08-03 19:49:51.000000 xicsrt-0.8.7/xicsrt/util/mirhdf5.py
--rw-r--r--   0 npablant (149941814) 1832971548      628 2021-08-03 19:49:51.000000 xicsrt-0.8.7/xicsrt/util/mirlogging.py
--rw-r--r--   0 npablant (149941814) 1832971548    11657 2022-05-20 19:28:21.000000 xicsrt-0.8.7/xicsrt/util/mirplot.py
--rw-r--r--   0 npablant (149941814) 1832971548     2679 2021-08-03 19:49:51.000000 xicsrt-0.8.7/xicsrt/util/profiler.py
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.286287 xicsrt-0.8.7/xicsrt/visual/
--rw-r--r--   0 npablant (149941814) 1832971548       76 2020-10-14 18:03:43.000000 xicsrt-0.8.7/xicsrt/visual/__init__.py
--rw-r--r--   0 npablant (149941814) 1832971548     7486 2022-05-20 19:28:21.000000 xicsrt-0.8.7/xicsrt/visual/detview.py
--rw-r--r--   0 npablant (149941814) 1832971548    13255 2022-05-20 19:28:21.000000 xicsrt-0.8.7/xicsrt/visual/xicsrt_2d__matplotlib.py
--rw-r--r--   0 npablant (149941814) 1832971548    12232 2021-07-10 01:56:10.000000 xicsrt-0.8.7/xicsrt/visual/xicsrt_3d__ipyvolume.py
--rw-r--r--   0 npablant (149941814) 1832971548    11807 2021-10-28 16:30:58.000000 xicsrt-0.8.7/xicsrt/visual/xicsrt_3d__plotly.py
--rw-r--r--   0 npablant (149941814) 1832971548    13149 2022-05-20 19:28:21.000000 xicsrt-0.8.7/xicsrt/xicsrt_config.py
--rw-r--r--   0 npablant (149941814) 1832971548     6497 2023-02-09 18:54:05.000000 xicsrt-0.8.7/xicsrt/xicsrt_io.py
--rw-r--r--   0 npablant (149941814) 1832971548     2770 2021-08-03 19:49:51.000000 xicsrt-0.8.7/xicsrt/xicsrt_multiprocessing.py
--rw-r--r--   0 npablant (149941814) 1832971548     1345 2021-07-13 18:33:20.000000 xicsrt-0.8.7/xicsrt/xicsrt_public.py
--rw-r--r--   0 npablant (149941814) 1832971548    13679 2023-02-09 18:54:05.000000 xicsrt-0.8.7/xicsrt/xicsrt_raytrace.py
-drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-03-08 14:39:10.266902 xicsrt-0.8.7/xicsrt.egg-info/
--rw-r--r--   0 npablant (149941814) 1832971548     2583 2023-03-08 14:39:10.000000 xicsrt-0.8.7/xicsrt.egg-info/PKG-INFO
--rw-r--r--   0 npablant (149941814) 1832971548     2880 2023-03-08 14:39:10.000000 xicsrt-0.8.7/xicsrt.egg-info/SOURCES.txt
--rw-r--r--   0 npablant (149941814) 1832971548        1 2023-03-08 14:39:10.000000 xicsrt-0.8.7/xicsrt.egg-info/dependency_links.txt
--rw-r--r--   0 npablant (149941814) 1832971548       47 2023-03-08 14:39:10.000000 xicsrt-0.8.7/xicsrt.egg-info/entry_points.txt
--rw-r--r--   0 npablant (149941814) 1832971548       24 2023-03-08 14:39:10.000000 xicsrt-0.8.7/xicsrt.egg-info/requires.txt
--rw-r--r--   0 npablant (149941814) 1832971548       16 2023-03-08 14:39:10.000000 xicsrt-0.8.7/xicsrt.egg-info/top_level.txt
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.872691 xicsrt-0.8.8/
+-rw-r--r--   0 npablant (149941814) 1832971548      495 2021-08-03 19:49:51.000000 xicsrt-0.8.8/AUTHORS
+-rw-r--r--   0 npablant (149941814) 1832971548     1120 2021-10-28 17:18:05.000000 xicsrt-0.8.8/LICENSE
+-rw-r--r--   0 npablant (149941814) 1832971548     2583 2023-05-02 19:46:28.872508 xicsrt-0.8.8/PKG-INFO
+-rw-r--r--   0 npablant (149941814) 1832971548     1961 2021-07-13 18:33:20.000000 xicsrt-0.8.8/README.md
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.818789 xicsrt-0.8.8/examples/
+-rw-r--r--   0 npablant (149941814) 1832971548      180 2020-10-14 18:03:43.000000 xicsrt-0.8.8/examples/__init__.py
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.819390 xicsrt-0.8.8/examples/example_00/
+-rw-r--r--   0 npablant (149941814) 1832971548        0 2020-10-14 18:03:43.000000 xicsrt-0.8.8/examples/example_00/__init__.py
+-rw-r--r--   0 npablant (149941814) 1832971548     2745 2021-10-28 16:30:58.000000 xicsrt-0.8.8/examples/example_00/example_00.py
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.819993 xicsrt-0.8.8/examples/example_01/
+-rw-r--r--   0 npablant (149941814) 1832971548        0 2020-10-14 18:03:43.000000 xicsrt-0.8.8/examples/example_01/__init__.py
+-rw-r--r--   0 npablant (149941814) 1832971548     2032 2021-10-28 16:30:58.000000 xicsrt-0.8.8/examples/example_01/example_01.py
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.820413 xicsrt-0.8.8/examples/example_02/
+-rw-r--r--   0 npablant (149941814) 1832971548        0 2021-10-28 16:30:58.000000 xicsrt-0.8.8/examples/example_02/__init__.py
+-rw-r--r--   0 npablant (149941814) 1832971548     1869 2021-10-28 16:30:58.000000 xicsrt-0.8.8/examples/example_02/example_02.py
+-rw-r--r--   0 npablant (149941814) 1832971548       38 2023-05-02 19:46:28.872747 xicsrt-0.8.8/setup.cfg
+-rw-r--r--   0 npablant (149941814) 1832971548     1568 2021-08-03 19:49:51.000000 xicsrt-0.8.8/setup.py
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.823044 xicsrt-0.8.8/xicsrt/
+-rw-r--r--   0 npablant (149941814) 1832971548      376 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/__init__.py
+-rw-r--r--   0 npablant (149941814) 1832971548     4230 2021-08-10 19:43:11.000000 xicsrt-0.8.8/xicsrt/__main__.py
+-rw-r--r--   0 npablant (149941814) 1832971548      956 2023-05-02 19:45:40.000000 xicsrt-0.8.8/xicsrt/_version.py
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.832419 xicsrt-0.8.8/xicsrt/filters/
+-rw-r--r--   0 npablant (149941814) 1832971548      672 2021-07-10 01:56:10.000000 xicsrt-0.8.8/xicsrt/filters/_XicsrtBundleFilter.py
+-rw-r--r--   0 npablant (149941814) 1832971548     1529 2021-07-10 01:56:11.000000 xicsrt-0.8.8/xicsrt/filters/_XicsrtBundleFilterSightline.py
+-rw-r--r--   0 npablant (149941814) 1832971548      119 2021-06-22 02:32:10.000000 xicsrt-0.8.8/xicsrt/filters/__init__.py
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.835846 xicsrt-0.8.8/xicsrt/objects/
+-rw-r--r--   0 npablant (149941814) 1832971548     2325 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/objects/_ConfigObject.py
+-rw-r--r--   0 npablant (149941814) 1832971548     6957 2021-08-03 19:49:51.000000 xicsrt-0.8.8/xicsrt/objects/_Dispatcher.py
+-rw-r--r--   0 npablant (149941814) 1832971548     5747 2021-10-28 17:18:05.000000 xicsrt-0.8.8/xicsrt/objects/_GeometryObject.py
+-rw-r--r--   0 npablant (149941814) 1832971548     2957 2021-07-13 18:33:20.000000 xicsrt-0.8.8/xicsrt/objects/_RayArray.py
+-rw-r--r--   0 npablant (149941814) 1832971548       54 2020-10-14 18:03:43.000000 xicsrt-0.8.8/xicsrt/objects/__init__.py
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.845852 xicsrt-0.8.8/xicsrt/optics/
+-rw-r--r--   0 npablant (149941814) 1832971548     6844 2023-03-08 14:39:53.000000 xicsrt-0.8.8/xicsrt/optics/_InteractCrystal.py
+-rw-r--r--   0 npablant (149941814) 1832971548     1085 2022-03-15 19:31:44.000000 xicsrt-0.8.8/xicsrt/optics/_InteractMirror.py
+-rw-r--r--   0 npablant (149941814) 1832971548     5512 2023-03-08 14:39:53.000000 xicsrt-0.8.8/xicsrt/optics/_InteractMosaicCrystal.py
+-rw-r--r--   0 npablant (149941814) 1832971548      474 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_InteractNone.py
+-rw-r--r--   0 npablant (149941814) 1832971548     1060 2021-11-24 00:54:59.000000 xicsrt-0.8.8/xicsrt/optics/_InteractObject.py
+-rw-r--r--   0 npablant (149941814) 1832971548    16330 2023-05-02 19:45:40.000000 xicsrt-0.8.8/xicsrt/optics/_ShapeMesh.py
+-rw-r--r--   0 npablant (149941814) 1832971548     3065 2022-03-15 19:31:44.000000 xicsrt-0.8.8/xicsrt/optics/_ShapeMeshSphere.py
+-rw-r--r--   0 npablant (149941814) 1832971548     6524 2021-10-28 17:18:05.000000 xicsrt-0.8.8/xicsrt/optics/_ShapeMeshTorus.py
+-rw-r--r--   0 npablant (149941814) 1832971548     2493 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_ShapeObject.py
+-rw-r--r--   0 npablant (149941814) 1832971548     1755 2022-01-13 02:02:40.000000 xicsrt-0.8.8/xicsrt/optics/_ShapePlane.py
+-rw-r--r--   0 npablant (149941814) 1832971548     3655 2023-02-27 22:56:39.000000 xicsrt-0.8.8/xicsrt/optics/_ShapeSphere.py
+-rw-r--r--   0 npablant (149941814) 1832971548    11512 2022-03-15 19:31:44.000000 xicsrt-0.8.8/xicsrt/optics/_TraceObject.py
+-rw-r--r--   0 npablant (149941814) 1832971548      615 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticAperture.py
+-rw-r--r--   0 npablant (149941814) 1832971548      661 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticDetector.py
+-rw-r--r--   0 npablant (149941814) 1832971548      434 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticMeshCrystal.py
+-rw-r--r--   0 npablant (149941814) 1832971548      436 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticMeshMirror.py
+-rw-r--r--   0 npablant (149941814) 1832971548      471 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticMeshMosaicCrystal.py
+-rw-r--r--   0 npablant (149941814) 1832971548     1154 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticMeshSphericalCrystal.py
+-rw-r--r--   0 npablant (149941814) 1832971548     1145 2021-10-28 17:18:05.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticMeshToroidalCrystal.py
+-rw-r--r--   0 npablant (149941814) 1832971548      444 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticPlanarCrystal.py
+-rw-r--r--   0 npablant (149941814) 1832971548      441 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticPlanarMirror.py
+-rw-r--r--   0 npablant (149941814) 1832971548      476 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticPlanarMosaicCrystal.py
+-rw-r--r--   0 npablant (149941814) 1832971548      451 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticSphericalCrystal.py
+-rw-r--r--   0 npablant (149941814) 1832971548      453 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticSphericalMirror.py
+-rw-r--r--   0 npablant (149941814) 1832971548      485 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticSphericalMosaicCrystal.py
+-rw-r--r--   0 npablant (149941814) 1832971548      118 2021-06-22 02:32:10.000000 xicsrt-0.8.8/xicsrt/optics/__init__.py
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.851632 xicsrt-0.8.8/xicsrt/sources/
+-rw-r--r--   0 npablant (149941814) 1832971548      927 2021-07-13 18:33:20.000000 xicsrt-0.8.8/xicsrt/sources/_XicsrtPlasmaCubic.py
+-rw-r--r--   0 npablant (149941814) 1832971548     2094 2021-07-13 18:33:20.000000 xicsrt-0.8.8/xicsrt/sources/_XicsrtPlasmaCylindrical.py
+-rw-r--r--   0 npablant (149941814) 1832971548    16914 2023-05-02 19:45:40.000000 xicsrt-0.8.8/xicsrt/sources/_XicsrtPlasmaGeneric.py
+-rw-r--r--   0 npablant (149941814) 1832971548     2807 2021-10-22 18:46:14.000000 xicsrt-0.8.8/xicsrt/sources/_XicsrtPlasmaToroidal.py
+-rw-r--r--   0 npablant (149941814) 1832971548     1338 2021-07-10 01:56:11.000000 xicsrt-0.8.8/xicsrt/sources/_XicsrtPlasmaToroidalDatafile.py
+-rw-r--r--   0 npablant (149941814) 1832971548     1588 2021-07-10 01:56:11.000000 xicsrt-0.8.8/xicsrt/sources/_XicsrtSourceDirected.py
+-rw-r--r--   0 npablant (149941814) 1832971548     1434 2021-08-03 19:49:51.000000 xicsrt-0.8.8/xicsrt/sources/_XicsrtSourceFocused.py
+-rw-r--r--   0 npablant (149941814) 1832971548    16222 2023-02-09 18:54:05.000000 xicsrt-0.8.8/xicsrt/sources/_XicsrtSourceGeneric.py
+-rw-r--r--   0 npablant (149941814) 1832971548      119 2021-06-22 02:32:10.000000 xicsrt-0.8.8/xicsrt/sources/__init__.py
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.863929 xicsrt-0.8.8/xicsrt/tools/
+-rw-r--r--   0 npablant (149941814) 1832971548      126 2020-10-14 18:03:43.000000 xicsrt-0.8.8/xicsrt/tools/__init__.py
+-rw-r--r--   0 npablant (149941814) 1832971548     5179 2021-07-13 18:33:20.000000 xicsrt-0.8.8/xicsrt/tools/xicsrt_aperture.py
+-rw-r--r--   0 npablant (149941814) 1832971548     3221 2021-08-03 19:49:51.000000 xicsrt-0.8.8/xicsrt/tools/xicsrt_bragg.py
+-rw-r--r--   0 npablant (149941814) 1832971548     3943 2022-03-15 19:31:44.000000 xicsrt-0.8.8/xicsrt/tools/xicsrt_doc.py
+-rw-r--r--   0 npablant (149941814) 1832971548    59887 2022-03-11 17:48:45.000000 xicsrt-0.8.8/xicsrt/tools/xicsrt_fb8.py
+-rw-r--r--   0 npablant (149941814) 1832971548     9352 2023-02-09 18:54:05.000000 xicsrt-0.8.8/xicsrt/tools/xicsrt_math.py
+-rw-r--r--   0 npablant (149941814) 1832971548     3251 2021-07-13 18:33:20.000000 xicsrt-0.8.8/xicsrt/tools/xicsrt_math_jax.py
+-rw-r--r--   0 npablant (149941814) 1832971548     3592 2021-07-21 02:18:26.000000 xicsrt-0.8.8/xicsrt/tools/xicsrt_misc.py
+-rw-r--r--   0 npablant (149941814) 1832971548      525 2023-02-09 18:54:05.000000 xicsrt-0.8.8/xicsrt/tools/xicsrt_physics.py
+-rw-r--r--   0 npablant (149941814) 1832971548    11674 2022-05-20 19:28:21.000000 xicsrt-0.8.8/xicsrt/tools/xicsrt_spread.py
+-rw-r--r--   0 npablant (149941814) 1832971548      781 2021-01-22 22:24:45.000000 xicsrt-0.8.8/xicsrt/tools/xicsrt_string.py
+-rw-r--r--   0 npablant (149941814) 1832971548     4330 2022-03-15 19:31:44.000000 xicsrt-0.8.8/xicsrt/tools/xicsrt_voigt.py
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.870482 xicsrt-0.8.8/xicsrt/util/
+-rw-r--r--   0 npablant (149941814) 1832971548      419 2021-01-22 22:24:45.000000 xicsrt-0.8.8/xicsrt/util/__init__.py
+-rw-r--r--   0 npablant (149941814) 1832971548     6582 2020-10-01 01:19:06.000000 xicsrt-0.8.8/xicsrt/util/mircolor.py
+-rw-r--r--   0 npablant (149941814) 1832971548    10815 2021-08-03 19:49:51.000000 xicsrt-0.8.8/xicsrt/util/mirhdf5.py
+-rw-r--r--   0 npablant (149941814) 1832971548      628 2021-08-03 19:49:51.000000 xicsrt-0.8.8/xicsrt/util/mirlogging.py
+-rw-r--r--   0 npablant (149941814) 1832971548    11657 2022-05-20 19:28:21.000000 xicsrt-0.8.8/xicsrt/util/mirplot.py
+-rw-r--r--   0 npablant (149941814) 1832971548     2679 2021-08-03 19:49:51.000000 xicsrt-0.8.8/xicsrt/util/profiler.py
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.872115 xicsrt-0.8.8/xicsrt/visual/
+-rw-r--r--   0 npablant (149941814) 1832971548       76 2020-10-14 18:03:43.000000 xicsrt-0.8.8/xicsrt/visual/__init__.py
+-rw-r--r--   0 npablant (149941814) 1832971548     7486 2022-05-20 19:28:21.000000 xicsrt-0.8.8/xicsrt/visual/detview.py
+-rw-r--r--   0 npablant (149941814) 1832971548    13255 2022-05-20 19:28:21.000000 xicsrt-0.8.8/xicsrt/visual/xicsrt_2d__matplotlib.py
+-rw-r--r--   0 npablant (149941814) 1832971548    12232 2021-07-10 01:56:10.000000 xicsrt-0.8.8/xicsrt/visual/xicsrt_3d__ipyvolume.py
+-rw-r--r--   0 npablant (149941814) 1832971548    11807 2021-10-28 16:30:58.000000 xicsrt-0.8.8/xicsrt/visual/xicsrt_3d__plotly.py
+-rw-r--r--   0 npablant (149941814) 1832971548    13149 2022-05-20 19:28:21.000000 xicsrt-0.8.8/xicsrt/xicsrt_config.py
+-rw-r--r--   0 npablant (149941814) 1832971548     6497 2023-02-09 18:54:05.000000 xicsrt-0.8.8/xicsrt/xicsrt_io.py
+-rw-r--r--   0 npablant (149941814) 1832971548     2770 2021-08-03 19:49:51.000000 xicsrt-0.8.8/xicsrt/xicsrt_multiprocessing.py
+-rw-r--r--   0 npablant (149941814) 1832971548     1345 2021-07-13 18:33:20.000000 xicsrt-0.8.8/xicsrt/xicsrt_public.py
+-rw-r--r--   0 npablant (149941814) 1832971548    13679 2023-02-09 18:54:05.000000 xicsrt-0.8.8/xicsrt/xicsrt_raytrace.py
+drwxr-xr-x   0 npablant (149941814) 1832971548        0 2023-05-02 19:46:28.831575 xicsrt-0.8.8/xicsrt.egg-info/
+-rw-r--r--   0 npablant (149941814) 1832971548     2583 2023-05-02 19:46:28.000000 xicsrt-0.8.8/xicsrt.egg-info/PKG-INFO
+-rw-r--r--   0 npablant (149941814) 1832971548     2880 2023-05-02 19:46:28.000000 xicsrt-0.8.8/xicsrt.egg-info/SOURCES.txt
+-rw-r--r--   0 npablant (149941814) 1832971548        1 2023-05-02 19:46:28.000000 xicsrt-0.8.8/xicsrt.egg-info/dependency_links.txt
+-rw-r--r--   0 npablant (149941814) 1832971548       47 2023-05-02 19:46:28.000000 xicsrt-0.8.8/xicsrt.egg-info/entry_points.txt
+-rw-r--r--   0 npablant (149941814) 1832971548       24 2023-05-02 19:46:28.000000 xicsrt-0.8.8/xicsrt.egg-info/requires.txt
+-rw-r--r--   0 npablant (149941814) 1832971548       16 2023-05-02 19:46:28.000000 xicsrt-0.8.8/xicsrt.egg-info/top_level.txt
```

### Comparing `xicsrt-0.8.7/LICENSE` & `xicsrt-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/PKG-INFO` & `xicsrt-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xicsrt
-Version: 0.8.7
+Version: 0.8.8
 Summary: A photon based raytracing application written in Python.
 Home-page: https://github.com/PrincetonUniversity/xicsrt
 Author: Novimir Antoniuk Pablant
 Author-email: npablant@pppl.gov
 Maintainer: Novimir Antoniuk Pablant
 Maintainer-email: npablant@pppl.gov
 License: MIT
```

### Comparing `xicsrt-0.8.7/README.md` & `xicsrt-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/examples/example_00/example_00.py` & `xicsrt-0.8.8/examples/example_00/example_00.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/examples/example_01/example_01.py` & `xicsrt-0.8.8/examples/example_01/example_01.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/examples/example_02/example_02.py` & `xicsrt-0.8.8/examples/example_02/example_02.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/setup.py` & `xicsrt-0.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/__main__.py` & `xicsrt-0.8.8/xicsrt/__main__.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/_version.py` & `xicsrt-0.8.8/xicsrt/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   - Old config files can no longer be loaded without conversion.
   - New output dictionaries may break existing external code.
 
 revision:
   - New release that does not break any compatibility.
 """
 
-__version__="0.8.7"
+__version__="0.8.8"
 
 from packaging import version
 from xicsrt.util import mirlogging
 log = mirlogging.getLogger('xicsrt')
 
 def warn_version(v_string):
     v_input = version.parse(v_string)
```

### Comparing `xicsrt-0.8.7/xicsrt/filters/_XicsrtBundleFilter.py` & `xicsrt-0.8.8/xicsrt/filters/_XicsrtBundleFilter.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/filters/_XicsrtBundleFilterSightline.py` & `xicsrt-0.8.8/xicsrt/filters/_XicsrtBundleFilterSightline.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/objects/_ConfigObject.py` & `xicsrt-0.8.8/xicsrt/objects/_ConfigObject.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/objects/_Dispatcher.py` & `xicsrt-0.8.8/xicsrt/objects/_Dispatcher.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/objects/_GeometryObject.py` & `xicsrt-0.8.8/xicsrt/objects/_GeometryObject.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/objects/_RayArray.py` & `xicsrt-0.8.8/xicsrt/objects/_RayArray.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_InteractCrystal.py` & `xicsrt-0.8.8/xicsrt/optics/_InteractCrystal.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_InteractMirror.py` & `xicsrt-0.8.8/xicsrt/optics/_InteractMirror.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_InteractMosaicCrystal.py` & `xicsrt-0.8.8/xicsrt/optics/_InteractMosaicCrystal.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_InteractObject.py` & `xicsrt-0.8.8/xicsrt/optics/_InteractObject.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_ShapeMesh.py` & `xicsrt-0.8.8/xicsrt/optics/_ShapeMesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
         p0 = mesh['points'][mesh['faces'][..., 0], :]
         p1 = mesh['points'][mesh['faces'][..., 1], :]
         p2 = mesh['points'][mesh['faces'][..., 2], :]
 
         epsilon = 1e-15
 
         num_rays = len(m)
-        hits = np.empty(num_rays, dtype=np.int)
+        hits = np.empty(num_rays, dtype=np.int64)
         m_temp = np.empty(num_rays, dtype=bool)
         m_temp_2 = np.zeros(num_rays, dtype=bool)
 
         for ii in range(mesh['faces'].shape[0]):
             m_temp[:] = m
             edge1 = p1[ii, :] - p0[ii, :]
             edge2 = p2[ii, :] - p0[ii, :]
@@ -348,15 +348,15 @@
         O = rays['origin']
         D = rays['direction']
 
         m =  mask.copy()
         X = np.full(D.shape, np.nan, dtype=np.float64)
 
         num_rays = len(m)
-        hits = np.empty(num_rays, dtype=np.int)
+        hits = np.empty(num_rays, dtype=np.int64)
         epsilon = 1e-15
 
         # Copying these makes the code easier to read,
         # but may increase memory usage for dense meshes.
         faces = mesh['faces'][faces_idx]
         p0 = mesh['points'][faces[..., 0], :]
         p1 = mesh['points'][faces[..., 1], :]
@@ -406,44 +406,44 @@
         return normals
 
     def mesh_get_index(self, hits, faces):
         """
         Match faces to face indexes, with a loop over faces.
         """
         profiler.start('mesh_get_index')
-        idx_hits = np.empty(hits.shape[0], dtype=np.int)
+        idx_hits = np.empty(hits.shape[0], dtype=np.int32)
         for ii, ff in enumerate(faces):
             m_temp = np.all(np.equal(ff, hits), axis=1)
             idx_hits[m_temp] = ii
         profiler.stop('mesh_get_index')
         return idx_hits
 
     def find_point_faces(self, p_idx, faces, mask=None):
         """
         Find all of the the faces that include a given mesh point.
         """
         profiler.start('find_point_faces')
         if mask is None:
             mask = np.ones(p_idx.shape, dtype=np.bool_)
         m = mask
-        p_faces_idx = np.zeros((8, len(m)), dtype=np.int)
+        p_faces_idx = np.zeros((8, len(m)), dtype=np.int32)
         p_faces_mask = np.zeros((8, len(m)), dtype=np.bool_)
         for ii_p in p_idx:
             ii_f = np.nonzero(np.equal(faces, p_idx[ii_p]))[0]
             faces_num = len(ii_f)
             p_faces_idx[:faces_num, ii_p] = ii_f
             p_faces_mask[:faces_num, ii_p] = True
         profiler.stop('find_point_faces')
         return p_faces_idx, p_faces_mask
 
     def find_near_faces(self, X, mesh, mask):
         m = mask
         profiler.start('find_near_faces')
         idx = mesh['points_tree'].query(X[m])[1]
 
-        faces_idx = np.zeros((8, len(m)), dtype=np.int)
+        faces_idx = np.zeros((8, len(m)), dtype=np.int32)
         faces_mask = np.zeros((8, len(m)), dtype=np.bool_)
 
         faces_idx[:, m] = mesh['p_faces_idx'][:, idx]
         faces_mask[:, m] = mesh['p_faces_mask'][:, idx]
         profiler.stop('find_near_faces')
         return faces_idx, faces_mask
```

### Comparing `xicsrt-0.8.7/xicsrt/optics/_ShapeMeshSphere.py` & `xicsrt-0.8.8/xicsrt/optics/_ShapeMeshSphere.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_ShapeMeshTorus.py` & `xicsrt-0.8.8/xicsrt/optics/_ShapeMeshTorus.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_ShapeObject.py` & `xicsrt-0.8.8/xicsrt/optics/_ShapeObject.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_ShapePlane.py` & `xicsrt-0.8.8/xicsrt/optics/_ShapePlane.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_ShapeSphere.py` & `xicsrt-0.8.8/xicsrt/optics/_ShapeSphere.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_TraceObject.py` & `xicsrt-0.8.8/xicsrt/optics/_TraceObject.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticAperture.py` & `xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticAperture.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticDetector.py` & `xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticDetector.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticMeshSphericalCrystal.py` & `xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticMeshSphericalCrystal.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/optics/_XicsrtOpticMeshToroidalCrystal.py` & `xicsrt-0.8.8/xicsrt/optics/_XicsrtOpticMeshToroidalCrystal.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/sources/_XicsrtPlasmaCubic.py` & `xicsrt-0.8.8/xicsrt/sources/_XicsrtPlasmaCubic.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/sources/_XicsrtPlasmaCylindrical.py` & `xicsrt-0.8.8/xicsrt/sources/_XicsrtPlasmaCylindrical.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/sources/_XicsrtPlasmaGeneric.py` & `xicsrt-0.8.8/xicsrt/sources/_XicsrtPlasmaGeneric.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
             count_rays_in_bundle.append(len(bundled_rays['mask']))
 
             profiler.stop("Ray Bundle Generation")
 
         profiler.start('Ray Bundle Collection')
         # append bundled rays together to form a single ray dictionary.    
         # create the final ray dictionary
-        total_rays = np.int(np.sum(count_rays_in_bundle))
+        total_rays = int(np.sum(count_rays_in_bundle))
         rays                = dict()
         rays['origin']      = np.zeros((total_rays,3), dtype=np.float64)
         rays['direction']   = np.zeros((total_rays,3), dtype=np.float64)
         rays['wavelength']  = np.zeros((total_rays), dtype=np.float64)
         rays['weight']      = np.zeros((total_rays), dtype=np.float64)
         rays['mask']        = np.ones((total_rays), dtype=np.bool_)
```

### Comparing `xicsrt-0.8.7/xicsrt/sources/_XicsrtPlasmaToroidal.py` & `xicsrt-0.8.8/xicsrt/sources/_XicsrtPlasmaToroidal.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/sources/_XicsrtPlasmaToroidalDatafile.py` & `xicsrt-0.8.8/xicsrt/sources/_XicsrtPlasmaToroidalDatafile.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/sources/_XicsrtSourceDirected.py` & `xicsrt-0.8.8/xicsrt/sources/_XicsrtSourceDirected.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/sources/_XicsrtSourceFocused.py` & `xicsrt-0.8.8/xicsrt/sources/_XicsrtSourceFocused.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/sources/_XicsrtSourceGeneric.py` & `xicsrt-0.8.8/xicsrt/sources/_XicsrtSourceGeneric.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/tools/xicsrt_aperture.py` & `xicsrt-0.8.8/xicsrt/tools/xicsrt_aperture.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/tools/xicsrt_bragg.py` & `xicsrt-0.8.8/xicsrt/tools/xicsrt_bragg.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/tools/xicsrt_doc.py` & `xicsrt-0.8.8/xicsrt/tools/xicsrt_doc.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/tools/xicsrt_fb8.py` & `xicsrt-0.8.8/xicsrt/tools/xicsrt_fb8.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/tools/xicsrt_math.py` & `xicsrt-0.8.8/xicsrt/tools/xicsrt_math.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/tools/xicsrt_math_jax.py` & `xicsrt-0.8.8/xicsrt/tools/xicsrt_math_jax.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/tools/xicsrt_misc.py` & `xicsrt-0.8.8/xicsrt/tools/xicsrt_misc.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/tools/xicsrt_physics.py` & `xicsrt-0.8.8/xicsrt/tools/xicsrt_physics.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/tools/xicsrt_spread.py` & `xicsrt-0.8.8/xicsrt/tools/xicsrt_spread.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/tools/xicsrt_string.py` & `xicsrt-0.8.8/xicsrt/tools/xicsrt_string.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/tools/xicsrt_voigt.py` & `xicsrt-0.8.8/xicsrt/tools/xicsrt_voigt.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/util/mircolor.py` & `xicsrt-0.8.8/xicsrt/util/mircolor.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/util/mirhdf5.py` & `xicsrt-0.8.8/xicsrt/util/mirhdf5.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/util/mirlogging.py` & `xicsrt-0.8.8/xicsrt/util/mirlogging.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/util/mirplot.py` & `xicsrt-0.8.8/xicsrt/util/mirplot.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/util/profiler.py` & `xicsrt-0.8.8/xicsrt/util/profiler.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/visual/detview.py` & `xicsrt-0.8.8/xicsrt/visual/detview.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/visual/xicsrt_2d__matplotlib.py` & `xicsrt-0.8.8/xicsrt/visual/xicsrt_2d__matplotlib.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/visual/xicsrt_3d__ipyvolume.py` & `xicsrt-0.8.8/xicsrt/visual/xicsrt_3d__ipyvolume.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/visual/xicsrt_3d__plotly.py` & `xicsrt-0.8.8/xicsrt/visual/xicsrt_3d__plotly.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/xicsrt_config.py` & `xicsrt-0.8.8/xicsrt/xicsrt_config.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/xicsrt_io.py` & `xicsrt-0.8.8/xicsrt/xicsrt_io.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/xicsrt_multiprocessing.py` & `xicsrt-0.8.8/xicsrt/xicsrt_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/xicsrt_public.py` & `xicsrt-0.8.8/xicsrt/xicsrt_public.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt/xicsrt_raytrace.py` & `xicsrt-0.8.8/xicsrt/xicsrt_raytrace.py`

 * *Files identical despite different names*

### Comparing `xicsrt-0.8.7/xicsrt.egg-info/PKG-INFO` & `xicsrt-0.8.8/xicsrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xicsrt
-Version: 0.8.7
+Version: 0.8.8
 Summary: A photon based raytracing application written in Python.
 Home-page: https://github.com/PrincetonUniversity/xicsrt
 Author: Novimir Antoniuk Pablant
 Author-email: npablant@pppl.gov
 Maintainer: Novimir Antoniuk Pablant
 Maintainer-email: npablant@pppl.gov
 License: MIT
```

### Comparing `xicsrt-0.8.7/xicsrt.egg-info/SOURCES.txt` & `xicsrt-0.8.8/xicsrt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

