# Comparing `tmp/ixcom-1.3.3.tar.gz` & `tmp/ixcom-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixcom-1.3.3.tar", last modified: Tue May  2 09:29:44 2023, max compression
+gzip compressed data, was "ixcom-1.3.4.tar", last modified: Tue May  2 09:50:11 2023, max compression
```

## Comparing `ixcom-1.3.3.tar` & `ixcom-1.3.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:29:44.683617 ixcom-1.3.3/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1069 2023-05-02 09:26:55.000000 ixcom-1.3.3/LICENSE
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       22 2023-05-02 09:26:55.000000 ixcom-1.3.3/MANIFEST.in
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-05-02 09:29:44.683617 ixcom-1.3.3/PKG-INFO
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      584 2023-05-02 09:26:55.000000 ixcom-1.3.3/README.md
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:29:44.679617 ixcom-1.3.3/ixcom/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      105 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/__init__.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     9498 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/cmdline.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1462 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/commands.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2780 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/crc16.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      304 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/data.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      401 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/exceptions.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8142 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/grep.py
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:29:44.679617 ixcom-1.3.3/ixcom/json-files/
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:29:44.683617 ixcom-1.3.3/ixcom/json-files/messages/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2982 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/json-files/messages/0x03_inssol.json
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:29:44.683617 ixcom-1.3.3/ixcom/json-files/parameters/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     4978 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/json-files/parameters/0731_parekf_startupv2.json
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8082 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/json-files/parameters/0760_parekf_imuconfig2.json
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37317 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/messages.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37288 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/parameters.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    71125 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/parser.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      273 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/plugin_messages.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    42576 2023-05-02 09:26:55.000000 ixcom-1.3.3/ixcom/protocol.py
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:29:44.683617 ixcom-1.3.3/ixcom.egg-info/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-05-02 09:29:44.000000 ixcom-1.3.3/ixcom.egg-info/PKG-INFO
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      581 2023-05-02 09:29:44.000000 ixcom-1.3.3/ixcom.egg-info/SOURCES.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        1 2023-05-02 09:29:44.000000 ixcom-1.3.3/ixcom.egg-info/dependency_links.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      189 2023-05-02 09:29:44.000000 ixcom-1.3.3/ixcom.egg-info/entry_points.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       33 2023-05-02 09:29:44.000000 ixcom-1.3.3/ixcom.egg-info/requires.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        6 2023-05-02 09:29:44.000000 ixcom-1.3.3/ixcom.egg-info/top_level.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       38 2023-05-02 09:29:44.683617 ixcom-1.3.3/setup.cfg
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1890 2023-05-02 09:26:55.000000 ixcom-1.3.3/setup.py
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:50:11.082598 ixcom-1.3.4/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1069 2023-05-02 09:48:14.000000 ixcom-1.3.4/LICENSE
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       22 2023-05-02 09:48:14.000000 ixcom-1.3.4/MANIFEST.in
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-05-02 09:50:11.082598 ixcom-1.3.4/PKG-INFO
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      584 2023-05-02 09:48:14.000000 ixcom-1.3.4/README.md
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:50:11.078598 ixcom-1.3.4/ixcom/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      105 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/__init__.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     9498 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/cmdline.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1462 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/commands.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2780 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/crc16.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      304 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/data.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      401 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/exceptions.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8142 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/grep.py
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:50:11.078598 ixcom-1.3.4/ixcom/json-files/
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:50:11.078598 ixcom-1.3.4/ixcom/json-files/messages/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2982 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/json-files/messages/0x03_inssol.json
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:50:11.078598 ixcom-1.3.4/ixcom/json-files/parameters/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     4978 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/json-files/parameters/0731_parekf_startupv2.json
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8082 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/json-files/parameters/0760_parekf_imuconfig2.json
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37317 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/messages.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37288 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/parameters.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    71125 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/parser.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      273 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/plugin_messages.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    42576 2023-05-02 09:48:14.000000 ixcom-1.3.4/ixcom/protocol.py
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:50:11.078598 ixcom-1.3.4/ixcom.egg-info/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-05-02 09:50:11.000000 ixcom-1.3.4/ixcom.egg-info/PKG-INFO
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      581 2023-05-02 09:50:11.000000 ixcom-1.3.4/ixcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        1 2023-05-02 09:50:11.000000 ixcom-1.3.4/ixcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      189 2023-05-02 09:50:11.000000 ixcom-1.3.4/ixcom.egg-info/entry_points.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       33 2023-05-02 09:50:11.000000 ixcom-1.3.4/ixcom.egg-info/requires.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        6 2023-05-02 09:50:11.000000 ixcom-1.3.4/ixcom.egg-info/top_level.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       38 2023-05-02 09:50:11.082598 ixcom-1.3.4/setup.cfg
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1973 2023-05-02 09:48:14.000000 ixcom-1.3.4/setup.py
```

### Comparing `ixcom-1.3.3/LICENSE` & `ixcom-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/PKG-INFO` & `ixcom-1.3.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixcom
-Version: 1.3.3
+Version: 1.3.4
 Summary: Library for communicating with xcom devices over network
 Home-page: http://www.imar-navigation.de
 Author: iMAR Navigation GmbH
 Author-email: support@imar-navigation.de
 License: UNKNOWN
 Project-URL: Documentation, https://ixcom.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/imar-navigation/ixcom-python
