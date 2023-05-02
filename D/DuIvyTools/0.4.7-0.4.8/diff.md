# Comparing `tmp/DuIvyTools-0.4.7.tar.gz` & `tmp/DuIvyTools-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DuIvyTools-0.4.7.tar", last modified: Fri Oct 28 14:56:48 2022, max compression
+gzip compressed data, was "dist\DuIvyTools-0.4.8.tar", last modified: Tue May  2 07:56:19 2023, max compression
```

## Comparing `DuIvyTools-0.4.7.tar` & `DuIvyTools-0.4.8.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2022-10-28 14:56:48.370106 DuIvyTools-0.4.7/
-drwxrwxrwx   0        0        0        0 2022-10-28 14:56:48.308285 DuIvyTools-0.4.7/DuIvyTools/
--rw-rw-rw-   0        0        0     8214 2022-10-28 13:29:58.000000 DuIvyTools-0.4.7/DuIvyTools/DCCM.py
--rw-rw-rw-   0        0        0     3569 2022-10-28 14:18:08.000000 DuIvyTools-0.4.7/DuIvyTools/DIT.py
--rw-rw-rw-   0        0        0     5598 2022-10-28 14:18:08.000000 DuIvyTools-0.4.7/DuIvyTools/FindCenter.py
--rw-rw-rw-   0        0        0    34672 2022-10-28 14:56:10.000000 DuIvyTools-0.4.7/DuIvyTools/HELP.py
--rw-rw-rw-   0        0        0    12422 2022-10-28 13:29:58.000000 DuIvyTools-0.4.7/DuIvyTools/HydrogenBond.py
--rw-rw-rw-   0        0        0     4096 2022-10-28 13:29:58.000000 DuIvyTools-0.4.7/DuIvyTools/MDP.py
--rw-rw-rw-   0        0        0     7718 2022-10-28 13:29:58.000000 DuIvyTools-0.4.7/DuIvyTools/MolMap.py
--rw-rw-rw-   0        0        0     1980 2022-10-28 13:29:58.000000 DuIvyTools-0.4.7/DuIvyTools/MplStyle.py
--rw-rw-rw-   0        0        0    17864 2022-10-28 14:18:08.000000 DuIvyTools-0.4.7/DuIvyTools/NDX.py
--rw-rw-rw-   0        0        0    28372 2022-10-28 13:29:58.000000 DuIvyTools-0.4.7/DuIvyTools/PipiDistAng.py
--rw-rw-rw-   0        0        0    34347 2022-10-28 13:29:58.000000 DuIvyTools-0.4.7/DuIvyTools/XPM.py
--rw-rw-rw-   0        0        0    59135 2022-10-28 13:29:58.000000 DuIvyTools-0.4.7/DuIvyTools/XVG.py
--rw-rw-rw-   0        0        0     1575 2022-10-28 13:29:58.000000 DuIvyTools-0.4.7/DuIvyTools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-28 14:56:48.363151 DuIvyTools-0.4.7/DuIvyTools/data/
--rw-rw-rw-   0        0        0      620 2022-10-28 13:29:58.000000 DuIvyTools-0.4.7/DuIvyTools/data/DIT.mplstyle
--rw-rw-rw-   0        0        0    10902 2022-03-06 14:03:31.000000 DuIvyTools-0.4.7/DuIvyTools/data/blank.mdp
--rw-rw-rw-   0        0        0     1307 2022-03-06 14:03:51.000000 DuIvyTools-0.4.7/DuIvyTools/data/em.mdp
--rw-rw-rw-   0        0        0     1161 2022-03-06 14:04:18.000000 DuIvyTools-0.4.7/DuIvyTools/data/ions.mdp
--rw-rw-rw-   0        0        0     3605 2022-07-07 10:51:11.000000 DuIvyTools-0.4.7/DuIvyTools/data/md.mdp
--rw-rw-rw-   0        0        0     3539 2022-07-07 10:51:11.000000 DuIvyTools-0.4.7/DuIvyTools/data/npt.mdp
--rw-rw-rw-   0        0        0     3293 2022-07-07 10:51:11.000000 DuIvyTools-0.4.7/DuIvyTools/data/nvt.mdp
--rw-rw-rw-   0        0        0   883814 2022-02-18 07:28:53.000000 DuIvyTools-0.4.7/DuIvyTools/data/pref_general.data
--rw-rw-rw-   0        0        0   926970 2022-02-18 07:28:53.000000 DuIvyTools-0.4.7/DuIvyTools/data/pref_glycine.data
--rw-rw-rw-   0        0        0   695254 2022-02-18 07:28:53.000000 DuIvyTools-0.4.7/DuIvyTools/data/pref_preproline.data
--rw-rw-rw-   0        0        0   641990 2022-02-18 07:28:53.000000 DuIvyTools-0.4.7/DuIvyTools/data/pref_proline.data
-drwxrwxrwx   0        0        0        0 2022-10-28 14:56:48.329246 DuIvyTools-0.4.7/DuIvyTools.egg-info/
--rw-rw-rw-   0        0        0     4040 2022-10-28 14:56:48.000000 DuIvyTools-0.4.7/DuIvyTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      810 2022-10-28 14:56:48.000000 DuIvyTools-0.4.7/DuIvyTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-28 14:56:48.000000 DuIvyTools-0.4.7/DuIvyTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2022-10-28 14:56:48.000000 DuIvyTools-0.4.7/DuIvyTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       72 2022-10-28 14:56:48.000000 DuIvyTools-0.4.7/DuIvyTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-10-28 14:56:48.000000 DuIvyTools-0.4.7/DuIvyTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4040 2022-10-28 14:56:48.368095 DuIvyTools-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     2573 2022-10-28 14:18:08.000000 DuIvyTools-0.4.7/README.md
--rw-rw-rw-   0        0        0       42 2022-10-28 14:56:48.370106 DuIvyTools-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1734 2022-10-28 13:29:58.000000 DuIvyTools-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:56:19.642347 DuIvyTools-0.4.8/
+drwxrwxrwx   0        0        0        0 2023-05-02 07:56:19.529783 DuIvyTools-0.4.8/DuIvyTools/
+-rw-rw-rw-   0        0        0     8214 2022-10-28 13:29:58.000000 DuIvyTools-0.4.8/DuIvyTools/DCCM.py
+-rw-rw-rw-   0        0        0     3694 2023-05-02 06:52:04.000000 DuIvyTools-0.4.8/DuIvyTools/DIT.py
+-rw-rw-rw-   0        0        0     6995 2023-05-01 10:10:30.000000 DuIvyTools-0.4.8/DuIvyTools/DSSP.py
+-rw-rw-rw-   0        0        0     5598 2022-10-28 14:18:08.000000 DuIvyTools-0.4.8/DuIvyTools/FindCenter.py
+-rw-rw-rw-   0        0        0    39729 2023-05-01 10:10:30.000000 DuIvyTools-0.4.8/DuIvyTools/HELP.py
+-rw-rw-rw-   0        0        0    25647 2023-05-01 10:10:31.000000 DuIvyTools-0.4.8/DuIvyTools/HydrogenBond.py
+-rw-rw-rw-   0        0        0     4096 2022-10-28 13:29:58.000000 DuIvyTools-0.4.8/DuIvyTools/MDP.py
+-rw-rw-rw-   0        0        0     7718 2022-10-28 13:29:58.000000 DuIvyTools-0.4.8/DuIvyTools/MolMap.py
+-rw-rw-rw-   0        0        0     1980 2022-10-28 13:29:58.000000 DuIvyTools-0.4.8/DuIvyTools/MplStyle.py
+-rw-rw-rw-   0        0        0    17864 2022-10-28 14:18:08.000000 DuIvyTools-0.4.8/DuIvyTools/NDX.py
+-rw-rw-rw-   0        0        0    28372 2022-10-28 13:29:58.000000 DuIvyTools-0.4.8/DuIvyTools/PipiDistAng.py
+-rw-rw-rw-   0        0        0    37040 2023-05-01 10:10:31.000000 DuIvyTools-0.4.8/DuIvyTools/XPM.py
+-rw-rw-rw-   0        0        0    62830 2023-05-01 10:10:32.000000 DuIvyTools-0.4.8/DuIvyTools/XVG.py
+-rw-rw-rw-   0        0        0     1575 2022-10-28 13:29:58.000000 DuIvyTools-0.4.8/DuIvyTools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:56:19.632146 DuIvyTools-0.4.8/DuIvyTools/data/
+-rw-rw-rw-   0        0        0      716 2022-11-02 03:49:56.000000 DuIvyTools-0.4.8/DuIvyTools/data/DIT.mplstyle
+-rw-rw-rw-   0        0        0    10902 2022-03-06 14:03:31.000000 DuIvyTools-0.4.8/DuIvyTools/data/blank.mdp
+-rw-rw-rw-   0        0        0     1307 2023-05-02 07:55:42.000000 DuIvyTools-0.4.8/DuIvyTools/data/em.mdp
+-rw-rw-rw-   0        0        0     1161 2022-03-06 14:04:18.000000 DuIvyTools-0.4.8/DuIvyTools/data/ions.mdp
+-rw-rw-rw-   0        0        0     3602 2023-05-02 07:55:14.000000 DuIvyTools-0.4.8/DuIvyTools/data/md.mdp
+-rw-rw-rw-   0        0        0     3657 2023-05-02 07:54:41.000000 DuIvyTools-0.4.8/DuIvyTools/data/npt.mdp
+-rw-rw-rw-   0        0        0     3368 2023-05-02 07:53:50.000000 DuIvyTools-0.4.8/DuIvyTools/data/nvt.mdp
+-rw-rw-rw-   0        0        0   883814 2022-02-18 07:28:53.000000 DuIvyTools-0.4.8/DuIvyTools/data/pref_general.data
+-rw-rw-rw-   0        0        0   926970 2022-02-18 07:28:53.000000 DuIvyTools-0.4.8/DuIvyTools/data/pref_glycine.data
+-rw-rw-rw-   0        0        0   695254 2022-02-18 07:28:53.000000 DuIvyTools-0.4.8/DuIvyTools/data/pref_preproline.data
+-rw-rw-rw-   0        0        0   641990 2022-02-18 07:28:53.000000 DuIvyTools-0.4.8/DuIvyTools/data/pref_proline.data
+drwxrwxrwx   0        0        0        0 2023-05-02 07:56:19.548476 DuIvyTools-0.4.8/DuIvyTools.egg-info/
+-rw-rw-rw-   0        0        0     5122 2023-05-02 07:56:19.000000 DuIvyTools-0.4.8/DuIvyTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-05-02 07:56:19.000000 DuIvyTools-0.4.8/DuIvyTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 07:56:19.000000 DuIvyTools-0.4.8/DuIvyTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-02 07:56:19.000000 DuIvyTools-0.4.8/DuIvyTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       72 2023-05-02 07:56:19.000000 DuIvyTools-0.4.8/DuIvyTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-02 07:56:19.000000 DuIvyTools-0.4.8/DuIvyTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5122 2023-05-02 07:56:19.640354 DuIvyTools-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3535 2023-05-02 07:39:17.000000 DuIvyTools-0.4.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 07:56:19.643343 DuIvyTools-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1734 2023-05-02 07:44:11.000000 DuIvyTools-0.4.8/setup.py
```

### Comparing `DuIvyTools-0.4.7/DuIvyTools/DCCM.py` & `DuIvyTools-0.4.8/DuIvyTools/DCCM.py`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/DIT.py` & `DuIvyTools-0.4.8/DuIvyTools/DIT.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from DuIvyTools.MDP import mdp_call_functions
 from DuIvyTools.HELP import help_call_functions, get_welcome_msg
 from DuIvyTools.PipiDistAng import pipi_dist_ang_call_functions
 from DuIvyTools.FindCenter import find_center_call_functions
 from DuIvyTools.HydrogenBond import hbond_call_functions
 from DuIvyTools.MolMap import mol_map_call_functions
 from DuIvyTools.DCCM import dccm_call_functions
+from DuIvyTools.DSSP import dssp_call_functions
 from DuIvyTools.MplStyle import mplstyle_call_functions
 
 
 logging.basicConfig(level=logging.INFO, format="%(levelname)s -> %(message)s")
 logger = logging.getLogger(__name__)
 
 
@@ -85,13 +86,15 @@
             find_center_call_functions(arguments)
         elif method == "hbond":
             hbond_call_functions(arguments)
         elif method == "mol_map":
             mol_map_call_functions(arguments)
         elif method == "dccm_ascii":
             dccm_call_functions(arguments)
+        elif method == "dssp":
+            dssp_call_functions(arguments)
         else:
             logging.error("unknown command {}".format(method))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DuIvyTools-0.4.7/DuIvyTools/FindCenter.py` & `DuIvyTools-0.4.8/DuIvyTools/FindCenter.py`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/HELP.py` & `DuIvyTools-0.4.8/DuIvyTools/HELP.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,24 +23,27 @@
 
         self.help_infos = {
             "xvg_show": """
 xvg_show: draw xvg data into line figures.
 
 :examples: 
     dit xvg_show -f test.xvg
+    dit xvg_show -f test.xvg --subplot
     dit xvg_show -f test.xvg -o test.png -ns
 
 :parameters:
     -f, --input
             specify the xvg file for input.
     -o, --output (optional)
             specify the output figure name. Figure will be saved in 300 dpi.
     -ns, --noshow (optional)
             if -ns is specified, figure won't be shown on screen. Usually work
             with -o to save figure directly.
+    -subplot, --subplot (optional)
+            whether to draw different data in subplots.
 """,
             "xvg_compare": """
 xvg_compare: comparison of xvg files, draw different data columns you selected
              into line figure.
 
 :examples:
     dit xvg_compare -f f1.xvg f2.xvg -c 1,2 2,3,4 -l l1 l2 l3 l4 l5
@@ -88,14 +91,22 @@
             specify the transparency for plotting confidence interval. 
             default == 0.4, only valid when -smv specified. 
     -o, --output (optional)
             specify the output figure name. Figure will be saved in 300 dpi.
     -ns, --noshow (optional)
             if -ns is specified, figure won't be shown on screen. Usually work
             with -o to save figure directly.
+    -xs, --xshrink (optional)
+            specify a factor for multiplication of x-axis. default == 1.0
+            For instance, if "-xs 0.001" is specified, all x-axis value of xvg
+            will multiply this value. x-axis 1000 will be shown as 1. 
+            Useful for converting the unit (ps) of time into (ns). Don't forget
+            to change xlabel too after specifing -xs.
+            I advise you'd better to use -tu in gmx commands for convertion of 
+            unit of x-axis.
 """,
             "xvg_ave": """
 xvg_ave: calculate the average of each column in xvg file.
 
 :examples:
     dit xvg_ave -f f1.xvg
     dit xvg_ave -f f1.xvg -s 1000 -e 2000
@@ -211,32 +222,48 @@
             specify the row index of column data which you want to stop 
             calculation.
     -o, --output (optional)
             specify the output figure name. Figure will be saved in 300 dpi.
     -ns, --noshow (optional)
             if -ns is specified, figure won't be shown on screen. Usually work
             with -o to save figure directly.
+    -xs, --xshrink (optional)
+            specify a factor for multiplication of x-axis. default == 1.0
+            For instance, if "-xs 0.001" is specified, all x-axis value of xvg
+            will multiply this value. x-axis 1000 will be shown as 1. 
+            Useful for converting the unit (ps) of time into (ns). Don't forget
+            to change xlabel too after specifing -xs.
+            I advise you'd better to use -tu in gmx commands for convertion of 
+            unit of x-axis.
+    -x, --xlabel (optional)
+            specify the x-label you want to show in figure.
+    -y, --ylabel (optional)
+            specify the y-label you want to show in figure.
 """,
             "xvg_show_scatter": """
 xvg_show_scatter: draw scatter figure.
 
 :examples:
     dit xvg_show_scatter -f f1.xvg -xi 0 -yi 1
+    dit xvg_show_scatter -f f1.xvg -xi 1 -yi 2 -c 0
     dit xvg_show_scatter -f f1.xvg -xi 0 -yi 1 -o test.png -ns
 
 :parameters:
     -f, --input
             specify the xvg file for input. 
             Only the first file is valid, others will be dropped.
     -xi, --x_index (optional)
             specify the index of column which you want to use as x data. 
             default == 0
     -yi, --y_index (optional)
             specify the index of column which you want to use as y data. 
             default == 1
+    -c, --column_select (optional)
+            specify the index of column which you want to use as color 
+            mapping, select only one index
     -o, --output (optional)
             specify the output figure name. Figure will be saved in 300 dpi.
     -ns, --noshow (optional)
             if -ns is specified, figure won't be shown on screen. Usually work
             with -o to save figure directly.
 """,
             "xvg_energy_compute": """
@@ -437,14 +464,43 @@
             For instance, if "-xs 0.001" is specified, all x-axis value of xpm
             will multiply this value. x-axis 1000 will be shown as 1. 
             Useful for converting the unit (ps) of time into (ns). Don't forget
             to change xlabel too after specifing -xs.
             I advise you'd better to use -tu in gmx commands for convertion of 
             unit of x-axis.
 """,
+            "xpm2dat": """
+xpm2dat: convert xpm file into N*N data file. 
+         when number of x-axis (or y-axis) is 1 more than width (or height) of
+         figure, the intermediate value of two adjacent values of x-axis (or
+         y-axis) will be calculated to suit the width (or height).
+
+:examples:
+    dit xpm2dat -f f1.xpm -o test.dat
+    dit xpm2dat -f f1.xpm -o test.dat -x xlabel -y ylabel
+    dit xpm2dat -f f1.xpm -o test.dat -x xlabel -xs 0.001
+
+:parameters:
+    -f, --input
+            specify the xpm file for input. 
+    -o, --output
+            specify the output dat file name.
+    -x, --xlabel (optional)
+            specify the x-label you want to write to csv file.
+    -y, --ylabel (optional)
+            specify the y-label you want to write to csv file.
+    -xs, --xshrink (optional)
+            specify a factor for multiplication of x-axis. default == 1.0
+            For instance, if "-xs 0.001" is specified, all x-axis value of xpm
+            will multiply this value. x-axis 1000 will be shown as 1. 
+            Useful for converting the unit (ps) of time into (ns). Don't forget
+            to change xlabel too after specifing -xs.
+            I advise you'd better to use -tu in gmx commands for convertion of 
+            unit of x-axis.
+""",
             "xpm2gpl": """
 xpm2gpl: convert xpm file into gnuplot script.
 
 :examples:
     dit xpm2gpl -f f1.xpm -o test.gpl
     dit xpm2gpl -f f1.xpm -o test.gpl -x xlabel -y ylabel -t title
     dit xpm2gpl -f f1.xpm -o test.gpl -x xlabel -xs 0.001
@@ -614,68 +670,57 @@
 :parameters:
     -o, --output
             specify an output mdp file to save the results.
     -a, --application
             specify the applications you want to use mdp file for. You can 
             select from: ions, em, nvt, npt, md, blank
 """,
-            "find_center": """
-find_center: find the center point and one atom which is nearest to the center
-             point from the gro file you specified. 
-
-:examples:
-    dit find_center -f test.gro 
-
-:parameters:
-    -f, --input
-            specify the gro file which only contain the molecule you want to 
-            find center point with
-""",
             "pipi_dist_ang": """
 pipi_dist_ang: to calculate the distance and angles between two rings or between 
                one ring and one vector defined by atom group or command line.
 
 :examples:
     dit pipi_dist_ang -f test.gro -n test.ndx 
     dit pipi_dist_ang -f test.gro -n test.ndx -select ring1 ring2
     dit pipi_dist_ang -f test.gro -n test.ndx -select ring1 -vg
     dit pipi_dist_ang -f test.gro -n test.ndx -select ring1 -vec 6 6 6 
 
 :parameters:
     -f, --input
             the gro file which contains frames of molecule coordinates
     -n, --index
-            the index file which contains atom index groups of rings or vector groups
-    -b
+            the index file which contains atom index groups of rings or 
+            vector groups
+    -b (optional)
             the frame number to start calculation, default=0
-    -dt
+    -dt (optional)
             the frame interval, default=1
     -o, --output
             the output filename to save results
-    -vg
+    -vg (optional)
             whether to get vector from index group, default=False
-    -vec
+    -vec (optional)
             specify the vector by command line, eg. -vec 6 6 6 
-    -select 
+    -select (optional)
             select the groups from command line
 """,
             "find_center": """
 find_center: to find the atom which is nearest to center of atom group. 
 
 :examples:
     dit find_center -f test.gro
     dit find_center -f test.gro -n index.ndx
     dit find_center -f test.gro -n index.ndx -aa
 
 :parameters:
     -f, --input
             the gro file which contains one frame of molecule coordinates
-    -n, --index
+    -n, --index (optional)
             the index file which you could select group from
-    -aa, --AllAtoms
+    -aa, --AllAtoms (optional)
             if to find center of one group atoms in all atoms
 """,
             "hbond": """
 hbond: A useful method to process hbond related files generated by `gmx hbond`,
         you can get hbond occupancy figure and table infos from `dit hbond`. 
         note: the hbond names will show on figure only when number of hbonds 
               less than 10. 
@@ -685,46 +730,70 @@
     dit hbond -f md.gro -n hbond.ndx -m hbmap.xpm -c 5 7 
     dit hbond -f md.gro -n hbond.ndx -m hbmap.xpm -c 5 7 0-3
     dit hbond -f md.gro -n hbond.ndx -m hbmap.xpm -o test.png -csv test.csv -ns
     dit hbond -f md.gro -n hbond.ndx -m hbmap.xpm -hnf d_resname(d_resnum)@d_atomname(d_atomnum)->h_atomname(h_atomnum)...a_resname(a_resnum)@a_atomname(a_atomnum) 
     dit hbond -f md.gro -n hbond.ndx -m hbmap.xpm -hnf "d_resname@d_atomname -> h_atomname ... a_resname@a_atomname" 
     dit hbond -f md.gro -n hbond.ndx -m hbmap.xpm -hnf "d_atomname@h_atomname -> a_atomname" 
     dit hbond -f md.gro -n hbond.ndx -m hbmap.xpm -hnf "number" 
+    dit hbond -f md.gro -n hbond.ndx -m hbmap.xpm -hnf id -so AND0,2,5-7
+    dit hbond -f md.gro -n hbond.ndx -m hbmap.xpm -hnf id -so OR0,2,5-7
 
 :parameters:
     -f, --input
             the gro file which contains one frame of molecule coordinates, 
             used to get atom names.
     -n, --index
             the index file generated by `gmx hbond`
     -m, --map
             the hbond map file (hbmap.xpm) generated by `gmx hbond`
-    -c, --select
+    -c, --select (optional)
             select the hbond id to only show the selected hbonds
-    -o, --output
+    -o, --output (optional)
             the figure name you want to save
-    -csv, --csv
+    -csv, --csv (optional)
             save the table infos into a csv whose name is specified here
-    -ns, --noshow
+    -ns, --noshow (optional)
             whether not to show figure, useful on computer without gui
-    -hnf, --hbond_name_format 
+    -hnf, --hbond_name_format (optional)
             define the hbond name format by user! 
             Each atom has four features: resname, resnum, atomname, atomnum. 
             Distinguish donor, hydrogen, acceptor by adding one prefix to each
             feature, like: d_resname, a_resnum, h_atomname. So you may able to
             define hbond name style by: 
             'd_resname(d_resnum)@d_atomname(d_atomnum)->h_atomname(h_atomnum)...a_resname(a_resnum)@a_atomname(a_atomnum)' 
             which is the default style, or also you could specify 
             'd_atomname@h_atomname...a_atomname' 
             or some format you would like.
-            Or you could just set hnf to be 'number' to show hbond id on figure
+            Or you could just set hnf to be 'number' or 'id' to show hbond id on figure
+    -genscript, --genscript (optional)
+            whether to generate scripts for calculating distance and angle of hbonds
+    )
+    -cda, --calc_distance_angle (optional)
+            whether to calculate distance and angle of hbonds from distance xvg file and angle xvg file
+    -distancefile, --distancefile (optional)
+            distance file of hbonds for input
+    -anglefile, --anglefile (optional)
+            angle file of hbonds for input
+    -xs, --xshrink (optional)
+            specify a factor for multiplication of x-axis. default == 1.0
+            For instance, if "-xs 0.001" is specified, all x-axis value of xvg
+            will multiply this value. x-axis 1000 will be shown as 1. 
+            Useful for converting the unit (ps) of time into (ns). Don't forget
+            to change xlabel too after specifing -xs.
+    -x, --xlabel (optional)
+            specify the xlabel of figures
+    -so, --set_operation (optional)
+            use AND or OR to perform set operation on hbonds, eg. `AND1,2,5-6`  
+            or `OR0,2-4,7`. The AND set or OR set of hbonds whose ids were after
+            key words will be calculated and shown in occupancy figure.  
 """,
             "mol_map": """
 mol_map:  map the coordinates of coor_file to atoms in name_file. The molecules
           in two pdb file need to share exactly same conformation.
+          **YOU ARE NOT SUPPOSED TO USE THIS COMMAND!**
 
 :examples:
     dit mol_map -n good.gro -c coor.pdb -o output.pdb
 
 :parameters:
     -n, --name
             the pdb file which contains infos with coordinates you don't want
@@ -743,33 +812,57 @@
     dit dccm_ascii -f covapic.dat -m gaussian -o res.png -noshow
     dit dccm_ascii -f covapic.dat -x Res -y Res -t DCCM
 
 :parameters:
     -f, --input 
             the dat file generated by `gmx covar` which stored the covarience
             matrix information
-    -o, --output
+    -o, --output (optional)
             specify the output figure name
-    -m, --mode
+    -m, --mode (optional)
             specify the figure style, "origin", "gaussian", "bio3d"(default)
-    -ns, --noshow
+    -ns, --noshow (optional)
             whether not to show figure
-    -x, --xlabel
+    -x, --xlabel (optional)
             specify the xlabel of figure
-    -y, --ylabel
+    -y, --ylabel (optional)
             specify the ylabel of figure
-    -t, --title
+    -t, --title (optional)
             specify the title of figure
 """,
             "show_style": """
 show_style: generate matplotlib style template. 
 
 :examples:
     dit show_style
 """,
+            "dssp": """
+dssp: read in one xpm of secondary structure file, output the DSSP plot, 
+      residue occupancy vs time figure, time occupancy vs residue figure. 
+
+:examples:
+    dit dssp -f dssp.xpm 
+    dit dssp -f dssp.xpm -xs 0.001 -x Time(ns)
+
+:parameters:
+    -f, --input 
+            input xpm of secondary structure
+    -x, --xlabel (optional)
+            specify the xlabel of xpm
+    -y, --ylabel (optional)
+            specify the ylabel of xpm
+    -t, --title (optional)
+            specify the title of xpm
+    -xs, --xshrink (optional)
+            specify a factor for multiplication of x-axis. default == 1.0
+            For instance, if "-xs 0.001" is specified, all x-axis value of xvg
+            will multiply this value. x-axis 1000 will be shown as 1. 
+            Useful for converting the unit (ps) of time into (ns). Don't forget
+            to change xlabel too after specifing -xs.
+""",
         }
 
     def print_help_infos(self, method: str) -> None:
         """print help messages"""
 
         if method in self.help_infos.keys():
             print(self.help_infos[method])
