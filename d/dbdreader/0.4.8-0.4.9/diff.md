# Comparing `tmp/dbdreader-0.4.8.tar.gz` & `tmp/dbdreader-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbdreader-0.4.8.tar", last modified: Tue Nov 30 17:50:52 2021, max compression
+gzip compressed data, was "dbdreader-0.4.9.tar", last modified: Mon May 16 11:33:31 2022, max compression
```

## Comparing `dbdreader-0.4.8.tar` & `dbdreader-0.4.9.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxr-x   0 lucas     (1001) lucas     (1001)        0 2021-11-30 17:50:52.345929 dbdreader-0.4.8/
--rw-rw-r--   0 lucas     (1001) lucas     (1001)    18009 2021-04-30 16:34:52.000000 dbdreader-0.4.8/COPYING
--rw-rw-r--   0 lucas     (1001) lucas     (1001)      162 2021-04-30 16:34:52.000000 dbdreader-0.4.8/MANIFEST.in
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     6137 2021-11-30 17:50:52.344930 dbdreader-0.4.8/PKG-INFO
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     4497 2021-11-30 17:50:37.000000 dbdreader-0.4.8/README.rst
--rwxrwxr-x   0 lucas     (1001) lucas     (1001)     2427 2021-04-30 16:34:52.000000 dbdreader-0.4.8/cac_gen.py
-drwxrwxr-x   0 lucas     (1001) lucas     (1001)        0 2021-11-30 17:50:52.342929 dbdreader-0.4.8/data/
--rw-rw-r--   0 lucas     (1001) lucas     (1001)   701666 2021-04-30 16:34:52.000000 dbdreader-0.4.8/data/amadeus-2014-204-05-000.dbd
--rw-rw-r--   0 lucas     (1001) lucas     (1001)   154402 2021-04-30 16:34:52.000000 dbdreader-0.4.8/data/amadeus-2014-204-05-000.ebd
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     3658 2021-04-30 16:34:52.000000 dbdreader-0.4.8/data/amadeus-2014-204-05-000.sbd
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     4802 2021-04-30 16:34:52.000000 dbdreader-0.4.8/data/amadeus-2014-204-05-000.tbd
--rw-rw-r--   0 lucas     (1001) lucas     (1001)      570 2021-04-30 16:34:52.000000 dbdreader-0.4.8/data/amadeus-2014-204-05-001.sbd
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     2036 2021-04-30 16:34:52.000000 dbdreader-0.4.8/data/amadeus-2014-204-05-001.tbd
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     3736 2021-04-30 16:34:52.000000 dbdreader-0.4.8/data/amadeus-2014-204-05-002.sbd
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     3981 2021-04-30 16:34:52.000000 dbdreader-0.4.8/data/amadeus-2014-204-05-002.tbd
--rw-rw-r--   0 lucas     (1001) lucas     (1001)   313627 2021-04-30 16:34:52.000000 dbdreader-0.4.8/data/ammonite-2008-028-01-000.mbd
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     2537 2021-11-27 13:11:25.000000 dbdreader-0.4.8/data/unit_887-2021-321-3-0.sbd
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     3065 2021-11-27 13:11:25.000000 dbdreader-0.4.8/data/unit_887-2021-321-3-0.tbd
-drwxrwxr-x   0 lucas     (1001) lucas     (1001)        0 2021-11-30 17:50:52.343930 dbdreader-0.4.8/dbdreader/
--rw-rw-r--   0 lucas     (1001) lucas     (1001)       71 2021-11-30 17:34:21.000000 dbdreader-0.4.8/dbdreader/__init__.py
--rw-rw-r--   0 lucas     (1001) lucas     (1001)    59084 2021-11-27 16:21:51.000000 dbdreader-0.4.8/dbdreader/dbdreader.py
-drwxrwxr-x   0 lucas     (1001) lucas     (1001)        0 2021-11-30 17:50:52.343930 dbdreader-0.4.8/dbdreader.egg-info/
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     6137 2021-11-30 17:50:52.000000 dbdreader-0.4.8/dbdreader.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1001) lucas     (1001)      876 2021-11-30 17:50:52.000000 dbdreader-0.4.8/dbdreader.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1001) lucas     (1001)        1 2021-11-30 17:50:52.000000 dbdreader-0.4.8/dbdreader.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1001) lucas     (1001)       36 2021-11-30 17:50:52.000000 dbdreader-0.4.8/dbdreader.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1001) lucas     (1001)        6 2021-11-30 17:50:52.000000 dbdreader-0.4.8/dbdreader.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1001) lucas     (1001)       21 2021-11-30 17:50:52.000000 dbdreader-0.4.8/dbdreader.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     4174 2021-04-30 16:34:52.000000 dbdreader-0.4.8/dbdrename.py
-drwxrwxr-x   0 lucas     (1001) lucas     (1001)        0 2021-11-30 17:50:52.344930 dbdreader-0.4.8/examples/
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     3501 2021-04-30 16:34:52.000000 dbdreader-0.4.8/examples/read_multiple_dbd_files.py
--rw-rw-r--   0 lucas     (1001) lucas     (1001)      705 2021-04-30 16:34:52.000000 dbdreader-0.4.8/examples/read_single_dbd_file.py
-drwxrwxr-x   0 lucas     (1001) lucas     (1001)        0 2021-11-30 17:50:52.344930 dbdreader-0.4.8/extension/
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     9541 2021-11-27 13:11:25.000000 dbdreader-0.4.8/extension/dbdreader.c
-drwxrwxr-x   0 lucas     (1001) lucas     (1001)        0 2021-11-30 17:50:52.344930 dbdreader-0.4.8/extension/include/
--rw-rw-r--   0 lucas     (1001) lucas     (1001)      747 2021-04-30 16:34:52.000000 dbdreader-0.4.8/extension/include/dbdreader.h
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     3500 2021-04-30 16:34:52.000000 dbdreader-0.4.8/extension/py_dbdreader.c
--rw-rw-r--   0 lucas     (1001) lucas     (1001)       38 2021-11-30 17:50:52.345929 dbdreader-0.4.8/setup.cfg
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     1271 2021-11-30 17:34:21.000000 dbdreader-0.4.8/setup.py
-drwxrwxr-x   0 lucas     (1001) lucas     (1001)        0 2021-11-30 17:50:52.344930 dbdreader-0.4.8/tests/
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     1464 2021-04-30 16:34:52.000000 dbdreader-0.4.8/tests/dbd_test.py
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     1823 2021-11-27 13:11:25.000000 dbdreader-0.4.8/tests/dbd_test_2.py
--rw-rw-r--   0 lucas     (1001) lucas     (1001)     8519 2021-11-27 16:24:00.000000 dbdreader-0.4.8/tests/dbdreader_test.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1004)        0 2022-05-16 11:33:31.461322 dbdreader-0.4.9/
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)    18009 2018-09-03 13:05:00.000000 dbdreader-0.4.9/COPYING
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)    35147 2018-09-03 13:05:00.000000 dbdreader-0.4.9/LICENSE
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)      162 2020-12-10 15:22:43.000000 dbdreader-0.4.9/MANIFEST.in
+-rw-r--r--   0 lucas     (1001) lucas     (1004)     5098 2022-05-16 11:33:31.461322 dbdreader-0.4.9/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1004)     4497 2021-12-15 10:42:58.000000 dbdreader-0.4.9/README.rst
+-rwxrwxr-x   0 lucas     (1001) lucas     (1004)     2427 2018-09-03 13:05:00.000000 dbdreader-0.4.9/cac_gen.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1004)        0 2022-05-16 11:33:31.459322 dbdreader-0.4.9/data/
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)   701666 2020-12-10 15:22:43.000000 dbdreader-0.4.9/data/amadeus-2014-204-05-000.dbd
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)   154402 2020-12-10 15:22:43.000000 dbdreader-0.4.9/data/amadeus-2014-204-05-000.ebd
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)     3658 2018-09-03 13:05:00.000000 dbdreader-0.4.9/data/amadeus-2014-204-05-000.sbd
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)     4802 2018-09-03 13:05:00.000000 dbdreader-0.4.9/data/amadeus-2014-204-05-000.tbd
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)      570 2018-09-03 13:05:00.000000 dbdreader-0.4.9/data/amadeus-2014-204-05-001.sbd
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)     2036 2018-09-03 13:05:00.000000 dbdreader-0.4.9/data/amadeus-2014-204-05-001.tbd
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)     3736 2018-09-03 13:05:00.000000 dbdreader-0.4.9/data/amadeus-2014-204-05-002.sbd
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)     3981 2018-09-03 13:05:00.000000 dbdreader-0.4.9/data/amadeus-2014-204-05-002.tbd
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)   313627 2020-12-10 15:22:43.000000 dbdreader-0.4.9/data/ammonite-2008-028-01-000.mbd
+-rw-r--r--   0 lucas     (1001) lucas     (1004)     2537 2021-11-29 12:23:35.000000 dbdreader-0.4.9/data/unit_887-2021-321-3-0.sbd
+-rw-r--r--   0 lucas     (1001) lucas     (1004)     3065 2021-11-29 12:23:35.000000 dbdreader-0.4.9/data/unit_887-2021-321-3-0.tbd
+drwxr-xr-x   0 lucas     (1001) lucas     (1004)        0 2022-05-16 11:33:31.459322 dbdreader-0.4.9/dbdreader/
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)       71 2022-05-16 09:27:51.000000 dbdreader-0.4.9/dbdreader/__init__.py
+-rw-r--r--   0 lucas     (1001) lucas     (1004)    59084 2022-05-16 09:13:47.000000 dbdreader-0.4.9/dbdreader/dbdreader.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1004)        0 2022-05-16 11:33:31.460322 dbdreader-0.4.9/dbdreader.egg-info/
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)     5098 2022-05-16 11:33:31.000000 dbdreader-0.4.9/dbdreader.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)      904 2022-05-16 11:33:31.000000 dbdreader-0.4.9/dbdreader.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)        1 2022-05-16 11:33:31.000000 dbdreader-0.4.9/dbdreader.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)       36 2022-05-16 11:33:31.000000 dbdreader-0.4.9/dbdreader.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)        6 2022-05-16 11:33:31.000000 dbdreader-0.4.9/dbdreader.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)       21 2022-05-16 11:33:31.000000 dbdreader-0.4.9/dbdreader.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)     4174 2018-09-03 13:05:00.000000 dbdreader-0.4.9/dbdrename.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1004)        0 2022-05-16 11:33:31.460322 dbdreader-0.4.9/examples/
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)     3501 2021-03-22 08:53:30.000000 dbdreader-0.4.9/examples/read_multiple_dbd_files.py
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)      705 2021-03-22 08:53:37.000000 dbdreader-0.4.9/examples/read_single_dbd_file.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1004)        0 2022-05-16 11:33:31.460322 dbdreader-0.4.9/extension/
+-rw-r--r--   0 lucas     (1001) lucas     (1004)    10065 2022-05-16 09:07:00.000000 dbdreader-0.4.9/extension/dbdreader.c
+drwxr-xr-x   0 lucas     (1001) lucas     (1004)        0 2022-05-16 11:33:31.461322 dbdreader-0.4.9/extension/include/
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)      747 2019-03-25 07:46:06.000000 dbdreader-0.4.9/extension/include/dbdreader.h
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)     3500 2019-03-25 07:46:06.000000 dbdreader-0.4.9/extension/py_dbdreader.c
+-rw-r--r--   0 lucas     (1001) lucas     (1004)       38 2022-05-16 11:33:31.461322 dbdreader-0.4.9/setup.cfg
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)     1271 2021-11-30 08:06:57.000000 dbdreader-0.4.9/setup.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1004)        0 2022-05-16 11:33:31.461322 dbdreader-0.4.9/tests/
+-rw-rw-r--   0 lucas     (1001) lucas     (1004)     1464 2020-12-10 15:22:43.000000 dbdreader-0.4.9/tests/dbd_test.py
+-rw-r--r--   0 lucas     (1001) lucas     (1004)     1823 2021-11-29 12:23:35.000000 dbdreader-0.4.9/tests/dbd_test_2.py
+-rw-r--r--   0 lucas     (1001) lucas     (1004)     3827 2022-05-16 09:08:57.000000 dbdreader-0.4.9/tests/dbd_test_3.py
+-rw-r--r--   0 lucas     (1001) lucas     (1004)     8519 2021-11-29 12:23:35.000000 dbdreader-0.4.9/tests/dbdreader_test.py
```

### Comparing `dbdreader-0.4.8/COPYING` & `dbdreader-0.4.9/COPYING`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/PKG-INFO` & `dbdreader-0.4.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,149 +1,153 @@
 Metadata-Version: 2.1
 Name: dbdreader
-Version: 0.4.8
+Version: 0.4.9
 Summary: A python module to access binary data files generated by Teledyne WebbResearch gliders
 Home-page: https://dbdreader.readthedocs.io/en/latest/
 Author: Lucas Merckelbach
 Author-email: lucas.merckelbach@hzg.de
 License: UNKNOWN
-Description: |PyPI version| |Docs badge| |License|
-        
-        DBDREADER
-        =========
-        
-        Change log
-        ----------
-        Version 0.4.8
-        
-        * Support for reading {demnst}bd files from G3S gliders (issue #6). (Thanks to Owain Jones)
-        
-        * Bug fix for correctly throwing an exception when cache file is missing(issue #5)
-        
-        Version 0.4.7
-        
-        * Bug fix for reading dbd files on Windows.
-        
-        * a wheel provided for CPython 3.9 on Windows 64 bit.  
-        
-        Version 0.4.6
-        
-        * Added  get_CTD_sync, a convenience method to retrieve CTD data, and other parameters mapped on the CTD time stamps. Also ensures time stamps are monotonically increasing.
-        
-        * Adds bounds to what values of latitude and longitude are considered valid.
-        
-        Version 0.4.5
-        
-        * dbdreader now ignores the first line of data in each binary file
-          
-        * dbdreader checks whether the value of the parameters read are finite, ignoring them if they are not.
-        
-        
-        Synopsis
-        --------
-        Slocum ocean gliders are autonomous underwater vehicles, used for
-        making oceanographic measurements. The data that these devices and
-        their sensors collect, are stored in binary data files. The python
-        module *dbdreader* provides the utilities to extract the data from the
-        binary files, so that they can be further analysed.
-        
-        Installation
-        ------------
-        The python module *dbdreader* can be installed from source, using the
-        standard method to install python code. Note that this method requires
-        an C-extension to be build. (The actual reading from files is done in
-        C for speed.) In order to build the extension successfully, you would
-        need a C-compiler. On Linux, this can be gcc, with supporting
-        development/header files for python. On Fedora you would do ``sudo dnf
-        install python3-devel``.
-        
-        Alternatively, dbdreader can also be installed from PyPi, using ``pip3
-        install dbdreader``.
-        
-        
-        Installation on Windows
-        -----------------------
-        If you want to install dbdreader from source, you will need a C
-        compiler as well to compile the C-extension. Besides the Python
-        environment you will need to install the Microsoft Visual Studio
-        Compiler. The community edition will do. When installing MVSC, make sure
-        you tick the box *python development* during the setup. Once installed
-        dbdreader can be installed, and the C-extension should be compiled
-        automatically.
-        
-        Installiation using pip, for example as in ``py -m pip install
-        dbdreader`` also requires the C compiler. For Python version 3.9,
-        however, a wheel is provided, which can be installed adding the option
-        ``--only-binary :all:`` to the pip command: ::
-        
-          $ pip install --only-binary :all: dbdreader
-        
-        
-        Documentation
-        -------------
-        Comprehensive documentation is provided at https://dbdreader.readthedocs.io/en/latest/
-        
-        Quick-start
-        -----------
-        For the impatient...
-        
-        The dbdreader module implements a class DBD() which provides the
-        machinery to read a single dbd file. The most commonly used methods
-        are:
-        
-        * get(parametername)
-        * get_sync(parametername, \*other_parameternames)
-        
-        The first method returs a tuple with time and values for requested
-        parameter. The second method, returns a tuple with time and values of
-        the first parameter requested, and of all further listed parameters,
-        all interpolated on the time base of the first parameter.
-        
-        Mostly, it is not one file that is required to be processed, but a
-        number of them. This interface is implemented by the MultiDBD
-        class. Files can either be specified as a list of filenames, or as a
-        pattern using wildcards.
-        
-        Examples
-        ^^^^^^^^
-        
-        To read a single file::
-        
-          >>> dbd = DBD("00010010.dbd")
-          >>> t, pitch = dbd.get("m_pitch")
-          >>> t, hdg, ptch, roll = dbd.get_sync("m_heading", "m_pitch", "m_roll)
-        
-        Or, doing the same, but using both dbd and ebd files::
-          
-          >>> dbd = DBD(pattern="00010010.[de]bd")
-          >>> t, pitch = dbd.get("m_pitch")
-          >>> t, hdg, ptch, roll = dbd.get_sync("m_heading", "m_pitch", "m_roll")
-          >>> t, p_ctd, p_nav = dbd.get_sync("sci_water_pressure", "m_water_pressure")
-        
-          
-        
-        Python 2
-        --------
-        Python 2.7 is not supported anymore. However, you should be able to
-        make the code able to run on python2.7 using the *future* package.
-        
-        * pip install future
-        * pasteurize dbdreader.
-        
-        For details see http://python-future.org/pasteurize.html.
-        
-        
-        .. |PyPI version| image:: https://badgen.net/pypi/v/dbdreader
-           :target: https://pypi.org/project/dbdreader
-        .. |Docs badge| image:: https://readthedocs.org/projects/dbdreader/badge/?version=latest
-           :target: https://dbdreader.readthedocs.io/en/latest/
-        .. |License| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
-           :target: https://www.gnu.org/licenses/gpl-3.0
-        
-        	 
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: COPYING
+
+|PyPI version| |Docs badge| |License|
+
+DBDREADER
+=========
+
+Change log
+----------
+Version 0.4.8
+
+* Support for reading {demnst}bd files from G3S gliders (issue #6). (Thanks to Owain Jones)
+
+* Bug fix for correctly throwing an exception when cache file is missing(issue #5)
+
+Version 0.4.7
+
+* Bug fix for reading dbd files on Windows.
+
+* a wheel provided for CPython 3.9 on Windows 64 bit.  
+
+Version 0.4.6
+
+* Added  get_CTD_sync, a convenience method to retrieve CTD data, and other parameters mapped on the CTD time stamps. Also ensures time stamps are monotonically increasing.
+
+* Adds bounds to what values of latitude and longitude are considered valid.
+
+Version 0.4.5
+
+* dbdreader now ignores the first line of data in each binary file
+  
+* dbdreader checks whether the value of the parameters read are finite, ignoring them if they are not.
+
+
+Synopsis
+--------
+Slocum ocean gliders are autonomous underwater vehicles, used for
+making oceanographic measurements. The data that these devices and
+their sensors collect, are stored in binary data files. The python
+module *dbdreader* provides the utilities to extract the data from the
+binary files, so that they can be further analysed.
+
+Installation
+------------
+The python module *dbdreader* can be installed from source, using the
+standard method to install python code. Note that this method requires
+an C-extension to be build. (The actual reading from files is done in
+C for speed.) In order to build the extension successfully, you would
+need a C-compiler. On Linux, this can be gcc, with supporting
+development/header files for python. On Fedora you would do ``sudo dnf
+install python3-devel``.
+
+Alternatively, dbdreader can also be installed from PyPi, using ``pip3
+install dbdreader``.
+
+
+Installation on Windows
+-----------------------
+If you want to install dbdreader from source, you will need a C
+compiler as well to compile the C-extension. Besides the Python
+environment you will need to install the Microsoft Visual Studio
+Compiler. The community edition will do. When installing MVSC, make sure
+you tick the box *python development* during the setup. Once installed
+dbdreader can be installed, and the C-extension should be compiled
+automatically.
+
+Installiation using pip, for example as in ``py -m pip install
+dbdreader`` also requires the C compiler. For Python version 3.9,
+however, a wheel is provided, which can be installed adding the option
+``--only-binary :all:`` to the pip command: ::
+
+  $ pip install --only-binary :all: dbdreader
+
+
+Documentation
+-------------
+Comprehensive documentation is provided at https://dbdreader.readthedocs.io/en/latest/
+
+Quick-start
+-----------
+For the impatient...
+
+The dbdreader module implements a class DBD() which provides the
+machinery to read a single dbd file. The most commonly used methods
+are:
+
+* get(parametername)
+* get_sync(parametername, \*other_parameternames)
+
+The first method returs a tuple with time and values for requested
+parameter. The second method, returns a tuple with time and values of
+the first parameter requested, and of all further listed parameters,
+all interpolated on the time base of the first parameter.
+
+Mostly, it is not one file that is required to be processed, but a
+number of them. This interface is implemented by the MultiDBD
+class. Files can either be specified as a list of filenames, or as a
+pattern using wildcards.
+
+Examples
+^^^^^^^^
+
+To read a single file::
+
+  >>> dbd = DBD("00010010.dbd")
+  >>> t, pitch = dbd.get("m_pitch")
+  >>> t, hdg, ptch, roll = dbd.get_sync("m_heading", "m_pitch", "m_roll)
+
+Or, doing the same, but using both dbd and ebd files::
+  
+  >>> dbd = DBD(pattern="00010010.[de]bd")
+  >>> t, pitch = dbd.get("m_pitch")
+  >>> t, hdg, ptch, roll = dbd.get_sync("m_heading", "m_pitch", "m_roll")
+  >>> t, p_ctd, p_nav = dbd.get_sync("sci_water_pressure", "m_water_pressure")
+
+  
+
+Python 2
+--------
+Python 2.7 is not supported anymore. However, you should be able to
+make the code able to run on python2.7 using the *future* package.
+
+* pip install future
+* pasteurize dbdreader.
+
+For details see http://python-future.org/pasteurize.html.
+
+
+.. |PyPI version| image:: https://badgen.net/pypi/v/dbdreader
+   :target: https://pypi.org/project/dbdreader
+.. |Docs badge| image:: https://readthedocs.org/projects/dbdreader/badge/?version=latest
+   :target: https://dbdreader.readthedocs.io/en/latest/
+.. |License| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
+   :target: https://www.gnu.org/licenses/gpl-3.0
+
+	 
+
+
```