```

### Comparing `ixcom-1.3.3/README.md` & `ixcom-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/ixcom/cmdline.py` & `ixcom-1.3.4/ixcom/cmdline.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/ixcom/commands.py` & `ixcom-1.3.4/ixcom/commands.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/ixcom/crc16.py` & `ixcom-1.3.4/ixcom/crc16.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/ixcom/grep.py` & `ixcom-1.3.4/ixcom/grep.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/ixcom/json-files/messages/0x03_inssol.json` & `ixcom-1.3.4/ixcom/json-files/messages/0x03_inssol.json`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/ixcom/json-files/parameters/0731_parekf_startupv2.json` & `ixcom-1.3.4/ixcom/json-files/parameters/0731_parekf_startupv2.json`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/ixcom/json-files/parameters/0760_parekf_imuconfig2.json` & `ixcom-1.3.4/ixcom/json-files/parameters/0760_parekf_imuconfig2.json`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/ixcom/messages.py` & `ixcom-1.3.4/ixcom/messages.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/ixcom/parameters.py` & `ixcom-1.3.4/ixcom/parameters.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/ixcom/parser.py` & `ixcom-1.3.4/ixcom/parser.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/ixcom/protocol.py` & `ixcom-1.3.4/ixcom/protocol.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/ixcom.egg-info/PKG-INFO` & `ixcom-1.3.4/ixcom.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixcom
-Version: 1.3.3
+Version: 1.3.4
 Summary: Library for communicating with xcom devices over network
 Home-page: http://www.imar-navigation.de
 Author: iMAR Navigation GmbH
 Author-email: support@imar-navigation.de
 License: UNKNOWN
 Project-URL: Documentation, https://ixcom.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/imar-navigation/ixcom-python
```

### Comparing `ixcom-1.3.3/ixcom.egg-info/SOURCES.txt` & `ixcom-1.3.4/ixcom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.3/setup.py` & `ixcom-1.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 
 if __name__ == '__main__':
 
     readmePath = os.path.join(os.path.dirname(__file__), 'README.md')
     long_description = open(readmePath, "rt").read()
 
     setup(name='ixcom',
-          version='1.3.3',
+          version='1.3.4',
           description='Library for communicating with xcom devices over network',
           author='iMAR Navigation GmbH',
           author_email='support@imar-navigation.de',
           url='http://www.imar-navigation.de',
           keywords=['XCOM', 'Inertial navigation', 'INS', 'iMAR', 'iNAT', 'GNSS', 'GPS', 'AHRS'],
           packages=['ixcom'],
+          package_data={'': ['ixcom/messages/*.json', 'ixcom/parameters/*.json']},
           entry_points={
             'console_scripts': [
                         'configdump2txt = ixcom.cmdline:configdump2txt',
                         'monitor2xcom = ixcom.cmdline:monitor2xcom',
                         'xcom_lookup = ixcom.cmdline:xcom_lookup',
                         'split_config = ixcom.cmdline:split_config',
                                 ],
```

