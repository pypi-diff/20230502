# Comparing `tmp/imod-0.8.0.tar.gz` & `tmp/imod-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imod-0.8.0.tar", last modified: Mon Oct 14 13:39:46 2019, max compression
+gzip compressed data, was "dist\imod-0.9.0.tar", last modified: Sun Jan 19 22:15:57 2020, max compression
```

## Comparing `imod-0.8.0.tar` & `imod-0.9.0.tar`

### file list

```diff
@@ -1,125 +1,246 @@
-drwxrwxrwx   0        0        0        0 2019-10-14 13:39:46.000000 imod-0.8.0/
-drwxrwxrwx   0        0        0        0 2019-10-14 13:39:46.000000 imod-0.8.0/imod/
-drwxrwxrwx   0        0        0        0 2019-10-14 13:39:46.000000 imod-0.8.0/imod/evaluate/
--rw-rw-rw-   0        0        0     7171 2019-10-01 09:40:59.000000 imod-0.8.0/imod/evaluate/budget.py
--rw-rw-rw-   0        0        0       45 2019-10-01 09:40:59.000000 imod-0.8.0/imod/evaluate/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-14 13:39:46.000000 imod-0.8.0/imod/flow/
--rw-rw-rw-   0        0        0     3391 2019-09-06 09:47:45.000000 imod-0.8.0/imod/flow/__init__.py
--rw-rw-rw-   0        0        0    35652 2019-09-06 10:53:10.000000 imod-0.8.0/imod/idf.py
--rw-rw-rw-   0        0        0    21333 2019-10-06 19:01:02.000000 imod-0.8.0/imod/ipf.py
-drwxrwxrwx   0        0        0        0 2019-10-14 13:39:46.000000 imod-0.8.0/imod/mf6/
--rw-rw-rw-   0        0        0      680 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/chd.py
--rw-rw-rw-   0        0        0     2910 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/dis.py
--rw-rw-rw-   0        0        0      899 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/drn.py
--rw-rw-rw-   0        0        0     1633 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/evt.py
--rw-rw-rw-   0        0        0      843 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/ghb.py
--rw-rw-rw-   0        0        0      603 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/ic.py
--rw-rw-rw-   0        0        0     6407 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/ims.py
--rw-rw-rw-   0        0        0     3791 2019-09-03 11:59:26.000000 imod-0.8.0/imod/mf6/model.py
--rw-rw-rw-   0        0        0     4029 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/npf.py
--rw-rw-rw-   0        0        0     1618 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/oc.py
--rw-rw-rw-   0        0        0     4696 2019-09-07 22:01:16.000000 imod-0.8.0/imod/mf6/out.py
--rw-rw-rw-   0        0        0     9668 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/pkgbase.py
--rw-rw-rw-   0        0        0      676 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/rch.py
--rw-rw-rw-   0        0        0      963 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/riv.py
--rw-rw-rw-   0        0        0     3360 2019-09-07 21:50:47.000000 imod-0.8.0/imod/mf6/simulation.py
--rw-rw-rw-   0        0        0     1230 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/sto.py
--rw-rw-rw-   0        0        0     1789 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/timedis.py
--rw-rw-rw-   0        0        0     1547 2019-10-14 12:31:54.000000 imod-0.8.0/imod/mf6/wel.py
--rw-rw-rw-   0        0        0      838 2019-09-03 11:59:26.000000 imod-0.8.0/imod/mf6/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-14 13:39:46.000000 imod-0.8.0/imod/prepare/
--rw-rw-rw-   0        0        0    14435 2019-10-14 11:52:26.000000 imod-0.8.0/imod/prepare/common.py
--rw-rw-rw-   0        0        0    17903 2019-10-01 09:40:59.000000 imod-0.8.0/imod/prepare/interpolate.py
--rw-rw-rw-   0        0        0     4804 2019-10-01 09:40:59.000000 imod-0.8.0/imod/prepare/layerregrid.py
--rw-rw-rw-   0        0        0    18870 2019-09-03 09:25:30.000000 imod-0.8.0/imod/prepare/pcg.py
--rw-rw-rw-   0        0        0    17865 2019-09-23 07:14:33.000000 imod-0.8.0/imod/prepare/regrid.py
--rw-rw-rw-   0        0        0     9832 2019-09-03 09:25:30.000000 imod-0.8.0/imod/prepare/reproject.py
--rw-rw-rw-   0        0        0    26335 2019-09-03 09:25:30.000000 imod-0.8.0/imod/prepare/spatial.py
--rw-rw-rw-   0        0        0     2805 2019-07-29 09:42:36.000000 imod-0.8.0/imod/prepare/subsoil.py
--rw-rw-rw-   0        0        0     3927 2019-07-23 15:11:12.000000 imod-0.8.0/imod/prepare/surface_water.py
--rw-rw-rw-   0        0        0     6583 2019-10-01 09:40:59.000000 imod-0.8.0/imod/prepare/voxelize.py
--rw-rw-rw-   0        0        0     1054 2019-09-03 09:25:30.000000 imod-0.8.0/imod/prepare/__init__.py
--rw-rw-rw-   0        0        0     9618 2019-10-14 09:31:43.000000 imod-0.8.0/imod/rasterio.py
--rw-rw-rw-   0        0        0    31123 2019-09-06 10:55:10.000000 imod-0.8.0/imod/run.py
-drwxrwxrwx   0        0        0        0 2019-10-14 13:39:46.000000 imod-0.8.0/imod/select/
--rw-rw-rw-   0        0        0    12726 2019-09-03 09:25:30.000000 imod-0.8.0/imod/select/cross_sections.py
--rw-rw-rw-   0        0        0     8105 2019-09-03 09:25:30.000000 imod-0.8.0/imod/select/points.py
--rw-rw-rw-   0        0        0      254 2019-07-23 15:11:12.000000 imod-0.8.0/imod/select/__init__.py
--rw-rw-rw-   0        0        0     6300 2019-07-23 15:11:12.000000 imod-0.8.0/imod/tec.py
-drwxrwxrwx   0        0        0        0 2019-10-14 13:39:46.000000 imod-0.8.0/imod/templates/
-drwxrwxrwx   0        0        0        0 2019-10-14 13:39:46.000000 imod-0.8.0/imod/templates/mf6/
--rw-rw-rw-   0        0        0     1111 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/exg-gwfgwf.j2
--rw-rw-rw-   0        0        0      744 2019-09-06 09:47:45.000000 imod-0.8.0/imod/templates/mf6/gwf-chd.j2
--rw-rw-rw-   0        0        0      818 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/gwf-dis.j2
--rw-rw-rw-   0        0        0     1015 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/gwf-disu.j2
--rw-rw-rw-   0        0        0      918 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/gwf-disv.j2
--rw-rw-rw-   0        0        0      792 2019-09-05 16:18:47.000000 imod-0.8.0/imod/templates/mf6/gwf-drn.j2
--rw-rw-rw-   0        0        0      895 2019-09-06 09:47:45.000000 imod-0.8.0/imod/templates/mf6/gwf-evt.j2
--rw-rw-rw-   0        0        0      718 2019-09-06 09:47:45.000000 imod-0.8.0/imod/templates/mf6/gwf-evta.j2
--rw-rw-rw-   0        0        0      792 2019-09-06 09:47:45.000000 imod-0.8.0/imod/templates/mf6/gwf-ghb.j2
--rw-rw-rw-   0        0        0      476 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/gwf-gnc.j2
--rw-rw-rw-   0        0        0      262 2019-09-06 09:47:45.000000 imod-0.8.0/imod/templates/mf6/gwf-hfb.j2
--rw-rw-rw-   0        0        0      168 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/gwf-ic.j2
--rw-rw-rw-   0        0        0     2221 2019-09-06 09:47:45.000000 imod-0.8.0/imod/templates/mf6/gwf-lak.j2
--rw-rw-rw-   0        0        0     1918 2019-09-06 09:47:45.000000 imod-0.8.0/imod/templates/mf6/gwf-maw.j2
--rw-rw-rw-   0        0        0      663 2019-09-06 09:47:45.000000 imod-0.8.0/imod/templates/mf6/gwf-mvr.j2
--rw-rw-rw-   0        0        0      487 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/gwf-nam.j2
--rw-rw-rw-   0        0        0     1845 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/gwf-npf.j2
--rw-rw-rw-   0        0        0      478 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/gwf-oc.j2
--rw-rw-rw-   0        0        0      802 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/gwf-rch.j2
--rw-rw-rw-   0        0        0      718 2019-09-06 09:47:45.000000 imod-0.8.0/imod/templates/mf6/gwf-rcha.j2
--rw-rw-rw-   0        0        0      792 2019-09-06 09:47:45.000000 imod-0.8.0/imod/templates/mf6/gwf-riv.j2
--rw-rw-rw-   0        0        0     1988 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/gwf-sfr.j2
--rw-rw-rw-   0        0        0      624 2019-09-06 09:47:45.000000 imod-0.8.0/imod/templates/mf6/gwf-sto.j2
--rw-rw-rw-   0        0        0     1715 2019-09-06 09:47:45.000000 imod-0.8.0/imod/templates/mf6/gwf-uzf.j2
--rw-rw-rw-   0        0        0      883 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/gwf-wel.j2
--rw-rw-rw-   0        0        0      856 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/sim-nam.j2
--rw-rw-rw-   0        0        0      371 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/sim-tdis.j2
--rw-rw-rw-   0        0        0     2368 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/sln-ims.j2
--rw-rw-rw-   0        0        0      271 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/utl-lak-tab.j2
--rw-rw-rw-   0        0        0      356 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/utl-obs.j2
--rw-rw-rw-   0        0        0      410 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/utl-tas.j2
--rw-rw-rw-   0        0        0      836 2019-09-03 11:59:26.000000 imod-0.8.0/imod/templates/mf6/utl-ts.j2
--rw-rw-rw-   0        0        0     1806 2019-06-18 09:29:11.000000 imod-0.8.0/imod/templates/runfile.j2
--rw-rw-rw-   0        0        0     8103 2019-06-18 09:29:11.000000 imod-0.8.0/imod/templates/seawat_runfile.j2
--rw-rw-rw-   0        0        0    14252 2019-10-14 11:52:26.000000 imod-0.8.0/imod/util.py
-drwxrwxrwx   0        0        0        0 2019-10-14 13:39:46.000000 imod-0.8.0/imod/visualize/
--rw-rw-rw-   0        0        0     1779 2019-10-06 19:01:02.000000 imod-0.8.0/imod/visualize/cross_sections.py
--rw-rw-rw-   0        0        0    10583 2019-10-05 18:36:19.000000 imod-0.8.0/imod/visualize/spatial.py
--rw-rw-rw-   0        0        0      456 2019-10-14 11:52:26.000000 imod-0.8.0/imod/visualize/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-14 13:39:46.000000 imod-0.8.0/imod/wq/
--rw-rw-rw-   0        0        0    21314 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/adv.py
--rw-rw-rw-   0        0        0     7195 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/bas.py
--rw-rw-rw-   0        0        0     7152 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/btn.py
--rw-rw-rw-   0        0        0     1553 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/chd.py
--rw-rw-rw-   0        0        0     8531 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/dis.py
--rw-rw-rw-   0        0        0     1598 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/drn.py
--rw-rw-rw-   0        0        0     3338 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/dsp.py
--rw-rw-rw-   0        0        0     2893 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/ghb.py
--rw-rw-rw-   0        0        0     8353 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/lpf.py
--rw-rw-rw-   0        0        0    19083 2019-10-05 18:36:19.000000 imod-0.8.0/imod/wq/model.py
--rw-rw-rw-   0        0        0     3532 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/oc.py
--rw-rw-rw-   0        0        0    15511 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/pkgbase.py
--rw-rw-rw-   0        0        0     3917 2019-07-29 09:42:37.000000 imod-0.8.0/imod/wq/pkggroup.py
--rw-rw-rw-   0        0        0     5393 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/rch.py
--rw-rw-rw-   0        0        0     3289 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/riv.py
--rw-rw-rw-   0        0        0    17208 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/slv.py
--rw-rw-rw-   0        0        0     3327 2019-06-20 06:37:31.000000 imod-0.8.0/imod/wq/timeutil.py
--rw-rw-rw-   0        0        0     6681 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/vdf.py
--rw-rw-rw-   0        0        0     6099 2019-10-14 12:31:54.000000 imod-0.8.0/imod/wq/wel.py
--rw-rw-rw-   0        0        0     1211 2019-09-23 07:14:33.000000 imod-0.8.0/imod/wq/__init__.py
--rw-rw-rw-   0        0        0      518 2019-10-14 13:39:46.000000 imod-0.8.0/imod/_version.py
--rw-rw-rw-   0        0        0     5287 2019-10-01 09:40:59.000000 imod-0.8.0/imod/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-14 13:39:46.000000 imod-0.8.0/imod.egg-info/
--rw-rw-rw-   0        0        0        1 2019-10-14 13:39:46.000000 imod-0.8.0/imod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4164 2019-10-14 13:39:46.000000 imod-0.8.0/imod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2019-10-14 13:39:46.000000 imod-0.8.0/imod.egg-info/requires.txt
--rw-rw-rw-   0        0        0     2496 2019-10-14 13:39:46.000000 imod-0.8.0/imod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        5 2019-10-14 13:39:46.000000 imod-0.8.0/imod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1081 2019-04-19 11:24:52.000000 imod-0.8.0/LICENSE
--rw-rw-rw-   0        0        0       86 2019-07-29 09:42:36.000000 imod-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4164 2019-10-14 13:39:46.000000 imod-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2821 2019-10-01 09:40:59.000000 imod-0.8.0/README.rst
--rw-rw-rw-   0        0        0      204 2019-10-14 13:39:46.000000 imod-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1935 2019-10-14 12:56:20.000000 imod-0.8.0/setup.py
--rw-rw-rw-   0        0        0    70636 2019-06-04 11:18:57.000000 imod-0.8.0/versioneer.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/
+-rw-rw-rw-   0        0        0       47 2019-10-17 19:38:59.000000 imod-0.9.0/.gitattributes
+-rw-rw-rw-   0        0        0     1598 2019-06-20 06:37:30.000000 imod-0.9.0/.gitignore
+-rw-rw-rw-   0        0        0      929 2020-01-19 12:10:15.000000 imod-0.9.0/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0     1081 2019-04-19 11:24:52.000000 imod-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0       37 2019-10-17 19:38:59.000000 imod-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4323 2020-01-19 22:15:57.000000 imod-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2953 2019-11-25 13:30:13.000000 imod-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/docs/
+-rw-rw-rw-   0        0        0      620 2019-04-11 12:02:20.000000 imod-0.9.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/docs/api/
+-rw-rw-rw-   0        0        0      197 2019-10-01 09:40:59.000000 imod-0.9.0/docs/api/evaluate.rst
+-rw-rw-rw-   0        0        0      187 2019-07-23 15:11:12.000000 imod-0.9.0/docs/api/flow.rst
+-rw-rw-rw-   0        0        0      142 2019-07-23 15:11:12.000000 imod-0.9.0/docs/api/idf.rst
+-rw-rw-rw-   0        0        0      142 2019-07-23 15:11:12.000000 imod-0.9.0/docs/api/ipf.rst
+-rw-rw-rw-   0        0        0      186 2019-09-03 11:59:26.000000 imod-0.9.0/docs/api/mf6.rst
+-rw-rw-rw-   0        0        0      192 2019-07-23 15:11:12.000000 imod-0.9.0/docs/api/prepare.rst
+-rw-rw-rw-   0        0        0      163 2019-07-23 15:11:12.000000 imod-0.9.0/docs/api/rasterio.rst
+-rw-rw-rw-   0        0        0      164 2019-07-23 15:11:12.000000 imod-0.9.0/docs/api/run.rst
+-rw-rw-rw-   0        0        0      209 2019-07-23 15:11:12.000000 imod-0.9.0/docs/api/select.rst
+-rw-rw-rw-   0        0        0      164 2019-07-23 15:11:12.000000 imod-0.9.0/docs/api/tec.rst
+-rw-rw-rw-   0        0        0      167 2019-07-23 15:11:12.000000 imod-0.9.0/docs/api/util.rst
+-rw-rw-rw-   0        0        0      192 2019-07-23 15:11:12.000000 imod-0.9.0/docs/api/visualize.rst
+-rw-rw-rw-   0        0        0      191 2019-07-23 15:11:12.000000 imod-0.9.0/docs/api/wq.rst
+-rw-rw-rw-   0        0        0      507 2019-10-01 09:40:59.000000 imod-0.9.0/docs/api.rst
+-rw-rw-rw-   0        0        0     7825 2020-01-19 22:12:59.000000 imod-0.9.0/docs/changelog.rst
+-rw-rw-rw-   0        0        0     5783 2019-10-17 19:38:59.000000 imod-0.9.0/docs/conf.py
+-rw-rw-rw-   0        0        0     5105 2019-10-14 13:36:20.000000 imod-0.9.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0      143 2019-06-20 06:37:30.000000 imod-0.9.0/docs/coordinates.rst
+-rw-rw-rw-   0        0        0       71 2019-06-20 06:37:30.000000 imod-0.9.0/docs/data-structures.rst
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/docs/examples/
+-rw-rw-rw-   0        0        0       75 2019-06-20 06:37:30.000000 imod-0.9.0/docs/examples/elder.rst
+-rw-rw-rw-   0        0        0      104 2019-06-20 06:37:30.000000 imod-0.9.0/docs/examples/freshwaterlens.rst
+-rw-rw-rw-   0        0        0       89 2019-06-20 06:37:30.000000 imod-0.9.0/docs/examples/henrycase.rst
+-rw-rw-rw-   0        0        0       89 2019-06-20 06:37:30.000000 imod-0.9.0/docs/examples/hydrocoin.rst
+-rw-rw-rw-   0        0        0      109 2019-06-20 06:37:30.000000 imod-0.9.0/docs/examples/saltwaterpocket.rst
+-rw-rw-rw-   0        0        0      121 2020-01-19 12:10:15.000000 imod-0.9.0/docs/examples/twri.rst
+-rw-rw-rw-   0        0        0      113 2019-06-20 06:37:30.000000 imod-0.9.0/docs/examples/verticalinterface.rst
+-rw-rw-rw-   0        0        0      581 2020-01-19 12:10:15.000000 imod-0.9.0/docs/examples.rst
+-rw-rw-rw-   0        0        0     3884 2020-01-19 22:12:59.000000 imod-0.9.0/docs/index.rst
+-rw-rw-rw-   0        0        0    12338 2019-07-23 15:11:12.000000 imod-0.9.0/docs/indexing.rst
+-rw-rw-rw-   0        0        0     8724 2019-07-23 15:11:12.000000 imod-0.9.0/docs/installation.rst
+-rw-rw-rw-   0        0        0      118 2019-06-20 06:37:30.000000 imod-0.9.0/docs/internals.rst
+-rwxrwxrwx   0        0        0      808 2019-04-11 12:02:20.000000 imod-0.9.0/docs/make.bat
+-rw-rw-rw-   0        0        0       69 2019-06-20 06:37:30.000000 imod-0.9.0/docs/model.rst
+-rw-rw-rw-   0        0        0     1901 2019-06-20 06:37:30.000000 imod-0.9.0/docs/overview.rst
+-rw-rw-rw-   0        0        0      118 2019-06-20 06:37:30.000000 imod-0.9.0/docs/post-processing.rst
+-rw-rw-rw-   0        0        0      184 2019-06-20 06:37:30.000000 imod-0.9.0/docs/regridding.rst
+-rw-rw-rw-   0        0        0      245 2019-06-20 06:37:30.000000 imod-0.9.0/docs/roadmap.rst
+-rw-rw-rw-   0        0        0      559 2019-10-17 19:38:59.000000 imod-0.9.0/environment.yml
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/examples/
+-rw-rw-rw-   0        0        0     6431 2019-09-07 21:50:47.000000 imod-0.9.0/examples/Brabant_steady-state.py
+-rw-rw-rw-   0        0        0     2939 2020-01-19 12:10:16.000000 imod-0.9.0/examples/Elder.py
+-rw-rw-rw-   0        0        0     2857 2019-09-07 21:50:47.000000 imod-0.9.0/examples/FreshwaterLens.py
+-rw-rw-rw-   0        0        0     2125 2019-09-07 21:50:47.000000 imod-0.9.0/examples/HenryCase.py
+-rw-rw-rw-   0        0        0     4912 2019-09-07 21:50:47.000000 imod-0.9.0/examples/Hydrocoin.py
+-rw-rw-rw-   0        0        0    11651 2019-09-07 21:50:47.000000 imod-0.9.0/examples/LHM_to_modflow6.py
+-rw-rw-rw-   0        0        0     2576 2020-01-19 12:10:16.000000 imod-0.9.0/examples/SaltwaterPocket.py
+-rw-rw-rw-   0        0        0    12673 2019-05-06 15:06:07.000000 imod-0.9.0/examples/SyntheticModel_Toth1963.ipynb
+-rw-rw-rw-   0        0        0     2805 2019-09-07 21:50:47.000000 imod-0.9.0/examples/VerticalInterface.py
+-rw-rw-rw-   0        0        0     6929 2019-05-06 15:06:10.000000 imod-0.9.0/examples/iMODSEAWAT_HenryCase.ipynb
+-rw-rw-rw-   0        0        0     3470 2020-01-19 12:10:16.000000 imod-0.9.0/examples/mf6_ex01_twri.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/imod/
+-rw-rw-rw-   0        0        0     5368 2019-10-17 19:38:59.000000 imod-0.9.0/imod/__init__.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/imod/array_io/
+-rw-rw-rw-   0        0        0       46 2019-10-25 15:36:01.000000 imod-0.9.0/imod/array_io/__init__.py
+-rw-rw-rw-   0        0        0    12662 2019-11-25 13:30:13.000000 imod-0.9.0/imod/array_io/reading.py
+-rw-rw-rw-   0        0        0     5218 2019-12-20 09:03:05.000000 imod-0.9.0/imod/array_io/writing.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/imod/evaluate/
+-rw-rw-rw-   0        0        0      157 2019-12-20 09:03:05.000000 imod-0.9.0/imod/evaluate/__init__.py
+-rw-rw-rw-   0        0        0     7171 2019-10-01 09:40:59.000000 imod-0.9.0/imod/evaluate/budget.py
+-rw-rw-rw-   0        0        0     4716 2019-12-20 09:03:05.000000 imod-0.9.0/imod/evaluate/constraints.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/imod/flow/
+-rw-rw-rw-   0        0        0     3391 2019-09-06 09:47:45.000000 imod-0.9.0/imod/flow/__init__.py
+-rw-rw-rw-   0        0        0    25672 2019-11-27 11:39:46.000000 imod-0.9.0/imod/idf.py
+-rw-rw-rw-   0        0        0    21331 2019-10-17 19:38:59.000000 imod-0.9.0/imod/ipf.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/imod/mf6/
+-rw-rw-rw-   0        0        0      873 2020-01-10 11:45:49.000000 imod-0.9.0/imod/mf6/__init__.py
+-rw-rw-rw-   0        0        0     2962 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/chd.py
+-rw-rw-rw-   0        0        0     3181 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/dis.py
+-rw-rw-rw-   0        0        0     2189 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/drn.py
+-rw-rw-rw-   0        0        0     3950 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/evt.py
+-rw-rw-rw-   0        0        0     2308 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/ghb.py
+-rw-rw-rw-   0        0        0     1680 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/ic.py
+-rw-rw-rw-   0        0        0    25483 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/ims.py
+-rw-rw-rw-   0        0        0     3791 2019-09-03 11:59:26.000000 imod-0.9.0/imod/mf6/model.py
+-rw-rw-rw-   0        0        0     5946 2020-01-10 11:45:49.000000 imod-0.9.0/imod/mf6/multimodel.py
+-rw-rw-rw-   0        0        0    14364 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/npf.py
+-rw-rw-rw-   0        0        0     1872 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/oc.py
+-rw-rw-rw-   0        0        0     4696 2019-09-07 22:01:16.000000 imod-0.9.0/imod/mf6/out.py
+-rw-rw-rw-   0        0        0     9833 2020-01-10 11:45:49.000000 imod-0.9.0/imod/mf6/pkgbase.py
+-rw-rw-rw-   0        0        0     2138 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/rch.py
+-rw-rw-rw-   0        0        0     2412 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/riv.py
+-rw-rw-rw-   0        0        0     3360 2019-12-20 09:24:59.000000 imod-0.9.0/imod/mf6/simulation.py
+-rw-rw-rw-   0        0        0     2714 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/sto.py
+-rw-rw-rw-   0        0        0     2544 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/timedis.py
+-rw-rw-rw-   0        0        0     3142 2019-12-20 09:03:05.000000 imod-0.9.0/imod/mf6/wel.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/imod/prepare/
+-rw-rw-rw-   0        0        0     1107 2020-01-17 12:16:42.000000 imod-0.9.0/imod/prepare/__init__.py
+-rw-rw-rw-   0        0        0    14435 2019-10-14 11:52:26.000000 imod-0.9.0/imod/prepare/common.py
+-rw-rw-rw-   0        0        0    17976 2019-11-25 13:30:13.000000 imod-0.9.0/imod/prepare/interpolate.py
+-rw-rw-rw-   0        0        0     4774 2020-01-17 12:16:42.000000 imod-0.9.0/imod/prepare/layerregrid.py
+-rw-rw-rw-   0        0        0    18870 2019-09-03 09:25:30.000000 imod-0.9.0/imod/prepare/pcg.py
+-rw-rw-rw-   0        0        0    17938 2019-11-25 13:30:13.000000 imod-0.9.0/imod/prepare/regrid.py
+-rw-rw-rw-   0        0        0    10314 2019-10-25 15:36:01.000000 imod-0.9.0/imod/prepare/reproject.py
+-rw-rw-rw-   0        0        0    26335 2019-09-03 09:25:30.000000 imod-0.9.0/imod/prepare/spatial.py
+-rw-rw-rw-   0        0        0     2805 2019-07-29 09:42:36.000000 imod-0.9.0/imod/prepare/subsoil.py
+-rw-rw-rw-   0        0        0     7531 2019-12-20 09:03:05.000000 imod-0.9.0/imod/prepare/surface_water.py
+-rw-rw-rw-   0        0        0     6583 2019-10-01 09:40:59.000000 imod-0.9.0/imod/prepare/voxelize.py
+-rw-rw-rw-   0        0        0    14679 2020-01-19 22:12:59.000000 imod-0.9.0/imod/rasterio.py
+-rw-rw-rw-   0        0        0    31123 2019-09-06 10:55:10.000000 imod-0.9.0/imod/run.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/imod/select/
+-rw-rw-rw-   0        0        0      313 2019-12-20 09:03:05.000000 imod-0.9.0/imod/select/__init__.py
+-rw-rw-rw-   0        0        0    12726 2019-09-03 09:25:30.000000 imod-0.9.0/imod/select/cross_sections.py
+-rw-rw-rw-   0        0        0     1511 2020-01-19 22:12:59.000000 imod-0.9.0/imod/select/layers.py
+-rw-rw-rw-   0        0        0     8105 2019-09-03 09:25:30.000000 imod-0.9.0/imod/select/points.py
+-rw-rw-rw-   0        0        0     6300 2019-07-23 15:11:12.000000 imod-0.9.0/imod/tec.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/imod/templates/
+-rw-rw-rw-   0        0        0     6198 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/generate_mf6_templates.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/imod/templates/mf6/
+-rw-rw-rw-   0        0        0      848 2020-01-10 11:45:49.000000 imod-0.9.0/imod/templates/mf6/exg-gwfgwf.j2
+-rw-rw-rw-   0        0        0      744 2019-09-06 09:47:45.000000 imod-0.9.0/imod/templates/mf6/gwf-chd.j2
+-rw-rw-rw-   0        0        0      818 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/gwf-dis.j2
+-rw-rw-rw-   0        0        0     1015 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/gwf-disu.j2
+-rw-rw-rw-   0        0        0      918 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/gwf-disv.j2
+-rw-rw-rw-   0        0        0      792 2019-09-05 16:18:47.000000 imod-0.9.0/imod/templates/mf6/gwf-drn.j2
+-rw-rw-rw-   0        0        0      895 2019-09-06 09:47:45.000000 imod-0.9.0/imod/templates/mf6/gwf-evt.j2
+-rw-rw-rw-   0        0        0      718 2019-09-06 09:47:45.000000 imod-0.9.0/imod/templates/mf6/gwf-evta.j2
+-rw-rw-rw-   0        0        0      792 2019-09-06 09:47:45.000000 imod-0.9.0/imod/templates/mf6/gwf-ghb.j2
+-rw-rw-rw-   0        0        0      476 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/gwf-gnc.j2
+-rw-rw-rw-   0        0        0      262 2019-09-06 09:47:45.000000 imod-0.9.0/imod/templates/mf6/gwf-hfb.j2
+-rw-rw-rw-   0        0        0      168 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/gwf-ic.j2
+-rw-rw-rw-   0        0        0     2221 2019-09-06 09:47:45.000000 imod-0.9.0/imod/templates/mf6/gwf-lak.j2
+-rw-rw-rw-   0        0        0     1918 2019-09-06 09:47:45.000000 imod-0.9.0/imod/templates/mf6/gwf-maw.j2
+-rw-rw-rw-   0        0        0      663 2019-09-06 09:47:45.000000 imod-0.9.0/imod/templates/mf6/gwf-mvr.j2
+-rw-rw-rw-   0        0        0      487 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/gwf-nam.j2
+-rw-rw-rw-   0        0        0     1845 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/gwf-npf.j2
+-rw-rw-rw-   0        0        0      478 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/gwf-oc.j2
+-rw-rw-rw-   0        0        0      802 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/gwf-rch.j2
+-rw-rw-rw-   0        0        0      718 2019-09-06 09:47:45.000000 imod-0.9.0/imod/templates/mf6/gwf-rcha.j2
+-rw-rw-rw-   0        0        0      792 2019-09-06 09:47:45.000000 imod-0.9.0/imod/templates/mf6/gwf-riv.j2
+-rw-rw-rw-   0        0        0     1988 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/gwf-sfr.j2
+-rw-rw-rw-   0        0        0      624 2019-09-06 09:47:45.000000 imod-0.9.0/imod/templates/mf6/gwf-sto.j2
+-rw-rw-rw-   0        0        0     1715 2019-09-06 09:47:45.000000 imod-0.9.0/imod/templates/mf6/gwf-uzf.j2
+-rw-rw-rw-   0        0        0      883 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/gwf-wel.j2
+-rw-rw-rw-   0        0        0      856 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/sim-nam.j2
+-rw-rw-rw-   0        0        0      371 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/sim-tdis.j2
+-rw-rw-rw-   0        0        0     2368 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/sln-ims.j2
+-rw-rw-rw-   0        0        0      271 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/utl-lak-tab.j2
+-rw-rw-rw-   0        0        0      356 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/utl-obs.j2
+-rw-rw-rw-   0        0        0      410 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/utl-tas.j2
+-rw-rw-rw-   0        0        0      836 2019-09-03 11:59:26.000000 imod-0.9.0/imod/templates/mf6/utl-ts.j2
+-rw-rw-rw-   0        0        0     1806 2019-06-18 09:29:11.000000 imod-0.9.0/imod/templates/runfile.j2
+-rw-rw-rw-   0        0        0     8103 2019-06-18 09:29:11.000000 imod-0.9.0/imod/templates/seawat_runfile.j2
+-rw-rw-rw-   0        0        0    14699 2019-12-20 09:03:05.000000 imod-0.9.0/imod/util.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/imod/visualize/
+-rw-rw-rw-   0        0        0      456 2019-10-14 11:52:26.000000 imod-0.9.0/imod/visualize/__init__.py
+-rw-rw-rw-   0        0        0     5963 2020-01-17 12:16:42.000000 imod-0.9.0/imod/visualize/cross_sections.py
+-rw-rw-rw-   0        0        0    10583 2019-10-05 18:36:19.000000 imod-0.9.0/imod/visualize/spatial.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/imod/wq/
+-rw-rw-rw-   0        0        0     1211 2019-09-23 07:14:33.000000 imod-0.9.0/imod/wq/__init__.py
+-rw-rw-rw-   0        0        0    21314 2019-10-14 12:31:54.000000 imod-0.9.0/imod/wq/adv.py
+-rw-rw-rw-   0        0        0     7200 2019-11-05 10:34:06.000000 imod-0.9.0/imod/wq/bas.py
+-rw-rw-rw-   0        0        0     7992 2019-12-20 09:03:05.000000 imod-0.9.0/imod/wq/btn.py
+-rw-rw-rw-   0        0        0     1553 2019-10-14 12:31:54.000000 imod-0.9.0/imod/wq/chd.py
+-rw-rw-rw-   0        0        0     8531 2019-10-14 12:31:54.000000 imod-0.9.0/imod/wq/dis.py
+-rw-rw-rw-   0        0        0     1598 2019-10-14 12:31:54.000000 imod-0.9.0/imod/wq/drn.py
+-rw-rw-rw-   0        0        0     3338 2019-10-14 12:31:54.000000 imod-0.9.0/imod/wq/dsp.py
+-rw-rw-rw-   0        0        0     2893 2019-10-14 12:31:54.000000 imod-0.9.0/imod/wq/ghb.py
+-rw-rw-rw-   0        0        0     9045 2019-11-05 10:34:06.000000 imod-0.9.0/imod/wq/lpf.py
+-rw-rw-rw-   0        0        0    20043 2019-12-20 09:03:05.000000 imod-0.9.0/imod/wq/model.py
+-rw-rw-rw-   0        0        0     3532 2019-10-14 12:31:54.000000 imod-0.9.0/imod/wq/oc.py
+-rw-rw-rw-   0        0        0    16389 2020-01-19 12:10:16.000000 imod-0.9.0/imod/wq/pkgbase.py
+-rw-rw-rw-   0        0        0     3917 2019-07-29 09:42:37.000000 imod-0.9.0/imod/wq/pkggroup.py
+-rw-rw-rw-   0        0        0     5393 2019-10-14 12:31:54.000000 imod-0.9.0/imod/wq/rch.py
+-rw-rw-rw-   0        0        0     3289 2019-10-14 12:31:54.000000 imod-0.9.0/imod/wq/riv.py
+-rw-rw-rw-   0        0        0    17208 2019-10-14 12:31:54.000000 imod-0.9.0/imod/wq/slv.py
+-rw-rw-rw-   0        0        0     3327 2019-06-20 06:37:31.000000 imod-0.9.0/imod/wq/timeutil.py
+-rw-rw-rw-   0        0        0     6681 2019-10-14 12:31:54.000000 imod-0.9.0/imod/wq/vdf.py
+-rw-rw-rw-   0        0        0     9502 2020-01-19 12:10:16.000000 imod-0.9.0/imod/wq/wel.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/imod.egg-info/
+-rw-rw-rw-   0        0        0     4323 2020-01-19 22:15:56.000000 imod-0.9.0/imod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5334 2020-01-19 22:15:57.000000 imod-0.9.0/imod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-01-19 22:15:56.000000 imod-0.9.0/imod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      215 2020-01-19 22:15:56.000000 imod-0.9.0/imod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2020-01-19 22:15:56.000000 imod-0.9.0/imod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-01-19 22:15:57.000000 imod-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1914 2020-01-19 22:12:59.000000 imod-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/tests/
+-rw-rw-rw-   0        0        0    12361 2019-12-20 09:03:05.000000 imod-0.9.0/tests/test_array_io.py
+-rw-rw-rw-   0        0        0     6481 2019-09-23 07:14:33.000000 imod-0.9.0/tests/test_benchmark.py
+-rw-rw-rw-   0        0        0     8297 2019-10-14 12:31:54.000000 imod-0.9.0/tests/test_common.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/tests/test_evaluate.py/
+-rw-rw-rw-   0        0        0     3533 2019-10-01 09:40:59.000000 imod-0.9.0/tests/test_evaluate.py/test_budget.py
+-rw-rw-rw-   0        0        0      934 2020-01-19 12:10:16.000000 imod-0.9.0/tests/test_examples.py
+-rw-rw-rw-   0        0        0     8557 2020-01-10 11:45:49.000000 imod-0.9.0/tests/test_idf.py
+-rw-rw-rw-   0        0        0     5707 2019-09-03 09:25:30.000000 imod-0.9.0/tests/test_interpolate.py
+-rw-rw-rw-   0        0        0    10682 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_ipf.py
+-rw-rw-rw-   0        0        0     4735 2020-01-17 12:16:42.000000 imod-0.9.0/tests/test_layerregrid.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/tests/test_mf6/
+-rw-rw-rw-   0        0        0    13768 2020-01-17 15:12:28.000000 imod-0.9.0/tests/test_mf6/test_ex01_twri.py
+-rw-rw-rw-   0        0        0     5220 2020-01-10 11:45:49.000000 imod-0.9.0/tests/test_mf6/test_ex32_periodicbc.py
+-rw-rw-rw-   0        0        0     1375 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_mf6/test_mf6_chd.py
+-rw-rw-rw-   0        0        0     1543 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_mf6/test_mf6_dis.py
+-rw-rw-rw-   0        0        0     1112 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_mf6/test_mf6_drn.py
+-rw-rw-rw-   0        0        0      423 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_mf6/test_mf6_ic.py
+-rw-rw-rw-   0        0        0      985 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_mf6/test_mf6_ims.py
+-rw-rw-rw-   0        0        0     1265 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_mf6/test_mf6_npf.py
+-rw-rw-rw-   0        0        0      636 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_mf6/test_mf6_oc.py
+-rw-rw-rw-   0        0        0      595 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_mf6/test_mf6_rch.py
+-rw-rw-rw-   0        0        0      625 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_mf6/test_mf6_riv.py
+-rw-rw-rw-   0        0        0     1208 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_mf6/test_mf6_wel.py
+-rw-rw-rw-   0        0        0     2334 2020-01-10 11:45:49.000000 imod-0.9.0/tests/test_mf6/test_multimodel.py
+-rw-rw-rw-   0        0        0     2511 2019-12-20 09:03:05.000000 imod-0.9.0/tests/test_rasterio.py
+-rw-rw-rw-   0        0        0    15813 2019-09-09 11:29:54.000000 imod-0.9.0/tests/test_regrid.py
+-rw-rw-rw-   0        0        0    10302 2019-10-25 15:36:01.000000 imod-0.9.0/tests/test_reproject.py
+-rw-rw-rw-   0        0        0    18319 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_run.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/tests/test_select/
+-rw-rw-rw-   0        0        0     3674 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_select/test_select_cross_sections.py
+-rw-rw-rw-   0        0        0     3749 2019-12-20 09:03:05.000000 imod-0.9.0/tests/test_select/test_select_layers.py
+-rw-rw-rw-   0        0        0     5381 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_select/test_select_points.py
+-rw-rw-rw-   0        0        0     7268 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_spatial.py
+-rw-rw-rw-   0        0        0    10399 2019-12-20 09:03:05.000000 imod-0.9.0/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/tests/test_visualize/
+-rw-rw-rw-   0        0        0     1426 2019-12-20 10:10:10.000000 imod-0.9.0/tests/test_visualize/test_visualize_cross_sections.py
+-rw-rw-rw-   0        0        0     3135 2019-12-20 09:03:05.000000 imod-0.9.0/tests/test_visualize/test_visualize_spatial.py
+-rw-rw-rw-   0        0        0     3838 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_voxelize.py
+drwxrwxrwx   0        0        0        0 2020-01-19 22:15:57.000000 imod-0.9.0/tests/test_wq/
+-rw-rw-rw-   0        0        0      603 2019-09-23 07:14:33.000000 imod-0.9.0/tests/test_wq/test_wq_adv.py
+-rw-rw-rw-   0        0        0     2598 2019-11-05 10:34:06.000000 imod-0.9.0/tests/test_wq/test_wq_bas.py
+-rw-rw-rw-   0        0        0     2819 2019-12-20 09:03:05.000000 imod-0.9.0/tests/test_wq/test_wq_btn.py
+-rw-rw-rw-   0        0        0     1594 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_wq/test_wq_chd.py
+-rw-rw-rw-   0        0        0     1964 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_wq/test_wq_dis.py
+-rw-rw-rw-   0        0        0     3882 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_wq/test_wq_drn.py
+-rw-rw-rw-   0        0        0     2482 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_wq/test_wq_dsp.py
+-rw-rw-rw-   0        0        0     1817 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_wq/test_wq_ghb.py
+-rw-rw-rw-   0        0        0     4244 2019-11-05 10:34:06.000000 imod-0.9.0/tests/test_wq/test_wq_lpf.py
+-rw-rw-rw-   0        0        0    16404 2019-10-25 15:36:01.000000 imod-0.9.0/tests/test_wq/test_wq_model.py
+-rw-rw-rw-   0        0        0      635 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_wq/test_wq_oc.py
+-rw-rw-rw-   0        0        0     4297 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_wq/test_wq_pkggroup.py
+-rw-rw-rw-   0        0        0     4155 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_wq/test_wq_rch.py
+-rw-rw-rw-   0        0        0     1959 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_wq/test_wq_riv.py
+-rw-rw-rw-   0        0        0     5103 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_wq/test_wq_slv.py
+-rw-rw-rw-   0        0        0     1845 2019-09-03 11:59:26.000000 imod-0.9.0/tests/test_wq/test_wq_timeutil.py
+-rw-rw-rw-   0        0        0      805 2019-09-06 09:47:45.000000 imod-0.9.0/tests/test_wq/test_wq_vdf.py
+-rw-rw-rw-   0        0        0     7630 2020-01-19 12:10:16.000000 imod-0.9.0/tests/test_wq/test_wq_wel.py
```

### Comparing `imod-0.8.0/imod/evaluate/budget.py` & `imod-0.9.0/imod/evaluate/budget.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/flow/__init__.py` & `imod-0.9.0/imod/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/ipf.py` & `imod-0.9.0/imod/ipf.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,16 +228,16 @@
     Read one or more IPF files to a single pandas.DataFrame, including associated
     (TXT) files.
 
     The different IPF files can be from different model layers,
     and column names may differ between them.
 
     Note that this function always returns a ``pandas.DataFrame``. IPF files
