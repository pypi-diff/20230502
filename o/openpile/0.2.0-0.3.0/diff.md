# Comparing `tmp/openpile-0.2.0.tar.gz` & `tmp/openpile-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-95t1783b/openpile-0.2.0.tar", last modified: Mon Apr 24 19:19:03 2023, max compression
+gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-72ls0hyh/openpile-0.3.0.tar", last modified: Tue May  2 19:18:08 2023, max compression
```

## Comparing `openpile-0.2.0.tar` & `openpile-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 19:18:54.000000 openpile-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-24 19:19:03.000000 openpile-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-24 19:18:54.000000 openpile-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-24 19:18:54.000000 openpile-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-24 19:19:03.000000 openpile-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 19:18:54.000000 openpile-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/analyses.py
--rw-r--r--   0 runner    (1001) docker     (123)    51654 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/construct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29111 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/core/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/core/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/core/txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/soilmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/Hb_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/Mb_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/mt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/py_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/qz_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/tz_curves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-24 19:18:54.000000 openpile-0.2.0/test/test_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 19:18:54.000000 openpile-0.2.0/test/test_pycurves.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-24 19:18:54.000000 openpile-0.2.0/test/test_utils_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 19:17:55.000000 openpile-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-02 19:18:08.000000 openpile-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-02 19:17:55.000000 openpile-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-02 19:17:55.000000 openpile-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-02 19:18:08.000000 openpile-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-02 19:17:55.000000 openpile-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/analyses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54305 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/construct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29111 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/core/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/core/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/core/txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/soilmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/Hb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/Mb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/mt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/py_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/qz_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/tz_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-02 19:17:55.000000 openpile-0.3.0/test/test_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-02 19:17:55.000000 openpile-0.3.0/test/test_pycurves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-02 19:17:55.000000 openpile-0.3.0/test/test_utils_misc.py
```

### Comparing `openpile-0.2.0/LICENSE.txt` & `openpile-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/PKG-INFO` & `openpile-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.2.0
+Version: 0.3.0
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
 Project-URL: Documentation, https://openpile.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/TchilDill/openpile
```

### Comparing `openpile-0.2.0/README.md` & `openpile-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/setup.cfg` & `openpile-0.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [metadata]
 name = openpile
 author = Guillaume Melin
 author_email = guillaume.melin@icloud.com
 license = GPLv3
 license_file = LICENSE.txt