@@ -808,22 +901,22 @@
 
 All commands are shown below:
     XVG:
         xvg_show, xvg_compare, xvg_ave, xvg_mvave, xvg2csv, xvg_rama
         xvg_show_distribution, xvg_show_stack, xvg_show_scatter
         xvg_energy_compute, xvg_combine, xvg_ave_bar, xvg_box
     XPM:
-        xpm_show, xpm2csv, xpm2gpl
+        xpm_show, xpm2csv, xpm2dat, xpm2gpl
     NDX:
         ndx_show, ndx_rm_dup, ndx_rm, ndx_preserve
         ndx_add, ndx_combine, ndx_rename
     MDP:
         mdp_gen
     Others:
-        find_center, pipi_dist_ang, hbond, mol_map, dccm_ascii
+        find_center, pipi_dist_ang, hbond, mol_map, dccm_ascii, dssp
     Matplotlib Style:
         show_style
 
 You can type `dit help <command>` or `dit <command> -h` for more help messages 
 about each command, like: `dit help xvg_show` or `dit xvg_show -h`. 
 
 And you can also modify the style of figures by adding (only) one mplstyle file
```

### Comparing `DuIvyTools-0.4.7/DuIvyTools/MDP.py` & `DuIvyTools-0.4.8/DuIvyTools/MDP.py`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/MolMap.py` & `DuIvyTools-0.4.8/DuIvyTools/MolMap.py`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/MplStyle.py` & `DuIvyTools-0.4.8/DuIvyTools/MplStyle.py`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/NDX.py` & `DuIvyTools-0.4.8/DuIvyTools/NDX.py`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/PipiDistAng.py` & `DuIvyTools-0.4.8/DuIvyTools/PipiDistAng.py`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/XPM.py` & `DuIvyTools-0.4.8/DuIvyTools/XPM.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,14 +335,75 @@
             z_title = (self.xpm_legend, "value")[len(self.xpm_legend) == 0]
             fo.write("{},{},{}\n".format(x_title, y_title, z_title))
             for i in range(len(x)):
                 fo.write("{:.6f},{:.6f},{:.6f}\n".format(x[i], y[i], v[i]))
         logging.info("extract data from {} successfully".format(self.xpmfile))
         logging.info("data are saved into {}".format(outcsv))
 
+    def xpm2dat(self, outdat: str = "") -> None:
+        """convert xpm file to dat file, N*N
+        outdat: the name of output dat file
+        """
+
+        if outdat == None:
+            outadat = ""
+        if outdat == "":
+            outdat = self.xpmfile[:-4] + ".dat"
+        if outdat[-4:] != ".dat":
+            logging.error("specify a output file with suffix dat")
+            sys.exit()
+        if os.path.exists(outdat):
+            logging.error("{} already in current directory".format(outdat))
+            sys.exit()
+
+        if self.xpm_type != "Continuous":
+            logging.error("can not extract data from xpm whose type is not Continuous")
+            sys.exit()
+
+        ## write results
+        with open(outdat, "w") as fo:
+            x_title = (self.xpm_xlabel, "x-axis")[len(self.xpm_xlabel) == 0]
+            y_title = (self.xpm_ylabel, "y-axis")[len(self.xpm_ylabel) == 0]
+            z_title = (self.xpm_legend, "value")[len(self.xpm_legend) == 0]
+            fo.write(
+                "# first line: {}; second line (bottom to top): {}; Values :{}\n".format(
+                    x_title, y_title, z_title
+                )
+            )
+            fo.write(",".join(["{:.4f}".format(item) for item in self.xpm_xaxis]))
+            fo.write("\n")
+            true_yaxis = ["{:.4f}".format(item) for item in self.xpm_yaxis]
+            true_yaxis.reverse()
+            fo.write(",".join(true_yaxis))
+            fo.write("\n")
+            for l in range(len(self.xpm_datalines)):
+                value = []
+                for i in range(
+                    0, self.xpm_width * self.xpm_char_per_pixel, self.xpm_char_per_pixel
+                ):
+                    value.append(
+                        float(
+                            self.notes[
+                                self.chars.index(
+                                    self.xpm_datalines[l][
+                                        i : i + self.xpm_char_per_pixel
+                                    ]
+                                )
+                            ]
+                        )
+                    )
+                fo.write(",".join(["{:.6f}".format(v) for v in value]))
+                fo.write("\n")
+        logging.info("extract data from {} successfully".format(self.xpmfile))
+        logging.info(
+            "{} * {} matrix data are saved into {}".format(
+                self.xpm_width, self.xpm_height, outdat
+            )
+        )
+
     def xpm2gpl(self, outgpl: str = "") -> None:
         """convert xpm file to gnuplot script
         outgpl: the name of output gnuplot script
         """
 
         ## check files
         if outgpl == None:
@@ -656,15 +717,16 @@
         xpm_xaxis = np.array(self.xpm_xaxis)
         xpm_yaxis = np.array(self.xpm_yaxis)
         img = np.array(values)
 
         ## draw 3d figure
         fig = plt.figure()
         plt.clf()
-        ax = fig.gca(projection="3d")
+        # ax = fig.gca(projection="3d")
+        ax = fig.add_subplot(projection="3d")
 
         ## interpolation
         IP_value = 1
         if IP == False:
             IP_value = 1
         elif IP == True:
             IP_value = 12
@@ -860,14 +922,17 @@
         if xpms2combine == None:
             logging.error("no input xpm files for combination")
             sys.exit()
         xpm_combine(xpms2combine, output, noshow)
     elif method == "xpm2csv":
         xpm = XPM(inputxpm, xlabel, ylabel, title, xshrink)
         xpm.xpm2csv(output)
+    elif method == "xpm2dat":
+        xpm = XPM(inputxpm, xlabel, ylabel, title, xshrink)
+        xpm.xpm2dat(output)
     elif method == "xpm2gpl":
         xpm = XPM(inputxpm, xlabel, ylabel, title, xshrink)
         xpm.xpm2gpl(output)
     else:
         logging.error("Wrong method you specified")
         sys.exit()
```