-    always contain spatial information, for which ``geopandas.GeoDataFrame``s
-    are a better fit, in principle. However, GeoDataFrames are not the best fit
+    always contain spatial information, for which ``geopandas.GeoDataFrame``
+    is a better fit, in principle. However, GeoDataFrames are not the best fit
     for the associated data.
 
     To perform spatial operations on the points, you're likely best served by
     (temporarily) creating a GeoDataFrame, doing the spatial operation, and
     then using the output to select values in the original DataFrame. Please
     refer to the examples.
```

### Comparing `imod-0.8.0/imod/mf6/dis.py` & `imod-0.9.0/imod/mf6/dis.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,43 +3,48 @@
 
 import imod
 from imod.mf6.pkgbase import Package
 
 
 class StructuredDiscretization(Package):
     """
-    The Drain package is used to simulate head-dependent flux boundaries. In the
-    Drain package if the head in the cell falls below a certain threshold, the
-    flux from the drain to the model cell drops to zero.
+    Discretization information for structered grids is specified using the file.
+    (DIS6) Only one discretization input file (DISU6, DISV6 or DIS6) can be
+    specified for a model.
+    https://water.usgs.gov/water-resources/software/MODFLOW-6/mf6io_6.0.4.pdf#page=35
 
     Parameters
     ----------
+    top: array of floats (xr.DataArray)
+        is the top elevation for each cell in the top model layer.
+    bottom: array of floats (xr.DataArray)
+        is the bottom elevation for each cell.
     idomain: array of integers (xr.DataArray)
-        Indicates the existence status of a cell. Horizontal discretization information will
-        be derived from the ``x`` and ``y`` coordinates of the DataArray.
-
-        If the IDOMAIN value for a cell is 0, the cell does not exist in the simulation. Input
-        and output values will be read and written for the cell, but internal to the program,
-        the cell is excluded from the solution. If the IDOMAIN value for a cell is 1, the cell
-        exists in the simulation. If the IDOMAIN value for a cell is -1, the cell does not exist
-        in the simulation. Furthermore, the first existing cell above will be connected to the
-        first existing cell below. This type of cell is referred to as a “vertical pass through”
-        cell.
+        Indicates the existence status of a cell. Horizontal discretization
+        information will be derived from the x and y coordinates of the
+        DataArray. If the idomain value for a cell is 0, the cell does not exist
+        in the simulation. Input and output values will be read and written for
+        the cell, but internal to the program, the cell is excluded from the
+        solution. If the idomain value for a cell is 1, the cell exists in the
+        simulation. if the idomain value for a cell is -1, the cell does not
+        exist in the simulation. Furthermore, the first existing cell above will
+        be connected to the first existing cell below. This type of cell is
+        referred to as a “vertical pass through”cell.
     """
 
     __slots__ = ("top", "bottom", "idomain")
     _pkg_id = "dis"
     _binary_data = {"top": np.float64, "bottom": np.float64, "idomain": np.int32}