-version = attr: openpile.__version__
 description = Library for geotechnical pile calculations.
 url = https://github.com/TchilDill/openpile
 keywords = Offshore Wind, PILE, Geotechnics, monopile, pin-piles, Geotechnical, calculations, PISA, winkler
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Programming Language :: Python
```

### Comparing `openpile-0.2.0/src/openpile/analyses.py` & `openpile-0.3.0/src/openpile/analyses.py`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/src/openpile/construct.py` & `openpile-0.3.0/src/openpile/construct.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,14 +183,120 @@
                 "I [m4]": second_moment_of_area,
             }
         )
 
     def __str__(self):
         return self.data.to_string()
 
+    @property
+    def bottom_elevation(self) -> float:
+        """
+        Bottom elevation of the pile [m VREF].
+        """
+        return self.top_elevation - sum(self.pile_sections["length"])
+
+    @property
+    def length(self) -> float:
+        """
+        Pile length [m].
+        """
+        return sum(self.pile_sections["length"])
+
+    @property
+    def volume(self) -> float:
+        """
+        Pile volume [m3].
+        """
+        A = self.data["Area [m2]"].values[1:]
+        L = np.abs(np.diff(self.data["Elevation [m]"].values))
+        return round((A * L).sum(), 2)
+
+    @property
+    def weight(self) -> float:
+        """
+        Pile weight [kN].
+        """
+        return round(self.volume * self._uw, 2)
+
+    @property
+    def E(self) -> float:
+        """
+        Young modulus of the pile material [kPa]. Thie value does not vary across and along the pile.
+        """
+        try:
+            return self._young_modulus
+        except AttributeError:
+            print("Please first create the pile with the Pile.create() method")
+        except Exception as e:
+            print(e)
+
+    @E.setter
+    def E(self, value: float) -> None:
+        try:
+            self._young_modulus = value
+        except AttributeError:
+            print("Please first create the pile with the Pile.create() method")
+        except Exception as e:
+            print(e)
+
+    @property
+    def I(self) -> float:
+        """
+        Second moment of area of the pile [m4].
+
+        The user can use the method :py:meth:`openpile.construct.Pile.set_I` to customise the second
+        moment of area for different sections of the pile.
+        """
+        try:
+            return self.data["I [m4]"]
+        except AttributeError:
+            print("Please first create the pile with the Pile.create() method")
+        except Exception as e:
+            print(e)
+
+    @property
+    def width(self) -> float:
+        """
+        Width of the pile [m]. (Used to compute soil springs)
+        """
+        try:
+            return self.data.loc[:, "Diameter [m]"]
+        except AttributeError:
+            print("Please first create the pile with the Pile.create() method")
+        except Exception as e:
+            print(e)
+
+    @width.setter
+    def width(self, value: float) -> None:
+        try:
+            self.data.loc[:, "Diameter [m]"] = value
+        except AttributeError:
+            print("Please first create the pile with the Pile.create() method")
+        except Exception as e:
+            print(e)
+
+    @property
+    def area(self) -> float:
+        "Sectional area of the pile [m2]"
+        try:
+            return self.data.loc[:, "Area [m2]"]
+        except AttributeError:
+            print("Please first create the pile with the Pile.create() method")
+        except Exception as e:
+            print(e)
+
+    @area.setter
+    def area(self, value: float) -> None:
+        try:
+            self.data.loc[:, "Area [m2]"] = value
+        except AttributeError:
+            print("Please first create the pile with the Pile.create() method")
+        except Exception as e:
+            print(e)
+
     @classmethod
     def create(
         cls,
         name: str,
         top_elevation: float,
         pile_sections: Dict[str, List[float]],
         kind: Literal[
@@ -248,15 +354,15 @@
         top_elevation: float,
         bottom_elevation: float,
         diameter: float,
         wt: float,
         material: str = "Steel",
     ):
         """A method to simplify the creation of a Pile instance.
-        This method creates a circular and hollow pile of constant diameter.
+        This method creates a circular and hollow pile of constant diameter and wall thickness.
 
         Parameters
         ----------
         name : str
             Pile/Structure's name.
         top_elevation : float
             top elevation of the pile [m VREF]
@@ -291,80 +397,14 @@
                     diameter,
                 ],
             },
         )
 
         return obj
 
-    @property
-    def bottom_elevation(self) -> float:
-        """
-        Bottom elevation of the pile [m VREF].
-        """
-        return self.top_elevation - sum(self.pile_sections["length"])
-
-    @property
-    def length(self) -> float:
-        """
-        Pile length [m].
-        """
-        return sum(self.pile_sections["length"])
-
-    @property
-    def volume(self) -> float:
-        """
-        Pile volume [m3].
-        """
-        A = self.data["Area [m2]"].values[1:]
-        L = np.abs(np.diff(self.data["Elevation [m]"].values))
-        return round((A * L).sum(), 2)
-
-    @property
-    def weight(self) -> float:
-        """
-        Pile weight [kN].
-        """
-        return round(self.volume * self._uw, 2)
-
-    @property
-    def E(self) -> float:
-        """
-        Young modulus of the pile material. Thie value does not vary across and along the pile.
-        """
-        try:
-            return self._young_modulus
-        except AttributeError:
-            print("Please first create the pile with the Pile.create() method")
-        except Exception as e:
-            print(e)
-
-    @E.setter
-    def E(self, value: float) -> None:
-        try:
-            self._young_modulus = value
-        except AttributeError:
-            print("Please first create the pile with the Pile.create() method")
-        except Exception as e:
-            print(e)
-
-    @property
-    def I(self) -> float:
-        """
-        Second moment of area of the pile.
-
-        The user can use the method :py:meth:`openpile.construct.Pile.set_I` to customise the second
-        moment of area for different sections of the pile.
-        """
-        try:
-            return self.data["I [m4]"]
-        except AttributeError:
-            print("Please first create the pile with the Pile.create() method")
-        except Exception as e:
-            print(e)
-
     def set_I(self, value: float, section: int) -> None:
         """set second moment of area for a particular section of the pile.
 
         Parameters
         ----------
         value : float
             new second moment of area [m4].
@@ -382,82 +422,62 @@
                 self.data.loc[section * 2 - 2, "I [m4]"] = value
                 self.data.loc[section * 2 - 1, "I [m4]"] = value
         except AttributeError:
             print("Please first create the pile with the Pile.create() method")
         except Exception as e:
             raise Exception
 
-    @property
-    def width(self) -> float:
-        """
-        Width of the pile. (Used to compute soil springs)
-        """
-        try:
-            return self.data.loc[:, "Diameter [m]"]
-        except AttributeError:
-            print("Please first create the pile with the Pile.create() method")
-        except Exception as e:
-            print(e)
+    def plot(self, assign=False):
+        """Creates a plot of the pile with the properties.
 
-    @width.setter
-    def width(self, value: float) -> None:
-        try:
-            self.data.loc[:, "Diameter [m]"] = value
-        except AttributeError:
-            print("Please first create the pile with the Pile.create() method")
-        except Exception as e:
-            print(e)
+        Parameters
+        ----------
+        assign : bool, optional
+            this parameter can be set to True to return the figure, by default False
 
-    @property
-    def area(self) -> float:
-        "Sectional area of the pile"
-        try:
-            return self.data.loc[:, "Area [m2]"]
-        except AttributeError:
-            print("Please first create the pile with the Pile.create() method")
-        except Exception as e:
-            print(e)
+        Returns
+        -------
+        matplotlib.pyplot.figure
+            only return the object if assign=True
 
-    @area.setter
-    def area(self, value: float) -> None:
-        try:
-            self.data.loc[:, "Area [m2]"] = value
-        except AttributeError:
-            print("Please first create the pile with the Pile.create() method")
-        except Exception as e:
-            print(e)
+        Example
+        -------
 
-    def plot(self, assign=False):
+        .. image:: _static/plots/Pile_plot.png
+           :width: 70%
+
+        """
         fig = graphics.pile_plot(self)
         return fig if assign else None
 
 
 @dataclass(config=PydanticConfig)
 class Layer:
     """A class to create a layer.
 
     The Layer stores information on the soil parameters of the layer as well
     as the relevant/representative constitutive model (aka. the soil spring).
 
     Parameters
     ----------
     name : str
-        Name of the layer, use for printout
+        Name of the layer, use for printout.
     top : float
-        top elevation of the layer in [m]
+        top elevation of the layer in [m].
     bottom : float
-        bottom elevation of the layer in [m]
+        bottom elevation of the layer in [m].
     weight : float
-        total unit weight in [kN/m3], cannot be lower than 10 kN/m3
+        total unit weight in [kN/m3], cannot be lower than 10.
     lateral_model : ConstitutiveModel
-        Lateral soil model of the layer, by default None
+        Lateral soil model of the layer, by default None.
     axial_model : ConstitutiveModel
-        Axial soil model of the layer, by default None
+        Axial soil model of the layer, by default None.
     color : str
-        soil layer color in HEX format (e.g. '#000000'), by default None
+        soil layer color in HEX format (e.g. '#000000'), by default None.
+        If None, the color is generated randomly.
 
 
     Example
     -------
 
     >>> from openpile.construct import Layer
     >>> from openpile.core.soilmodels import API_clay
@@ -521,27 +541,27 @@
 
     Additionally, a soil profile can include discrete information at given elevation such as CPT
     (Cone Penetration Test) data. Not Implemented yet!
 
     Parameters
     ----------
     name : str
-        Name of the soil profile, used for printout and plots
+        Name of the soil profile, used for printout and plots.
     top_elevation : float
-        top elevation of the soil profile in [m VREF]
+        top elevation of the soil profile in [m VREF].
     water_line : float
-        elevation of the water table in [m VREF]
+        elevation of the water table in [m VREF].
     layers : list[Layer]
-        list of layers for the soil profile
+        list of layers for the soil profile.
     cpt_data : np.ndarray
-        cpt data table
+        cpt data table with
         1st col: elevation [m],
         2nd col: cone resistance [kPa],
-        3rd col: sleeve friction [kPa]
-        4th col: pore pressure u2 [kPa]
+        3rd col: sleeve friction [kPa],
+        4th col: pore pressure u2 [kPa].
 
     Example
     -------
 
     >>> from openpile.construct import SoilProfile, Layer
     >>> from openpile.core.soilmodels import API_sand, API_clay
 
@@ -641,19 +661,37 @@
             out += f"Layer {i}\n" + "-" * 30 + "\n"
             out += f"{layer}\n" + "~" * 30 + "\n"
         return out
 
     @property
     def bottom_elevation(self) -> float:
         """
-        Bottom elevation of the soil profile.
+        Bottom elevation of the soil profile [m VREF].
         """
         return self.top_elevation - sum([abs(x.top - x.bottom) for x in self.layers])
 
     def plot(self, assign=False):
+        """Creates a plot illustrating the stratigraphy.
+
+        Parameters
+        ----------
+        assign : bool, optional
+            this parameter can be set to True to return the figure, by default False
+
+        Returns
+        -------
+        matplotlib.pyplot.figure
+            only return the object if assign=True
+
+        Example
+        -------
+
+        .. image:: _static/plots/SoilProfile_plot.png
+           :scale: 70%
+        """
         fig = graphics.soil_plot(self)
         return fig if assign is True else None
 
 
 @dataclass(config=PydanticConfig)
 class Model:
     """
@@ -663,31 +701,31 @@
     Additionally, a soil profile can be fed to the Model, and soil springs can be created.
 
     Parameters
     ----------
     name : str
         Name of the model
     pile : Pile
-        Pile instance to be included in the model
+        Pile instance to be included in the model.
     soil : Optional[SoilProfile], optional
-        SoilProfile instance, by default None
+        SoilProfile instance, by default None.
     element_type : str, optional
-        can be of ['EulerBernoulli','Timoshenko'], by default 'Timoshenko'
+        can be of ['EulerBernoulli','Timoshenko'], by default 'Timoshenko'.
     x2mesh : List[float], optional
-        additional elevations to be included in the mesh, by default none
+        additional elevations to be included in the mesh, by default none.
     coarseness : float, optional
-        maximum distance in meters between two nodes of the mesh, by default 0.5
+        maximum distance in meters between two nodes of the mesh, by default 0.5.
     distributed_lateral : bool, optional
-        include distributed lateral springs, by default True
+        include distributed lateral springs, by default True.
     distributed_moment : bool, optional
-        include distributed moment springs, by default False
+        include distributed moment springs, by default False.
     base_shear : bool, optional
-        include lateral spring at pile toe, by default False
+        include lateral spring at pile toe, by default False.
     base_moment : bool, optional
-        include moment spring at pile toe, by default False
+        include moment spring at pile toe, by default False.
 
 
     Example
     -------
 
     >>> from openpile.construct import Pile, Model, Layer
     >>> from openpile.core.soilmodels import API_sand
@@ -753,40 +791,21 @@
     #: whether to include t-z springs in the calculations
     distributed_axial: bool = False
     #: whether to include Q-z spring in the calculations
     base_axial: bool = False
 
     @root_validator(skip_on_failure=True)
     def soil_and_pile_bottom_elevation_match(cls, values):  # pylint: disable=no-self-argument
-        if values["pile"].bottom_elevation < values["soil"].bottom_elevation:
-            raise UserWarning("The pile ends deeper than the soil profile.")
+        if values["soil"] is None:
+            pass
+        else:
+            if values["pile"].bottom_elevation < values["soil"].bottom_elevation:
+                raise UserWarning("The pile ends deeper than the soil profile.")
         return values
 
-    def get_structural_properties(self) -> pd.DataFrame:
-        """
-        Returns a table with the structural properties of the pile sections.
-        """
-        try:
-            return self.element_properties
-        except AttributeError:
-            print("Data not found. Please create Model with the Model.create() method.")
-        except Exception as e:
-            print(e)
-
-    def get_soil_properties(self) -> pd.DataFrame:
-        """
-        Returns a table with the soil main properties and soil models of each element.
-        """
-        try:
-            return self.soil_properties
-        except AttributeError:
-            print("Data not found. Please create Model with the Model.create() method.")
-        except Exception as e:
-            print(e)
-
     def __post_init__(self):
         def check_springs(arr):
             check_nan = np.isnan(arr).any()
             check_negative = (arr < 0).any()
 
             return check_nan or check_negative
 
@@ -1046,46 +1065,56 @@
         self.element_properties["E [kPa]"] = self.pile.E
         # delete Elevation [m] column
         self.element_properties.drop("Elevation [m]", inplace=True, axis=1)
         # reset index
         self.element_properties.reset_index(inplace=True, drop=True)
 
         # create soil properties
-        self.soil_properties = pd.merge_asof(
-            left=self.element_coordinates[["x_top [m]", "x_bottom [m]"]].sort_values(
-                by=["x_top [m]"]
-            ),
-            right=get_soil_profile().sort_values(by=["Top soil layer [m]"]),
-            left_on="x_top [m]",
-            right_on="Top soil layer [m]",
-            direction="forward",
-        ).sort_values(by=["x_top [m]"], ascending=False)
-        # add elevation of element w.r.t. ground level
-        self.soil_properties["xg_top [m]"] = (
-            self.soil_properties["x_top [m]"] - self.soil.top_elevation
-        )
-        self.soil_properties["xg_bottom [m]"] = (
-            self.soil_properties["x_bottom [m]"] - self.soil.top_elevation
-        )
-        # add vertical stress at top and bottom of each element
-        condition_below_water_table = self.soil_properties["x_top [m]"] <= self.soil.water_line
-        self.soil_properties["Unit Weight [kN/m3]"][condition_below_water_table] = (
-            self.soil_properties["Unit Weight [kN/m3]"][condition_below_water_table] - 10.0
-        )
-        s = (
-            self.soil_properties["x_top [m]"] - self.soil_properties["x_bottom [m]"]
-        ) * self.soil_properties["Unit Weight [kN/m3]"]
-        self.soil_properties["sigma_v top [kPa]"] = np.insert(
-            s.cumsum().values[:-1],
-            np.where(self.soil_properties["x_top [m]"].values == self.soil.top_elevation)[0],
-            0.0,
-        )
-        self.soil_properties["sigma_v bottom [kPa]"] = s.cumsum()
-        # reset index
-        self.soil_properties.reset_index(inplace=True, drop=True)
+        if self.soil is not None:
+            self.soil_properties = pd.merge_asof(
+                left=self.element_coordinates[["x_top [m]", "x_bottom [m]"]].sort_values(
+                    by=["x_top [m]"]
+                ),
+                right=get_soil_profile().sort_values(by=["Top soil layer [m]"]),
+                left_on="x_top [m]",
+                right_on="Top soil layer [m]",
+                direction="forward",
+            ).sort_values(by=["x_top [m]"], ascending=False)
+            # add elevation of element w.r.t. ground level
+            self.soil_properties["xg_top [m]"] = (
+                self.soil_properties["x_top [m]"] - self.soil.top_elevation
+            )
+            self.soil_properties["xg_bottom [m]"] = (
+                self.soil_properties["x_bottom [m]"] - self.soil.top_elevation
+            )
+            # add vertical stress at top and bottom of each element
+            condition_below_water_table = self.soil_properties["x_top [m]"] <= self.soil.water_line
+            self.soil_properties["Unit Weight [kN/m3]"][condition_below_water_table] = (
+                self.soil_properties["Unit Weight [kN/m3]"][condition_below_water_table] - 10.0
+            )
+            s = (
+                self.soil_properties["x_top [m]"] - self.soil_properties["x_bottom [m]"]
+            ) * self.soil_properties["Unit Weight [kN/m3]"]
+            self.soil_properties["sigma_v top [kPa]"] = np.insert(
+                s.cumsum().values[:-1],
+                np.where(self.soil_properties["x_top [m]"].values == self.soil.top_elevation)[0],
+                0.0,
+            )
+            self.soil_properties["sigma_v bottom [kPa]"] = s.cumsum()
+            # reset index
+            self.soil_properties.reset_index(inplace=True, drop=True)
+
+            # Create arrays of springs
+            (
+                self._py_springs,
+                self._mt_springs,
+                self._Hb_spring,
+                self._Mb_spring,
+                self._tz_springs,
+            ) = create_springs()
 
         # Initialise nodal global forces with link to nodes_coordinates (used for force-driven calcs)
         self.global_forces = self.nodes_coordinates.copy()
         self.global_forces["Px [kN]"] = 0
         self.global_forces["Py [kN]"] = 0
         self.global_forces["Mz [kNm]"] = 0
 
@@ -1097,33 +1126,105 @@
 
         # Initialise nodal global support with link to nodes_coordinates (used for defining boundary conditions)
         self.global_restrained = self.nodes_coordinates.copy()
         self.global_restrained["Tx"] = False
         self.global_restrained["Ty"] = False
         self.global_restrained["Rz"] = False
 
-        # Create arrays of springs
-        (
-            self._py_springs,
-            self._mt_springs,
-            self._Hb_spring,
-            self._Mb_spring,
-            self._tz_springs,
-        ) = create_springs()
+    @property
+    def py_springs(self) -> pd.DataFrame:
+        """Table with p-y springs computed for the given Model.
+
+        Returns
+        -------
+        pd.DataFrame (or None if no SoilProfile is present)
+            Table with p-y springs, i.e. p-value [kN/m] and y-value [m].
+        """
+        if self.soil is None:
+            return None
+        else:
+            return misc.get_springs(
+                springs=self._py_springs,
+                elevations=self.nodes_coordinates["x [m]"].values,
+                kind="p-y",
+            )
+
+    @property
+    def embedment(self) -> float:
+        """Pile embedment length [m].
+
+        Returns
+        -------
+        float (or None if no SoilProfile is present)
+            Pile embedment
+        """
+        if self.soil is None:
+            return None
+        else:
+            return self.soil.top_elevation - self.pile.bottom_elevation
+
+    @property
+    def top(self) -> float:
+        """top elevation of the model [m].
+
+        Returns
+        -------
+        float
+        """
+        if self.soil is None:
+            return self.pile.top_elevation
+        else:
+            return max(self.pile.top_elevation, self.soil.top_elevation, self.soil.water_line)
+
+    @property
+    def bottom(self) -> float:
+        """bottom elevation of the model [m].
+
+        Returns
+        -------
+        float
+        """
+
+        if self.soil is None:
+            return self.pile.bottom_elevation
+        else:
+            return min(self.pile.bottom_elevation, self.soil.bottom_elevation)
+
+    def get_structural_properties(self) -> pd.DataFrame:
+        """
+        Returns a table with the structural properties of the pile sections.
+        """
+        try:
+            return self.element_properties
+        except AttributeError:
+            print("Data not found. Please create Model with the Model.create() method.")
+        except Exception as e:
+            print(e)
+
+    def get_soil_properties(self) -> pd.DataFrame:
+        """
+        Returns a table with the soil main properties and soil models of each element.
+        """
+        try:
+            return self.soil_properties
+        except AttributeError:
+            print("Data not found. Please create Model with the Model.create() method.")
+        except Exception as e:
+            print(e)
 
     def get_pointload(self, output=False, verbose=True):
         """
         Returns the point loads currently defined in the mesh via printout statements.
 
         Parameters
         ----------
         output : bool, optional
-            If true, it returns the printout statements as a variable, by default False
+            If true, it returns the printout statements as a variable, by default False.
         verbose : float, optional
-            if True, printout statements printed automaically (ideal for use with iPython), by default True
+            if True, printout statements printed automaically (ideal for use with iPython), by default True.
         """
         out = ""
         try:
             for idx, elevation, _, Px, Py, Mz in self.global_forces.itertuples(name=None):
                 if any([Px, Py, Mz]):
                     string = f"\nLoad applied at elevation {elevation} m (node no. {idx}): Px = {Px} kN, Py = {Py} kN, Mx = {Mz} kNm."
                     if verbose is True:
@@ -1148,21 +1249,21 @@
         .. note:
             If run several times at the same elevation, the loads are overwritten by the last command.
 
 
         Parameters
         ----------
         elevation : float, optional
-            the elevation must match the elevation of a node, by default 0.0
+            the elevation must match the elevation of a node, by default 0.0.
         Py : float, optional
-            Shear force in kN, by default None
+            Shear force in kN, by default None.
         Px : float, optional
-            Normal force in kN, by default None
+            Normal force in kN, by default None.
         Mz : float, optional
-            Bending moment in kNm, by default None
+            Bending moment in kNm, by default None.
         """
 
         # identify if one node is at given elevation or if load needs to be split
         nodes_elevations = self.nodes_coordinates["x [m]"].values
         # check if corresponding node exist
         check = np.isclose(nodes_elevations, np.tile(elevation, nodes_elevations.shape), atol=0.001)
 
@@ -1205,21 +1306,21 @@
 
         .. note::
             for defining supports, this function should not be used, rather use `.set_support()`.
 
         Parameters
         ----------
         elevation : float, optional
-            the elevation must match the elevation of a node, by default 0.0
+            the elevation must match the elevation of a node, by default 0.0.
         Ty : float, optional
-            Translation along y-axis, by default None
+            Translation along y-axis, by default None.
         Tx : float, optional
-            Translation along x-axis, by default None
+            Translation along x-axis, by default None.
         Rz : float, optional
-            Rotation around z-axis, by default None
+            Rotation around z-axis, by default None.
         """
 
         try:
             # identify if one node is at given elevation or if load needs to be split
             nodes_elevations = self.nodes_coordinates["x [m]"].values
             # check if corresponding node exist
             check = np.isclose(
@@ -1270,21 +1371,21 @@
         .. note:
             If run several times at the same elevation, the support are overwritten by the last command.
 
 
         Parameters
         ----------
         elevation : float, optional
-            the elevation must match the elevation of a node, by default 0.0
+            the elevation must match the elevation of a node, by default 0.0.
         Ty : bool, optional
-            Translation along y-axis, by default False
+            Translation along y-axis, by default False.
         Tx : bool, optional
-            Translation along x-axis, by default False
+            Translation along x-axis, by default False.
         Rz : bool, optional
-            Rotation around z-axis, by default False
+            Rotation around z-axis, by default False.
         """
 
         try:
             # identify if one node is at given elevation or if load needs to be split
             nodes_elevations = self.nodes_coordinates["x [m]"].values
             # check if corresponding node exist
             check = np.isclose(
@@ -1311,14 +1412,39 @@
                         "Support not applied! The chosen elevation is not meshed as a node. Please include elevation in `x2mesh` variable when creating the Model."
                     )
         except Exception:
             print("\n!User Input Error! Please create Model first with the Model.create().\n")
             raise
 
     def plot(self, assign=False):
+        """Create a plot of the model with the mesh and boundary conditions.
+
+        Parameters
+        ----------
+        assign : bool, optional
+            this parameter can be set to True to return the figure, by default False.
+
+        Returns
+        -------
+        matplotlib.pyplot.figure
+            only return the object if assign=True.
+
+        Examples
+        --------
+
+        *Plot without SoilProfile fed to the model:*
+
+        .. image:: _static/plots/Model_no_soil_plot.png
+           :scale: 70%
+
+        *Plot with SoilProfile fed to the model:*
+
+        .. image:: _static/plots/Model_with_soil_plot.png
+           :scale: 70%
+        """
         fig = graphics.connectivity_plot(self)
         return fig if assign else None
 
     @classmethod
     def create(
         cls,
         name: str,
@@ -1387,39 +1513,7 @@
             stacklevel=2,
         )
 
         return obj
 
     def __str__(self):
         return self.element_properties.to_string()
-
-    @property
-    def py_springs(self) -> pd.DataFrame:
-        """Table with p-y springs computed for the given Model.
-
-        Returns
-        -------
-        pd.DataFrame (or None if no SoilProfile is present)
-            Table with p-y springs.
-        """
-        if self.soil is None:
-            return None
-        else:
-            return misc.get_springs(
-                springs=self._py_springs,
-                elevations=self.nodes_coordinates["x [m]"].values,
-                kind="p-y",
-            )
-
-    @property
-    def embedment(self) -> float:
-        """Pile embedment length [m].
-
-        Returns
-        -------
-        float (or None if no SoilProfile is present)
-            Pile embedment
-        """
-        if self.soil is None:
-            return None
-        else:
-            return self.soil.top_elevation - self.pile.bottom_elevation
```

