# Comparing `tmp/pyCOREPOS-0.1.8.tar.gz` & `tmp/pyCOREPOS-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyCOREPOS-0.1.8.tar", last modified: Mon Jan  2 22:56:42 2023, max compression
+gzip compressed data, was "dist/pyCOREPOS-0.1.9.tar", last modified: Tue May  2 03:17:50 2023, max compression
```

## Comparing `pyCOREPOS-0.1.8.tar` & `pyCOREPOS-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2014-01-28 16:56:01.000000 pyCOREPOS-0.1.8/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       28 2014-10-17 02:31:47.000000 pyCOREPOS-0.1.8/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)      930 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      112 2018-05-31 03:33:51.000000 pyCOREPOS-0.1.8/README.rst
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/corepos/
--rw-r--r--   0 lance     (1000) lance     (1000)     1010 2020-07-16 02:42:12.000000 pyCOREPOS-0.1.8/corepos/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-01-02 22:56:22.000000 pyCOREPOS-0.1.8/corepos/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)    16348 2021-02-09 22:11:35.000000 pyCOREPOS-0.1.8/corepos/api.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/corepos/db/
--rw-r--r--   0 lance     (1000) lance     (1000)      975 2021-12-31 03:47:38.000000 pyCOREPOS-0.1.8/corepos/db/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/corepos/db/lane_op/
--rw-r--r--   0 lance     (1000) lance     (1000)     1053 2021-07-09 01:32:22.000000 pyCOREPOS-0.1.8/corepos/db/lane_op/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9851 2021-11-04 22:27:21.000000 pyCOREPOS-0.1.8/corepos/db/lane_op/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1256 2020-02-28 03:41:42.000000 pyCOREPOS-0.1.8/corepos/db/model.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/corepos/db/office_op/
--rw-r--r--   0 lance     (1000) lance     (1000)     1092 2020-02-28 03:35:39.000000 pyCOREPOS-0.1.8/corepos/db/office_op/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    56954 2022-12-02 16:03:43.000000 pyCOREPOS-0.1.8/corepos/db/office_op/model.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/corepos/db/office_trans/
--rw-r--r--   0 lance     (1000) lance     (1000)     1104 2020-02-28 03:43:38.000000 pyCOREPOS-0.1.8/corepos/db/office_trans/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4516 2022-03-27 04:03:38.000000 pyCOREPOS-0.1.8/corepos/db/office_trans/model.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/corepos/db/office_trans_archive/
--rw-r--r--   0 lance     (1000) lance     (1000)     1056 2022-03-26 19:40:33.000000 pyCOREPOS-0.1.8/corepos/db/office_trans_archive/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1291 2022-03-27 04:03:51.000000 pyCOREPOS-0.1.8/corepos/db/office_trans_archive/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1913 2020-03-30 19:26:08.000000 pyCOREPOS-0.1.8/corepos/db/util.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4913 2020-08-16 21:08:07.000000 pyCOREPOS-0.1.8/corepos/enum.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/corepos/trans/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2020-02-28 03:45:53.000000 pyCOREPOS-0.1.8/corepos/trans/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/corepos/trans/db/
--rw-r--r--   0 lance     (1000) lance     (1000)     1261 2020-02-28 03:44:35.000000 pyCOREPOS-0.1.8/corepos/trans/db/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1280 2020-02-28 03:45:20.000000 pyCOREPOS-0.1.8/corepos/trans/db/model.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/pyCOREPOS.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)      930 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/pyCOREPOS.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      697 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/pyCOREPOS.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/pyCOREPOS.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       47 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/pyCOREPOS.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        8 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/pyCOREPOS.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2023-01-02 22:56:42.000000 pyCOREPOS-0.1.8/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     3721 2020-03-13 22:01:03.000000 pyCOREPOS-0.1.8/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2014-01-28 16:56:01.000000 pyCOREPOS-0.1.9/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       28 2014-10-17 02:31:47.000000 pyCOREPOS-0.1.9/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)      880 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      112 2018-05-31 03:33:51.000000 pyCOREPOS-0.1.9/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/corepos/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1010 2020-07-16 02:42:12.000000 pyCOREPOS-0.1.9/corepos/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-05-02 03:17:30.000000 pyCOREPOS-0.1.9/corepos/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    16348 2021-02-09 22:11:35.000000 pyCOREPOS-0.1.9/corepos/api.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/corepos/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)      975 2021-12-31 03:47:38.000000 pyCOREPOS-0.1.9/corepos/db/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/corepos/db/lane_op/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1053 2021-07-09 01:32:22.000000 pyCOREPOS-0.1.9/corepos/db/lane_op/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9797 2023-02-15 18:50:07.000000 pyCOREPOS-0.1.9/corepos/db/lane_op/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1256 2020-02-28 03:41:42.000000 pyCOREPOS-0.1.9/corepos/db/model.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/corepos/db/office_op/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1092 2020-02-28 03:35:39.000000 pyCOREPOS-0.1.9/corepos/db/office_op/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    56902 2023-02-15 18:50:33.000000 pyCOREPOS-0.1.9/corepos/db/office_op/model.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/corepos/db/office_trans/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1104 2020-02-28 03:43:38.000000 pyCOREPOS-0.1.9/corepos/db/office_trans/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4389 2023-02-15 18:50:57.000000 pyCOREPOS-0.1.9/corepos/db/office_trans/model.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/corepos/db/office_trans_archive/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1056 2022-03-26 19:40:33.000000 pyCOREPOS-0.1.9/corepos/db/office_trans_archive/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1266 2023-02-15 18:51:14.000000 pyCOREPOS-0.1.9/corepos/db/office_trans_archive/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1913 2020-03-30 19:26:08.000000 pyCOREPOS-0.1.9/corepos/db/util.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4913 2020-08-16 21:08:07.000000 pyCOREPOS-0.1.9/corepos/enum.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/corepos/trans/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2020-02-28 03:45:53.000000 pyCOREPOS-0.1.9/corepos/trans/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/corepos/trans/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1261 2020-02-28 03:44:35.000000 pyCOREPOS-0.1.9/corepos/trans/db/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1280 2020-02-28 03:45:20.000000 pyCOREPOS-0.1.9/corepos/trans/db/model.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/pyCOREPOS.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)      880 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/pyCOREPOS.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      697 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/pyCOREPOS.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/pyCOREPOS.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       52 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/pyCOREPOS.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        8 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/pyCOREPOS.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       38 2023-05-02 03:17:50.000000 pyCOREPOS-0.1.9/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     3672 2023-02-15 18:49:50.000000 pyCOREPOS-0.1.9/setup.py
```

### Comparing `pyCOREPOS-0.1.8/COPYING.txt` & `pyCOREPOS-0.1.9/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/PKG-INFO` & `pyCOREPOS-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pyCOREPOS
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python Interface to CORE POS
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: COPYING.txt
 
 
 pyCOREPOS
 =========