### Comparing `dbdreader-0.4.8/README.rst` & `dbdreader-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/cac_gen.py` & `dbdreader-0.4.9/cac_gen.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/data/amadeus-2014-204-05-000.dbd` & `dbdreader-0.4.9/data/amadeus-2014-204-05-000.dbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/data/amadeus-2014-204-05-000.ebd` & `dbdreader-0.4.9/data/amadeus-2014-204-05-000.ebd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/data/amadeus-2014-204-05-000.sbd` & `dbdreader-0.4.9/data/amadeus-2014-204-05-000.sbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/data/amadeus-2014-204-05-000.tbd` & `dbdreader-0.4.9/data/amadeus-2014-204-05-000.tbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/data/amadeus-2014-204-05-001.sbd` & `dbdreader-0.4.9/data/amadeus-2014-204-05-001.sbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/data/amadeus-2014-204-05-001.tbd` & `dbdreader-0.4.9/data/amadeus-2014-204-05-001.tbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/data/amadeus-2014-204-05-002.sbd` & `dbdreader-0.4.9/data/amadeus-2014-204-05-002.sbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/data/amadeus-2014-204-05-002.tbd` & `dbdreader-0.4.9/data/amadeus-2014-204-05-002.tbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/data/ammonite-2008-028-01-000.mbd` & `dbdreader-0.4.9/data/ammonite-2008-028-01-000.mbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/data/unit_887-2021-321-3-0.sbd` & `dbdreader-0.4.9/data/unit_887-2021-321-3-0.sbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/data/unit_887-2021-321-3-0.tbd` & `dbdreader-0.4.9/data/unit_887-2021-321-3-0.tbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/dbdreader/dbdreader.py` & `dbdreader-0.4.9/dbdreader/dbdreader.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/dbdreader.egg-info/PKG-INFO` & `dbdreader-0.4.9/dbdreader.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,149 +1,153 @@
 Metadata-Version: 2.1
 Name: dbdreader