### Comparing `openpile-0.2.0/src/openpile/core/kernel.py` & `openpile-0.3.0/src/openpile/core/kernel.py`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/src/openpile/core/misc.py` & `openpile-0.3.0/src/openpile/core/misc.py`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/src/openpile/core/txt.py` & `openpile-0.3.0/src/openpile/core/txt.py`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/src/openpile/core/validation.py` & `openpile-0.3.0/src/openpile/core/validation.py`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/src/openpile/soilmodels.py` & `openpile-0.3.0/src/openpile/soilmodels.py`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/src/openpile/utils/Hb_curves.py` & `openpile-0.3.0/src/openpile/utils/Hb_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/src/openpile/utils/Mb_curves.py` & `openpile-0.3.0/src/openpile/utils/Mb_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/src/openpile/utils/graphics.py` & `openpile-0.3.0/src/openpile/utils/graphics.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,18 +59,19 @@
         axis.set_ylabel("")
 
     return fig
 
 
 def soil_plot(SoilProfile):
     def add_soil_profile(SoilProfile, ax, pile=None):
+
         ax.set_title(label=f"Soil Profile overview - {SoilProfile.name}")
+        ax.set_xlim(left=0, right=1)
 
         # make data
-        ax.set_xlim(left=0, right=1)
         offset = 5
         yBot = SoilProfile.bottom_elevation
         if pile is None:
             yTop = max(SoilProfile.top_elevation + offset, SoilProfile.water_line + offset)
         else:
             yTop = max(
                 SoilProfile.top_elevation + offset,
@@ -82,34 +83,44 @@
         ax.set_ylim(bottom=yBot, top=yTop)
         ax.set_ylabel("Elevation [m VREF]")
         ax.set_xticks([])
 
         for layer in SoilProfile.layers:
             ax.add_patch(
                 Rectangle(
-                    xy=(0, layer.bottom),
-                    width=1,
+                    xy=(-100, layer.bottom),
+                    width=200,
                     height=layer.top - layer.bottom,
                     facecolor=layer.color,
                 )
             )
+
             ax.text(
                 0.02,
                 0.5 * (layer.top + layer.bottom),
                 layer.name,
                 bbox={"facecolor": [0.98, 0.96, 0.85], "alpha": 1, "edgecolor": "none", "pad": 1},
             )
 
+        ax.plot(
+            np.array([-100, 0.1, 100]),
+            SoilProfile.water_line + np.zeros((3)),
+            mfc="dodgerblue",
+            marker=7,
+            linewidth=1,
+            color="dodgerblue",
+        )
+
         # grid
         ax.minorticks_on()
         ax.grid()
         ax.grid(axis="y", which="minor", color=[0.75, 0.75, 0.75], linestyle="-", linewidth=0.5)
 
         ax.plot(
-            np.array([-1, 0.1, 2]),
+            np.array([-100, 0.1, 100]),
             SoilProfile.water_line + np.zeros((3)),
             mfc="dodgerblue",
             marker=7,
             linewidth=1,
             color="dodgerblue",
         )
 
@@ -173,18 +184,18 @@
     ax.grid(which="both")
 
     # plot mesh with + scatter points to see nodes.
     x = model.nodes_coordinates["x [m]"]
     y = model.nodes_coordinates["y [m]"]
     ax.plot(y, x, "-k", marker="+")
 
-    total_length = max(
-        (model.nodes_coordinates["x [m]"].max() - model.nodes_coordinates["x [m]"].min()),
-        (model.nodes_coordinates["y [m]"].max() - model.nodes_coordinates["y [m]"].min()),
-    )
+    total_length = (
+        (model.nodes_coordinates["x [m]"].max() - model.nodes_coordinates["x [m]"].min()) ** 2
+        + (model.nodes_coordinates["y [m]"].max() - model.nodes_coordinates["y [m]"].min()) ** 2
+    ) ** (0.5)
 
     ylim = ax.get_ylim()
 
     # plots SUPPORTS
     # Plot supports along x
     support_along_x = model.global_restrained["Tx"].values
     support_along_x_down = np.copy(support_along_x)
@@ -296,19 +307,57 @@
                             (-arrow_length / 1.5, yval),
                             (arrow_length / 1.5, yval),
                             connectionstyle="arc3,rad=-0.5",
                             **kw,
                         )
                     )
 
