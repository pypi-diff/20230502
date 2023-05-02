# Comparing `tmp/pyometiff-0.0.8.tar.gz` & `tmp/pyometiff-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyometiff-0.0.8.tar", last modified: Fri Sep 24 14:46:59 2021, max compression
+gzip compressed data, was "pyometiff-0.0.9.tar", last modified: Tue Jan 11 11:02:27 2022, max compression
```

## Comparing `pyometiff-0.0.8.tar` & `pyometiff-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-24 14:46:59.661247 pyometiff-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    37486 2021-09-24 14:46:44.000000 pyometiff-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5124 2021-09-24 14:46:59.657247 pyometiff-0.0.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     3621 2021-09-24 14:46:44.000000 pyometiff-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-24 14:46:59.657247 pyometiff-0.0.8/pyometiff/
--rwxr-xr-x   0 runner    (1001) docker     (121)      150 2021-09-24 14:46:44.000000 pyometiff-0.0.8/pyometiff/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10289 2021-09-24 14:46:44.000000 pyometiff-0.0.8/pyometiff/omereader.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9884 2021-09-24 14:46:44.000000 pyometiff-0.0.8/pyometiff/omewriter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    69655 2021-09-24 14:46:44.000000 pyometiff-0.0.8/pyometiff/omexml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-24 14:46:59.657247 pyometiff-0.0.8/pyometiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5124 2021-09-24 14:46:59.000000 pyometiff-0.0.8/pyometiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-09-24 14:46:59.000000 pyometiff-0.0.8/pyometiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-24 14:46:59.000000 pyometiff-0.0.8/pyometiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-09-24 14:46:59.000000 pyometiff-0.0.8/pyometiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-09-24 14:46:59.000000 pyometiff-0.0.8/pyometiff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-24 14:46:59.661247 pyometiff-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1191 2021-09-24 14:46:44.000000 pyometiff-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 11:02:27.695344 pyometiff-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    37486 2022-01-11 11:02:11.000000 pyometiff-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     5124 2022-01-11 11:02:27.695344 pyometiff-0.0.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3621 2022-01-11 11:02:11.000000 pyometiff-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 11:02:27.691344 pyometiff-0.0.9/pyometiff/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      150 2022-01-11 11:02:11.000000 pyometiff-0.0.9/pyometiff/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10289 2022-01-11 11:02:11.000000 pyometiff-0.0.9/pyometiff/omereader.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11054 2022-01-11 11:02:11.000000 pyometiff-0.0.9/pyometiff/omewriter.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    69470 2022-01-11 11:02:11.000000 pyometiff-0.0.9/pyometiff/omexml.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 11:02:27.695344 pyometiff-0.0.9/pyometiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5124 2022-01-11 11:02:27.000000 pyometiff-0.0.9/pyometiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-01-11 11:02:27.000000 pyometiff-0.0.9/pyometiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-11 11:02:27.000000 pyometiff-0.0.9/pyometiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-01-11 11:02:27.000000 pyometiff-0.0.9/pyometiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-11 11:02:27.000000 pyometiff-0.0.9/pyometiff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-11 11:02:27.695344 pyometiff-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1068 2022-01-11 11:02:11.000000 pyometiff-0.0.9/setup.py
```

### Comparing `pyometiff-0.0.8/LICENSE` & `pyometiff-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyometiff-0.0.8/PKG-INFO` & `pyometiff-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyometiff
-Version: 0.0.8
+Version: 0.0.9
 Summary: Read and Write OME-TIFFs in Python
 Home-page: https://github.com/filippocastelli/pyometiff
 Author: Filippo Maria Castelli
 Author-email: castelli@lens.unifi.it
 License: UNKNOWN
 Description: ## About
```

### Comparing `pyometiff-0.0.8/README.md` & `pyometiff-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyometiff-0.0.8/pyometiff/omereader.py` & `pyometiff-0.0.9/pyometiff/omereader.py`

 * *Files identical despite different names*

### Comparing `pyometiff-0.0.8/pyometiff/omewriter.py` & `pyometiff-0.0.9/pyometiff/omewriter.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 # This software is distributed WITHOUT ANY WARRANTY.
 # See the GNU General Public License v3.0 for further details.
 
 # A copy of the GNU General Public License v3.0 should be included in pyometiff,
 # if you didn't receive a copy, visit <http://www.gnu.org/licenses/>.
 
 # Copyright (c) 2021, Filippo Maria Castelli