### Comparing `DuIvyTools-0.4.7/DuIvyTools/XVG.py` & `DuIvyTools-0.4.8/DuIvyTools/XVG.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,30 +42,32 @@
     __init__: read xvg file and extract infos
     calc_average: calculate the average of xvg data
     calc_mvave: calculate the moving average of xvg data
     xvg2csv : convert xvg data to csv format
     draw: draw xvg data to figure
     """
 
-    def __init__(self, xvgfile: str = "") -> None:
+    def __init__(self, xvgfile: str = "", xshrink: float = 1.0) -> None:
         """read xvg file and extract infos"""
 
         self.xvg_filename = xvgfile
         self.xvg_title = ""
         self.xvg_xlabel = ""
         self.xvg_ylabel = ""
         self.xvg_legends = []
         self.xvg_column_num = 0
         self.xvg_row_num = 0
         self.xvg_columns = []
 
         self.data_heads = []
         self.data_columns = []
 
-        ## check kand read xpm file
+        ## check and read xpm file
+        if xshrink <= 0:
+            logging.warning("The parameter xshrink should be larger than zero")
         if not os.path.exists(xvgfile):
             logging.error("no {} in current directory".format(xvgfile))
             sys.exit()
         if xvgfile[-4:] != ".xvg":
             logging.error("specify a xvg file with suffix xvg")
             sys.exit()
         with open(xvgfile, "r") as fo:
@@ -111,15 +113,15 @@
                 )
                 sys.exit()
         if self.xvg_column_num == 0 or self.xvg_row_num == 0:
             logging.error("no data line detected in xvg file")
             sys.exit()
 
         self.data_heads.append(self.xvg_xlabel)
-        self.data_columns.append([float(c) for c in self.xvg_columns[0]])
+        self.data_columns.append([float(c) * xshrink for c in self.xvg_columns[0]])
         if len(self.xvg_legends) == 0 and len(self.xvg_columns) > 1:
             self.data_heads.append(self.xvg_ylabel)
             self.data_columns.append([float(c) for c in self.xvg_columns[1]])
         if len(self.xvg_legends) > 0 and len(self.xvg_columns) > len(self.xvg_legends):
             items = [item.strip() for item in self.xvg_ylabel.split(",")]
             heads = [l for l in self.xvg_legends]
             if len(items) == len(self.xvg_legends):
@@ -261,14 +263,51 @@
         """
 
         plt.clf()
         column_num = len(self.data_columns)
         x_min = np.min(self.data_columns[0])
         x_max = np.max(self.data_columns[0])
         x_space = int((x_max - x_min) / 100)