```

### Comparing `pyCOREPOS-0.1.8/corepos/__init__.py` & `pyCOREPOS-0.1.9/corepos/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/corepos/api.py` & `pyCOREPOS-0.1.9/corepos/api.py`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/corepos/db/__init__.py` & `pyCOREPOS-0.1.9/corepos/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/corepos/db/lane_op/__init__.py` & `pyCOREPOS-0.1.9/corepos/db/lane_op/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/corepos/db/lane_op/model.py` & `pyCOREPOS-0.1.9/corepos/db/lane_op/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  pyCOREPOS -- Python Interface to CORE POS
-#  Copyright © 2018-2021 Lance Edgar
+#  Copyright © 2018-2023 Lance Edgar
 #
 #  This file is part of pyCOREPOS.
 #
 #  pyCOREPOS is free software: you can redistribute it and/or modify it under
 #  the terms of the GNU General Public License as published by the Free
 #  Software Foundation, either version 3 of the License, or (at your option)
 #  any later version.
@@ -21,19 +21,18 @@
 #
 ################################################################################
 """
 Data model for CORE POS "lane_op" DB
 """
 
 import sqlalchemy as sa
-# from sqlalchemy import orm
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy import orm
 
 
-Base = declarative_base()
+Base = orm.declarative_base()
 
 
 class Department(Base):
     """
     Represents a department within the organization.
     """
     __tablename__ = 'departments'
```

### Comparing `pyCOREPOS-0.1.8/corepos/db/model.py` & `pyCOREPOS-0.1.9/corepos/db/model.py`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/corepos/db/office_op/__init__.py` & `pyCOREPOS-0.1.9/corepos/db/office_op/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/corepos/db/office_op/model.py` & `pyCOREPOS-0.1.9/corepos/db/office_op/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  pyCOREPOS -- Python Interface to CORE POS
-#  Copyright © 2018-2021 Lance Edgar
+#  Copyright © 2018-2023 Lance Edgar
 #
 #  This file is part of pyCOREPOS.
 #
 #  pyCOREPOS is free software: you can redistribute it and/or modify it under
 #  the terms of the GNU General Public License as published by the Free
 #  Software Foundation, either version 3 of the License, or (at your option)
 #  any later version.
@@ -25,21 +25,20 @@
 """
 
 import datetime
 import logging
 
 import sqlalchemy as sa
 from sqlalchemy import orm
-from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.ext.associationproxy import association_proxy
 
 
 log = logging.getLogger(__name__)
 
-Base = declarative_base()
+Base = orm.declarative_base()
 
 
 class StringableDateTime(sa.TypeDecorator):
     """
     Sort of a hack, to let us string-ify certain DateTime values when
     generating "raw" SQL output.
