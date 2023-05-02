# Comparing `tmp/tpfi-1.0.2.tar.gz` & `tmp/tpfi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpfi-1.0.2.tar", max compression
+gzip compressed data, was "tpfi-1.0.3.tar", max compression
```

## Comparing `tpfi-1.0.2.tar` & `tpfi-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-05-01 13:22:49.013242 tpfi-1.0.2/LICENSE
--rw-r--r--   0        0        0     2251 2023-05-01 13:22:49.013242 tpfi-1.0.2/README.md
--rw-r--r--   0        0        0      417 2023-05-01 13:22:49.021242 tpfi-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      123 2023-05-01 13:22:49.021242 tpfi-1.0.2/src/tpfi/__init__.py
--rw-r--r--   0        0        0    14658 2023-05-01 13:22:49.021242 tpfi-1.0.2/src/tpfi/tpfi.py
--rw-r--r--   0        0        0     5167 2023-05-01 13:22:49.021242 tpfi-1.0.2/src/tpfi/utils.py
--rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 tpfi-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-02 02:26:53.131746 tpfi-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2251 2023-05-02 02:26:53.131746 tpfi-1.0.3/README.md
+-rw-r--r--   0        0        0      417 2023-05-02 02:26:53.139746 tpfi-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-05-02 02:26:53.139746 tpfi-1.0.3/src/tpfi/__init__.py
+-rw-r--r--   0        0        0    14943 2023-05-02 02:26:53.139746 tpfi-1.0.3/src/tpfi/tpfi.py
+-rw-r--r--   0        0        0     5167 2023-05-02 02:26:53.139746 tpfi-1.0.3/src/tpfi/utils.py
+-rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 tpfi-1.0.3/PKG-INFO
```

### Comparing `tpfi-1.0.2/LICENSE` & `tpfi-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tpfi-1.0.2/README.md` & `tpfi-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tpfi-1.0.2/src/tpfi/tpfi.py` & `tpfi-1.0.3/src/tpfi/tpfi.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 def plot_tpf(
     ax_tpf: Axes,
     tpf: Union[TessTargetPixelFile, KeplerTargetPixelFile],
     r: Table,
     cmap: str,
     c_star: str,
     c_mask: str,
+    show_ticklabels: bool,
     mag_limit: float,
     ax_cb: Axes = None,
 ):
     """
     Plot the identification charts.
 
     Parameters
@@ -155,14 +156,16 @@
         The table of the Gaia objects in the area of TPF
     cmap: str
         The colormap to use
     c_star: str
         The color of the stars
     c_mask: str
         The color of the pipeline mask
+    show_ticklabels: bool
+        Whether to show the tick labels
     mag_limit: float
         The magnitude limit (Gaia G mag) to plot the stars in the TPF
     ax_cb: `matplotlib.axes.Axes`
         A matplotlib axes object to plot the color bar into
     """
 
     # TPF plot
@@ -177,18 +180,24 @@
 
     image = median_flux / 10**division
 
     im, norm = imshow_norm(image, ax_tpf, stretch=SqrtStretch(), origin="lower", cmap=cmap, zorder=0)
     x_pixel, y_pixel = tpf.shape[1:][1], tpf.shape[1:][0]
     ax_tpf.set_xlim(-0.5, x_pixel - 0.5)
     ax_tpf.set_ylim(-0.5, y_pixel - 0.5)