+        if column_num == 2:
+            plt.plot(self.data_columns[0], self.data_columns[1])
+            plt.ylabel(self.data_heads[1])
+        else:
+            for i in range(1, column_num):
+                plt.plot(
+                    self.data_columns[0], self.data_columns[i], label=self.data_heads[i]
+                )
+            plt.legend()
+        if int(x_min - x_space) < int(x_max + x_space) - 1.0:
+            plt.xlim(int(x_min - x_space), int(x_max + x_space))
+        plt.xlabel(self.data_heads[0])
+        plt.title(self.xvg_title)
+        plt.tight_layout()
+
+        if outpng != None:
+            if os.path.exists(outpng):
+                logging.error("{} already in current directory".format(outpng))
+                sys.exit()
+            plt.savefig(outpng, dpi=300)
+        if noshow == False:
+            plt.show()
+
+    def draw_subplot(self, outpng: str = "", noshow: bool = False) -> None:
+        """
+        draw xvg data into figure by subplots
+
+        :parameters:
+            outpng: the output picture file name.
+            noshow: whether not to show figure in GUI.
+        """
+
+        plt.clf()
+        column_num = len(self.data_columns)
+        x_min = np.min(self.data_columns[0])
+        x_max = np.max(self.data_columns[0])
+        x_space = int((x_max - x_min) / 100)
         grid = (plt.GridSpec(1, column_num), plt.GridSpec(2, int(column_num / 2)))[
             column_num > 2
         ]
         for i in range(1, column_num):
             ## use grid for subplots layout
             if i == column_num - 1:
                 ax = plt.subplot(
@@ -282,15 +321,16 @@
                     grid[
                         (1, 0)[i - 1 < int((column_num) / 2)],
                         (i - 1) % int((column_num) / 2),
                     ]
                 )
             ax.plot(self.data_columns[0], self.data_columns[i])
             ax.set_ylabel(self.data_heads[i])