+    ax.set_ylim(ylim[0] - 0.11 * total_length, ylim[1] + 0.11 * total_length)
+
+    if model.soil is not None:
+
+        ax.set_ylim(
+            min(model.bottom, ylim[0]) - 0.11 * total_length,
+            max(model.top, ylim[1]) + 0.11 * total_length,
+        )
+
+        for layer in model.soil.layers:
+            ax.add_patch(
+                Rectangle(
+                    xy=(-2 * total_length, layer.bottom),
+                    width=4 * total_length,
+                    height=layer.top - layer.bottom,
+                    facecolor=layer.color,
+                    alpha=0.4,
+                )
+            )
+
+            ax.text(
+                -1 * total_length,
+                0.5 * (layer.top + layer.bottom) + 0.1 * (layer.top - layer.bottom),
+                layer.name,
+                bbox={"facecolor": [0.98, 0.96, 0.85], "alpha": 1, "edgecolor": "none", "pad": 1},
+            )
+
+            ax.plot(
+                np.array([-2 * total_length, -0.6 * total_length, 2 * total_length]),
+                model.soil.water_line + np.zeros((3)),
+                mfc="dodgerblue",
+                marker=7,
+                linewidth=1,
+                color="dodgerblue",
+            )
+        ax.set_xlim((-0.7 * total_length, 0.3 * total_length))
+
+    else:
+        ax.set_xlim((-0.5 * total_length, 0.5 * total_length))
+
     for arrow in arrows:
         ax.add_patch(arrow)
 