+    _template = Package._initialize_template(_pkg_id)
 
     def __init__(self, top, bottom, idomain):
         super(__class__, self).__init__()
         self["top"] = top
         self["bottom"] = bottom
         self["idomain"] = idomain
-        self._initialize_template()
 
     def _delrc(self, dx):
         """
         dx means dx or dy
         """
         if isinstance(dx, (int, float)):
             return f"constant {dx}"
```

### Comparing `imod-0.8.0/imod/mf6/model.py` & `imod-0.9.0/imod/mf6/model.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/mf6/oc.py` & `imod-0.9.0/imod/mf6/oc.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 import numpy as np
 
 from imod.mf6.pkgbase import Package
 
 
 class OutputControl(Package):
     """
-    Attributes
-    ----------
+    The Output Control Option determines how and when heads are printed to the
+    listing file and/or written to a separate binary output file.
+    https://water.usgs.gov/water-resources/software/MODFLOW-6/mf6io_6.0.4.pdf#page=47
 
+    Parameters
+    ----------
     save_head : bool, or xr.DataArray of bools
-        Bool per stress period
+        Bool per stress period.
     save_budget : bool, or xr.DataArray of bools
-        Bool per stress period
+        Bool per stress period.
     """
 
     __slots__ = ("save_head", "save_budget")
     _pkg_id = "oc"