-            plt.xlim(int(x_min - x_space), int(x_max + x_space))
+            if int(x_min - x_space) < int(x_max + x_space) - 1.0:
+                plt.xlim(int(x_min - x_space), int(x_max + x_space))
             plt.xlabel(self.data_heads[0])
         if column_num > 2:
             plt.suptitle(self.xvg_title)
         else:
             plt.title(self.xvg_title)
         plt.tight_layout()
 
@@ -374,14 +414,16 @@
         self,
         column_select: list = [],
         legend_list: list = [],
         start: int = 0,
         end: int = None,
         outpng: str = "",
         noshow: bool = False,
+        xlabel: str = None,
+        ylabel: str = None,
     ) -> None:
         """
         draw xvg data into stacking figure
 
         :parameters:
             column_select: a list to store the column indexs you want to stack
             legend_list: a list to store legends specified by user
@@ -446,16 +488,22 @@
                 stack_data,
                 [0 for _ in range(len(stack_data))],
                 label=labels[index_id],
             )
             ylim_max = (ylim_max, max(stack_data))[ylim_max < max(stack_data)]
             ylim_min = (ylim_min, min(stack_data))[ylim_min > min(stack_data)]
         # print(ylim_min, ylim_max)
-        plt.xlabel(self.data_heads[0])
-        plt.ylabel(self.xvg_ylabel)
+        if xlabel != None:
+            plt.xlabel(xlabel)
+        else:
+            plt.xlabel(self.data_heads[0])
+        if ylabel != None:
+            plt.ylabel(ylabel)
+        else:
+            plt.ylabel(self.xvg_ylabel)
         plt.title("Stacked plot of " + self.xvg_title)
         plt.xlim(
             np.min(self.data_columns[0][start:end]),
             np.max(self.data_columns[0][start:end]),
         )
         plt.ylim(ylim_min, ylim_max)
         plt.legend(loc=3)
@@ -468,25 +516,27 @@
         if noshow == False:
             plt.show()
 
     def draw_scatter(
         self,
         x_index: int = 0,
         y_index: int = None,
+        color_index: int = None,
         outpng: str = "",
         noshow: bool = False,
     ) -> None:
         """
         draw xvg data to scatter plot
 
         :parameters:
             x_index: the column index of x values for scatter plot
             y_index: the column index of y values for scatter plot
-            outpng: the output picture file name.
-            noshow: whether not to show figure in GUI.
+            color_index: the column index for color value
+            outpng: the output picture file name
+            noshow: whether not to show figure in GUI
         """
 
         ## check parameters
         if x_index >= len(self.data_columns) or x_index < 0:
             logging.warning("x_index not in proper range, use default value.")
             x_index = 0
         if y_index == None:
@@ -494,15 +544,33 @@
         else:
             if y_index >= len(self.data_columns) or y_index < 0:
                 logging.warning("y_index not in proper range, use default value.")
                 y_index = (len(self.data_columns) - 1, 1)[len(self.data_columns) >= 2]
 
         ## draw scatter plot
         plt.clf()
-        plt.scatter(self.data_columns[x_index], self.data_columns[y_index])
+        if color_index != None:
+            if color_index >= len(self.data_columns):
+                logging.error(
+                    "color_index you specified is out of range ({})".format(
+                        len(self.data_columns)
+                    )
+                )
+                sys.exit()
+            plt.scatter(
+                self.data_columns[x_index],
+                self.data_columns[y_index],
+                c=self.data_columns[color_index],
+                cmap="coolwarm",
+            )
+            plt.colorbar(
+                label=self.data_heads[color_index], orientation="vertical", shrink=0.8
+            )
+        else:
+            plt.scatter(self.data_columns[x_index], self.data_columns[y_index])
         plt.ylabel(self.data_heads[y_index])
         plt.xlabel(self.data_heads[x_index])
         plt.title(
             "Scatter plot of {} vs {}".format(
                 self.data_heads[x_index], self.data_heads[y_index]
             )
         )
@@ -917,14 +985,15 @@
     title: str = None,
     showMV: bool = False,
     windowsize: int = 50,
     confidence: float = 0.90,
     alpha: float = 0.4,
     outpng: str = "",
     noshow: bool = False,
+    xshrink: float = None,
 ) -> None:
     """
     comparison of xvgfiles, draw different columns into figure.
 
     :parameters:
         xvgfiles: a list to store all xvg files you want to compare
         column_select: a list to store the columns you select to compare
@@ -979,18 +1048,20 @@
     else:
         column_select = [[columns] for columns in column_select]
     if len(legend_list) != 0 and len(legend_list) != sum(
         [len(column) for column in column_select]
     ):
         logging.error("number of legends you input can not pair to columns you select")
         sys.exit()
+    if xshrink == None:
+        xshrink = 1.0
 
     ## draw comparison
     plt.clf()
-    XVGS = [XVG(xvg) for xvg in xvgfiles]
+    XVGS = [XVG(xvg, xshrink) for xvg in xvgfiles]
     legend_count, xmin, xmax = 0, None, None
     for id, column_indexs in enumerate(column_select):
         xvg = XVGS[id]
         if showMV == True:
             _, mvaves, highs, lows = xvg.calc_mvave(windowsize, confidence)
         else:
             _, mvaves, highs, lows = [], [], [], []
@@ -1340,18 +1411,23 @@
 
 def xvg2csv(xvgfile: str = "", outcsv: str = "") -> None:
     """convert xvg file to csv file"""
     xvg = XVG(xvgfile)
     xvg.xvg2csv(outcsv)
 
 
-def xvg_show(xvgfile: str = "", outpng: str = "", noshow: bool = False) -> None:
+def xvg_show(
+    xvgfile: str = "", outpng: str = "", noshow: bool = False, subplot=False
+) -> None:
     """visualization of xvg file"""
     xvg = XVG(xvgfile)
-    xvg.draw(outpng, noshow)
+    if subplot == True:
+        xvg.draw_subplot(outpng, noshow)
+    else:
+        xvg.draw(outpng, noshow)
 
 
 def xvg_show_distribution(
     xvgfile: str = "", bin: int = 100, outpng: str = "", noshow: bool = False
 ) -> None:
     """visualization of distribution of xvg data"""
     if bin == None:
@@ -1364,32 +1440,48 @@
     xvgfile: str = "",
     column_select: list = [],
     legend_list: list = [],
     start: int = 0,
     end: int = None,
     outpng: str = "",
     noshow: bool = False,
+    xshrink: float = None,
+    xlabel: str = None,
+    ylabel: str = None,
 ) -> None:
     """visualization of stacked xvg data"""
-    xvg = XVG(xvgfile)
-    xvg.draw_stacking(column_select, legend_list, start, end, outpng, noshow)
+    if xshrink == None:
+        xshrink = 1.0
+    xvg = XVG(xvgfile, xshrink)
+    xvg.draw_stacking(
+        column_select, legend_list, start, end, outpng, noshow, xlabel, ylabel
+    )
 
 
 def xvg_show_scatter(
     xvgfile: str = "",
     x_index: int = 0,
     y_index: int = None,
+    column_select: list = [],
     outpng: str = "",
     noshow: bool = False,
 ) -> None:
     """visualization of scatter plot of xvg file"""
+    color_index = None
+    if len(column_select) == 1 and isinstance(column_select[-1], int):
+        color_index = int(column_select[-1])
+    elif len(column_select) == 0:
+        pass
+    else:
+        logging.error("There should be only one color index which is a number")
+        sys.exit()
     if x_index == None:
         x_index = 0
     xvg = XVG(xvgfile)
-    xvg.draw_scatter(x_index, y_index, outpng, noshow)
+    xvg.draw_scatter(x_index, y_index, color_index, outpng, noshow)
 
 
 def xvg_call_functions(arguments: list = None):
     """call functions by method"""
 
     if arguments == None:
         arguments = [argv for argv in sys.argv]
@@ -1443,14 +1535,20 @@
         "-ac",
         "--ave2csv",
         help="the output csv file name to save averages, used in xvg_bar_draw",
     )
     parser.add_argument(
         "-xt", "--xtitles", nargs="+", help="the x tick labels for box comparison"
     )