-    ax.set_ylim(ylim[0] - 0.11 * total_length, ylim[1] + 0.11 * total_length)
-
     return fig
 
 
 def U_plot(axis: plt.axis, result):
     # TODO docstring
 
     axis.set_ylabel("Elevation [m VREF]", fontsize=8)
```

### Comparing `openpile-0.2.0/src/openpile/utils/mt_curves.py` & `openpile-0.3.0/src/openpile/utils/mt_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/src/openpile/utils/py_curves.py` & `openpile-0.3.0/src/openpile/utils/py_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/src/openpile/utils/qz_curves.py` & `openpile-0.3.0/src/openpile/utils/qz_curves.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,41 +28,41 @@
     sig : float
         Vertical effective stress [unit: kPa]
     delta : float
         interface friction angle [unit: degrees]
     D : float
         Pile diameter [unit: m]
     output_length : int, optional
-        Number of discrete point along the springs, cannot be lower than 7, by default 7
+        Number of discrete point along the springs, cannot be lower than 8, by default 8
 
     Returns
     -------
     numpy 1darray
         Q vector [unit: kPa]
     numpy 1darray
         z vector [unit: m]
     """
-    # cannot have less than 7
-    if output_length < 7:
-        output_length = 7
+    # cannot have less than 8
+    if output_length < 8:
+        output_length = 8
 
     # important variables
     delta_table = np.array([0, 15, 20, 25, 30, 35, 100], dtype=np.float32)
     Nq_table = np.array([8, 8, 12, 20, 40, 50, 50], dtype=np.float32)
     Qmax_table = np.array([1900, 1900, 2900, 4800, 9600, 12000, 12000], dtype=np.float32)
 
     Nq = np.interp(delta, delta_table, Nq_table)
     Qmax = np.interp(delta, delta_table, Qmax_table)
 
     # Unit end-bearing [kPa]
     f = min(Qmax, sig * Nq)
 
     # piecewise function
-    zlist = [0.0, 0.002, 0.013, 0.042, 0.073, 0.100, 0.200]
-    Qlist = [0.0, 0.25, 0.50, 0.75, 0.90, 1.00, 1.00]
+    zlist = [-0.002, 0.0, 0.002, 0.013, 0.042, 0.073, 0.100, 0.200]
+    Qlist = [0.0, 0.0, 0.25, 0.50, 0.75, 0.90, 1.00, 1.00]
 
     # determine z vector
     z = np.array(zlist, dtype=np.float32) * D
 
     # define t vector
     Q = np.array(Qlist, dtype=np.float32) * f
 
@@ -98,33 +98,33 @@
     Parameters
     ----------
     Su : float
         Undrained shear strength [unit: kPa]
     D: float
         Pile diameter [unit: m]
     output_length : int, optional
-        Number of discrete point along the springs, cannot be lower than 7, by default 7
+        Number of discrete point along the springs, cannot be lower than 8, by default 8
 
     Returns
     -------
     numpy 1darray
         Q vector [unit: kPa]
     numpy 1darray
         z vector [unit: m]
     """