+    _template = Package._initialize_template(_pkg_id)
 
     def __init__(self, save_head, save_budget):
         super(__class__, self).__init__()
         self["save_head"] = save_head
         self["save_budget"] = save_budget
-        self._initialize_template()
 
     def render(self, directory, pkgname, globaltimes):
         d = {}
         modelname = directory.stem
         if self["save_head"].values.any():
             d["headfile"] = (directory / f"{modelname}.hds").as_posix()
         if self["save_budget"].any():
```

### Comparing `imod-0.8.0/imod/mf6/out.py` & `imod-0.9.0/imod/mf6/out.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/mf6/pkgbase.py` & `imod-0.9.0/imod/mf6/pkgbase.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,24 +29,25 @@
             return False
         # Test numpy bool (not singleton)
         elif isinstance(value, np.bool_) and not value:
             return False
         else:
             return True
 
-    def _initialize_template(self):
+    @staticmethod
+    def _initialize_template(pkg_id):
         loader = jinja2.PackageLoader("imod", "templates/mf6")
         env = jinja2.Environment(loader=loader)
-        if self._pkg_id == "ims":
+        if pkg_id == "ims":
             fname = "sln-ims.j2"
-        elif self._pkg_id == "tdis":
+        elif pkg_id == "tdis":
             fname = "sim-tdis.j2"
         else:
-            fname = f"gwf-{self._pkg_id}.j2"
-        self._template = env.get_template(fname)
+            fname = f"gwf-{pkg_id}.j2"
+        return env.get_template(fname)
 
     def write_blockfile(self, directory, pkgname, globaltimes=None):
         content = self.render(directory, pkgname, globaltimes)
         filename = directory / f"{pkgname}.{self._pkg_id}"
         with open(filename, "w") as f:
             f.write(content)
 
@@ -81,14 +82,18 @@
         return listarr
 
     def write_binaryfile(self, outpath, ds):
         """
         data is a xr.Dataset with only the binary variables"""
         arrays = []
         for datavar in ds.data_vars:
+            if ds[datavar].shape == ():
+                raise ValueError(
+                    f"{datavar} in {ds._pkg_id} package cannot be a scalar"
+                )
             arrays.append(ds[datavar].values)
         if "layer" in ds.coords and "layer" not in ds.dims:
             layer = ds["layer"].values
         else:
             layer = None
         sparse_data = self.to_sparse(arrays, layer)
         outpath.parent.mkdir(exist_ok=True, parents=True)
```

### Comparing `imod-0.8.0/imod/mf6/simulation.py` & `imod-0.9.0/imod/mf6/simulation.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/mf6/timedis.py` & `imod-0.9.0/imod/mf6/timedis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,41 @@
 import numpy as np
 
 from imod.mf6.pkgbase import Package
 
 
 class TimeDiscretization(Package):