```

### Comparing `pyCOREPOS-0.1.8/corepos/db/office_trans/__init__.py` & `pyCOREPOS-0.1.9/corepos/db/office_trans/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/corepos/db/office_trans/model.py` & `pyCOREPOS-0.1.9/corepos/db/office_trans/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  pyCOREPOS -- Python Interface to CORE POS
-#  Copyright © 2018-2020 Lance Edgar
+#  Copyright © 2018-2023 Lance Edgar
 #
 #  This file is part of pyCOREPOS.
 #
 #  pyCOREPOS is free software: you can redistribute it and/or modify it under
 #  the terms of the GNU General Public License as published by the Free
 #  Software Foundation, either version 3 of the License, or (at your option)
 #  any later version.
@@ -20,25 +20,21 @@
 #  pyCOREPOS.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
 CORE POS Transaction Data Model
 """
 
-from __future__ import unicode_literals, absolute_import
-
-import six
 import sqlalchemy as sa
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy import orm
 
 
-Base = declarative_base()
+Base = orm.declarative_base()
 
 
-@six.python_2_unicode_compatible
 class TransactionDetailBase(object):
     """
     Represents a POS transaction detail record.
     """
 
     # store
     store_row_id = sa.Column(sa.Integer(), primary_key=True, nullable=False)
```

### Comparing `pyCOREPOS-0.1.8/corepos/db/office_trans_archive/__init__.py` & `pyCOREPOS-0.1.9/corepos/db/office_trans_archive/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/corepos/db/office_trans_archive/model.py` & `pyCOREPOS-0.1.9/corepos/trans/db/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  pyCOREPOS -- Python Interface to CORE POS
-#  Copyright © 2018-2022 Lance Edgar
+#  Copyright © 2018-2020 Lance Edgar
 #
 #  This file is part of pyCOREPOS.
 #
 #  pyCOREPOS is free software: you can redistribute it and/or modify it under
 #  the terms of the GNU General Public License as published by the Free
 #  Software Foundation, either version 3 of the License, or (at your option)
 #  any later version.
@@ -20,20 +20,15 @@
 #  pyCOREPOS.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
 CORE POS Transaction Data Model
 """
 
-from sqlalchemy.ext.declarative import declarative_base
+from __future__ import unicode_literals, absolute_import
 
-from corepos.db.office_trans.model import TransactionDetailBase
+import warnings
+warnings.warn("The `corepos.trans.db.model` module is deprecated!  "
+              "Please use `corepos.db.office_trans.model` instead.",
+              DeprecationWarning)
 
-
-Base = declarative_base()
-
-
-class TransactionDetail(TransactionDetailBase, Base):
-    """
-    Represents a POS transaction detail record.
-    """
-    __tablename__ = 'bigArchive'
+from corepos.db.office_trans.model import *
```

### Comparing `pyCOREPOS-0.1.8/corepos/db/util.py` & `pyCOREPOS-0.1.9/corepos/db/util.py`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/corepos/enum.py` & `pyCOREPOS-0.1.9/corepos/enum.py`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/corepos/trans/db/__init__.py` & `pyCOREPOS-0.1.9/corepos/trans/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/pyCOREPOS.egg-info/PKG-INFO` & `pyCOREPOS-0.1.9/pyCOREPOS.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pyCOREPOS
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python Interface to CORE POS
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: COPYING.txt
 
 
 pyCOREPOS
 =========
```

### Comparing `pyCOREPOS-0.1.8/pyCOREPOS.egg-info/SOURCES.txt` & `pyCOREPOS-0.1.9/pyCOREPOS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyCOREPOS-0.1.8/setup.py` & `pyCOREPOS-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  pyCOREPOS -- Python Interface to CORE POS
-#  Copyright © 2018-2020 Lance Edgar
+#  Copyright © 2018-2023 Lance Edgar
 #
 #  This file is part of pyCOREPOS.
 #
 #  pyCOREPOS is free software: you can redistribute it and/or modify it under
 #  the terms of the GNU General Public License as published by the Free
 #  Software Foundation, either version 3 of the License, or (at your option)
 #  any later version.
@@ -59,15 +59,15 @@
     # encountered then they should be filed as such.
     #
     # package                           # low                   high
 
     'mysql-connector-python',           # 8.0.6
     'requests',                         # 2.23.0
     'six',                              # 1.12.0
-    'SQLAlchemy',                       # 0.9.8
+    'SQLAlchemy>=1.4',                  # 1.4.0
 ]
 
 
 setup(
     name = "pyCOREPOS",
     version = __version__,
     author = "Lance Edgar",
@@ -83,15 +83,14 @@
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Topic :: Office/Business',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 
     install_requires = requires,
     packages = find_packages(),
 )
```

