# Comparing `tmp/planetmapper-1.6.5.tar.gz` & `tmp/planetmapper-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.6.5.tar", last modified: Mon Apr 24 16:42:54 2023, max compression
+gzip compressed data, was "planetmapper-1.7.0.tar", last modified: Tue May  2 13:21:03 2023, max compression
```

## Comparing `planetmapper-1.6.5.tar` & `planetmapper-1.7.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:42:54.498190 planetmapper-1.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-24 16:42:54.498190 planetmapper-1.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-24 16:42:40.000000 planetmapper-1.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:42:54.494190 planetmapper-1.6.5/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    72134 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (123)    99198 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:42:54.494190 planetmapper-1.6.5/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   116259 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    43334 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-24 16:42:40.000000 planetmapper-1.6.5/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:42:54.494190 planetmapper-1.6.5/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-24 16:42:54.000000 planetmapper-1.6.5/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-24 16:42:54.000000 planetmapper-1.6.5/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:42:54.000000 planetmapper-1.6.5/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 16:42:54.000000 planetmapper-1.6.5/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-24 16:42:54.000000 planetmapper-1.6.5/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 16:42:54.000000 planetmapper-1.6.5/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 16:42:40.000000 planetmapper-1.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:42:54.498190 planetmapper-1.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-24 16:42:40.000000 planetmapper-1.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:42:54.494190 planetmapper-1.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-04-24 16:42:40.000000 planetmapper-1.6.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-24 16:42:40.000000 planetmapper-1.6.5/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-04-24 16:42:40.000000 planetmapper-1.6.5/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-04-24 16:42:40.000000 planetmapper-1.6.5/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 16:42:40.000000 planetmapper-1.6.5/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-24 16:42:40.000000 planetmapper-1.6.5/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-24 16:42:40.000000 planetmapper-1.6.5/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-04-24 16:42:40.000000 planetmapper-1.6.5/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-24 16:42:40.000000 planetmapper-1.6.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:21:03.983509 planetmapper-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-02 13:21:03.983509 planetmapper-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-02 13:20:42.000000 planetmapper-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:21:03.979509 planetmapper-1.7.0/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75150 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110519 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:21:03.979509 planetmapper-1.7.0/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116259 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45504 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:21:03.979509 planetmapper-1.7.0/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-02 13:21:03.000000 planetmapper-1.7.0/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-02 13:21:03.000000 planetmapper-1.7.0/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:21:03.000000 planetmapper-1.7.0/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-02 13:21:03.000000 planetmapper-1.7.0/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 13:21:03.000000 planetmapper-1.7.0/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 13:21:03.000000 planetmapper-1.7.0/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 13:20:42.000000 planetmapper-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 13:21:03.983509 planetmapper-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-02 13:20:42.000000 planetmapper-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:21:03.983509 planetmapper-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25986 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19129 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_utils.py
```

### Comparing `planetmapper-1.6.5/PKG-INFO` & `planetmapper-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.6.5
+Version: 1.7.0
 Summary: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
```

### Comparing `planetmapper-1.6.5/README.md` & `planetmapper-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/planetmapper/__init__.py` & `planetmapper-1.7.0/planetmapper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     This code is in active development, so may contain bugs! Any issues, bugs and 
     suggestions can be 
     `reported on GitHub <https://github.com/ortk95/planetmapper/issues/new>`__.
 """
 from .common import __version__, __author__, __url__
 from .base import SpiceBase, set_kernel_path, get_kernel_path
-from .body import Body
+from .body import Body, DEFAULT_WIREFRAME_FORMATTING
 from .body_xy import Backplane, BodyXY
 from .observation import Observation
 from .basic_body import BasicBody
 from . import gui
 from . import utils
 from . import kernel_downloader
 from . import data_loader
@@ -94,13 +94,14 @@
     'BodyXY',
     'Observation',
     'BasicBody',
     'gui',
     'utils',
     'kernel_downloader',
     'data_loader',
+    'DEFAULT_WIREFRAME_FORMATTING',
 ]
 
 
 def main():
     """:meta private:"""
     gui._main()
```

### Comparing `planetmapper-1.6.5/planetmapper/base.py` & `planetmapper-1.7.0/planetmapper/base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/planetmapper/basic_body.py` & `planetmapper-1.7.0/planetmapper/basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/planetmapper/body.py` & `planetmapper-1.7.0/planetmapper/body.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 import datetime
-from typing import Callable, Literal, cast
+from collections import defaultdict
+from typing import Callable, Literal, cast, TypedDict, Any
+
+try:
+    from typing import Unpack
+except ImportError:
+    from typing_extensions import Unpack
 
 import matplotlib.patheffects as path_effects
 import matplotlib.pyplot as plt
 import matplotlib.transforms
 import numpy as np
 import spiceypy as spice
 from matplotlib.axes import Axes
@@ -13,14 +19,75 @@
     SpiceSPKINSUFFDATA,
 )
 
 from . import data_loader, utils
 from .base import SpiceBase, Numeric
 from .basic_body import BasicBody
 
+_WireframeComponent = Literal[
+    'all',
+    'grid',
+    'equator',
+    'prime_meridian',
+    'limb',
+    'limb_illuminated',
+    'terminator',
+    'ring',
+    'pole',
+    'coordinate_of_interest_lonlat',
+    'coordinate_of_interest_radec',
+    'other_body_of_interest_marker',
+    'other_body_of_interest_label',
+    'map_boundary',
+]
+
+
+class _WireframeKwargs(TypedDict, total=False):
+    label_poles: bool
+    add_title: bool
+    grid_interval: float
+    indicate_equator: bool
+    indicate_prime_meridian: bool
+    formatting: dict[_WireframeComponent, dict[str, Any]] | None
+    color: str | tuple[float, float, float]
+
+
+DEFAULT_WIREFRAME_FORMATTING: dict[_WireframeComponent, dict[str, Any]] = {
+    'all': dict(color='k'),
+    'grid': dict(alpha=0.5, linestyle=':'),
+    'equator': dict(linestyle='-'),
+    'prime_meridian': dict(linestyle='-'),
+    'limb': dict(linewidth=0.5),
+    'limb_illuminated': dict(),
+    'terminator': dict(linestyle='--'),
+    'ring': dict(linewidth=0.5),
+    'pole': dict(
+        ha='center',
+        va='center',
+        size='small',
+        weight='bold',
+        path_effects=[
+            path_effects.Stroke(linewidth=3, foreground='w'),
+            path_effects.Normal(),
+        ],
+        clip_on=True,
+    ),
+    'coordinate_of_interest_lonlat': dict(marker='x'),
+    'coordinate_of_interest_radec': dict(marker='+'),
+    'other_body_of_interest_marker': dict(marker='+'),
+    'other_body_of_interest_label': dict(
+        size='small',
+        ha='center',
+        va='center',
+        alpha=0.5,
+        clip_on=True,
+    ),
+    'map_boundary': dict(),
+}
+
 
 class Body(SpiceBase):
     """
     Class representing an astronomical body observed at a specific time.
 
     Generally only `target`, `utc` and `observer` need to be changed. The additional
     parameters allow customising the exact settings used in the internal SPICE
@@ -1526,203 +1593,232 @@
         if len(poles) == 0:
             # if no poles are visible, show both
             for lon, lat, s in pole_options:
                 poles.append((lon, lat, f'({s})'))
 
         return poles
 