-    # cannot have less than 7
-    if output_length < 7:
-        output_length = 7
+    # cannot have less than 8
+    if output_length < 8:
+        output_length = 8
 
     # Unit end-bearing [kPa]
     f = 9 * Su
 
     # piecewise function
-    zlist = [0.0, 0.002, 0.013, 0.042, 0.073, 0.100, 0.200]
-    Qlist = [0.0, 0.25, 0.50, 0.75, 0.90, 1.00, 1.00]
+    zlist = [-0.002, 0.0, 0.002, 0.013, 0.042, 0.073, 0.100, 0.200]
+    Qlist = [0.0, 0.0, 0.25, 0.50, 0.75, 0.90, 1.00, 1.00]
 
     # determine z vector
     z = np.array(zlist, dtype=np.float32) * D
 
     # define t vector
     Q = np.array(Qlist, dtype=np.float32) * f
```

### Comparing `openpile-0.2.0/src/openpile/utils/tz_curves.py` & `openpile-0.3.0/src/openpile/utils/tz_curves.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 # API clay function
 @njit(cache=True)
 def api_clay(
     sig: float,
     Su: float,
     D: float,
     residual: float = 0.9,
-    output_length: int = 8,
+    tensile_factor: float = 1.0,
+    output_length: int = 15,
 ):
     """
     Creates the API clay t-z curve from relevant input.
 
     Parameters
     ----------
     sig: float
@@ -31,27 +32,29 @@
     Su : float
         Undrained shear strength [unit: kPa]
     D: float
         Pile diameter [unit: m]
     residual: float
         residual strength after peak strength, according to API-RP-2A,
         this value is between 0.7 and 0.9, default to 0.9
+    tensile_factor: float
+        strength factor for negative values of the curve
     output_length : int, optional
-        Number of discrete point along the springs, cannot be lower than 7, by default 7
+        Number of discrete point along the springs, cannot be lower than 15, by default 15
 
     Returns
     -------
     numpy 1darray
         t vector [unit: kPa]
     numpy 1darray
         z vector [unit: m]
     """