-    ax_tpf.set_xticks(np.arange(0, x_pixel, 1))
-    ax_tpf.set_yticks(np.arange(0, y_pixel, 1))
-    ax_tpf.set_xticklabels(np.arange(1, x_pixel + 1, 1))
-    ax_tpf.set_yticklabels(np.arange(1, y_pixel + 1, 1))
+
+    if show_ticklabels:
+        ax_tpf.set_xticks(np.arange(0, x_pixel, 1))
+        ax_tpf.set_yticks(np.arange(0, y_pixel, 1))
+        ax_tpf.set_xticklabels(np.arange(1, x_pixel + 1, 1))
+        ax_tpf.set_yticklabels(np.arange(1, y_pixel + 1, 1))
+    else:
+        ax_tpf.set_xticks([])
+        ax_tpf.set_yticks([])
+
     ax_tpf.yaxis.set_ticks_position("right")
     ax_tpf.invert_xaxis()
 
     if r is None:
         at = AnchoredText("No Gaia DR3 Data", frameon=False, loc="upper left", prop=dict(size=13))
         ax_tpf.add_artist(at)
     else:
@@ -254,14 +263,15 @@
 def plot_identification(
     tpf: Union[TessTargetPixelFile, KeplerTargetPixelFile],
     ax: Axes = None,
     mag_limit: float = None,
     cmap: str = "viridis",
     c_star: str = "red",
     c_mask: str = "tomato",
+    show_ticklabels: bool = True,
     verbose: bool = False,
 ):
     """
     Plot the identification chart for a given target pixel file (TPF).
 
     The function creates a combined identification chart, including the sky image and
     the TPF with stars' positions, magnitudes, and pipeline aperture.
@@ -277,14 +287,16 @@
         (18 for TESS, 19.5 for Kepler/K2)
     cmap : str, optional
         The colormap to use for the TPF. Default is 'viridis'.
     c_star: str, optional
         The color of the stars in the TPF. Default is 'red'.
     c_mask: str, optional
         The color of the pipeline mask in the TPF. Default is 'tomato'.
+    show_ticklabels : bool, optional
+        Whether to show the tick labels in the TPF. Default is True.
     verbose : bool, optional
         Whether to print out progress messages. Default is False.
 
     Returns
     -------
     ax : `matplotlib.axes.Axes`
         The matplotlib axes object.
@@ -299,15 +311,15 @@
     divider = make_axes_locatable(ax)
     ax_tpf = divider.append_axes("right", size="100%", pad=0.1)
     ax_cb = divider.append_axes("right", size="8%", pad=0.35)
 
     plot_sky(ax, tpf, verbose)
 
     r = query_nearby_gaia_objects(tpf, verbose=verbose)
-    plot_tpf(ax_tpf, tpf, r, cmap, c_star, c_mask, ax_cb=ax_cb, mag_limit=mag_limit)
+    plot_tpf(ax_tpf, tpf, r, cmap, c_star, c_mask, show_ticklabels, mag_limit, ax_cb)
 
 
 def plot_season(
     label: str,
     ax: Axes = None,
     mag_limit: float = 19.5,
     cmap: str = "gray_r",
@@ -395,12 +407,10 @@
         ax_list.append(divider.append_axes("right", size=f"{percent}%", pad=0.1))
 
     plot_sky(ax, tpf_list[max_index], verbose)
 
     r = query_nearby_gaia_objects(tpf_list[max_index], verbose=verbose)
     for i, tpf in enumerate(tpf_list):
         if tpf is not None:
-            plot_tpf(ax_list[i], tpf_list[i], r, cmap, c_star, c_mask, mag_limit)
+            plot_tpf(ax_list[i], tpf_list[i], r, cmap, c_star, c_mask, False, mag_limit)
             at = AnchoredText(f"Season {i + 1}", frameon=False, loc="upper left", prop=dict(size=13), zorder=100)
             ax_list[i].add_artist(at)
-        ax_list[i].set_xticks([])
-        ax_list[i].set_yticks([])
```

### Comparing `tpfi-1.0.2/src/tpfi/utils.py` & `tpfi-1.0.3/src/tpfi/utils.py`

 * *Files identical despite different names*

### Comparing `tpfi-1.0.2/PKG-INFO` & `tpfi-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpfi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Plot identification charts for Kepler, K2 and TESS.
 Home-page: https://github.com/keyuxing/tpfi
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