+    @staticmethod
+    def _get_wireframe_kw(
+        *,
+        base_formatting: dict[str, Any] | None = None,
+        common_formatting: dict[str, Any] | None = None,
+        formatting: dict[_WireframeComponent, dict[str, Any]] | None = None,
+    ) -> dict[_WireframeComponent, dict[str, Any]]:
+        formatting = formatting or {}
+        base_formatting = base_formatting or {}
+        common_formatting = common_formatting or {}
+
+        # deal with passing plot_wireframe_radec args to e.g. plot_wireframe_km
+        for k in ('show', 'dms_ticks'):
+            common_formatting.pop(k, None)
+
+        kwargs: dict[_WireframeComponent, dict[str, Any]] = defaultdict(dict)
+        for k in set(DEFAULT_WIREFRAME_FORMATTING.keys()) | set(formatting.keys()):
+            kwargs[k] = (
+                base_formatting
+                | DEFAULT_WIREFRAME_FORMATTING.get('all', {})
+                | DEFAULT_WIREFRAME_FORMATTING.get(k, {})
+                | common_formatting
+                | formatting.get('all', {})
+                | formatting.get(k, {})
+            )
+        return kwargs
+
     def _plot_wireframe(
         self,
         transform: None | matplotlib.transforms.Transform,
         ax: Axes | None = None,
-        color: str | tuple[float, float, float] = 'k',
         label_poles: bool = True,
         add_title: bool = True,
         grid_interval: float = 30,
         indicate_equator: bool = False,
         indicate_prime_meridian: bool = False,
-        **kwargs,
+        formatting: dict[_WireframeComponent, dict[str, Any]] | None = None,
+        **common_formatting,
     ) -> Axes:
         """Plot generic wireframe representation of the observation"""
         if ax is None:
             ax = cast(Axes, plt.gca())
-
         if transform is None:
             transform = ax.transData
         else:
             transform = transform + ax.transData
 