-
+import logging
 from pathlib import Path
 from typing import Union
 from lxml import etree as ET
 import numpy as np
 import tifffile
 from pyometiff.omexml import OMEXML, get_pixel_type, xsd_now
 
-BYTE_BOUNDARY = 2 ** 21
+BYTE_BOUNDARY = 2 ** 32
 
 
 class InvalidDimensionOrderingError(Exception):
     """exception for invalid dimensional ordering"""
 
     def __init__(self, message: str, **kwargs):
         super().__init__(**kwargs)
@@ -44,26 +44,41 @@
             metadata: dict,
             overwrite: bool = False,
             dimension_order: str = "STZCYX",
             photometric: str = "minisblack",
             explicit_tiffdata: bool = False,
             compression: str = None,
             arr_shape: Union[list, tuple] = None,
-
+            bigtiff: bool = False,
     ):
+        """
+        OMETIFFWriter class for writing OME-TIFF files.
+
+        :param fpath: path to the file to be written
+        :param array: array to be written
+        :param metadata: dictionary containing the metadata to be written
+        :param overwrite: if True, overwrite the file if it already exists
+        :param dimension_order: dimension ordering of the array
+        :param photometric: photometric interpretation of the array, "minisblack" or "miniswhite"
+        :param explicit_tiffdata: if True, explicitly write the tiffdata tag, otherwise it is written automatically [DEBUG ONLY]
+        :param compression: compression type, if None, no compression is used
+        :param arr_shape: shape of the array, if None, it is inferred from the array
+        :param bigtiff: if True, use bigtiff format. File sizes exceeding 4GB will automatically be written in bigtiff format
+        """
+
         self.fpath = Path(fpath)
         self.array = array
         self.metadata = metadata
         self.overwrite = overwrite
         self.dimension_order = dimension_order
         self.photometric = photometric
         self.explicit_tiffdata = explicit_tiffdata
         self.compression = compression
         self.arr_shape = arr_shape