+    """
+    Timing for all models of the simulation is controlled by the Temporal
+    Discretization (TDIS) Package.
+    https://water.usgs.gov/water-resources/software/MODFLOW-6/mf6io_6.0.4.pdf#page=17
+
+    Paremeters
+    ----------
+    timestep_duration: float
+        is the length of a stress period. (PERLEN)
+    n_timesteps: int, optional
+        is the number of time steps in a stress period (nstp).
+        Default value: 1
+    timestep_multiplier: float, optional
+        is the multiplier for the length of successive time steps. The length of
+        a time step is calculated by multiplying the length of the previous time
+        step by timestep_multiplier (TSMULT).
+        Default value: 1.0
+    """
+
     __slots__ = ("timestep_duration", "n_timesteps", "timestep_multiplier")
     _pkg_id = "tdis"
+    _template = Package._initialize_template(_pkg_id)
 
     def __init__(self, timestep_duration, n_timesteps=1, timestep_multiplier=1.0):
         super(__class__, self).__init__()
         self["timestep_duration"] = timestep_duration
         self["n_timesteps"] = n_timesteps
         self["timestep_multiplier"] = timestep_multiplier
-        self._initialize_template()
 
     def render(self):
         d = {}
         d["time_units"] = "days"
         timestep_duration = self["timestep_duration"]
         n_timesteps = self["n_timesteps"]
         timestep_multiplier = self["timestep_multiplier"]
```

### Comparing `imod-0.8.0/imod/mf6/__init__.py` & `imod-0.9.0/imod/mf6/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,7 +20,9 @@
 from imod.mf6.out import open_hds
 from imod.mf6.rch import Recharge
 from imod.mf6.riv import River
 from imod.mf6.simulation import Modflow6Simulation
 from imod.mf6.sto import Storage
 from imod.mf6.timedis import TimeDiscretization
 from imod.mf6.wel import Well
+
+from imod.mf6 import multimodel
```

### Comparing `imod-0.8.0/imod/prepare/common.py` & `imod-0.9.0/imod/prepare/common.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/prepare/interpolate.py` & `imod-0.9.0/imod/prepare/interpolate.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,17 +280,25 @@
 
     return dst
 
 
 @numba.njit(cache=True)
 def _interp_3d(src, dst, *inds_weights):
     # Unpack the variadic arguments
-    ii, weights_z, within_z, jj, weights_y, within_y, kk, weights_x, within_x = (
-        inds_weights
-    )
+    (
+        ii,
+        weights_z,
+        within_z,
+        jj,
+        weights_y,
+        within_y,
+        kk,
+        weights_x,
+        within_x,
+    ) = inds_weights
     # i, j, k are indices of dst array
     for i, (iz, wz, in_z) in enumerate(zip(ii, weights_z, within_z)):
         if iz < 0:
             continue
 
         for j, (iy, wy, in_y) in enumerate(zip(jj, weights_y, within_y)):
             if iy < 0:
```

### Comparing `imod-0.8.0/imod/prepare/layerregrid.py` & `imod-0.9.0/imod/prepare/layerregrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 METHODS = common.METHODS.copy()
 METHODS.pop("conductance")
 METHODS.pop("nearest")
 METHODS.pop("multilinear")
 
 
 @numba.njit(cache=True)
-def _regrid_layers(
-    src, dst, src_top, dst_top, src_bot, dst_bot, values, weights, method
-):
+def _regrid_layers(src, dst, src_top, dst_top, src_bot, dst_bot, method):
     """
     Maps one set of layers unto the other.
     """
     nlayer_src, nrow, ncol = src.shape
     nlayer_dst = dst.shape[0]
     values = np.zeros(nlayer_src)
     weights = np.zeros(nlayer_src)
@@ -48,52 +46,53 @@
 
                     overlap = common._overlap((db, dt), (sb, st))
                     if overlap == 0:
                         continue
 
                     has_value = True
                     values[count] = src[jj, i, j]
-                    values[count] = overlap
+                    weights[count] = overlap
                     count += 1
                 else:
                     if has_value:
                         dst[ii, i, j] = method(values, weights)
                         # Reset
                         values[:count] = 0
                         weights[:count] = 0
 
     return dst
 
 
 class LayerRegridder:
     """
-    Object to repeatedly voxelize similar objects. Compiles once on first call,
-    can then be repeatedly called without JIT compilation overhead.
+    Object to repeatedly regrid layers from similar objects. Compiles 
+    once on first call, \can then be repeatedly called without 
+    JIT compilation overhead.
 
     Attributes
     ----------
     method : str, function
         The method to use for regridding. Default available methods are:
         ``{"mean", "harmonic_mean", "geometric_mean", "sum", "minimum",
         "maximum", "mode", "median", "max_overlap"}``
     """
 
     def __init__(self, method):
         _method = common._get_method(method, METHODS)
         self.method = _method
-        self.first_call = True
+        self._first_call = True
 
     def _make_regrid(self):
         """
         Use closure to avoid numba overhead
         """
         jit_method = numba.njit(self.method)
 
         @numba.njit
-        def regrid(src, dst, src_top, dst_top, src_bot, dst_bot, weights, values):
+        def regrid(src, dst, src_top, dst_top, src_bot, dst_bot):
             return _regrid_layers(
                 src, dst, src_top, dst_top, src_bot, dst_bot, jit_method
             )
 
         self._regrid = regrid
 
     def regrid(
@@ -130,17 +129,17 @@
             destination_top,
         ]:
             if not da.dims == ("layer", "y", "x"):
                 raise ValueError(
                     "Dimensions for top, bottom, and source have to be exactly"
                     f' ("layer", "y", "x"). Got instead {dim_format(da.dims)}.'
                 )
-        for da in [bottom, source]:
-            for (k1, v1), (_, v2) in zip(top.coords.items(), da.coords.items()):
-                if not v1.equals(v2):
+        for da in [source_bottom, source]:
+            for (k1, v1) in source_top.coords.items():
+                if not v1.equals(da.coords[k1]):
                     raise ValueError(f"Input coordinates do not match along {k1}")
 
         if self._first_call:
             self._make_regrid()
             self._first_call = False
 
         dst = xr.full_like(destination_top, np.nan, dtype=source.dtype)
```

### Comparing `imod-0.8.0/imod/prepare/pcg.py` & `imod-0.9.0/imod/prepare/pcg.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/prepare/regrid.py` & `imod-0.9.0/imod/prepare/regrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,17 +128,25 @@
     ----------
     src : np.array
     dst : np.array
     src_coords : tuple of np.arrays of edges
     dst_coords : tuple of np.arrays of edges
     method : numba.njit'ed function
     """
-    ii, blocks_iz, blocks_weights_z, jj, blocks_iy, blocks_weights_y, kk, blocks_ix, blocks_weights_x = (
-        inds_weights
-    )
+    (
+        ii,
+        blocks_iz,
+        blocks_weights_z,
+        jj,
+        blocks_iy,
+        blocks_weights_y,
+        kk,
+        blocks_ix,
+        blocks_weights_x,
+    ) = inds_weights
 
     # i, j, k are indices of dst array
     # block_i contains indices of src array
     # block_w contains weights of src array
     for counti, i in enumerate(ii):
         block_iz = blocks_iz[counti]
         block_wz = blocks_weights_z[counti]
```

### Comparing `imod-0.8.0/imod/prepare/reproject.py` & `imod-0.9.0/imod/prepare/reproject.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,16 @@
     """
     src_height, src_width = source.y.size, source.x.size
     bounds = rasterio.transform.array_bounds(src_height, src_width, src_transform)
     dst_transform, dst_width, dst_height = rasterio.warp.calculate_default_transform(
         src_crs, dst_crs, src_width, src_height, *bounds
     )
     # from: http://xarray.pydata.org/en/stable/generated/xarray.open_rasterio.html