-        gridline_kwargs = dict(
-            color=color,
-            alpha=0.5,
-            transform=transform,
-            **kwargs,
+        kwargs = self._get_wireframe_kw(
+            base_formatting=dict(transform=transform),
+            common_formatting=common_formatting,
+            formatting=formatting,
         )
+
         lons = np.arange(0, 360, grid_interval)
         for lon, (ra, dec) in zip(lons, self.visible_lon_grid_radec(lons)):
             ax.plot(
                 ra,
                 dec,
-                linestyle='-' if lon == 0 and indicate_prime_meridian else ':',
-                **gridline_kwargs,
+                **kwargs['grid']
+                | (
+                    kwargs['prime_meridian']
+                    if lon == 0 and indicate_prime_meridian
+                    else {}
+                ),
             )
         lats = np.arange(-90, 90, grid_interval)
         for lat, (ra, dec) in zip(lats, self.visible_lat_grid_radec(lats)):
             ax.plot(
                 ra,
                 dec,
-                linestyle='-' if lat == 0 and indicate_equator else ':',
-                **gridline_kwargs,
+                **kwargs['grid']
+                | (kwargs['equator'] if lat == 0 and indicate_equator else {}),
             )
 
-        ax.plot(
-            *self.limb_radec(),
-            color=color,
-            linewidth=0.5,
-            transform=transform,
-            **kwargs,
-        )
-        ax.plot(
-            *self.terminator_radec(),
-            color=color,
-            linestyle='--',
-            transform=transform,
-            **kwargs,
-        )
+        ax.plot(*self.limb_radec(), **kwargs['limb'])
+        ax.plot(*self.terminator_radec(), **kwargs['terminator'])
 
         ra_day, dec_day, ra_night, dec_night = self.limb_radec_by_illumination()
-        ax.plot(ra_day, dec_day, color=color, transform=transform, **kwargs)
+        ax.plot(ra_day, dec_day, **kwargs['limb_illuminated'])
 
         if label_poles:
             for lon, lat, s in self.get_poles_to_plot():
                 ra, dec = self.lonlat2radec(lon, lat)
-                ax.text(
-                    ra,
-                    dec,
-                    s,
-                    ha='center',
-                    va='center',
-                    size='small',
-                    weight='bold',
-                    color=color,
-                    path_effects=[
-                        path_effects.Stroke(linewidth=3, foreground='w'),
-                        path_effects.Normal(),
-                    ],
-                    transform=transform,
-                    clip_on=True,
-                    **kwargs,
-                )
+                ax.text(ra, dec, s, **kwargs['pole'])
 
         for lon, lat in self.coordinates_of_interest_lonlat:
             if self.test_if_lonlat_visible(lon, lat):
                 ra, dec = self.lonlat2radec(lon, lat)
-                ax.scatter(
-                    ra,
-                    dec,
-                    marker='x',  # type: ignore
-                    color=color,
-                    transform=transform,
-                    **kwargs,
-                )
+                ax.scatter(ra, dec, **kwargs['coordinate_of_interest_lonlat'])
         for ra, dec in self.coordinates_of_interest_radec:
-            ax.scatter(
-                ra,
-                dec,
-                marker='+',  # type: ignore
-                color=color,
-                transform=transform,
-                **kwargs,
-            )
+            ax.scatter(ra, dec, **kwargs['coordinate_of_interest_radec'])
 
         for radius in self.ring_radii:
             ra, dec = self.ring_radec(radius)
-            ax.plot(ra, dec, color=color, linewidth=0.5, transform=transform, **kwargs)
+            ax.plot(ra, dec, **kwargs['ring'])
 
         for body in self.other_bodies_of_interest:
             ra = body.target_ra
             dec = body.target_dec
             ax.text(
-                ra,
-                dec,
-                body.target + '\n',
-                size='small',
-                ha='center',
-                va='center',
-                color=color,
-                alpha=0.5,
-                transform=transform,
-                clip_on=True,
-                **kwargs,
-            )
-            ax.scatter(
-                ra,
-                dec,
-                marker='+',  # type: ignore
-                color=color,
-                transform=transform,
-                **kwargs,
+                ra, dec, body.target + '\n', **kwargs['other_body_of_interest_label']
             )
+            ax.scatter(ra, dec, **kwargs['other_body_of_interest_marker'])
+
         if add_title:
             ax.set_title(self.get_description(multiline=True))
         return ax
 
     def plot_wireframe_radec(
         self,
         ax: Axes | None = None,
-        color: str | tuple[float, float, float] = 'k',
         *,
-        label_poles: bool = True,
-        add_title: bool = True,
+        dms_ticks: bool = True,
         add_axis_labels: bool = True,
-        grid_interval: float = 30,
-        indicate_equator: bool = False,
-        indicate_prime_meridian: bool = False,
         aspect_adjustable: Literal['box', 'datalim'] = 'datalim',
-        dms_ticks: bool = True,
         show: bool = False,
-        **kwargs,
+        **wireframe_kwargs: Unpack[_WireframeKwargs],
     ) -> Axes:
         """
         Plot basic wireframe representation of the observation using RA/Dec sky
         coordinates.
 
+        See also :func:`plot_wireframe_km` and :func:`BodyXY.plot_wireframe_xy` to plot
+        the wireframe in other coordinate systems.
+
+        To plot a wireframe with the default appearance, simply use: ::
+
+            body.plot_wireframe_radec()
+
+        To customise the appearance of the plot, you can use the `formatting` and
+        `**kwargs` arguments which can be used to pass arguments to the Matplotlib
+        plotting functions. The `formatting` argument can be used to customise
+        individual components, and the `**kwargs` argument can be used to customise
+        all components at once.
+
+        For example, to change the colour of the entire wireframe to red, you can
+        use: ::
+
+            body.plot_wireframe_radec(color='r')
+
+        To change just the plotted terminator and dayside limb to red, use: ::
+
+            body.plot_wireframe_radec(
+                formatting={
+                    'terminator': {'color': 'r'},
+                    'limb_illuminated': {'color': 'r'},
+                },
+            )
+
+        The order of precedence for the formatting is the `formatting` argument, then
+        `**kwargs`, then the default formatting. For example, the following plot will
+        be red with a thin blue grid and green poles: ::
+
+            body.plot_wireframe_radec(
+                color='r',
+                formatting={
+                    'grid': {'color': 'b', 'linewidth': 0.5, 'linestyle': '-'},
+                    'pole': {'color': 'g'},
+                },
+            )
+
+        Individual components can be hidden by setting `visible` to `False`. For
+        example, to hide the terminator, use: ::
+
+            body.plot_wireframe_radec(formatting={'terminator': {'visible': False}})
+
+        The default formatting is defined in :data:`DEFAULT_WIREFRAME_FORMATTING`. This
+        can be modified after importing PlanetMapper to change the default appearance of
+        all wireframes: ::
+
+            import planetmapper
+            planetmapper.DEFAULT_WIREFRAME_FORMATTING['grid']['color'] = 'b'
+            planetmapper.DEFAULT_WIREFRAME_FORMATTING['grid']['linestyle'] = '--'
+
+            body.plot_wireframe_radec() # This would have a blue dashed grid
+            body.plot_wireframe_radec(color='r') # This would be red with a dashed grid
+
         Args:
             ax: Matplotlib axis to use for plotting. If `ax` is None (the default), uses
                 `plt.gca()` to get the currently active axis.
-            color: Matplotlib color used for to plot the wireframe.
             label_poles: Toggle labelling the poles of the target body.
             add_title: Add title generated by :func:`get_description` to the axis.
             add_axis_labels: Add axis labels.
             grid_interval: Spacing between grid lines in degrees.
             indicate_equator: Toggle indicating the equator with a solid line.
             indicate_prime_meridian: Toggle indicating the prime meridian with a solid
                 line.
             aspect_adjustable: Set `adjustable` parameter when setting the aspect ratio.
                 Passed to :func:`matplotlib.axes.Axes.set_aspect`.
             dms_ticks: Toggle between showing ticks as degrees, minutes and seconds
-                (e.g. 12°34′56″) or decimal degrees (e.g. 12.582).
+                (e.g. 12°34′56″) or decimal degrees (e.g. 12.582). This argument is only
+                applicable for :func:`plot_wireframe_radec`.
             show: Toggle immediately showing the plotted figure with `plt.show()`.
+            formatting: Dictionary of formatting options for the wireframe components.
+                The keys of this dictionary are the names of the wireframe components
+                and the values are dictionaries of keyword arguments to pass to the
+                Matplotlib plotting function for that component. For example, to set the
+                `color` of the plotted rings to red, you could use::
+
+                    body.plot_wireframe_radec(formatting={'ring': {'color': 'r'}})
+
+                The following components can be formatted: `grid`, `equator`,
+                `prime_meridian`, `limb`, `limb_illuminated`, `terminator`, `ring`,
+                `pole`, `coordinate_of_interest_lonlat`, `coordinate_of_interest_radec`,
+                `other_body_of_interest_marker`, `other_body_of_interest_label`.
+
             **kwargs: Additional arguments are passed to Matplotlib plotting functions
-                (useful for e.g. specifying `zorder`).
+                for all components. This is useful for specifying properties like
+                `color` to customise the entire wireframe rather than a single
+                component. For example, to make the entire wireframe red, you could
+                use::
+
+                    body.plot_wireframe_radec(color='r')
 
         Returns:
             The axis containing the plotted wireframe.
         """
-        ax = self._plot_wireframe(
-            transform=None,
-            ax=ax,
-            color=color,
-            label_poles=label_poles,
-            add_title=add_title,
-            grid_interval=grid_interval,
-            indicate_equator=indicate_equator,
-            indicate_prime_meridian=indicate_prime_meridian,
-            **kwargs,
-        )
+        ax = self._plot_wireframe(transform=None, ax=ax, **wireframe_kwargs)
 
         utils.format_radec_axes(
             ax,
             self.target_dec,
             dms_ticks=dms_ticks,
             add_axis_labels=add_axis_labels,
             aspect_adjustable=aspect_adjustable,
@@ -1731,63 +1827,30 @@
         if show:
             plt.show()
         return ax
 
     def plot_wireframe_km(
         self,
         ax: Axes | None = None,
-        color: str | tuple[float, float, float] = 'k',
         *,
-        label_poles: bool = True,
-        add_title: bool = True,
         add_axis_labels: bool = True,
-        grid_interval: float = 30,
-        indicate_equator: bool = False,
-        indicate_prime_meridian: bool = False,
         aspect_adjustable: Literal['box', 'datalim'] = 'datalim',
         show: bool = False,
-        **kwargs,
+        **wireframe_kwargs: Unpack[_WireframeKwargs],
     ) -> Axes:
         """
         Plot basic wireframe representation of the observation on a target centred
-        frame.
-
-        Args:
-            ax: Matplotlib axis to use for plotting. If `ax` is None (the default), uses
-                `plt.gca()` to get the currently active axis.
-            color: Matplotlib color used for to plot the wireframe.
-            label_poles: Toggle labelling the poles of the target body.
-            add_title: Add title generated by :func:`get_description` to the axis.
-            add_axis_labels: Add axis labels.
-            grid_interval: Spacing between grid lines in degrees.
-            indicate_equator: Toggle indicating the equator with a solid line.
-            indicate_prime_meridian: Toggle indicating the prime meridian with a solid
-                line.
-            aspect_adjustable: Set `adjustable` parameter when setting the aspect ratio.
-                Passed to :func:`matplotlib.axes.Axes.set_aspect`.
-            show: Toggle immediately showing the plotted figure with `plt.show()`.
-            **kwargs: Additional arguments are passed to Matplotlib plotting functions
-                (useful for e.g. specifying `zorder`).
+        frame. See :func:`plot_wireframe_radec` for details of accepted arguments.
 
         Returns:
             The axis containing the plotted wireframe.
         """
 
         transform = self.matplotlib_radec2km_transform()
-        ax = self._plot_wireframe(
-            transform=transform,
-            ax=ax,
-            color=color,
-            label_poles=label_poles,
-            add_title=add_title,
-            grid_interval=grid_interval,
-            indicate_equator=indicate_equator,
-            indicate_prime_meridian=indicate_prime_meridian,
-            **kwargs,
-        )
+        ax = self._plot_wireframe(transform=transform, ax=ax, **wireframe_kwargs)
         if add_axis_labels:
             ax.set_xlabel('Projected distance (km)')
             ax.set_ylabel('Projected distance (km)')
             ax.ticklabel_format(style='sci', scilimits=(-3, 3))
         ax.set_aspect(1, adjustable=aspect_adjustable)
 
         if show:
```

### Comparing `planetmapper-1.6.5/planetmapper/body_xy.py` & `planetmapper-1.7.0/planetmapper/body_xy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import datetime
 import math
 import warnings
 import functools
+import io
 from typing import (
+    cast,
     Any,
     Callable,
     Concatenate,
     Iterable,
     Literal,
     NamedTuple,
     ParamSpec,
@@ -26,15 +28,20 @@
 import numpy as np
 import pyproj
 import scipy.interpolate
 from matplotlib.axes import Axes
 from matplotlib.collections import QuadMesh
 from spiceypy.utils.exceptions import NotFoundError
 
-from .body import Body
+from .body import (
+    Body,
+    _WireframeKwargs,
+    _WireframeComponent,
+    DEFAULT_WIREFRAME_FORMATTING,
+)
 from .progress import progress_decorator
 
 T = TypeVar('T')
 S = TypeVar('S')
 P = ParamSpec('P')
 
 
@@ -935,80 +942,14 @@
         Update the transformation returned by :func:`matplotlib_radec2xy_transform`
         to use the latest disc parameter values `(x0, y0, r0, rotation)`.
         """
         self._get_matplotlib_radec2xy_transform_radians().set_matrix(
             self._get_radec2xy_matrix_radians()
         )
 
-    # Plotting
-    def plot_wireframe_xy(
-        self,
-        ax: Axes | None = None,
-        color: str | tuple[float, float, float] = 'k',
-        *,
-        label_poles: bool = True,
-        add_title: bool = True,
-        add_axis_labels: bool = True,
-        grid_interval: float = 30,
-        indicate_equator: bool = False,
-        indicate_prime_meridian: bool = False,
-        aspect_adjustable: Literal['box', 'datalim'] = 'box',
-        show: bool = False,
-        **kwargs,
-    ) -> Axes:
-        """
-        Plot basic wireframe representation of the observation using image pixel
-        coordinates.
-
-        Args:
-            ax: Matplotlib axis to use for plotting. If `ax` is None (the default), uses
-                `plt.gca()` to get the currently active axis.
-            color: Matplotlib color used for to plot the wireframe.
-            label_poles: Toggle labelling the poles of the target body.
-            add_title: Add title generated by :func:`get_description` to the axis.
-            add_axis_labels: Add axis labels.
-            grid_interval: Spacing between grid lines in degrees.
-            indicate_equator: Toggle indicating the equator with a solid line.
-            indicate_prime_meridian: Toggle indicating the prime meridian with a solid
-                line.
-            aspect_adjustable: Set `adjustable` parameter when setting the aspect ratio.
-                Passed to :func:`matplotlib.axes.Axes.set_aspect`.
-            show: Toggle immediately showing the plotted figure with `plt.show()`.
-            **kwargs: Additional arguments are passed to Matplotlib plotting functions
-                (useful for e.g. specifying `zorder`).
-
-        Returns:
-            The axis containing the plotted wireframe.
-        """
-        # Generate affine transformation from radec in degrees -> xy
-        transform = self.matplotlib_radec2xy_transform()
-        ax = self._plot_wireframe(
-            transform=transform,
-            ax=ax,
-            color=color,
-            label_poles=label_poles,
-            add_title=add_title,
-            grid_interval=grid_interval,
-            indicate_equator=indicate_equator,
-            indicate_prime_meridian=indicate_prime_meridian,
-            **kwargs,
-        )
-
-        if self._test_if_img_size_valid():
-            ax.set_xlim(-0.5, self._nx - 0.5)
-            ax.set_ylim(-0.5, self._ny - 0.5)
-        if add_axis_labels:
-            ax.set_xlabel('x (pixels)')
-            ax.set_ylabel('y (pixels)')
-        ax.set_aspect(1, adjustable=aspect_adjustable)
-
-        if show:
-            plt.show()
-        return ax
-
     # Mapping
     def map_img(
         self,
         img: np.ndarray,
         *,
         interpolation: Literal['nearest', 'linear', 'quadratic', 'cubic'] = 'linear',
         propagate_nan: bool = True,
@@ -1117,14 +1058,419 @@
         y0 = max(math.floor(y), 0)
         y1 = min(math.ceil(y), self._ny - 1)
         return nans[y0, x0] or nans[y0, x1] or nans[y1, x0] or nans[y1, x1]
 
     def _xy_in_image_frame(self, x: float, y: float) -> bool:
         return (-0.5 < x < self._nx - 0.5) and (-0.5 < y < self._ny - 0.5)
 
+    # Plotting
+    def plot_wireframe_xy(
+        self,
+        ax: Axes | None = None,
+        *,
+        add_axis_labels: bool = True,
+        aspect_adjustable: Literal['box', 'datalim'] = 'box',
+        show: bool = False,
+        **wireframe_kwargs: Unpack[_WireframeKwargs],
+    ) -> Axes:
+        """
+        Plot basic wireframe representation of the observation using image pixel
+        coordinates. See :func:`Body.plot_wireframe_radec` for details of accepted
+        arguments.
+
+        Returns:
+            The axis containing the plotted wireframe.
+        """
+        transform = self.matplotlib_radec2xy_transform()
+        ax = self._plot_wireframe(transform=transform, ax=ax, **wireframe_kwargs)
+
+        if self._test_if_img_size_valid():
+            ax.set_xlim(-0.5, self._nx - 0.5)
+            ax.set_ylim(-0.5, self._ny - 0.5)
+        if add_axis_labels:
+            ax.set_xlabel('x (pixels)')
+            ax.set_ylabel('y (pixels)')
+        ax.set_aspect(1, adjustable=aspect_adjustable)
+
+        if show:
+            plt.show()
+        return ax
+
+    def plot_map_wireframe(
+        self,
+        ax: Axes | None = None,
+        label_poles: bool = True,
+        add_title: bool = True,
+        add_axis_labels: bool = True,
+        grid_interval: float = 30,
+        indicate_equator: bool = True,
+        indicate_prime_meridian: bool = True,
+        aspect_adjustable: Literal['box', 'datalim'] = 'box',
+        formatting: dict[_WireframeComponent, dict[str, Any]] | None = None,
+        common_formatting: dict[str, Any] | None = None,
+        **map_kwargs: Unpack[_MapKwargs],
+    ):
+        """
+        Plot wireframe (e.g. gridlines) of the map projection of the observation. See
+        :func:`Body.plot_wireframe_radec` for details of accepted arguments.
+
+        For example, to plot an orthographic map's wireframe with a red boundary and
+        dashed gridlines, you can use: ::
+
+            body.plot_map_wireframe(
+                projection='orthographic',
+                lat=45,
+                formatting={
+                    'grid': {'linestyle': '--'},
+                    'map_boundary': {'color': 'red'},
+                }
+            )
+        """
+        if ax is None:
+            ax = cast(Axes, plt.gca())
+
+        kwargs = self._get_wireframe_kw(
+            common_formatting=common_formatting, formatting=formatting
+        )
+        _, _, _, _, transformer, map_kw_used = self.generate_map_coordinates(
+            **map_kwargs
+        )
+        projection = map_kw_used['projection']
+
+        ax.set_aspect(1, adjustable=aspect_adjustable)
+
+        lon_ticks = np.arange(0, 360.0001, grid_interval)
+        lat_ticks = np.arange(-90, 90.0001, grid_interval)
+
+        if projection == 'azimuthal':
+            # Run separately for either side of equator to reduce issues for azimuthal
+            # where the grid lines overplot each other. We still can get issues for e.g.
+            # lat=45, but this fixes the most common cases of lat=0,90,-90 and it's a
+            # relatively minor cosmetic bug so is probably more-or-less fine as-is.
+            npts = 360
+            lats_to_plot = [np.linspace(-90, 0, npts), np.linspace(0, 90, npts)]
+        else:
+            npts = 720
+            lats_to_plot = [np.linspace(-90, 90, npts)]
+        for lon in lon_ticks:
+            if lon == 360 or (lon == 0 and projection == 'rectangular'):
+                continue
+            for lats in lats_to_plot:
+                # pylint: disable-next=unpacking-non-sequence
+                x, y = transformer.transform(lon * np.ones(npts), lats)
+                ax.plot(
+                    x,
+                    y,
+                    **kwargs['grid']
+                    | (
+                        kwargs['prime_meridian']
+                        if lon == 0 and indicate_prime_meridian
+                        else {}
+                    ),
+                )
+        npts = 720
+        for lat in lat_ticks:
+            if lat in {-90, 90}:
+                continue
+            # pylint: disable-next=unpacking-non-sequence
+            x, y = transformer.transform(np.linspace(0, 360, npts), lat * np.ones(npts))
+            ax.plot(
+                x,
+                y,
+                **kwargs['grid']
+                | (kwargs['equator'] if lat == 0 and indicate_equator else {}),
+            )
+
+        boundary: tuple[np.ndarray, np.ndarray] | None = None
+        # Formulae for boundaries based on Cartopy CRS boundaries
+        if projection == 'orthographic':
+            # Elipse boundary - https://math.stackexchange.com/questions/91132
+            x0 = self.r_eq
+            theta = np.radians(map_kw_used['lat'])
+            y0 = np.sqrt(
+                self.r_eq**2 * (np.sin(theta)) ** 2
+                + self.r_polar**2 * (np.cos(theta)) ** 2
+            )
+            t = np.linspace(0, -2 * np.pi, 100)
+            boundary = (x0 * np.cos(t), y0 * np.sin(t))
+        elif projection == 'azimuthal':
+            # Circular boundary
+            x0 = y0 = self.r_eq * np.pi
+            t = np.linspace(0, -2 * np.pi, 100)
+            boundary = (x0 * np.cos(t), y0 * np.sin(t))
+
+        if boundary:
+            ax.plot(*boundary, **kwargs['map_boundary'])
+
+        if label_poles and projection != 'rectangular':
+            for lat, s in ((90, 'N'), (-90, 'S')):
+                # pylint: disable-next=unpacking-non-sequence
+                x, y = transformer.transform(0, lat)
+                if math.isfinite(x) and math.isfinite(y):
+                    ax.text(x, y, s, **kwargs['pole'])
+
+        if add_axis_labels:
+            if projection == 'rectangular':
+                if self.positive_longitude_direction == 'W':
+                    ax.set_xlim(360, 0)
+                else:
+                    ax.set_xlim(0, 360)
+                ax.set_ylim(-90, 90)
+                ax.set_xlabel(
+                    f'Planetographic longitude ({self.positive_longitude_direction})'
+                )
+                ax.set_ylabel('Planetographic latitude')
+
+                ax.set_xticks(lon_ticks)
+                ax.set_xticklabels(
+                    [f'{x:.0f}°' if x % 90 == 0 else '' for x in lon_ticks]
+                )
+
+                ax.set_yticks(lat_ticks)
+                ax.set_yticklabels(
+                    [f'{y:.0f}°' if y % 90 == 0 else '' for y in lat_ticks]
+                )
+            elif projection in {'orthographic', 'azimuthal'}:
+                ax.set_xticks([])
+                ax.set_yticks([])
+
+        if add_title:
+            ax.set_title(self.get_description(multiline=True))
+        return ax
+
+    def plot_map(
+        self,
+        map_img: np.ndarray,
+        ax: Axes | None = None,
+        *,
+        wireframe_kwargs: dict[str, Any] | None = None,
+        **kwargs,
+    ) -> QuadMesh:
+        """
+        Utility function to easily plot a mapped image using `plt.imshow` with
+        appropriate extents, axis labels, gridlines etc.
+
+        Args:
+            map_img: Image to plot.
+            ax: Matplotlib axis to use for plotting. If `ax` is None (the default), then
+                a new figure and axis is created.
+            wireframe_kwargs: Dictionary of arguments passed to
+                :func:`plot_map_wireframe`.
+            **kwargs: Additional arguments are passed to
+                :func:`generate_map_coordinates` to specify the map projection used, and
+                to Matplotlib's `pcolormesh` to customise the plot. For example, can be
+                used to set the colormap of the plot using e.g.
+                `body.plot_map(..., projection='orthographic', cmap='Greys')`.
+
+        Returns:
+            Handle returned by Matplotlib's `pcolormesh`.
+        """
+        if ax is None:
+            fig, ax = plt.subplots()
+
+        map_kwargs = {}
+        for k in set(_MapKwargs.__optional_keys__) | set(_MapKwargs.__required_keys__):
+            if k in kwargs:
+                map_kwargs[k] = kwargs.pop(k)
+
+        _, _, xx, yy, _, _ = self.generate_map_coordinates(**map_kwargs)
+        h = ax.pcolormesh(xx, yy, map_img, **kwargs)
+        self.plot_map_wireframe(ax=ax, **(wireframe_kwargs or {}), **map_kwargs)
+        return h
+
+    def imshow_map(self, *args, **kwargs):
+        """
+        Alias for `plot_map` for backwards compatibility.
+
+        :meta private:
+        """
+        # backwards compatibility
+        return self.plot_map(*args, **kwargs)
+
+    # Wireframe generation
+    def _get_wireframe_overlay(
+        self,
+        *,
+        output_size: int | None,
+        dpi: int,
+        nx: int,
+        ny: int,
+        rgba: bool,
+        plot_fn: Callable[[Axes], Any],
+    ) -> np.ndarray:
+        output_size = output_size or max(nx, ny)
+        s = output_size / dpi
+        if nx > ny:
+            figsize = (s, s * ny / nx)
+        else:
+            figsize = (s * nx / ny, s)
+
+        fig = plt.figure(figsize=figsize, dpi=dpi, facecolor='w')
+        ax = fig.add_axes([0, 0, 1, 1], facecolor='w')
+        plot_fn(ax)
+        ax.axis('off')
+        ax.set_xticks([])
+        ax.set_yticks([])
+
+        with io.BytesIO() as io_buf:
+            fig.savefig(io_buf, format='raw', dpi=dpi, transparent=rgba)
+            io_buf.seek(0)
+            img_arr = np.frombuffer(io_buf.getvalue(), dtype=np.uint8)
+        plt.close(fig)
+        img = img_arr.reshape((fig.canvas.get_width_height()[::-1]) + (4,))
+        if not rgba:
+            img = np.asarray(np.mean(img[:, :, :3], axis=-1), dtype=np.uint8)
+        img = np.flipud(img)  # Make consistent with FITS orientation
+        return img
+
+    def get_wireframe_overlay_img(
+        self,
+        output_size: int | None = 1500,
+        dpi: int = 200,
+        rgba: bool = False,
+        **plot_kwargs,
+    ) -> np.ndarray:
+        """
+        .. warning ::
+
+            This is a beta feature and the API may change in future.
+
+        Generate a wireframe image of the target.
+
+        This effectively generates an image version of :func:`plot_wireframe_xy` which
+        can then be used as an overlay on top of the observation when creating figures
+        in other applications.
+
+        See also :func:`get_wireframe_overlay_map`.
+
+        .. note ::
+
+            The returned image data follows the FITS orientation convention (with the
+            origin at the bottom left) so may need to be flipped vertically in some
+            applications. If needed, the image can be flipped in Python using: ::
+
+                np.flipud(body.get_wireframe_overlay_img())
+
+        .. hint ::
+
+            If you are creating plots with Matplotlib, it is generally better to use
+            :func:`plot_wireframe_xy` directly rather than generating an image as it
+            will produce a higher quality plot.
+
+        Args:
+            output_size: Size of the output image in pixels. This will be the length of
+                the longest side of the image. The other side will be scaled accordingly
+                to maintain the aspect ratio of the observed data. If `size` is `None`,
+                then the size is set to match the size of the observed data.
+            dpi: Dots per inch of the output image. This can be used to control the size
+                of plotted elements in the output image - larger `dpi` values will
+                produce larger plotted elements.
+            rgba: By default, the returned image only has a single greyscale channel. If
+                `rgba` is `True`, then the returned image has 4 channels (red, green,
+                blue, alpha) which can be used to more easily overlay the wireframe on
+                top of the observed data in other applications.
+            **plot_kwargs: Additional arguments passed to :func:`plot_wireframe_xy`.
+        Returns:
+            Image of the wireframe which has the same aspect ratio as the observed data.
+        """
+        # TODO remove beta note when stable
+        return self._get_wireframe_overlay(
+            output_size=output_size,
+            dpi=dpi,
+            nx=self._nx,
+            ny=self._ny,
+            rgba=rgba,
+            plot_fn=lambda ax: self.plot_wireframe_xy(
+                ax=ax,
+                color='k',
+                add_axis_labels=False,
+                add_title=False,
+                **plot_kwargs or {},
+            ),
+        )
+
+    def get_wireframe_overlay_map(
+        self,
+        output_size: int | None = 1500,
+        dpi: int = 200,
+        rgba: bool = False,
+        plot_kwargs: dict[str, Any] | None = None,
+        **map_kwargs: Unpack[_MapKwargs],
+    ) -> np.ndarray:
+        """
+        .. warning ::
+
+            This is a beta feature and the API may change in future.
+
+        Generate a wireframe map of the target.
+
+        This effectively generates an image version of :func:`plot_map_wireframe` which
+        can then be used as an overlay on top of the mapped observation when creating
+        figures in other applications.
+
+        See also :func:`get_wireframe_overlay_img`.
+
+        .. note ::
+
+            The returned image data follows the FITS orientation convention (with the
+            origin at the bottom left) so may need to be flipped vertically in some
+            applications. If needed, the image can be flipped in Python using: ::
+
+                np.flipud(body.get_wireframe_overlay_map())
+
+        .. hint ::
+
+            If you are creating plots with Matplotlib, it is generally better to use
+            :func:`plot_map_wireframe` directly rather than generating an image as it
+            will produce a higher quality plot.
+
+        Args:
+            output_size: Size of the output image in pixels. This will be the length of
+                the longest side of the map. The other side will be scaled accordingly
+                to maintain the aspect ratio of the observed data. If `size` is `None`,
+                then the size is set to match the pixel size of the map.
+            dpi: Dots per inch of the output image. This can be used to control the size
+                of plotted elements in the output image - larger `dpi` values will
+                produce larger plotted elements.
+            rgba: By default, the returned image only has a single greyscale channel. If
+                `rgba` is `True`, then the returned image has 4 channels (red, green,
+                blue, alpha) which can be used to more easily overlay the wireframe on
+                top of the observed data in other applications.
+            plot_kwargs: Dictionary of arguments passed to :func:`plot_map_wireframe`.
+            **map_kwargs: Additional arguments passed to
+                :func:`generate_map_coordinates` to specify map projection to use.
+        Returns:
+            Image of the map wireframe which has the same aspect ratio as the map.
+        """
+        # TODO remove beta note when stable
+        lons, lats, xx, yy, transformer, map_kw_used = self.generate_map_coordinates(
+            **map_kwargs
+        )
+        nx = xx.shape[1]
+        ny = yy.shape[0]
+
+        def plot_fn(ax: Axes):
+            self.plot_map_wireframe(
+                ax=ax,
+                add_axis_labels=False,
+                add_title=False,
+                **(plot_kwargs or {}) | dict(common_formatting=dict(color='k')),
+                **map_kwargs,
+            )
+            # Add dx/dy to the limits to ensure the wireframe covers all of each pixel
+            # as the xx and yy coordinates only give the centre of each pixel
+            dx = abs(xx[0][1] - xx[0][0])/2
+            ax.set_xlim(np.nanmin(xx) - dx, np.nanmax(xx) + dx)
+            dy = abs(yy[1][0] - yy[0][0])/2
+            ax.set_ylim(np.nanmin(yy) - dy, np.nanmax(yy) + dy)
+
+        return self._get_wireframe_overlay(
+            output_size=output_size, dpi=dpi, nx=nx, ny=ny, rgba=rgba, plot_fn=plot_fn
+        )
+
     # Backplane management
     @staticmethod
     def standardise_backplane_name(name: str) -> str:
         """
         Create a standardised version of a backplane name when finding and registering
         backplanes.
 
@@ -1315,16 +1661,16 @@
         Plot a map of backplane values on the target body.
 
         Args:
             name: Name of the desired backplane.
             ax: Matplotlib axis to use for plotting. If `ax` is None (the default), then
                 a new figure and axis is created.
             show: Toggle showing the plotted figure with `plt.show()`
-            plot_kwargs: Passed to Matplotlib's `pcolormesh` when plotting the backplane
-                map. For example, can be used to set the colormap of the plot using
+            plot_kwargs: Passed to :func:`plot_map` when plotting the backplane map. For
+                example, can be used to set the colormap of the plot using
                 `body.plot_backplane_map(..., plot_kwargs=dict(cmap='Greys'))`.
             **map_kwargs: Additional arguments are passed to
                 :func:`generate_map_coordinates` to specify and customise the map
                 projection.
         Returns:
             The axis containing the plotted data.
         """
@@ -1335,110 +1681,18 @@
         im = self.plot_map(
             backplane.get_map(**map_kwargs),
             ax=ax,
             **map_kwargs,
             **plot_kwargs or {},
         )
         plt.colorbar(im, label=backplane.description)
-        ax.set_title(self.get_description(multiline=True))
         if show:
             plt.show()
         return ax
 
-    def plot_map(
-        self,
-        map_img: np.ndarray,
-        ax: Axes | None = None,
-        grid: bool = True,
-        **kwargs,
-    ) -> QuadMesh:
-        """
-        Utility function to easily plot a mapped image using `plt.imshow` with
-        appropriate extents, axis labels etc.
-
-        Args:
-            map_img: Image to plot.
-            ax: Matplotlib axis to use for plotting. If `ax` is None (the default), then
-                a new figure and axis is created.
-            grid: Toggle plotting a lon/lat grid.
-            **kwargs: Additional arguments are passed to
-                :func:`generate_map_coordinates` to specify the map projection used, and
-                to Matplotlib's `pcolormesh` to customise the plot. For example, can be
-                used to set the colormap of the plot using e.g.
-                `body.plot_map(..., projection='orthographic', cmap='Greys')`.
-
-        Returns:
-            Handle returned by Matplotlib's `pcolormesh`.
-        """
-        if ax is None:
-            fig, ax = plt.subplots()
-
-        map_kwargs = {}
-        for k in set(_MapKwargs.__optional_keys__) | set(_MapKwargs.__required_keys__):
-            if k in kwargs:
-                map_kwargs[k] = kwargs.pop(k)
-
-        _, _, xx, yy, transformer, map_kw_used = self.generate_map_coordinates(
-            **map_kwargs
-        )
-        projection = map_kw_used['projection']
-
-        h = ax.pcolormesh(xx, yy, map_img, **kwargs)
-        ax.set_aspect(1, adjustable='box')
-
-        step = 30
-        lon_ticks = np.arange(0, 360.1, step)
-        lat_ticks = np.arange(-90, 90.1, step)
-
-        if projection == 'rectangular':
-            if self.positive_longitude_direction == 'W':
-                ax.set_xlim(360, 0)
-            else:
-                ax.set_xlim(0, 360)
-            ax.set_ylim(-90, 90)
-            ax.set_xlabel(
-                f'Planetographic longitude ({self.positive_longitude_direction})'
-            )
-            ax.set_ylabel('Planetographic latitude')
-
-            ax.set_xticks(lon_ticks)
-            ax.set_xticklabels([f'{x:.0f}°' if x % 90 == 0 else '' for x in lon_ticks])
-
-            ax.set_yticks(lat_ticks)
-            ax.set_yticklabels([f'{y:.0f}°' if y % 90 == 0 else '' for y in lat_ticks])
-
-        if grid:
-            grid_kw = dict(color='k', alpha=0.5, linewidth=1)
-            npts = 360
-            for lon in lon_ticks:
-                if lon == 360:
-                    continue
-                # pylint: disable-next=unpacking-non-sequence
-                x, y = transformer.transform(
-                    lon * np.ones(npts), np.linspace(-90, 90, npts)
-                )
-                ax.plot(x, y, **grid_kw, linestyle='-' if lon == 0 else ':')
-
-            for lat in lat_ticks:
-                # pylint: disable-next=unpacking-non-sequence
-                x, y = transformer.transform(
-                    np.linspace(0, 360, npts), lat * np.ones(npts)
-                )
-                ax.plot(x, y, **grid_kw, linestyle='-' if lat == 0 else ':')
-        return h
-
-    def imshow_map(self, *args, **kwargs):
-        """
-        Alias for `plot_map` for backwards compatibility.
-
-        :meta private:
-        """
-        # backwards compatibility
-        return self.plot_map(*args, **kwargs)
-
     # Mapping projection internals
     @_cache_stable_result
     def generate_map_coordinates(
         self,
         projection: str = 'rectangular',
         degree_interval: float = 1,
         lon: float = 0,
@@ -2579,8 +2833,46 @@
         )
         msg.append(
             '- Map function: :func:`planetmapper.{}`'.format(
                 bp.get_map.__qualname__  # type: ignore
             )
         )
         msg.append('')
+
+    msg.append('------------')
+    msg.append('')
+    msg.append('Wireframe images')
+    msg.append('=' * len(msg[-1]))
+    msg.append('')
+
+    msg.append(
+        'In addition to the above backplanes, a `WIREFRAME` backplane is also included '
+        'by default in saved FITS files. This backplane contains a "wireframe" image '
+        'of the body, which shows latitude/longitude gridlines, labels poles, displays '
+        'the body\'s limb etc. These wireframe images can be used to help orient the '
+        'observations, and can be used as an overlay if you are creating figures from '
+        'the FITS files.'
+    )
+    msg.append('')
+
+    msg.append(
+        'The wireframe images are a graphical guide rather than containing any '
+        'scientific data, so they are not registered like the other backplanes. '
+        'Note that the wireframe images have a fixed size, so they will not be the '
+        'same size as the data/mapped data (although the aspect ratio will be the '
+        'same).'
+    )
+    msg.append('')
+
+    msg.append(
+        '- Image function: :func:`planetmapper.{}`'.format(
+            body.get_wireframe_overlay_img.__qualname__
+        )
+    )
+    msg.append(
+        '- Map function: :func:`planetmapper.{}`'.format(
+            body.get_wireframe_overlay_map.__qualname__
+        )
+    )
+    msg.append('')
+
     return '\n'.join(msg)
```

### Comparing `planetmapper-1.6.5/planetmapper/data/rings.json` & `planetmapper-1.7.0/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/planetmapper/data_loader.py` & `planetmapper-1.7.0/planetmapper/data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/planetmapper/gui.py` & `planetmapper-1.7.0/planetmapper/gui.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/planetmapper/kernel_downloader.py` & `planetmapper-1.7.0/planetmapper/kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/planetmapper/observation.py` & `planetmapper-1.7.0/planetmapper/observation.py`

 * *Files 4% similar despite different names*

```diff
@@ -617,15 +617,15 @@
         called manually.
 
         Args:
             header: FITS Header which the metadata will be added to in-place. If
                 `header` is `None`, then :attr:`header` will be modified.
         """
         self.append_to_header(
-            'VERSION', common.__version__, 'Planet Mapper version.', header=header
+            'VERSION', common.__version__, 'PlanetMapper version.', header=header
         )
         self.append_to_header('URL', common.__url__, 'Webpage.', header=header)
         self.append_to_header(
             'DATE',
             datetime.datetime.now().strftime('%Y-%m-%dT%H:%M:%S'),
             'File generation datetime.',
             header=header,
@@ -818,15 +818,21 @@
             date=self.dtm.strftime('%Y-%m-%dT%H%M%S'),
             extension=extension,
             suffix=suffix,
         )
 
     @progress_decorator
     def save_observation(
-        self, path: str, *, show_progress: bool = False, print_info: bool = True
+        self,
+        path: str,
+        *,
+        include_wireframe: bool = True,
+        wireframe_kwargs: dict[str, Any] | None = None,
+        show_progress: bool = False,
+        print_info: bool = True,
     ) -> None:
         """
         Save a FITS file containing the observed data and generated backplanes.
 
         The primary HDU in the FITS file will be the :attr:`data` and :attr:`header`
         of the observed data, with appropriate metadata automatically added to the
         header by :func:`add_header_metadata`. The backplanes are generated from all the
@@ -834,14 +840,20 @@
         HDUs in the FITS file.
 
         For larger image sizes, the backplane generation can be slow, so this function
         may take some time to complete.
 
         Args:
             path: Filepath of output file.
+            include_wireframe: Toggle generating and saving wireframe overlay image as
+                an additional backplane of the output FITS file. The wireframe is
+                generated by :func:`BodyXY.get_wireframe_overlay_img`.
+            wireframe_kwargs: Dictionary of keyword arguments passed to
+                :func:`BodyXY.get_wireframe_overlay_img` to customise the wireframe
+                overlay.
             show_progress: Display a progress bar rather than printing progress info.
                 This does not have an effect if `show_progress=True` was set when
                 creating this `Observation`.
             print_info: Toggle printing of progress information (defaults to `True`).
         """
         if show_progress and self._get_progress_hook() is None:
             print_info = False
@@ -863,17 +875,29 @@
             hdul = fits.HDUList([fits.PrimaryHDU(data=data, header=header)])
             for bp_idx, (name, backplane) in enumerate(self.backplanes.items()):
                 self._update_progress_hook((bp_idx + 1) / progress_max)
                 if print_info:
                     print(' Creating backplane:', name)
                 img = backplane.get_img()
                 header = fits.Header([('ABOUT', backplane.description)])
-                header.add_comment('Backplane generated by Planet Mapper software.')
+                header.add_comment('Backplane generated by PlanetMapper software.')
                 hdu = fits.ImageHDU(data=img, header=header, name=name)
                 hdul.append(hdu)
+
+            if include_wireframe:
+                if print_info:
+                    print(' Creating wireframe...')
+                wireframe = self.get_wireframe_overlay_img(**wireframe_kwargs or {})
+                header = fits.Header([('ABOUT', 'Wireframe image overlay')])
+                header.add_comment(
+                    'Wireframe overlay generated by PlanetMapper software.'
+                )
+                hdu = fits.ImageHDU(data=wireframe, header=header, name='WIREFRAME')
+                hdul.append(hdu)
+
             if print_info:
                 print(' Saving file...')
             utils.check_path(path)
             hdul.writeto(path, overwrite=True, output_verify='warn')
         if print_info:
             print('File saved')
 
@@ -882,16 +906,18 @@
             self._remove_progress_hook()
 
     @progress_decorator
     def save_mapped_observation(
         self,
         path: str,
         *,
-        include_backplanes: bool = True,
         interpolation: Literal['nearest', 'linear', 'quadratic', 'cubic'] = 'linear',
+        include_backplanes: bool = True,
+        include_wireframe: bool = True,
+        wireframe_kwargs: dict[str, Any] | None = None,
         show_progress: bool = False,
         print_info: bool = True,
         **map_kwargs: Unpack[_MapKwargs],
     ) -> None:
         """
         Save a FITS file containing the mapped observation in a cylindrical projection.
 
@@ -899,19 +925,25 @@
         data is saved by default.
 
         For larger image sizes, the map projection and backplane generation can be slow,
         so this function may take some time to complete.
 
         Args:
             path: Filepath of output file.
-            include_backplanes: Toggle generating and saving backplanes to output FITS
-                file.
             interpolation: Interpolation used when mapping. This can either any of
                 `'nearest'`, `'linear'`, `'quadratic'` or `'cubic'`. Passed to
                 :func:`BodyXY.map_img`.
+            include_backplanes: Toggle generating and saving backplanes to output FITS
+                file.
+            include_wireframe: Toggle generating and saving wireframe overlay map as an
+                additional backplane of the output FITS file. The wireframe is generated
+                by :func:`BodyXY.get_wireframe_overlay_map`.
+            wireframe_kwargs: Dictionary of keyword arguments passed to
+                :func:`BodyXY.get_wireframe_overlay_map` to customise the wireframe
+                overlay.
             show_progress: Display a progress bar rather than printing progress info.
                 This does not have an effect if `show_progress=True` was set when
                 creating this `Observation`.
             print_info: Toggle printing of progress information (defaults to `True`).
             **map_kwargs: Additional arguments are passed to
                 :func:`BodyXY.generate_map_coordinates` to specify and customise the map
                 projection.
@@ -942,19 +974,33 @@
             if include_backplanes:
                 for bp_idx, (name, backplane) in enumerate(self.backplanes.items()):
                     self._update_progress_hook((bp_idx + 1) / progress_max)
                     if print_info:
                         print(' Creating backplane:', name)
                     img = backplane.get_map(**map_kwargs)
                     header = fits.Header([('ABOUT', backplane.description)])
-                    header.add_comment('Backplane generated by Planet Mapper software.')
+                    header.add_comment('Backplane generated by PlanetMapper software.')
                     self._add_map_wcs_to_header(header, **map_kwargs)
 
                     hdu = fits.ImageHDU(data=img, header=header, name=name)
                     hdul.append(hdu)
+
+            if include_wireframe:
+                if print_info:
+                    print(' Creating wireframe...')
+                wireframe = self.get_wireframe_overlay_map(
+                    **wireframe_kwargs or {}, **map_kwargs
+                )
+                header = fits.Header([('ABOUT', 'Wireframe map overlay')])
+                header.add_comment(
+                    'Wireframe overlay generated by PlanetMapper software.'
+                )
+                hdu = fits.ImageHDU(data=wireframe, header=header, name='WIREFRAME')
+                hdul.append(hdu)
+
             if print_info:
                 print(' Saving file...')
             utils.check_path(path)
             hdul.writeto(path, overwrite=True, output_verify='warn')
         if print_info:
             print('File saved')
```

### Comparing `planetmapper-1.6.5/planetmapper/progress.py` & `planetmapper-1.7.0/planetmapper/progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/planetmapper/utils.py` & `planetmapper-1.7.0/planetmapper/utils.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.7.0/planetmapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.6.5
+Version: 1.7.0
 Summary: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
```

### Comparing `planetmapper-1.6.5/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.7.0/planetmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/setup.py` & `planetmapper-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/tests/test_base.py` & `planetmapper-1.7.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/tests/test_basic_body.py` & `planetmapper-1.7.0/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/tests/test_body.py` & `planetmapper-1.7.0/tests/test_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.5/tests/test_body_xy.py` & `planetmapper-1.7.0/tests/test_body_xy.py`

 * *Files 3% similar despite different names*

```diff
@@ -379,14 +379,35 @@
         )
 
     def test_plot_wireframe(self):
         fig, ax = plt.subplots()
         self.body.plot_wireframe_km(ax=ax)
         plt.close(fig)
 
+        fig, ax = plt.subplots()
+        self.body.plot_map_wireframe(ax=ax)
+        plt.close(fig)
+
+        fig, ax = plt.subplots()
+        self.body.plot_map_wireframe(ax=ax, projection='orthographic', lat=56)
+        plt.close(fig)
+
+        fig, ax = plt.subplots()
+        self.body.plot_map_wireframe(ax=ax, projection='azimuthal', lat=-90)
+        plt.close(fig)
+    
+    def test_get_wireframe_overlay(self):
+        img = self.body.get_wireframe_overlay_img(output_size=100)
+        self.assertEqual(max(img.shape), 100)
+        self.assertEqual(len(img.shape), 2)
+
+        img = self.body.get_wireframe_overlay_map(output_size=100)
+        self.assertEqual(max(img.shape), 100)
+        self.assertEqual(len(img.shape), 2)
+
     def test_map_img(self):
         self.body.set_img_size(4, 3)
         self.body.set_disc_params(2, 1, 1.5, 45.678)
 
         image = np.array(
             [
                 [-1.0, 2.2, 3.3, 4.4],
```

### Comparing `planetmapper-1.6.5/tests/test_init.py` & `planetmapper-1.7.0/tests/test_init.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,16 +6,21 @@
 
 class TestInit(unittest.TestCase):
     def test_init(self):
         self.assertEqual(planetmapper.__author__, 'Oliver King')
         self.assertEqual(planetmapper.__url__, 'https://github.com/ortk95/planetmapper')
 
     def test_version(self):
-        self.assertEqual(planetmapper.__version__.count('.'), 2)
         self.assertEqual(planetmapper.__version__.strip(), planetmapper.__version__)
+        self.assertEqual(planetmapper.__version__.count('.'), 2)
+        self.assertEqual(len(planetmapper.__version__.split('.')), 3)
+        self.assertTrue(all(x.isdigit() for x in planetmapper.__version__.split('.')))
 
+        self.assertEqual(
+            str(version.Version(planetmapper.__version__)), planetmapper.__version__
+        )
         self.assertGreater(
             version.Version(planetmapper.__version__), version.Version('1.6.2')
         )
-        self.assertEqual(
-            str(version.Version(planetmapper.__version__)), planetmapper.__version__
+        self.assertLess(
+            version.Version(planetmapper.__version__), version.Version('2.0.0')
         )
```

### Comparing `planetmapper-1.6.5/tests/test_observation.py` & `planetmapper-1.7.0/tests/test_observation.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,15 +136,14 @@
             self.assertIsNone(obs.path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertEqual(obs.header, header)
             self.assertTrue(np.array_equal(obs.data, data))
 
-
         with self.subTest('image+header'):
             data = np.ones((5, 6))
             header = fits.Header(
                 {'OBJECT': 'jupiter', 'TELESCOP': 'HST', 'DATE-OBS': '2005-01-01'}
             )
             obs = Observation(
                 data=data,
@@ -356,66 +355,110 @@
     def test_save_observation(self):
         self.observation.set_disc_params(2.5, 3.1, 3.9, 123.456)
         self.observation.set_disc_method('<<<test>>>')
 
         path = os.path.join(common_testing.TEMP_PATH, 'test_nav.fits')
 
         # test progress bar here too
-        self.observation.save_observation(path, show_progress=True)
+        self.observation.save_observation(
+            path, show_progress=True, wireframe_kwargs=dict(output_size=20, dpi=20)
+        )
         self.compare_fits_to_reference(path)
 
     def test_save_mapped_observation(self):
         self.observation.set_disc_params(2.5, 3.1, 3.9, 123.456)
         self.observation.set_disc_method('<<<test>>>')
 
         map_kwargs = {
             'rectangular-nearest': dict(degree_interval=30, interpolation='nearest'),
-            'rectangular-linear': dict(degree_interval=30, interpolation='linear'),
+            'rectangular-linear': dict(
+                degree_interval=30, interpolation='linear', include_wireframe=False
+            ),
             'rectangular-quadratic': dict(
-                degree_interval=30, interpolation='quadratic'
+                degree_interval=30,
+                interpolation='quadratic',
+                include_backplanes=False,
+                include_wireframe=False,
+            ),
+            'rectangular-cubic': dict(
+                degree_interval=30,
+                interpolation='cubic',
+                include_backplanes=False,
+                include_wireframe=False,
+            ),
+            'orthographic-1': dict(
+                projection='orthographic', size=10, include_wireframe=False
+            ),
+            'orthographic-2': dict(
+                projection='orthographic',
+                lat=90,
+                size=5,
             ),
-            'rectangular-cubic': dict(degree_interval=30, interpolation='cubic'),
-            'orthographic-1': dict(projection='orthographic', size=10),
-            'orthographic-2': dict(projection='orthographic', lat=90, size=5),
             'orthographic-3': dict(
-                projection='orthographic', lat=-21.3, lon=-42, size=4
+                projection='orthographic',
+                lat=-21.3,
+                lon=-42,
+                size=4,
+                include_wireframe=False,
+            ),
+            'azimuthal-1': dict(
+                projection='azimuthal', size=10, include_wireframe=False
+            ),
+            'azimuthal-2': dict(
+                projection='azimuthal',
+                lat=-90,
+                size=5,
+            ),
+            'azimuthal-3': dict(
+                projection='azimuthal',
+                lat=42,
+                lon=12.345,
+                size=4,
+                include_wireframe=False,
             ),
-            'azimuthal-1': dict(projection='azimuthal', size=10),
-            'azimuthal-2': dict(projection='azimuthal', lat=-90, size=5),
-            'azimuthal-3': dict(projection='azimuthal', lat=42, lon=12.345, size=4),
         }
 
         for map_type, map_kw in map_kwargs.items():
             with self.subTest(
                 map_type=map_type,
             ):
                 path = os.path.join(common_testing.TEMP_PATH, f'map_{map_type}.fits')
-                self.observation.save_mapped_observation(path, **map_kw)
+                self.observation.save_mapped_observation(
+                    path, **map_kw, wireframe_kwargs=dict(output_size=20, dpi=20)
+                )
                 self.compare_fits_to_reference(path)
 
     def compare_fits_to_reference(self, path: str):
         filename = os.path.basename(path)
         path_ref = os.path.join(common_testing.DATA_PATH, 'outputs', filename)
         with fits.open(path) as hdul, fits.open(path_ref) as hdul_ref:
-            self.assertEqual(len(hdul), len(hdul_ref))
+            with self.subTest('Number of backplanes', filename=filename):
+                self.assertEqual(len(hdul), len(hdul_ref))
             for hdu, hdu_ref in zip(hdul, hdul_ref):
                 self.assertEqual(hdu.name, hdu_ref.name)
                 extname = hdu.name
                 with self.subTest(filename=filename, extname=extname):
                     data = hdu.data
                     data_ref = hdu_ref.data
                     self.assertEqual(data.shape, data_ref.shape)
-                    self.assertTrue(np.allclose(data, data_ref, equal_nan=True))
+
+                    # Significantly increase tolerance for wireframe as it is generated
+                    # from a Matplotlib plot, so is sensitive to the OS/environment
+                    # (e.g. fonts available), and is only a cosmetic backplane anyway
+                    # so the actual values don't matter anywhere near as much as the
+                    # other backplanes.
+                    atol = 64 if extname == 'WIREFRAME' else 1e-8 # 1e-8 is the default
+                    self.assertTrue(np.allclose(data, data_ref, atol=atol, equal_nan=True))
 
                 header = hdu.header
                 header_ref = hdu_ref.header
                 with self.subTest(filename=filename, extname=extname):
                     self.assertEqual(set(header.keys()), set(header_ref.keys()))
 
-                keys_to_skip = ['*DATE*', '*VERSION*']
+                keys_to_skip = {'*DATE*', '*VERSION*'}
                 for key in header.keys():
                     if any(
                         fnmatch.fnmatch(key.casefold(), pattern.casefold())
                         for pattern in keys_to_skip
                     ):
                         continue
                     value = header[key]
```

### Comparing `planetmapper-1.6.5/tests/test_utils.py` & `planetmapper-1.7.0/tests/test_utils.py`

 * *Files identical despite different names*