+    parser.add_argument(
+        "-subplot", "--subplot", action="store_true", help="whether to show in subplots"
+    )
+    parser.add_argument(
+        "-xs", "--xshrink", type=float, help="modify x-axis by multipling xshrink"
+    )
 
     if len(arguments) < 2:
         logging.error("no input parameters, -h or --help for help messages")
         sys.exit()
     method = arguments[1]
     # print(method)
     if method in ["-h", "--help"]:
@@ -1494,32 +1592,40 @@
     if method == "xvg_ave":
         xvg_calc_ave(firstfile, args.start, args.end)
     elif method == "xvg_mvave":
         xvg_calc_mvave2csv(firstfile, args.output, args.windowsize, args.confidence)
     elif method == "xvg2csv":
         xvg2csv(firstfile, args.output)
     elif method == "xvg_show":
-        xvg_show(firstfile, args.output, args.noshow)
+        xvg_show(firstfile, args.output, args.noshow, args.subplot)
     elif method == "xvg_rama":
         xvg_ramachandran(firstfile, args.output, args.noshow)
     elif method == "xvg_show_distribution":
         xvg_show_distribution(firstfile, args.bin, args.output, args.noshow)
     elif method == "xvg_show_stack":
         xvg_show_stacking(
             firstfile,
             column_select,
             legend_list,
             args.start,
             args.end,
             args.output,
             args.noshow,
+            args.xshrink,
+            args.xlabel,
+            args.ylabel,
         )
     elif method == "xvg_show_scatter":
         xvg_show_scatter(
-            firstfile, args.x_index, args.y_index, args.output, args.noshow
+            firstfile,
+            args.x_index,
+            args.y_index,
+            column_select,
+            args.output,
+            args.noshow,
         )
     elif method == "xvg_energy_compute":
         energy_compute(xvgfiles, args.output)
     elif method == "xvg_combine":  # [], [[],[]]
         xvg_combine(xvgfiles, column_select, args.output)
     elif method == "xvg_compare":  # [], [[], []]
         xvg_compare(
@@ -1533,14 +1639,15 @@
             args.title,
             args.showMV,
             args.windowsize,
             args.confidence,
             args.alpha,
             args.output,
             args.noshow,
+            args.xshrink,
         )
     elif method == "xvg_ave_bar":  # [[], []], []
         xvg_bar_compare(
             xvgfiles,
             column_select,
             legend_list,
             args.xtitles,
```

### Comparing `DuIvyTools-0.4.7/DuIvyTools/__init__.py` & `DuIvyTools-0.4.8/DuIvyTools/__init__.py`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/data/DIT.mplstyle` & `DuIvyTools-0.4.8/DuIvyTools/data/DIT.mplstyle`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ## Matplotlib style for DuIvyTools
+## https://matplotlib.org/stable/tutorials/introductory/customizing.html#the-matplotlibrc-file
 
 axes.labelsize:     12
 axes.linewidth:     1
 xtick.labelsize:    12
 ytick.labelsize:    12
 ytick.left:         True
 ytick.direction:    in
```

### Comparing `DuIvyTools-0.4.7/DuIvyTools/data/blank.mdp` & `DuIvyTools-0.4.8/DuIvyTools/data/blank.mdp`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/data/em.mdp` & `DuIvyTools-0.4.8/DuIvyTools/data/em.mdp`

 * *Files 2% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 ; Parameters describing how to find the neighbors of each atom and how to calculate the interactions
 ;------------------------------------------------------------------------------
 nstlist		    = 1		    ; Frequency to update the neighbor list and long range forces
 cutoff-scheme   = Verlet
 ns_type		    = grid		; Method to determine neighbor list (simple, grid)
 rlist		    = 1.0		; Cut-off for making neighbor list (short range forces)
 coulombtype	    = PME		; Treatment of long range electrostatic interactions
-rcoulomb	    = 1.0		; long range electrostatic cut-off
-rvdw		    = 1.0		; long range Van der Waals cut-off
+rcoulomb	    = 1.2		; long range electrostatic cut-off
+rvdw		    = 1.2		; long range Van der Waals cut-off
 pbc		        = xyz 		; Periodic Boundary Conditions
```

### Comparing `DuIvyTools-0.4.7/DuIvyTools/data/ions.mdp` & `DuIvyTools-0.4.8/DuIvyTools/data/ions.mdp`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/data/md.mdp` & `DuIvyTools-0.4.8/DuIvyTools/data/npt.mdp`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
-; a MD template, suit for normal MD
+; a NPT template, suit for normal NPT
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 
-
-title       = Protein-ligand complex MD simulation 
+title       = Protein-ligand complex NPT equilibration 
+define      = -DPOSRES  ; position restrain the protein and ligand
 
 ; Run parameters
 ;------------------------------------------------------------------------------
-integrator  = md          ; leap-frog integrator
-nsteps      = 50000000    ; 100ns
-dt          = 0.002       ; 2 fs
+integrator  = md        ; leap-frog integrator
+nsteps      = 50000     ; 2 * 50000 = 100 ps
+dt          = 0.002     ; 2 fs
 
 ; Output control
 ;------------------------------------------------------------------------------
-nstxout             = 0         ; suppress .trr output 
-nstvout             = 0         ; suppress .trr output
-nstenergy           = 5000      ; save energies every 10.0 ps
-nstlog              = 5000      ; update log file every 10.0 ps
-nstxout-compressed  = 5000      ; write .xtc trajectory every 10.0 ps
+nstxout     =                  ; save coordinates every 1.0 ps
+nstvout     =                  ; save velocities every 1.0 ps
+nstenergy   = 500              ; save energies every 1.0 ps
+nstlog      = 500              ; update log file every 1.0 ps
+nstxout-compressed  = 500      ; write .xtc trajectory every 1.0 ps
 compressed-x-grps   = System
-; energygrps          = Protein Ligand     ; comment it for GPU calculation
+; energygrps  = Protein Ligand
 
 ; remove rot+trans during running
 ; -----------------------------------------------------------------------------
 ; comm-mode   = Angular
 ; comm-grps   = Protein
 
 ; Bond parameters
 ;------------------------------------------------------------------------------
 continuation    = yes           ; first dynamics run
 constraint_algorithm = lincs    ; holonomic constraints 
-constraints     = all-bonds     ; all bonds (even heavy atom-H bonds) constrained
+constraints     = h-bonds       ; all bonds (even heavy atom-H bonds) constrained
 lincs_iter      = 1             ; accuracy of LINCS
 lincs_order     = 4             ; also related to accuracy
 
 ; Neighborsearching
 ;------------------------------------------------------------------------------
 cutoff-scheme   = Verlet
 ns_type         = grid      ; search neighboring grid cells
 nstlist         = 10        ; 20 fs, largely irrelevant with Verlet
-rcoulomb        = 1.4       ; short-range electrostatic cutoff (in nm)
-rvdw            = 1.4       ; short-range van der Waals cutoff (in nm)
+rcoulomb        = 1.2       ; short-range electrostatic cutoff (in nm)
+rvdw            = 1.2       ; short-range van der Waals cutoff (in nm)
 
 ; Electrostatics
 ;------------------------------------------------------------------------------
 coulombtype     = PME       ; Particle Mesh Ewald for long-range electrostatics
 pme_order       = 4         ; cubic interpolation
 fourierspacing  = 0.16      ; grid spacing for FFT
 
 ; Temperature coupling
 ;------------------------------------------------------------------------------
 tcoupl      = V-rescale                     ; modified Berendsen thermostat
-tc-grps     = Protein Non-Protein           ; two coupling groups - more accurate
+tc-grps     = Water Non-Water               ; two coupling groups - more accurate
 tau_t       = 0.1   0.1                     ; time constant, in ps
-ref_t       = 310   310                     ; reference temperature, one for each group, in K
+ref_t       = 300   300                     ; reference temperature, one for each group, in K
 
-; Pressure coupling 
+; Pressure coupling
 ;------------------------------------------------------------------------------
-pcoupl      = Parrinello-Rahman             ; pressure coupling is on for NPT
+pcoupl      = Berendsen   ;Parrinello-Rahman  ; pressure coupling is on for NPT
 pcoupltype  = isotropic                     ; uniform scaling of box vectors
 tau_p       = 2.0                           ; time constant, in ps
 ref_p       = 1.0                           ; reference pressure, in bar
-compressibility = 4.5e-5                    ; isothermal compressibility of water, bar^-1
+compressibility = 4.5e-5           ; isothermal compressibility of water, bar^-1
+refcoord_scaling    = com
 
 ; Periodic boundary conditions
 ;------------------------------------------------------------------------------
 pbc         = xyz       ; 3-D PBC
 
 ; Dispersion correction
 ;------------------------------------------------------------------------------
 DispCorr    = EnerPres  ; account for cut-off vdW scheme
 
 ; Velocity generation
 ;------------------------------------------------------------------------------
-gen_vel     = no        ; assign velocities from Maxwell distribution
+gen_vel     = no        ; velocity generation off after NVT
```

### Comparing `DuIvyTools-0.4.7/DuIvyTools/data/npt.mdp` & `DuIvyTools-0.4.8/DuIvyTools/data/nvt.mdp`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
-; a NPT template, suit for normal NPT
+; a NVT template, suit for normal NVT
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 
-title       = Protein-ligand complex NPT equilibration 
-define      = -DPOSRES  ; position restrain the protein and ligand
+title       = Protein-ligand complex NVT equilibration 
+define      = -DPOSRES  ; position restrain the protein
 
 ; Run parameters
-;------------------------------------------------------------------------------
+; -----------------------------------------------------------------------------
 integrator  = md        ; leap-frog integrator
-nsteps      = 50000     ; 2 * 50000 = 100 ps
+nsteps      = 50000     ; 0.002 * 50000 = 100 ps
 dt          = 0.002     ; 2 fs
 
 ; Output control
-;------------------------------------------------------------------------------
-nstxout     = 500       ; save coordinates every 1.0 ps
-nstvout     = 500       ; save velocities every 1.0 ps
-nstenergy   = 500       ; save energies every 1.0 ps
-nstlog      = 500       ; update log file every 1.0 ps
-energygrps  = Protein Ligand
+; -----------------------------------------------------------------------------
+nstxout     =                  ; save coordinates every 1.0 ps
+nstvout     =                  ; save velocities every 1.0 ps
+nstenergy   = 500              ; save energies every 1.0 ps
+nstlog      = 500              ; update log file every 1.0 ps
+nstxout-compressed  = 500      ; write .xtc trajectory every 1.0 ps
+compressed-x-grps   = System
+; energygrps  = Protein Ligand
 
 ; remove rot+trans during running
 ; -----------------------------------------------------------------------------
 ; comm-mode   = Angular
 ; comm-grps   = Protein
 
 ; Bond parameters
-;------------------------------------------------------------------------------
-continuation    = yes           ; first dynamics run
+; -----------------------------------------------------------------------------
+continuation    = no            ; first dynamics run
 constraint_algorithm = lincs    ; holonomic constraints 
-constraints     = all-bonds     ; all bonds (even heavy atom-H bonds) constrained
+constraints     = h-bonds       ; all bonds (even heavy atom-H bonds) constrained
 lincs_iter      = 1             ; accuracy of LINCS
 lincs_order     = 4             ; also related to accuracy
 
 ; Neighborsearching
-;------------------------------------------------------------------------------
+; -----------------------------------------------------------------------------
 cutoff-scheme   = Verlet
 ns_type         = grid      ; search neighboring grid cells
 nstlist         = 10        ; 20 fs, largely irrelevant with Verlet
-rcoulomb        = 1.4       ; short-range electrostatic cutoff (in nm)
-rvdw            = 1.4       ; short-range van der Waals cutoff (in nm)
+rcoulomb        = 1.2       ; short-range electrostatic cutoff (in nm)
+rvdw            = 1.2       ; short-range van der Waals cutoff (in nm)
 
 ; Electrostatics
-;------------------------------------------------------------------------------
+; -----------------------------------------------------------------------------
 coulombtype     = PME       ; Particle Mesh Ewald for long-range electrostatics
 pme_order       = 4         ; cubic interpolation
 fourierspacing  = 0.16      ; grid spacing for FFT
 
 ; Temperature coupling
-;------------------------------------------------------------------------------
-tcoupl      = V-rescale                     ; modified Berendsen thermostat
-tc-grps     = Protein Non-Protein           ; two coupling groups - more accurate
-tau_t       = 0.1   0.1                     ; time constant, in ps
-ref_t       = 310   310                     ; reference temperature, one for each group, in K
+; -----------------------------------------------------------------------------
+tcoupl      = V-rescale        ; modified Berendsen thermostat
+tc-grps     = Water Non-Water  ; two coupling groups - more accurate
+tau_t       = 0.1   0.1        ; time constant, in ps
+ref_t       = 300   300        ; reference temperature, one for each group, in K
 
 ; Pressure coupling
-;------------------------------------------------------------------------------
-pcoupl      = Berendsen   ; Parrinello-Rahman   ; pressure coupling is on for NPT
-pcoupltype  = isotropic                     ; uniform scaling of box vectors
-tau_p       = 2.0                           ; time constant, in ps
-ref_p       = 1.0                           ; reference pressure, in bar
-compressibility = 4.5e-5                    ; isothermal compressibility of water, bar^-1
-refcoord_scaling    = com
+; -----------------------------------------------------------------------------
+pcoupl      = no        ; no pressure coupling in NVT
 
 ; Periodic boundary conditions
-;------------------------------------------------------------------------------
+; -----------------------------------------------------------------------------
 pbc         = xyz       ; 3-D PBC
 
 ; Dispersion correction
-;------------------------------------------------------------------------------
+; -----------------------------------------------------------------------------
 DispCorr    = EnerPres  ; account for cut-off vdW scheme
 
 ; Velocity generation
-;------------------------------------------------------------------------------
-gen_vel     = no        ; velocity generation off after NVT 
+; -----------------------------------------------------------------------------
+gen_vel     = yes       ; assign velocities from Maxwell distribution
+gen_temp    = 300       ; temperature for Maxwell distribution
+gen_seed    = -1        ; generate a random seed
+
```

### Comparing `DuIvyTools-0.4.7/DuIvyTools/data/pref_general.data` & `DuIvyTools-0.4.8/DuIvyTools/data/pref_general.data`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/data/pref_glycine.data` & `DuIvyTools-0.4.8/DuIvyTools/data/pref_glycine.data`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/data/pref_preproline.data` & `DuIvyTools-0.4.8/DuIvyTools/data/pref_preproline.data`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools/data/pref_proline.data` & `DuIvyTools-0.4.8/DuIvyTools/data/pref_proline.data`

 * *Files identical despite different names*

### Comparing `DuIvyTools-0.4.7/DuIvyTools.egg-info/PKG-INFO` & `DuIvyTools-0.4.8/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,106 +1,102 @@
-Metadata-Version: 2.1
-Name: DuIvyTools
-Version: 0.4.7
-Summary: A tool for GROMACS results analysis and visualization
-Home-page: https://github.com/CharlesHahn/DuIvyTools
-Author: CharlesHahn
-Author-email: 
-License: UNKNOWN
-Download-URL: https://github.com/CharlesHahn/DuIvyTools
-Description: # DuIvyTools
-        [![PyPI version](https://badge.fury.io/py/DuIvyTools.svg)](https://badge.fury.io/py/DuIvyTools)
-        ![PyPI - Downloads](https://img.shields.io/pypi/dm/DuIvyTools)
-        ![PyPI - License](https://img.shields.io/pypi/l/DuIvyTools)
-        
-        
-        ```
-          *******           **                  **********               **
-         /**////**         /**          **   **/////**///               /**
-         /**    /** **   **/** **    **//** **     /**  ******   ****** /**  ******
-         /**    /**/**  /**/**/**   /** //***      /** **////** **////**/** **//// 
-         /**    /**/**  /**/**//** /**   /**       /**/**   /**/**   /**/**//***** 
-         /**    ** /**  /**/** //****    **        /**/**   /**/**   /**/** /////**
-         /*******  //******/**  //**    **         /**//****** //****** *** ****** 
-         ///////    ////// //    //    //          //  //////   ////// /// //////
-        ```
-        
-        DuIvyTools (DIT) is a simple analysis and visualization tool for GROMACS result
-        files (.xvg, .xpm, .ndx, .mdp). 
-        
-        This tool can perform data visualization and convertion, and may be able to 
-        cover daily simple tasks when analyzing results of molecular dynamics 
-        simulations by GROMACS. 
-        
-        ## Intro
-        
-        The usage of DIT is similar to GMX, type `dit` and followed by commands and 
-        parameters, like:
-        
-        ```bash
-        dit xvg_show -f test.xvg
-        dit xpm_show -f test.xpm -ip
-        ```
-        
-        Type `dit help` for more messages.
-        
-        visit https://github.com/CharlesHahn/DuIvy/tree/master/Articles/20220310-DIT 
-        for more introductions in Chinese.
-        
-        
-        ## Install
-        
-        This tool is a python3 library which you can install it by `pip`.
-        
-        ```bash
-        pip install DuIvyTools
-        ```
-        
-        ## Commands
-        
-        This tool contains quite a lot commands.
-        
-        ```
-        For XVG files:
-            xvg_show, xvg_compare, xvg_ave, xvg_mvave, xvg2csv, xvg_rama
-            xvg_show_distribution, xvg_show_stack, xvg_show_scatter
-            xvg_energy_compute, xvg_combine, xvg_ave_bar, xvg_box
-        For XPM files:
-            xpm_show, xpm2csv, xpm2gpl
-        For NDX files:
-            ndx_show, ndx_rm_dup, ndx_rm, ndx_preserve
-            ndx_add, ndx_combine, ndx_rename
-        For MDP files:
-            mdp_gen
-        Others:
-            find_center, pipi_dist_ang, hbond, mol_map, dccm_ascii
-        Matplotlib Style:
-            show_style
-        ```
-        
-        
-        ## Cite 
-        
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7261532.svg)](https://doi.org/10.5281/zenodo.7261532)
-        
-        ## still working 
-        
-        - [ ] **readthedocs**
-        - [ ] xtick of xvg shrink
-        - [ ] xvg_show one plot mode
-        - [ ] latex or format parser for matplotlib
-        - [ ] Discrete xpm to csv, convert notes to numbers
-        - [ ] python test
-        - [ ] better output (color, error ... )
-        - [ ] build a GUI maybe
-        
-        
-Platform: cross-platform
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Intended Audience :: Science/Research
-Description-Content-Type: text/markdown
-Provides-Extra: test
+DuIvyTools
+
+[![PyPI version](https://badge.fury.io/py/DuIvyTools.svg)](https://badge.fury.io/py/DuIvyTools)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/DuIvyTools)
+![PyPI - License](https://img.shields.io/pypi/l/DuIvyTools)
+[![Documentation Status](https://readthedocs.org/projects/duivytools/badge/?version=latest)](https://duivytools.readthedocs.io/zh_CN/latest/?badge=latest)
+[![commits-since](https://img.shields.io/github/commits-since/CharlesHahn/DuIvyTools/v0.4.7.svg)](https://github.com/CharlesHahn/DuIvyTools/compare/v0.4.7...master)
+[![Python Version](https://img.shields.io/pypi/pyversions/DuIvyTools.svg)](https://pypi.org/project/DuIvyTools)
+
+```
+  *******           **                  **********               **
+ /**////**         /**          **   **/////**///               /**
+ /**    /** **   **/** **    **//** **     /**  ******   ****** /**  ******
+ /**    /**/**  /**/**/**   /** //***      /** **////** **////**/** **//// 
+ /**    /**/**  /**/**//** /**   /**       /**/**   /**/**   /**/**//***** 
+ /**    ** /**  /**/** //****    **        /**/**   /**/**   /**/** /////**
+ /*******  //******/**  //**    **         /**//****** //****** *** ****** 
+ ///////    ////// //    //    //          //  //////   ////// /// //////
+```
+
+DuIvyTools (DIT) is a simple analysis and visualization tool for GROMACS result
+files (.xvg, .xpm, .ndx, .mdp). 
+
+This tool can perform data visualization and convertion, and may be able to 
+cover daily simple tasks when analyzing results of molecular dynamics 
+simulations by GROMACS. 
+
+## Intro
+
+The usage of DIT is similar to GMX, type `dit` and followed by commands and 
+parameters, like:
+
+```bash
+dit xvg_show -f test.xvg
+dit xpm_show -f test.xpm -ip
+```
+
+Type `dit help` for more messages.
+
+visit https://github.com/CharlesHahn/DuIvy/tree/master/Articles/20220310-DIT 
+for more introductions in Chinese.
+
+
+## Install
+
+This tool is a python3 library which you can install it by `pip`.
+
+```bash
+pip install DuIvyTools
+```
+
+## Commands
+
+This tool contains quite a lot commands.
+
+```
+For XVG files:
+    xvg_show, xvg_compare, xvg_ave, xvg_mvave, xvg2csv, xvg_rama
+    xvg_show_distribution, xvg_show_stack, xvg_show_scatter
+    xvg_energy_compute, xvg_combine, xvg_ave_bar, xvg_box
+For XPM files:
+    xpm_show, xpm2csv, xpm2dat, xpm2gpl
+For NDX files:
+    ndx_show, ndx_rm_dup, ndx_rm, ndx_preserve
+    ndx_add, ndx_combine, ndx_rename
+For MDP files:
+    mdp_gen
+Others:
+    find_center, pipi_dist_ang, hbond, mol_map, dccm_ascii, dssp
+Matplotlib Style:
+    show_style
+
+You can type `dit help <command>` or `dit <command> -h` for more help messages 
+about each command, like: `dit help xvg_show` or `dit xvg_show -h`. 
+```
+
+
+## Cite 
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6339993.svg)](https://doi.org/10.5281/zenodo.6339993)
+
+## still working
+
+- [x] hbond - merge, AND, OR
+- [x] DSSP: SS vs AA
+
+
+## further features in v0.5.0
+
+- [ ] ! the parsing of files should be isolated from figure plotting
+- [ ] ! re-design all arguments parsing part
+- [ ] ! plotting engines: matplotlib, plotext, gnuplot
+- [ ] ! Procedures
+- [ ] ! tidy help info and documentation
+- [ ] mdmat dmf.xpm
+- [ ] Discrete xpm to csv, convert notes to numbers
+- [ ] better output (color, error ... )
+- [ ] use plotext to create plot in terminal !
+- [ ] python test
+- [ ] latex or format parser for matplotlib
+- [ ] volume occupancy of ligand during MD
+- [ ] build a GUI maybe (webapp?)
```

### Comparing `DuIvyTools-0.4.7/DuIvyTools.egg-info/SOURCES.txt` & `DuIvyTools-0.4.8/DuIvyTools.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 DuIvyTools/DCCM.py
 DuIvyTools/DIT.py
+DuIvyTools/DSSP.py
 DuIvyTools/FindCenter.py
 DuIvyTools/HELP.py
 DuIvyTools/HydrogenBond.py
 DuIvyTools/MDP.py
 DuIvyTools/MolMap.py
 DuIvyTools/MplStyle.py
 DuIvyTools/NDX.py
```

### Comparing `DuIvyTools-0.4.7/PKG-INFO` & `DuIvyTools-0.4.8/DuIvyTools.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: DuIvyTools
-Version: 0.4.7
+Version: 0.4.8
 Summary: A tool for GROMACS results analysis and visualization
 Home-page: https://github.com/CharlesHahn/DuIvyTools
 Author: CharlesHahn
 Author-email: 
 License: UNKNOWN
 Download-URL: https://github.com/CharlesHahn/DuIvyTools
-Description: # DuIvyTools
+Description: DuIvyTools
+        
         [![PyPI version](https://badge.fury.io/py/DuIvyTools.svg)](https://badge.fury.io/py/DuIvyTools)
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/DuIvyTools)
         ![PyPI - License](https://img.shields.io/pypi/l/DuIvyTools)
-        
+        [![Documentation Status](https://readthedocs.org/projects/duivytools/badge/?version=latest)](https://duivytools.readthedocs.io/zh_CN/latest/?badge=latest)
+        [![commits-since](https://img.shields.io/github/commits-since/CharlesHahn/DuIvyTools/v0.4.7.svg)](https://github.com/CharlesHahn/DuIvyTools/compare/v0.4.7...master)
+        [![Python Version](https://img.shields.io/pypi/pyversions/DuIvyTools.svg)](https://pypi.org/project/DuIvyTools)
         
         ```
           *******           **                  **********               **
          /**////**         /**          **   **/////**///               /**
          /**    /** **   **/** **    **//** **     /**  ******   ****** /**  ******
          /**    /**/**  /**/**/**   /** //***      /** **////** **////**/** **//// 
          /**    /**/**  /**/**//** /**   /**       /**/**   /**/**   /**/**//***** 
@@ -61,43 +64,55 @@
         
         ```
         For XVG files:
             xvg_show, xvg_compare, xvg_ave, xvg_mvave, xvg2csv, xvg_rama
             xvg_show_distribution, xvg_show_stack, xvg_show_scatter
             xvg_energy_compute, xvg_combine, xvg_ave_bar, xvg_box
         For XPM files:
-            xpm_show, xpm2csv, xpm2gpl
+            xpm_show, xpm2csv, xpm2dat, xpm2gpl
         For NDX files:
             ndx_show, ndx_rm_dup, ndx_rm, ndx_preserve
             ndx_add, ndx_combine, ndx_rename
         For MDP files:
             mdp_gen
         Others:
-            find_center, pipi_dist_ang, hbond, mol_map, dccm_ascii
+            find_center, pipi_dist_ang, hbond, mol_map, dccm_ascii, dssp
         Matplotlib Style:
             show_style
+        
+        You can type `dit help <command>` or `dit <command> -h` for more help messages 
+        about each command, like: `dit help xvg_show` or `dit xvg_show -h`. 
         ```
         
         
         ## Cite 
         
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7261532.svg)](https://doi.org/10.5281/zenodo.7261532)
+        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6339993.svg)](https://doi.org/10.5281/zenodo.6339993)
         
-        ## still working 
+        ## still working
+        
+        - [x] hbond - merge, AND, OR
+        - [x] DSSP: SS vs AA
         
-        - [ ] **readthedocs**
-        - [ ] xtick of xvg shrink
-        - [ ] xvg_show one plot mode
-        - [ ] latex or format parser for matplotlib
-        - [ ] Discrete xpm to csv, convert notes to numbers
-        - [ ] python test
-        - [ ] better output (color, error ... )
-        - [ ] build a GUI maybe
         
+        ## further features in v0.5.0
         
+        - [ ] ! the parsing of files should be isolated from figure plotting
+        - [ ] ! re-design all arguments parsing part
+        - [ ] ! plotting engines: matplotlib, plotext, gnuplot
+        - [ ] ! Procedures
+        - [ ] ! tidy help info and documentation
+        - [ ] mdmat dmf.xpm
+        - [ ] Discrete xpm to csv, convert notes to numbers
+        - [ ] better output (color, error ... )
+        - [ ] use plotext to create plot in terminal !
+        - [ ] python test
+        - [ ] latex or format parser for matplotlib
+        - [ ] volume occupancy of ligand during MD
+        - [ ] build a GUI maybe (webapp?)
 Platform: cross-platform
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
```

### Comparing `DuIvyTools-0.4.7/setup.py` & `DuIvyTools-0.4.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # "pytest-cov",
     # to be able to run `python setup.py checkdocs`
     # "collective.checkdocs",
     # "pygments",
 ]
 
 
-__version__ = "0.4.7"
+__version__ = "0.4.8"
 long_description = ""
 
 with open("README.md", "r") as fo:
     long_description = fo.read()
 
 
 setup(
```