-Version: 0.4.8
+Version: 0.4.9
 Summary: A python module to access binary data files generated by Teledyne WebbResearch gliders
 Home-page: https://dbdreader.readthedocs.io/en/latest/
 Author: Lucas Merckelbach
 Author-email: lucas.merckelbach@hzg.de
 License: UNKNOWN
-Description: |PyPI version| |Docs badge| |License|
-        
-        DBDREADER
-        =========
-        
-        Change log
-        ----------
-        Version 0.4.8
-        
-        * Support for reading {demnst}bd files from G3S gliders (issue #6). (Thanks to Owain Jones)
-        
-        * Bug fix for correctly throwing an exception when cache file is missing(issue #5)
-        
-        Version 0.4.7
-        
-        * Bug fix for reading dbd files on Windows.
-        
-        * a wheel provided for CPython 3.9 on Windows 64 bit.  
-        
-        Version 0.4.6
-        
-        * Added  get_CTD_sync, a convenience method to retrieve CTD data, and other parameters mapped on the CTD time stamps. Also ensures time stamps are monotonically increasing.
-        
-        * Adds bounds to what values of latitude and longitude are considered valid.
-        
-        Version 0.4.5
-        
-        * dbdreader now ignores the first line of data in each binary file
-          
-        * dbdreader checks whether the value of the parameters read are finite, ignoring them if they are not.
-        
-        
-        Synopsis
-        --------
-        Slocum ocean gliders are autonomous underwater vehicles, used for
-        making oceanographic measurements. The data that these devices and
-        their sensors collect, are stored in binary data files. The python
-        module *dbdreader* provides the utilities to extract the data from the
-        binary files, so that they can be further analysed.
-        
-        Installation
-        ------------
-        The python module *dbdreader* can be installed from source, using the
-        standard method to install python code. Note that this method requires
-        an C-extension to be build. (The actual reading from files is done in
-        C for speed.) In order to build the extension successfully, you would
-        need a C-compiler. On Linux, this can be gcc, with supporting
-        development/header files for python. On Fedora you would do ``sudo dnf
-        install python3-devel``.
-        
-        Alternatively, dbdreader can also be installed from PyPi, using ``pip3
-        install dbdreader``.
-        
-        
-        Installation on Windows
-        -----------------------
-        If you want to install dbdreader from source, you will need a C
-        compiler as well to compile the C-extension. Besides the Python
-        environment you will need to install the Microsoft Visual Studio
-        Compiler. The community edition will do. When installing MVSC, make sure
-        you tick the box *python development* during the setup. Once installed
-        dbdreader can be installed, and the C-extension should be compiled
-        automatically.
-        
-        Installiation using pip, for example as in ``py -m pip install
-        dbdreader`` also requires the C compiler. For Python version 3.9,
-        however, a wheel is provided, which can be installed adding the option
-        ``--only-binary :all:`` to the pip command: ::
-        
-          $ pip install --only-binary :all: dbdreader
-        
-        
-        Documentation
-        -------------
-        Comprehensive documentation is provided at https://dbdreader.readthedocs.io/en/latest/
-        
-        Quick-start
-        -----------
-        For the impatient...
-        
-        The dbdreader module implements a class DBD() which provides the
-        machinery to read a single dbd file. The most commonly used methods
-        are:
-        
-        * get(parametername)
-        * get_sync(parametername, \*other_parameternames)
-        
-        The first method returs a tuple with time and values for requested
-        parameter. The second method, returns a tuple with time and values of
-        the first parameter requested, and of all further listed parameters,
-        all interpolated on the time base of the first parameter.
-        
-        Mostly, it is not one file that is required to be processed, but a
-        number of them. This interface is implemented by the MultiDBD
-        class. Files can either be specified as a list of filenames, or as a
-        pattern using wildcards.
-        
-        Examples
-        ^^^^^^^^
-        
-        To read a single file::
-        
-          >>> dbd = DBD("00010010.dbd")
-          >>> t, pitch = dbd.get("m_pitch")
-          >>> t, hdg, ptch, roll = dbd.get_sync("m_heading", "m_pitch", "m_roll)
-        
-        Or, doing the same, but using both dbd and ebd files::
-          
-          >>> dbd = DBD(pattern="00010010.[de]bd")
-          >>> t, pitch = dbd.get("m_pitch")
-          >>> t, hdg, ptch, roll = dbd.get_sync("m_heading", "m_pitch", "m_roll")
-          >>> t, p_ctd, p_nav = dbd.get_sync("sci_water_pressure", "m_water_pressure")
-        
-          
-        
-        Python 2
-        --------
-        Python 2.7 is not supported anymore. However, you should be able to
-        make the code able to run on python2.7 using the *future* package.
-        
-        * pip install future
-        * pasteurize dbdreader.
-        
-        For details see http://python-future.org/pasteurize.html.
-        
-        
-        .. |PyPI version| image:: https://badgen.net/pypi/v/dbdreader
-           :target: https://pypi.org/project/dbdreader
-        .. |Docs badge| image:: https://readthedocs.org/projects/dbdreader/badge/?version=latest
-           :target: https://dbdreader.readthedocs.io/en/latest/
-        .. |License| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
-           :target: https://www.gnu.org/licenses/gpl-3.0
-        
-        	 
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: COPYING
+
+|PyPI version| |Docs badge| |License|
+
+DBDREADER
+=========
+
+Change log
+----------
+Version 0.4.8
+
+* Support for reading {demnst}bd files from G3S gliders (issue #6). (Thanks to Owain Jones)
+
+* Bug fix for correctly throwing an exception when cache file is missing(issue #5)
+
+Version 0.4.7
+
+* Bug fix for reading dbd files on Windows.
+
+* a wheel provided for CPython 3.9 on Windows 64 bit.  
+
+Version 0.4.6
+
+* Added  get_CTD_sync, a convenience method to retrieve CTD data, and other parameters mapped on the CTD time stamps. Also ensures time stamps are monotonically increasing.
+
+* Adds bounds to what values of latitude and longitude are considered valid.
+
+Version 0.4.5
+
+* dbdreader now ignores the first line of data in each binary file
+  
+* dbdreader checks whether the value of the parameters read are finite, ignoring them if they are not.
+
+
+Synopsis
+--------
+Slocum ocean gliders are autonomous underwater vehicles, used for
+making oceanographic measurements. The data that these devices and
+their sensors collect, are stored in binary data files. The python
+module *dbdreader* provides the utilities to extract the data from the
+binary files, so that they can be further analysed.
+
+Installation
+------------
+The python module *dbdreader* can be installed from source, using the
+standard method to install python code. Note that this method requires
+an C-extension to be build. (The actual reading from files is done in
+C for speed.) In order to build the extension successfully, you would
+need a C-compiler. On Linux, this can be gcc, with supporting
+development/header files for python. On Fedora you would do ``sudo dnf
+install python3-devel``.
+
+Alternatively, dbdreader can also be installed from PyPi, using ``pip3
+install dbdreader``.
+
+
+Installation on Windows
+-----------------------
+If you want to install dbdreader from source, you will need a C
+compiler as well to compile the C-extension. Besides the Python
+environment you will need to install the Microsoft Visual Studio
+Compiler. The community edition will do. When installing MVSC, make sure
+you tick the box *python development* during the setup. Once installed
+dbdreader can be installed, and the C-extension should be compiled
+automatically.
+
+Installiation using pip, for example as in ``py -m pip install
+dbdreader`` also requires the C compiler. For Python version 3.9,
+however, a wheel is provided, which can be installed adding the option
+``--only-binary :all:`` to the pip command: ::
+
+  $ pip install --only-binary :all: dbdreader
+
+
+Documentation
+-------------
+Comprehensive documentation is provided at https://dbdreader.readthedocs.io/en/latest/
+
+Quick-start
+-----------
+For the impatient...
+
+The dbdreader module implements a class DBD() which provides the
+machinery to read a single dbd file. The most commonly used methods
+are:
+
+* get(parametername)
+* get_sync(parametername, \*other_parameternames)
+
+The first method returs a tuple with time and values for requested
+parameter. The second method, returns a tuple with time and values of
+the first parameter requested, and of all further listed parameters,
+all interpolated on the time base of the first parameter.
+
+Mostly, it is not one file that is required to be processed, but a
+number of them. This interface is implemented by the MultiDBD
+class. Files can either be specified as a list of filenames, or as a
+pattern using wildcards.
+
+Examples
+^^^^^^^^
+
+To read a single file::
+
+  >>> dbd = DBD("00010010.dbd")
+  >>> t, pitch = dbd.get("m_pitch")
+  >>> t, hdg, ptch, roll = dbd.get_sync("m_heading", "m_pitch", "m_roll)
+
+Or, doing the same, but using both dbd and ebd files::
+  
+  >>> dbd = DBD(pattern="00010010.[de]bd")
+  >>> t, pitch = dbd.get("m_pitch")
+  >>> t, hdg, ptch, roll = dbd.get_sync("m_heading", "m_pitch", "m_roll")
+  >>> t, p_ctd, p_nav = dbd.get_sync("sci_water_pressure", "m_water_pressure")
+
+  
+
+Python 2
+--------
+Python 2.7 is not supported anymore. However, you should be able to
+make the code able to run on python2.7 using the *future* package.
+
+* pip install future
+* pasteurize dbdreader.
+
+For details see http://python-future.org/pasteurize.html.
+
+
+.. |PyPI version| image:: https://badgen.net/pypi/v/dbdreader
+   :target: https://pypi.org/project/dbdreader
+.. |Docs badge| image:: https://readthedocs.org/projects/dbdreader/badge/?version=latest
+   :target: https://dbdreader.readthedocs.io/en/latest/
+.. |License| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
+   :target: https://www.gnu.org/licenses/gpl-3.0
+
+	 
+
+
```

### Comparing `dbdreader-0.4.8/dbdreader.egg-info/SOURCES.txt` & `dbdreader-0.4.9/dbdreader.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 COPYING
+LICENSE
 MANIFEST.in
 README.rst
 cac_gen.py
 dbdrename.py
 setup.py
 data/amadeus-2014-204-05-000.dbd
 data/amadeus-2014-204-05-000.ebd
@@ -26,8 +27,9 @@
 examples/read_multiple_dbd_files.py
 examples/read_single_dbd_file.py
 extension/dbdreader.c
 extension/py_dbdreader.c
 extension/include/dbdreader.h
 tests/dbd_test.py
 tests/dbd_test_2.py
+tests/dbd_test_3.py
 tests/dbdreader_test.py
```

### Comparing `dbdreader-0.4.8/dbdrename.py` & `dbdreader-0.4.9/dbdrename.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/examples/read_multiple_dbd_files.py` & `dbdreader-0.4.9/examples/read_multiple_dbd_files.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/examples/read_single_dbd_file.py` & `dbdreader-0.4.9/examples/read_single_dbd_file.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/extension/dbdreader.c` & `dbdreader-0.4.9/extension/dbdreader.c`

 * *Files 4% similar despite different names*

```diff
@@ -254,15 +254,15 @@
 	  */
 	  read_result[i]=FILLVALUE;
 	}
       }
       
       if (!writing_first_line){
 	for(i=0; i<nv; i++){
-	  if ((offsets[i]>=min_offset_value) && (i!=nti) && isfinite(read_result[i])){
+	  if ((offsets[i]>=min_offset_value) && (i!=nti)){
 	    j=i-(int)(i>nti);
 	    /* add read_result to result */
 	    add_to_array(read_result[nti],
 			 read_result[i],
 			 result[j],ndata[j]);
 	    ndata[j]+=1;
 	  }
@@ -319,14 +319,23 @@
       if (field == UPDATED) {
 	idx=contains(variable_index,vi,nvt);
 	if (idx!=-1){
 	  /* the update value is one of the wanted variables 
 	     so record its position */
 	  offsets[idx]=*chunksize;
 	  variable_counter+=1;
+	  /* in case we ask for the time parameter explicitly, then we need to read this variable twice,
+             once as the time variable (first vector to return) and then as the variable itself (second vector
+             to return). Then the index is repeated in vi[]. The second entry gets an offset == - 2, so it will 
+	     not be read. To fix this, we can copy the offset if a duplicate value in vi is encountered.
+	  */
+	  if ( vi[variable_counter-1] == vi[variable_counter] ) {
+	    offsets[idx+1] = offsets[idx];
+	    variable_counter+=1;
+	  }
 	}
 	*chunksize+=FileInfo.byteSizes[variable_index];
       }
       else if (field==SAME) {
 	idx=contains(variable_index,vi,nvt);
 	if (idx!=-1){
 	  /* this variable is asked for but has an old value.
```

### Comparing `dbdreader-0.4.8/extension/include/dbdreader.h` & `dbdreader-0.4.9/extension/include/dbdreader.h`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/extension/py_dbdreader.c` & `dbdreader-0.4.9/extension/py_dbdreader.c`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/setup.py` & `dbdreader-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/tests/dbd_test.py` & `dbdreader-0.4.9/tests/dbd_test.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/tests/dbd_test_2.py` & `dbdreader-0.4.9/tests/dbd_test_2.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.4.8/tests/dbdreader_test.py` & `dbdreader-0.4.9/tests/dbdreader_test.py`

 * *Files identical despite different names*