-
+        self.use_bigtiff = bigtiff
         self.init_file()
 
     def init_file(self):
         self._array, self._dimension_order = self._adjust_dims(
             array=self.array,
             dimension_order=self.dimension_order,
             shape=self.arr_shape
@@ -81,25 +96,30 @@
         tree.write(str(xml_fpath),
                    encoding="utf-8",
                    method="xml",
                    pretty_print=True,
                    xml_declaration=True)
 
     @staticmethod
-    def _use_bigtiff(array):
+    def _should_use_bigtiff(array):
         if array is None:
             return False
         else:
             file_size = array.size * array.itemsize
             return file_size > BYTE_BOUNDARY
 
     def write_stack(self, array, xml_meta):
-        self.use_bigtiff = self._use_bigtiff(array)
-        self.use_bigtiff = True
-        with tifffile.TiffWriter(str(self.fpath), bigtiff=self.use_bigtiff) as tif:
+        should_use_bigtiff = self._should_use_bigtiff(array)
+
+        use_bigtiff = self.use_bigtiff or should_use_bigtiff
+
+        if should_use_bigtiff and (self.use_bigtiff is False):
+            logging.warning("array size is larger than 4GB, using BigTIFF")
+
+        with tifffile.TiffWriter(str(self.fpath), bigtiff=use_bigtiff) as tif:
             tif.save(
                 array, description=xml_meta, photometric=self.photometric, metadata=None, compression=self.compression
             )
 
     def gen_meta(self):
         ox = OMEXML()
         ox.image().set_ID("Image:0")
```

### Comparing `pyometiff-0.0.8/pyometiff/omexml.py` & `pyometiff-0.0.9/pyometiff/omexml.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 # Copyright (c) 2009-2014 Broad Institute
 # All rights reserved.
 
 
 """omexml.py read and write OME xml
 """
 
-from __future__ import absolute_import, unicode_literals
 import datetime
 import logging
 from functools import reduce
 import re
 import uuid
 from xml.etree import cElementTree as ElementTree
 
@@ -39,34 +38,33 @@
 
 
 def xsd_now():
     """Return the current time in xsd:dateTime format"""
     return datetime.datetime.now().isoformat()
 
 
-DEFAULT_NOW = xsd_now()
 #
 # The namespaces
 #
 NS_BINARY_FILE = "http://www.openmicroscopy.org/Schemas/BinaryFile/2013-06"
 NS_ORIGINAL_METADATA = "openmicroscopy.org/OriginalMetadata"
 NS_DEFAULT = "http://www.openmicroscopy.org/Schemas/{ns_key}/2013-06"
 NS_RE = r"http://www.openmicroscopy.org/Schemas/(?P<ns_key>.*)/[0-9/-]"
 
-default_xml = """<?xml version="1.0" encoding="UTF-8"?>
+default_xml = f"""<?xml version="1.0" encoding="UTF-8"?>
 <!-- Warning: this comment is an OME-XML metadata block, which contains
 crucial dimensional parameters and other important metadata. Please edit
 cautiously (if at all), and back up the original data before doing so.
 For more information, see the OME-TIFF documentation:
 https://docs.openmicroscopy.org/latest/ome-model/ome-tiff/ -->
 <OME xmlns="http://www.openmicroscopy.org/Schemas/OME/2016-06"
      xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xsi:schemaLocation="http://www.openmicroscopy.org/Schemas/OME/2016-06 http://www.openmicroscopy.org/Schemas/OME/2016-06/ome.xsd">
     <Image ID="Image:0" Name="default.png">
-        <AcquisitionDate>%(DEFAULT_NOW)s</AcquisitionDate>
+        <AcquisitionDate>{xsd_now()}</AcquisitionDate>
         <Pixels BigEndian="false"
                 DimensionOrder="XYCZT"
                 ID="Pixels:0"
                 Interleaved="false"
                 SizeC="1"
                 SizeT="1"
                 SizeX="512"
@@ -74,15 +72,15 @@
                 SizeZ="1"
                 Type="uint8">
             <Channel ID="Channel:0:0" SamplesPerPixel="1">
                 <LightPath/>
             </Channel>
         </Pixels>
     </Image>
-</OME>""".format(ns_ome_default=NS_DEFAULT.format(ns_key='ome'), ns_sa_default=NS_DEFAULT.format(ns_key='sa'))
+</OME>"""
 
 #
 # These are the OME-XML pixel types - not all supported by subimager
 #
 PT_INT8 = "int8"
 PT_INT16 = "int16"
 PT_INT32 = "int32"
```

### Comparing `pyometiff-0.0.8/pyometiff.egg-info/PKG-INFO` & `pyometiff-0.0.9/pyometiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyometiff
-Version: 0.0.8
+Version: 0.0.9
 Summary: Read and Write OME-TIFFs in Python
 Home-page: https://github.com/filippocastelli/pyometiff
 Author: Filippo Maria Castelli
 Author-email: castelli@lens.unifi.it
 License: UNKNOWN
 Description: ## About
```

### Comparing `pyometiff-0.0.8/setup.py` & `pyometiff-0.0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from setuptools import setup, find_packages
 from pyometiff import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+with open("requirements", "r") as fh:
+    requirements = fh.read().splitlines()
+
 setup(
     name="pyometiff",
     version=__version__,
     description="Read and Write OME-TIFFs in Python",
     packages=find_packages(exclude=("tests",)),
-    # py_modules = ["omereader", "omewriter", "omexml"],
-    # package_dir = {"": "pyometiff"},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
         # "Operating System :: Os Independent",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["numpy",
-                      "tifffile>2020.10.1",
-                      "imagecodecs",
-                      "lxml"],
+    install_requires=requirements,
     extras_require={
         "dev": ["pytest>3.7", "mock"],
     },
     url="https://github.com/filippocastelli/pyometiff",
     author="Filippo Maria Castelli",
     author_email="castelli@lens.unifi.it",
 )
```