-    # cannot have less than 8
-    if output_length < 8:
-        output_length = 8
+    # cannot have less than 15
+    if output_length < 15:
+        output_length = 15
 
     # important variables
     if sig == 0.0:
         psi = Su / 0.001
     else:
         psi = Su / sig
 
@@ -65,17 +68,18 @@
 
     # piecewise function
     zlist = [0.0, 0.0016, 0.0031, 0.0057, 0.0080, 0.0100, 0.0200, 0.0300]
     tlist = [0.0, 0.3, 0.5, 0.75, 0.90, 1.00, residual, residual]
 
     # determine z vector
     z = np.array(zlist, dtype=np.float32) * D
-
+    z = np.concatenate((-z[-1:0:-1], z))
     # define t vector
     t = np.array(tlist, dtype=np.float32) * f
+    t = np.concatenate((-tensile_factor * t[-1:0:-1], t))
 
     add_values = output_length - len(z)
     add_z_values = np.zeros((add_values), dtype=np.float32)
     add_t_values = np.zeros((add_values), dtype=np.float32)
 
     for i in range(add_values):
         add_z_values[i] = (0.02 + random() * 0.01) * D
@@ -94,40 +98,43 @@
 
 # API sand function
 @njit(cache=True)
 def api_sand(
     sig: float,
     delta: float,
     K: float = 0.8,
-    output_length: int = 4,
+    tensile_factor: float = 1.0,
+    output_length: int = 7,
 ):
     """
     Creates the API sand t-z curve from relevant input.
 
     Parameters
     ----------
     sig: float
         Vertical effective stress [unit: kPa]
     delta: float
         interface friction angle [unit: degrees]
     K: float
         coefficient of lateral pressure (0.8 for open-ended piles and 1.0 for cloased-ended)
+    tensile_factor: float
+        strength factor for negative values of the curve
     output_length : int, optional
-        Number of discrete point along the springs, cannot be lower than 4, by default 4
+        Number of discrete point along the springs, cannot be lower than 7, by default 7
 
     Returns
     -------
     numpy 1darray
         t vector [unit: kPa]
     numpy 1darray
         z vector [unit: m]
     """