-    x, y = (
-        np.meshgrid(np.arange(dst_width) + 0.5, np.arange(dst_height) + 0.5)
-        * dst_transform
+    x, y = dst_transform * np.meshgrid(
+        np.arange(dst_width) + 0.5, np.arange(dst_height) + 0.5
     )
     dst = xr.DataArray(
         data=np.zeros((dst_height, dst_width), source.dtype),
         coords={"y": y[:, 0], "x": x[0, :]},
         dims=("y", "x"),
     )
     return dst_transform, dst
@@ -64,22 +63,20 @@
         ``y`` and ``x``.
     like: xarray DataArray
         Example DataArray that shows what the resampled result should look like 
         in terms of coordinates. Must contain dimensions ``y`` and ``x``.
     src_crs: string, dict, rasterio.crs.CRS
         Coordinate system of ``source``. Options:
 
-        * string: e.g. ``"+init=EPSG:4326"``
-        * dict: e.g. ``{"init":"EPSG:4326"}``
+        * string: e.g. ``"EPSG:4326"``
         * rasterio.crs.CRS
     dst_crs: string, dict, rasterio.crs.CRS
         Coordinate system of result. Options:
 
-        * string: e.g. ``"+init=EPSG:4326"``
-        * dict: e.g. ``{"init":"EPSG:4326"}``
+        * string: e.g. ``"EPSG:4326"``
         * rasterio.crs.CRS
     use_src_attrs: boolean
         If True: Use metadata in ``source.attrs``, as generated by ``xarray.open_rasterio()``, to do 
         reprojection.
     method: string
         The method to use for resampling/reprojection.
         Defaults to "nearest". GDAL methods are available:
@@ -117,44 +114,58 @@
     >>> dims = ("y", "x")
     >>> coords = {"y": np.arange(200_000.0, 100_000.0, -100.0), "x": np.arange(0.0, 100_000.0, 100.0)}
     >>> b = xr.DataArray(data=np.empty((200, 100)), coords=coords, dims=dims)
     >>> c = imod.rasterio.reproject(source=a, like=b)
 
     Reproject a DataArray from one coordinate system (WGS84, EPSG:4326) to another (UTM30N, EPSG:32630):
 
-    >>> c = imod.rasterio.reproject(source=a, src_crs="+init=EPSG:4326", dst_crs="+init=EPSG:32630")
+    >>> c = imod.rasterio.reproject(source=a, src_crs="EPSG:4326", dst_crs="EPSG:32630")
 
     Get the reprojected DataArray in the desired shape and coordinates by providing ``like``:
 
-    >>> c = imod.rasterio.reproject(source=a, like=b, src_crs="+init=EPSG:4326", dst_crs="+init=EPSG:32630")
+    >>> c = imod.rasterio.reproject(source=a, like=b, src_crs="EPSG:4326", dst_crs="EPSG:32630")
 
     Open a single band raster, and reproject to RD new coordinate system (EPSG:28992), without explicitly specifying ``src_crs``.
     ``src_crs`` is taken from ``a.attrs``, so the raster file has to include coordinate system metadata for this to work.
 
     >>> a = xr.open_rasterio("example.tif").squeeze("band")
-    >>> c = imod.rasterio.reproject(source=a, use_src_attrs=True, dst_crs="+init=EPSG:28992")
+    >>> c = imod.rasterio.reproject(source=a, use_src_attrs=True, dst_crs="EPSG:28992")
 
     In case of a rotated ``source``, provide ``src_transform`` directly or ``use_src_attrs=True`` to rely on generated attributes:
 
     >>> rotated = xr.open_rasterio("rotated_example.tif").squeeze("band")
-    >>> c = imod.rasterio.reproject(source=rotated, dst_crs="+init=EPSG:28992", reproject_kwargs={"src_transform":affine.Affine(...)})
-    >>> c = imod.rasterio.reproject(source=rotated, dst_crs="+init=EPSG:28992", use_src_attrs=True)
+    >>> c = imod.rasterio.reproject(source=rotated, dst_crs="EPSG:28992", reproject_kwargs={"src_transform":affine.Affine(...)})
+    >>> c = imod.rasterio.reproject(source=rotated, dst_crs="EPSG:28992", use_src_attrs=True)
     """
     if not source.dims == ("y", "x"):
         raise ValueError(
             "reproject does not support dimensions other than ``x`` and ``y`` for ``source``."
         )
     if like is not None:
         if not like.dims == ("y", "x"):
             raise ValueError(
                 "reproject does not support dimensions other than ``x`` and ``y`` for ``like``."
             )
     if use_src_attrs:  # only provided when reproject is necessary
-        src_crs = rasterio.crs.CRS.from_string(source.attrs["crs"])
-        src_nodata = source.attrs["nodatavals"][0]
+        src_crs = source.attrs["crs"]
+        if isinstance(src_crs, str):
+            if "epsg:" in src_crs.lower():
+                # Workaround for xr.open_rasterio generation proj4 strings
+                # https://github.com/mapbox/rasterio/issues/1809
+                epsg_code = src_crs.lower().split("epsg:")[-1]
+                src_crs = rasterio.crs.CRS.from_epsg(epsg_code)
+            else:
+                src_crs = rasterio.crs.CRS.from_string(src_crs)
+        elif isinstance(src, rasterio.crs.CRS):
+            pass
+        else:
+            raise ValueError(
+                f"Invalid src_crs: {src_crs}. Must be either str or rasterio.crs.CRS object"
+            )
+        src_nodata = source.attrs.get("nodatavals", [None])[0]
 
     resampling_methods = {e.name: e for e in rasterio.enums.Resampling}
 
     if isinstance(method, str):
         try:
             resampling_method = resampling_methods[method]
         except KeyError as e:
```

### Comparing `imod-0.8.0/imod/prepare/spatial.py` & `imod-0.9.0/imod/prepare/spatial.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/prepare/subsoil.py` & `imod-0.9.0/imod/prepare/subsoil.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/prepare/voxelize.py` & `imod-0.9.0/imod/prepare/voxelize.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/prepare/__init__.py` & `imod-0.9.0/imod/prepare/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,7 +21,8 @@
     fill,
     gdal_rasterize,
     laplace_interpolate,
     rasterize,
     rasterize_celltable,
 )
 from imod.prepare.voxelize import Voxelizer
+from imod.prepare.layerregrid import LayerRegridder
```

### Comparing `imod-0.8.0/imod/run.py` & `imod-0.9.0/imod/run.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/select/cross_sections.py` & `imod-0.9.0/imod/select/cross_sections.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/select/points.py` & `imod-0.9.0/imod/select/points.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/tec.py` & `imod-0.9.0/imod/tec.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/exg-gwfgwf.j2` & `imod-0.9.0/imod/templates/mf6/gwf-disv.j2`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 begin options
-{%- if auxiliary is defined -%}  auxiliary {{auxiliary(naux)}}{%- endif -%}
-{%- if print_input is defined -%}  print_input{%- endif -%}
-{%- if print_flows is defined -%}  print_flows{%- endif -%}
-{%- if save_flows is defined -%}  save_flows{%- endif -%}
-{%- if cell_averaging is defined -%}  cell_averaging {{cell_averaging}}{%- endif -%}
-{%- if cvoptions is defined -%}  variablecv {%- if dewatered is defined -%}dewatered{%- endif -%}{%- endif -%}
-{%- if newton is defined -%}  newton{%- endif -%}
-{%- if gnc_filerecord is defined -%}  gnc6 filein {{gnc6_filename}}{%- endif -%}
-{%- if mvr_filerecord is defined -%}  mvr6 filein {{mvr6_filename}}{%- endif -%}
-{%- if obs_filerecord is defined -%}  obs6 filein {{obs6_filename}}{%- endif -%}
+{%- if length_units is defined -%}  length_units {{length_units}}{%- endif -%}
+{%- if nogrb is defined -%}  nogrb{%- endif -%}
+{%- if xorigin is defined -%}  xorigin {{xorigin}}{%- endif -%}
+{%- if yorigin is defined -%}  yorigin {{yorigin}}{%- endif -%}
+{%- if angrot is defined -%}  angrot {{angrot}}{%- endif -%}
 end options
 
 begin dimensions
-  nexg {{nexg}}
+  nlay {{nlay}}
+  ncpl {{ncpl}}
+  nvert {{nvert}}
 end dimensions
 
-begin exchangedata
-  {{cellidm1}} {{cellidm2}} {{ihc}} {{cl1}} {{cl2}} {{hwva}} {%- if aux is defined -%}{{aux(naux)}}{%- endif -%}
-  {{cellidm1}} {{cellidm2}} {{ihc}} {{cl1}} {{cl2}} {{hwva}} {%- if aux is defined -%}{{aux(naux)}}{%- endif -%}
+begin griddata
+  top
+    {top}
+  botm {% if layered is sameas true %}layered{% endif %}
+    {botm}
+{%- if idomain is defined -%}  idomain {% if layered is sameas true %}layered{% endif %}
+    {idomain}{%- endif -%}
+end griddata
+
+begin vertices
+  {{iv}} {{xv}} {{yv}}
+  {{iv}} {{xv}} {{yv}}
+  ...
+end vertices
+
+begin cell2d
+  {{icell2d}} {{xc}} {{yc}} {{ncvert}} {{icvert(ncvert)}}
+  {{icell2d}} {{xc}} {{yc}} {{ncvert}} {{icvert(ncvert)}}
   ...
-end exchangedata
+end cell2d
```

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-chd.j2` & `imod-0.9.0/imod/templates/mf6/gwf-chd.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-dis.j2` & `imod-0.9.0/imod/templates/mf6/gwf-dis.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-disu.j2` & `imod-0.9.0/imod/templates/mf6/gwf-disu.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-drn.j2` & `imod-0.9.0/imod/templates/mf6/gwf-drn.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-evt.j2` & `imod-0.9.0/imod/templates/mf6/gwf-evt.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-evta.j2` & `imod-0.9.0/imod/templates/mf6/gwf-evta.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-ghb.j2` & `imod-0.9.0/imod/templates/mf6/gwf-ghb.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-lak.j2` & `imod-0.9.0/imod/templates/mf6/gwf-lak.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-maw.j2` & `imod-0.9.0/imod/templates/mf6/gwf-maw.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-mvr.j2` & `imod-0.9.0/imod/templates/mf6/gwf-mvr.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-npf.j2` & `imod-0.9.0/imod/templates/mf6/gwf-npf.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-rch.j2` & `imod-0.9.0/imod/templates/mf6/gwf-rch.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-rcha.j2` & `imod-0.9.0/imod/templates/mf6/gwf-rcha.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-riv.j2` & `imod-0.9.0/imod/templates/mf6/gwf-riv.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-sfr.j2` & `imod-0.9.0/imod/templates/mf6/gwf-sfr.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-sto.j2` & `imod-0.9.0/imod/templates/mf6/gwf-sto.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-uzf.j2` & `imod-0.9.0/imod/templates/mf6/gwf-uzf.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/gwf-wel.j2` & `imod-0.9.0/imod/templates/mf6/gwf-wel.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/sim-nam.j2` & `imod-0.9.0/imod/templates/mf6/sim-nam.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/sln-ims.j2` & `imod-0.9.0/imod/templates/mf6/sln-ims.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/mf6/utl-ts.j2` & `imod-0.9.0/imod/templates/mf6/utl-ts.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/runfile.j2` & `imod-0.9.0/imod/templates/runfile.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/templates/seawat_runfile.j2` & `imod-0.9.0/imod/templates/seawat_runfile.j2`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/util.py` & `imod-0.9.0/imod/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,30 +45,37 @@
     if pattern is not None:
         if isinstance(pattern, Pattern):
             d = pattern.match(stem).groupdict()
         else:
             pattern = pattern.lower()
             # Get the variables between curly braces
             in_curly = re.compile(r"{(.*?)}").findall(pattern)
-            regex_parts = {key: f"(?P<{key}>[\\w-]+)" for key in in_curly}
+            regex_parts = {key: f"(?P<{key}>[\\w.-]+)" for key in in_curly}
             # Format the regex string, by filling in the variables
             simple_regex = pattern.format(**regex_parts)
             re_pattern = re.compile(simple_regex)
             # Use it to get the required variables
             d = re_pattern.match(stem).groupdict()
     else:  # Default to "iMOD conventions": {name}_{time}_l{layer}
         has_layer = bool(re.search(r"_l\d+$", stem))
+        has_species = bool(
+            re.search(r"conc_\d{8,14}_c\d{1,3}", stem)
+        )  # We are strict in recognizing species
         try:  # try for time
             base_pattern = r"(?P<name>[\w-]+)_(?P<time>[0-9-]{6,})"
+            if has_species:
+                base_pattern += r"_c(?P<species>[0-9]+)"
             if has_layer:
                 base_pattern += r"_l(?P<layer>[0-9]+)"
             re_pattern = re.compile(base_pattern)
             d = re_pattern.match(stem).groupdict()
         except AttributeError:  # probably no time
             base_pattern = r"(?P<name>[\w-]+)"
+            if has_species:
+                base_pattern += r"_c(?P<species>[0-9]+)"
             if has_layer:
                 base_pattern += r"_l(?P<layer>[0-9]+)"
             re_pattern = re.compile(base_pattern)
             d = re_pattern.match(stem).groupdict()
     return d
 
 
@@ -117,48 +124,51 @@
     Alternatively, the most pragmatic solution may be to just rename your files.
     """
     path = pathlib.Path(path)
     # We'll ignore upper case
     stem = path.stem.lower()
 
     d = _groupdict(stem, pattern)
+    dims = list(d.keys())
+    # If name is not provided, generate one from other fields
+    if "name" not in d.keys():
+        d["name"] = "_".join(d.values())
+    else:
+        dims.remove("name")
 
     # TODO: figure out what to with user specified variables
     # basically type inferencing via regex?
-    # if purely numericdcal \d* -> int or float
+    # if purely numerical \d* -> int or float
     #    if \d*\.\d* -> float
     # else: keep as string
 
-    # If name is not provided, generate one from other fields
-    if "name" not in d.keys():
-        d["name"] = "_".join(d.values())
-
-    # steady-state as time identifier isn't picked up by <time>[0-9] regex, so strip from name
-    steady = False
-    if "steady-state" in d["name"]:
-        steady = True
-        d["name"] = d["name"].replace("_steady-state", "")
-        d["time"] = "steady-state"
-
     # String -> type conversion
     if "layer" in d.keys():
         d["layer"] = int(d["layer"])
-    if "time" in d.keys() and not steady:
+    if "species" in d.keys():
+        d["species"] = int(d["species"])
+    if "time" in d.keys():
         # iMOD supports two datetime formats
         # try fast options first
         try:
             try:
                 d["time"] = datetime.datetime.strptime(d["time"], "%Y%m%d%H%M%S")
             except ValueError:
                 d["time"] = datetime.datetime.strptime(d["time"], "%Y%m%d")
         except ValueError:  # Try fullblown dateutil date parser
             d["time"] = dateutil.parser.parse(d["time"])
+    if "steady-state" in d["name"]:
+        # steady-state as time identifier isn't picked up by <time>[0-9] regex
+        d["name"] = d["name"].replace("_steady-state", "")
+        d["time"] = "steady-state"
+        dims.append("time")
 
     d["extension"] = path.suffix
     d["directory"] = path.parent
+    d["dims"] = dims
     return d
 
 
 def _convert_datetimes(times, use_cftime):
     """
     Return times as np.datetime64[ns] or cftime.DatetimeProlepticGregorian
     depending on whether the dates fall within the inclusive bounds of
@@ -235,15 +245,15 @@
         if hastime:
             time = d["time"]
             if time == "steady-state":
                 d["timestr"] = time
             else:
                 # Change time to datetime.datetime
                 if isinstance(time, np.datetime64):
-                    d["time"] = time.item()
+                    d["time"] = time.astype("datetime64[us]").item()
                 elif isinstance(time, cftime.datetime):
                     # Take first six elements of timetuple and convert to datetime
                     d["time"] = datetime.datetime(*time.timetuple()[:6])
         s = pattern.format(**d)
 
     if "directory" in d:
         return pathlib.Path(d["directory"]) / s
```

### Comparing `imod-0.8.0/imod/visualize/spatial.py` & `imod-0.9.0/imod/visualize/spatial.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/adv.py` & `imod-0.9.0/imod/wq/adv.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/bas.py` & `imod-0.9.0/imod/wq/bas.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,23 +58,15 @@
         "    {%- endfor %}\n"
         "    hnoflo = {{inactive_head}}\n"
         "    {%- for layer, value in starting_head.items() %}\n"
         "    strt_l{{layer}} = {{value}}\n"
         "    {%- endfor -%}"
     )
 
-    def __init__(
-        self,
-        ibound,
-        top,
-        bottom,
-        starting_head,
-        inactive_head=1.0e30,
-        confining_bed_below=0,
-    ):
+    def __init__(self, ibound, top, bottom, starting_head, inactive_head=1.0e30):
         self._check_ibound(ibound)
         super(__class__, self).__init__()
         self["ibound"] = ibound
         self["top"] = top
         self["bottom"] = bottom
         self["starting_head"] = starting_head
         self["inactive_head"] = inactive_head
@@ -117,15 +109,15 @@
             value = util.compose(d).as_posix()
         else:
             if not da.shape == ():
                 raise ValueError("Top should either be 2d or a scalar value")
             value = float(da)
         return value
 
-    def _render_dis(self, directory):
+    def _render_dis(self, directory, confining_bed_below):
         """
         Renders part of runfile that ends up under [dis] section.
         """
         d = {}
         d["top"] = self._compose_top(directory)
         d["bottom"] = self._compose_values_layer("bottom", directory)
         d["nlay"], d["nrow"], d["ncol"] = self["ibound"].shape
@@ -135,29 +127,30 @@
             dx, _, _ = util.coord_reference(self["x"])
             dy, _, _ = util.coord_reference(self["y"])
         else:
             dx = self.coords["dx"]
             dy = self.coords["dy"]
         d["dx"] = abs(float(dx))
         d["dy"] = abs(float(dy))
+        d["confining_bed_below"] = confining_bed_below
 
         # Non-time dependent part of dis
         # Can be inferred from ibound
         _dis_template = jinja2.Template(
             "[dis]\n"
             "    nlay = {{nlay}}\n"
             "    nrow = {{nrow}}\n"
             "    ncol = {{ncol}}\n"
             "    delc_r? = {{dy}}\n"
             "    delr_c? = {{dx}}\n"
             "    top = {{top}}\n"
             "    {%- for layer, value in bottom.items() %}\n"
             "    botm_l{{layer}} = {{value}}\n"
             "    {%- endfor %}\n"
-            "    laycbd_l? = 0"
+            "    laycbd_l? = {{confining_bed_below}}"
         )
 
         return _dis_template.render(d)
 
     def thickness(self):
         """
         Computes layer thickness from top and bottom data.
```

### Comparing `imod-0.8.0/imod/wq/btn.py` & `imod-0.9.0/imod/wq/btn.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,25 +64,30 @@
     __slots__ = (
         "icbund",
         "starting_concentration",
         "porosity",
         "n_species",
         "inactive_concentration",
         "minimum_active_thickness",
+        "thickness",
     )
     _pkg_id = "btn"
 
     _mapping = (("icbund", "icbund"), ("dz", "thickness"), ("prsity", "porosity"))
 
     _template = jinja2.Template(
         "[btn]\n"
+        "    ncomp = {{n_species}}\n"  # Number of components
+        "    mcomp = {{n_species}}\n"  # Number of mobile components
         "    thkmin = {{minimum_active_thickness}}\n"
         "    cinact = {{inactive_concentration}}\n"
-        "    {%- for layer, value in starting_concentration.items() %}\n"
-        "    sconc_t1_l{{layer}} = {{value}}\n"
+        "    {%- for species, layerdict in starting_concentration.items() %}\n"
+        "        {%- for layer, value in layerdict.items() %}\n"
+        "    sconc_t{{species}}_l{{layer}} = {{value}}\n"
+        "        {%- endfor -%}\n"
         "    {%- endfor -%}\n"
         "    {%- for name, dictname in mapping -%}\n"
         "        {%- for layer, value in dicts[dictname].items() %}\n"
         "    {{name}}_l{{layer}} = {{value}}\n"
         "        {%- endfor -%}\n"
         "    {%- endfor -%}\n"
     )
@@ -100,15 +105,15 @@
         self["icbund"] = icbund
         self["starting_concentration"] = starting_concentration
         self["porosity"] = porosity
         self["n_species"] = n_species
         self["inactive_concentration"] = inactive_concentration
         self["minimum_active_thickness"] = minimum_active_thickness
 
-    def _render(self, directory, thickness):
+    def _render(self, directory):
         """
         Renders part of [btn] section that does not depend on time,
         and can be inferred without checking the BoundaryConditions.
 
         Parameters
         ----------
         directory : str
@@ -120,32 +125,45 @@
         rendered : str
         """
         d = {}
         dicts = {}
         d["mapping"] = self._mapping
         # Starting concentration also includes a species, and can't be written
         # in the same way as the other variables; _T? in the runfile
-        d["starting_concentration"] = self._compose_values_layer(
-            "starting_concentration", directory
-        )
+        if "species" in self["starting_concentration"].coords:
+            starting_concentration = {}
+
+            for i, species in enumerate(
+                self["starting_concentration"]["species"].values
+            ):
+                da = self["starting_concentration"].sel(species=species)
+                starting_concentration[i + 1] = self._compose_values_layer(
+                    "starting_concentration", directory, da=da
+                )
+
+            d["starting_concentration"] = starting_concentration
+        else:
+            d["starting_concentration"] = {
+                1: self._compose_values_layer("starting_concentration", directory)
+            }
 
         # Collect which entries are complex (multi-dim)
         data_vars = [t[1] for t in self._mapping]
         for varname in self.data_vars.keys():
             if varname == "starting_concentration":
                 continue  # skip it, as mentioned above
             if varname in data_vars:  # multi-dim entry
                 dicts[varname] = self._compose_values_layer(varname, directory)
             else:  # simple entry, just get the scalar value
                 d[varname] = self[varname].values
 
         # Add these from the outside, thickness from BasicFlow
         # layer_type from LayerPropertyFlow
         dicts["thickness"] = self._compose_values_layer(
-            "thickness", directory, da=thickness
+            "thickness", directory, da=self.thickness
         )
         d["dicts"] = dicts
         return self._template.render(d)
 
     def _pkgcheck(self, ibound=None):
         to_check = [
             "starting_concentration",
@@ -158,11 +176,13 @@
         active_cells = self["icbund"] != 0
         if (active_cells & np.isnan(self["starting_concentration"])).any():
             raise ValueError(
                 f"Active cells in icbund may not have a nan value in starting_concentration in {self}"
             )
 
         _, nlabels = scipy.ndimage.label(active_cells.values)
-        if nlabels > 1:
-            raise ValueError(
-                f"{nlabels} disconnected model domain detected in the icbund in {self}"
-            )
+
+
+#        if nlabels > 1:
+#            raise ValueError(
+#                f"{nlabels} disconnected model domain detected in the icbund in {self}"
+#            )
```

### Comparing `imod-0.8.0/imod/wq/chd.py` & `imod-0.9.0/imod/wq/chd.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/dis.py` & `imod-0.9.0/imod/wq/dis.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/drn.py` & `imod-0.9.0/imod/wq/drn.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/dsp.py` & `imod-0.9.0/imod/wq/dsp.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/ghb.py` & `imod-0.9.0/imod/wq/ghb.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/lpf.py` & `imod-0.9.0/imod/wq/lpf.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,14 +86,17 @@
         is the head that is assigned to cells that are converted to dry during a
         simulation (HDRY). Although this value plays no role in the model calculations,
         it is useful as an indicator when looking at the resulting heads that
         are output from the model. HDRY is thus similar to HNOFLO in the Basic
         Package, which is the value assigned to cells that are no-flow cells at
         the start of a model simulation.
         Default value: 1.0e20.
+    confining_bed_k_vertical : float, optional
+        is the vertical hydraulic conductivity of a Quasi-three-dimensional
+        confining bed below a layer (VKCB).
     """
 
     __slots__ = (
         "k_horizontal",
         "k_vertical",
         "horizontal_anisotropy",
         "interblock",
@@ -101,26 +104,28 @@
         "specific_storage",
         "specific_yield",
         "save_budget",
         "layer_wet",
         "interval_wet",
         "method_wet",
         "head_dry",
+        "confining_bed_k_vertical",
     )
     _pkg_id = "lpf"
 
     _mapping = (
         ("laytyp", "layer_type"),
         ("layavg", "interblock"),
         ("chani", "horizontal_anisotropy"),
         ("hk", "k_horizontal"),
         ("vka", "k_vertical"),
         ("ss", "specific_storage"),
         ("sy", "specific_yield"),
         ("laywet", "layer_wet"),
+        ("vkcb", "confining_bed_k_vertical"),
     )
 
     _template = jinja2.Template(
         "[lpf]\n"
         "    ilpfcb = {{save_budget}}\n"
         "    hdry = {{head_dry}}\n"
         "    layvka_l? = 0\n"
@@ -146,32 +151,37 @@
         specific_storage=0.0001,
         specific_yield=0.15,
         save_budget=False,
         layer_wet=0,
         interval_wet=0.001,
         method_wet="wetfactor",
         head_dry=1.0e20,
+        confining_bed_k_vertical=None,
     ):
         super(__class__, self).__init__()
         self["k_horizontal"] = k_horizontal
         self["k_vertical"] = k_vertical
         self["horizontal_anisotropy"] = horizontal_anisotropy
         self["interblock"] = interblock
         self["layer_type"] = layer_type
         self["specific_storage"] = specific_storage
         self["specific_yield"] = specific_yield
         self["save_budget"] = save_budget
         self["layer_wet"] = layer_wet
         self["interval_wet"] = interval_wet
         self["method_wet"] = method_wet
         self["head_dry"] = head_dry
+        if confining_bed_k_vertical is not None:
+            self["confining_bed_k_vertical"] = confining_bed_k_vertical
 
     def _render(self, directory, *args, **kwargs):
         d = {}
-        d["mapping"] = self._mapping
+        # Don't include absentee members (in this case confining_bed_k_vertical)
+        mapping = tuple([(k, v) for k, v in self._mapping if v in self.data_vars])
+        d["mapping"] = mapping
         dicts = {}
 
         da_vars = [t[1] for t in self._mapping]
         for varname in self.data_vars.keys():
             if varname in da_vars:
                 dicts[varname] = self._compose_values_layer(varname, directory)
             else:
@@ -186,9 +196,11 @@
         to_check = [
             "k_horizontal",
             "k_vertical",
             "horizontal_anisotropy",
             "specific_storage",
             "specific_yield",
         ]
+        if "confining_bed_k_vertical" in self.data_vars:
+            to_check.append("confining_bed_k_vertical")
         self._check_positive(to_check)
         self._check_location_consistent(to_check)
```

### Comparing `imod-0.8.0/imod/wq/model.py` & `imod-0.9.0/imod/wq/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,14 +56,34 @@
                             directory=directory / key,
                             cmap=cmap,
                             overlays=overlays,
                             quantile_colorscale=quantile_colorscale,
                             figsize=figsize,
                         )
 
+    def sel(self, **dimensions):
+        selmodel = type(self)(self.modelname, self.check)
+        for pgkname, pkg in self.items():
+            sel_dims = {k: v for k, v in dimensions.items() if k in pkg}
+            if len(this_dims) == 0:
+                selmodel[pkgname] = pkg
+            else:
+                selmodel[pkgname] = pkg.loc[sel_dims]
+        return selmodel
+
+    def isel(self, **dimensions):
+        selmodel = type(self)(self.modelname, self.check)
+        for pgkname, pkg in self.items():
+            sel_dims = {k: v for k, v in dimensions.items() if k in pkg}
+            if len(this_dims) == 0:
+                selmodel[pkgname] = pkg
+            else:
+                selmodel[pkgname] = pkg[sel_dims]
+        return selmodel
+
 
 class SeawatModel(Model):
     """
     Attributes
     ----------
     modelname : str
     check : str, optional
@@ -283,15 +303,22 @@
         return self[pkgkey]._render(
             directory=directory / pkgkey, globaltimes=globaltimes
         )
 
     def _render_dis(self, directory, globaltimes):
         baskey = self._get_pkgkey("bas6")
         diskey = self._get_pkgkey("dis")
-        bas_content = self[baskey]._render_dis(directory=directory.joinpath(baskey))
+        lpfkey = self._get_pkgkey("lpf")
+        if "confining_bed_k_vertical" in self[lpfkey].data_vars:
+            cbb = 1
+        else:
+            cbb = 0
+        bas_content = self[baskey]._render_dis(
+            directory=directory.joinpath(baskey), confining_bed_below=cbb
+        )
         dis_content = self[diskey]._render(globaltimes=globaltimes)
         return bas_content + dis_content
 
     def _render_groups(self, directory, globaltimes):
         baskey = self._get_pkgkey("bas6")
         nlayer = self[baskey]["ibound"].shape[0]
         package_groups = self._group()
@@ -320,21 +347,19 @@
             self[pksfkey]._compute_load_balance_weight(self[baskey]["ibound"])
             return self[pksfkey]._render(directory=directory.joinpath(pksfkey))
 
     def _render_btn(self, directory, globaltimes):
         baskey = self._get_pkgkey("bas6")
         btnkey = self._get_pkgkey("btn")
         diskey = self._get_pkgkey("dis")
-        thickness = self[baskey].thickness()
+        self[btnkey]["thickness"] = self[baskey].thickness()
 
         if btnkey is None:
             raise ValueError("No BasicTransport package provided.")
-        btn_content = self[btnkey]._render(
-            directory=directory.joinpath(btnkey), thickness=thickness
-        )
+        btn_content = self[btnkey]._render(directory=directory.joinpath(btnkey))
         dis_content = self[diskey]._render_btn(globaltimes=globaltimes)
         return btn_content + dis_content
 
     def _render_transportsolver(self, directory):
         gcgkey = self._get_pkgkey("gcg")
         pkstkey = self._get_pkgkey("pkst")
         if gcgkey and pkstkey:
```

### Comparing `imod-0.8.0/imod/wq/oc.py` & `imod-0.9.0/imod/wq/oc.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/pkgbase.py` & `imod-0.9.0/imod/wq/pkgbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,41 +89,51 @@
         Returns
         -------
         values : dict
             Dictionary containing the {layer number: path to file}.
             Alternatively: {layer number: scalar value}. The layer number may be
             a wildcard (e.g. '?').
         """
+        pattern = "{name}"
+
         values = {}
         if da is None:
             da = self[varname]
 
         d = {"directory": directory, "name": varname, "extension": ".idf"}
+
+        if "species" in da.coords:
+            d["species"] = da.coords["species"].values
+            pattern += "_c{species}"
+
         if time is not None:
             d["time"] = time
+            pattern += "_{time:%Y%m%d%H%M%S}"
 
         # Scalar value or not?
         # If it's a scalar value we can immediately write
         # otherwise, we have to write a file path
         if "y" not in da.coords and "x" not in da.coords:
             idf = False
         else:
             idf = True
 
         if "layer" not in da.coords:
             if idf:
-                values["?"] = util.compose(d).as_posix()
+                pattern += "{extension}"
+                values["?"] = util.compose(d, pattern=pattern).as_posix()
             else:
                 values["?"] = da.values[()]
 
         else:
+            pattern += "_l{layer}{extension}"
             for layer in np.atleast_1d(da.coords["layer"].values):
                 if idf:
                     d["layer"] = layer
-                    values[layer] = util.compose(d).as_posix()
+                    values[layer] = util.compose(d, pattern=pattern).as_posix()
                 else:
                     if "layer" in da.dims:
                         values[layer] = da.sel(layer=layer).values[()]
                     else:
                         values[layer] = da.values[()]
 
         return values
@@ -148,15 +158,28 @@
     def save(self, directory):
         for name, da in self.data_vars.items():
             if "y" in da.coords and "x" in da.coords:
                 path = pathlib.Path(directory).joinpath(name)
                 if isinstance(da, xr.DataArray):
                     if "layer" in da.dims:
                         da = da.dropna(dim="layer", how="all")
-                imod.idf.save(path, da)
+
+                if "species" in da.coords:
+                    if "time" in da.coords:
+                        imod.idf.save(
+                            path,
+                            da,
+                            pattern="{name}_c{species}_{time:%Y%m%d%H%M%S}_l{layer}{extension}",
+                        )
+                    else:
+                        imod.idf.save(
+                            path, da, pattern="{name}_c{species}_l{layer}{extension}"
+                        )
+                else:
+                    imod.idf.save(path, da)
 
     def _check_positive(self, varnames):
         for var in varnames:
             # Take care with nan values
             if (self[var] < 0).any():
                 raise ValueError(f"{var} in {self} must be positive")
 
@@ -213,14 +236,23 @@
         "        {%- for time, timedict in dicts[dictname].items() -%}"
         "            {%- for layer, value in timedict.items() %}\n"
         "    {{name}}_p{{time}}_s{{system_index}}_l{{layer}} = {{value}}\n"
         "            {%- endfor -%}\n"
         "        {%- endfor -%}"
         "    {%- endfor -%}"
     )
+    _ssm_template = jinja2.Template(
+        "{%- for species, timedict in concentration.items() -%}"
+        "    {%- for time, layerdict in timedict.items() -%}"
+        "       {%- for layer, value in layerdict.items() %}\n"
+        "    c{{pkg_id}}_t{{species}}_p{{time}}_l{{layer}} = {{value}}\n"
+        "        {%- endfor -%}"
+        "    {%- endfor -%}"
+        "{%- endfor -%}"
+    )
 
     def _add_timemap(self, varname, value, use_cftime):
         if value is not None:
             if varname not in self:
                 raise ValueError(
                     f"{varname} does not occur in {self}\n cannot add timemap"
                 )
@@ -286,18 +318,20 @@
                 runfile_times = np.concatenate([da_times, timemap_values])[inds]
             else:
                 runfile_times = package_times = da_times
 
             starts_ends = timeutil.forcing_starts_ends(package_times, globaltimes)
 
             for time, start_end in zip(runfile_times, starts_ends):
-                values[start_end] = self._compose_values_layer(varname, directory, time)
+                values[start_end] = self._compose_values_layer(
+                    varname, directory, time=time, da=da
+                )
 
         else:
-            values["?"] = self._compose_values_layer(varname, directory)
+            values["?"] = self._compose_values_layer(varname, directory, da=da)
 
         return values
 
     def _max_active_n(self, varname, nlayer):
         """
         Determine the maximum active number of cells that are active
         during a stress period.
@@ -375,16 +409,15 @@
         rendered : str
             The rendered runfile SSM part for a single boundary condition system.
         """
 
         if "concentration" not in self:
             return ""
 
-        d = {}
-        d["pkg_id"] = self._pkg_id
+        d = {"pkg_id": self._pkg_id}
         if "species" in self["concentration"].coords:
             concentration = {}
             for i, species in enumerate(self["concentration"]["species"].values):
                 concentration[i + 1] = self._compose_values_timelayer(
                     varname="concentration",
                     da=self["concentration"].sel(species=species),
                     globaltimes=globaltimes,
@@ -397,18 +430,8 @@
                     da=self["concentration"],
                     globaltimes=globaltimes,
                     directory=directory,
                 )
             }
         d["concentration"] = concentration
 
-        _ssm_template = jinja2.Template(
-            "{%- for species, timedict in concentration.items() -%}"
-            "    {%- for time, layerdict in timedict.items() -%}"
-            "       {%- for layer, value in layerdict.items() %}\n"
-            "    c{{pkg_id}}_t{{species}}_p{{time}}_l{{layer}} = {{value}}\n"
-            "        {%- endfor -%}"
-            "    {%- endfor -%}"
-            "{%- endfor -%}"
-        )
-
-        return _ssm_template.render(d)
+        return self._ssm_template.render(d)
```

### Comparing `imod-0.8.0/imod/wq/pkggroup.py` & `imod-0.9.0/imod/wq/pkggroup.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/rch.py` & `imod-0.9.0/imod/wq/rch.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/riv.py` & `imod-0.9.0/imod/wq/riv.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/slv.py` & `imod-0.9.0/imod/wq/slv.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/timeutil.py` & `imod-0.9.0/imod/wq/timeutil.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/vdf.py` & `imod-0.9.0/imod/wq/vdf.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/wq/__init__.py` & `imod-0.9.0/imod/wq/__init__.py`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/imod/__init__.py` & `imod-0.9.0/imod/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pathlib
+import pkg_resources
 import warnings
 
 import numpy as np
 import pandas as pd
 
 # submodules
 from imod import idf
@@ -17,18 +18,19 @@
 import imod.flow
 import imod.prepare
 import imod.mf6
 import imod.wq
 import imod.select
 import imod.visualize
 
-from imod._version import get_versions
-
-__version__ = get_versions()["version"]
-del get_versions
+try:
+    __version__ = pkg_resources.get_distribution(__name__).version
+except pkg_resources.DistributionNotFound:
+    # package is not installed
+    pass
 
 
 def write(path, model, name=None, runfile_parameters=None):
     warnings.warn("imod.write is moved, use imod.flow.write instead.", FutureWarning)
     return imod.flow.write(
         path, model, name=name, runfile_parameters=runfile_parameters
     )
```

### Comparing `imod-0.8.0/imod.egg-info/PKG-INFO` & `imod-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: imod
-Version: 0.8.0
-Summary: Work with iMOD MODFLOW models
+Version: 0.9.0
+Summary: Make massive MODFLOW models
 Home-page: https://gitlab.com/deltares/imod/imod-python
 Author: Martijn Visser
 Author-email: martijn.visser@deltares.nl
 License: MIT
 Description: .. image:: https://gitlab.com/deltares/imod/imod-python/badges/master/pipeline.svg
            :target: https://gitlab.com/deltares/imod/imod-python/commits/master
         .. image:: https://gitlab.com/deltares/imod/imod-python/badges/master/coverage.svg
            :target: https://gitlab.com/deltares/imod/imod-python/commits/master
+        .. image:: https://mybinder.org/badge_logo.svg
+           :target: https://mybinder.org/v2/gh/Deltares/iMOD-DSD-International-2019/master
         
         Work with `iMOD <https://oss.deltares.nl/web/imod>`__ MODFLOW models in
         Python.
         
         Documentation: https://imod.xyz/
         
         Source code: https://gitlab.com/deltares/imod/imod-python
@@ -71,15 +73,15 @@
         This Python package was written primarily by Martijn Visser and Huite Bootsma at Deltares.
         
 Keywords: imod modflow groundwater modeling
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Provides-Extra: dev
```

### Comparing `imod-0.8.0/LICENSE` & `imod-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imod-0.8.0/PKG-INFO` & `imod-0.9.0/imod.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: imod
-Version: 0.8.0
-Summary: Work with iMOD MODFLOW models
+Version: 0.9.0
+Summary: Make massive MODFLOW models
 Home-page: https://gitlab.com/deltares/imod/imod-python
 Author: Martijn Visser
 Author-email: martijn.visser@deltares.nl
 License: MIT
 Description: .. image:: https://gitlab.com/deltares/imod/imod-python/badges/master/pipeline.svg
            :target: https://gitlab.com/deltares/imod/imod-python/commits/master
         .. image:: https://gitlab.com/deltares/imod/imod-python/badges/master/coverage.svg
            :target: https://gitlab.com/deltares/imod/imod-python/commits/master
+        .. image:: https://mybinder.org/badge_logo.svg
+           :target: https://mybinder.org/v2/gh/Deltares/iMOD-DSD-International-2019/master
         
         Work with `iMOD <https://oss.deltares.nl/web/imod>`__ MODFLOW models in
         Python.
         
         Documentation: https://imod.xyz/
         
         Source code: https://gitlab.com/deltares/imod/imod-python
@@ -71,15 +73,15 @@
         This Python package was written primarily by Martijn Visser and Huite Bootsma at Deltares.
         
 Keywords: imod modflow groundwater modeling
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Provides-Extra: dev
```

### Comparing `imod-0.8.0/README.rst` & `imod-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 .. image:: https://gitlab.com/deltares/imod/imod-python/badges/master/pipeline.svg
    :target: https://gitlab.com/deltares/imod/imod-python/commits/master
 .. image:: https://gitlab.com/deltares/imod/imod-python/badges/master/coverage.svg
    :target: https://gitlab.com/deltares/imod/imod-python/commits/master
+.. image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/Deltares/iMOD-DSD-International-2019/master
 
 Work with `iMOD <https://oss.deltares.nl/web/imod>`__ MODFLOW models in
 Python.
 
 Documentation: https://imod.xyz/
 
 Source code: https://gitlab.com/deltares/imod/imod-python
```

### Comparing `imod-0.8.0/setup.py` & `imod-0.9.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from setuptools import setup, find_packages
-import versioneer
 
 with open("README.rst") as f:
     long_description = f.read()
 
 setup(
     name="imod",
-    version=versioneer.get_version(),
-    cmdclass=versioneer.get_cmdclass(),
-    description="Work with iMOD MODFLOW models",
+    description="Make massive MODFLOW models",
     long_description=long_description,
     url="https://gitlab.com/deltares/imod/imod-python",
     author="Martijn Visser",
     author_email="martijn.visser@deltares.nl",
     license="MIT",
     packages=find_packages(),
     package_dir={"imod": "imod"},
     package_data={"imod": ["templates/*.j2", "templates/mf6/*.j2"]},
     test_suite="tests",
+    use_scm_version=True,
+    setup_requires=["setuptools_scm"],
     python_requires=">=3.6",
     install_requires=[
         "numba",
         "numpy",
         "scipy",
         "matplotlib",
         "xarray>=0.11",
@@ -47,15 +46,15 @@
         "optional": ["rasterio>=1", "geopandas"],
     },
     classifiers=[
         # https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
-        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Hydrology",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     keywords="imod modflow groundwater modeling",
```