-    # cannot have less than 4
-    if output_length < 4:
-        output_length = 4
+    # cannot have less than 7
+    if output_length < 7:
+        output_length = 7
 
     # important variables
     delta_table = np.array([0, 15, 20, 25, 30, 35, 100], dtype=np.float32)
     fs_max_table = np.array([47.8, 47.8, 67, 81.3, 95.7, 114.8, 114.8], dtype=np.float32)
 
     # limit unit skin friction according to API ref page 59
     fs_max = np.interp(delta, delta_table, fs_max_table)
@@ -137,17 +144,18 @@
 
     # piecewise function
     zlist = [0.0, 0.0254, 0.03, 0.04]
     tlist = [0.0, 1.0, 1.0, 1.0]
 
     # determine z vector
     z = np.array(zlist, dtype=np.float32)
-
+    z = np.concatenate((-z[-1:0:-1], z))
     # define t vector
     t = np.array(tlist, dtype=np.float32) * f
+    t = np.concatenate((-tensile_factor * t[-1:0:-1], t))
 
     add_values = output_length - len(z)
     add_z_values = np.zeros((add_values), dtype=np.float32)
     add_t_values = np.zeros((add_values), dtype=np.float32)
 
     for i in range(add_values):
         add_z_values[i] = 0.03 + random() * 0.01
```

### Comparing `openpile-0.2.0/src/openpile.egg-info/PKG-INFO` & `openpile-0.3.0/src/openpile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.2.0
+Version: 0.3.0
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
 Project-URL: Documentation, https://openpile.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/TchilDill/openpile
```

### Comparing `openpile-0.2.0/src/openpile.egg-info/SOURCES.txt` & `openpile-0.3.0/src/openpile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/test/test_construct.py` & `openpile-0.3.0/test/test_construct.py`

 * *Files identical despite different names*

### Comparing `openpile-0.2.0/test/test_utils_misc.py` & `openpile-0.3.0/test/test_utils_misc.py`

 * *Files identical despite different names*

