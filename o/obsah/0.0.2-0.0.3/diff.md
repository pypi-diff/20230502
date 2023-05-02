# Comparing `tmp/obsah-0.0.2.tar.gz` & `tmp/obsah-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/obsah-0.0.2.tar", last modified: Fri Sep 11 10:35:11 2020, max compression
+gzip compressed data, was "obsah-0.0.3.tar", last modified: Tue May  2 07:48:40 2023, max compression
```

## Comparing `obsah-0.0.2.tar` & `obsah-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-11 10:35:11.000000 obsah-0.0.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2020-09-11 10:33:29.000000 obsah-0.0.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-09-11 10:33:29.000000 obsah-0.0.2/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1277 2020-09-11 10:35:11.000000 obsah-0.0.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-09-11 10:33:29.000000 obsah-0.0.2/requirements-docs.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      353 2020-09-11 10:33:29.000000 obsah-0.0.2/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2020-09-11 10:33:29.000000 obsah-0.0.2/.pylintrc
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-09-11 10:35:11.000000 obsah-0.0.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    18092 2020-09-11 10:33:29.000000 obsah-0.0.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2020-09-11 10:33:29.000000 obsah-0.0.2/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2020-09-11 10:33:29.000000 obsah-0.0.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-11 10:35:11.000000 obsah-0.0.2/obsah/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-11 10:35:11.000000 obsah-0.0.2/obsah/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-09-11 10:33:29.000000 obsah-0.0.2/obsah/data/.keep
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2020-09-11 10:33:29.000000 obsah-0.0.2/obsah/__main__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    12170 2020-09-11 10:33:29.000000 obsah-0.0.2/obsah/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-09-11 10:33:29.000000 obsah-0.0.2/requirements-test.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-11 10:35:11.000000 obsah-0.0.2/obsah.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1277 2020-09-11 10:35:11.000000 obsah-0.0.2/obsah.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-11 10:35:11.000000 obsah-0.0.2/obsah.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2020-09-11 10:35:11.000000 obsah-0.0.2/obsah.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-11 10:35:11.000000 obsah-0.0.2/obsah.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      378 2020-09-11 10:35:11.000000 obsah-0.0.2/obsah.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2020-09-11 10:35:11.000000 obsah-0.0.2/obsah.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-09-11 10:35:11.000000 obsah-0.0.2/obsah.egg-info/entry_points.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:48:40.906631 obsah-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 07:48:36.000000 obsah-0.0.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-02 07:48:36.000000 obsah-0.0.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-02 07:48:36.000000 obsah-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-02 07:48:36.000000 obsah-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-02 07:48:40.906631 obsah-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-02 07:48:36.000000 obsah-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:48:40.902631 obsah-0.0.3/obsah/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12403 2023-05-02 07:48:36.000000 obsah-0.0.3/obsah/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-02 07:48:36.000000 obsah-0.0.3/obsah/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:48:40.906631 obsah-0.0.3/obsah/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:48:36.000000 obsah-0.0.3/obsah/data/.keep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:48:40.902631 obsah-0.0.3/obsah.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-02 07:48:40.000000 obsah-0.0.3/obsah.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-02 07:48:40.000000 obsah-0.0.3/obsah.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:48:40.000000 obsah-0.0.3/obsah.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 07:48:40.000000 obsah-0.0.3/obsah.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:48:40.000000 obsah-0.0.3/obsah.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-02 07:48:40.000000 obsah-0.0.3/obsah.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 07:48:40.000000 obsah-0.0.3/obsah.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 07:48:36.000000 obsah-0.0.3/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-02 07:48:36.000000 obsah-0.0.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 07:48:36.000000 obsah-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 07:48:40.906631 obsah-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-02 07:48:36.000000 obsah-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `obsah-0.0.2/PKG-INFO` & `obsah-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 Metadata-Version: 2.1
 Name: obsah
-Version: 0.0.2
+Version: 0.0.3
 Summary: packaging wrapper using ansible
 Home-page: https://github.com/theforeman/obsah
 Author: The Foreman Project
 Author-email: foreman-dev@googlegroups.com
-License: UNKNOWN
-Description: # obsah - easily build CLI applications using ansible playbooks
-        
-        [![Documentation Status](https://readthedocs.org/projects/obsah/badge/?version=latest)](https://obsah.readthedocs.io/en/latest/)
-        
-        `obsah` is an Ansible wrapper that will help you to build CLI applications by writing Ansible playbooks.
-        
-        ## necessary tools
-        
-        - `python` (2 or 3)
-        - `ansible`
-        
+License: GPL-2.0-only
+Project-URL: Documentation, https://obsah.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/theforeman/obsah
 Keywords: ansible foreman packaging koji brew mock
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=2.7, <4, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
 Provides-Extra: argcomplete
+License-File: LICENSE
+
+# obsah - easily build CLI applications using ansible playbooks
+
+[![Documentation Status](https://readthedocs.org/projects/obsah/badge/?version=latest)](https://obsah.readthedocs.io/en/latest/)
+
+`obsah` is an Ansible wrapper that will help you to build CLI applications by writing Ansible playbooks.
+
+## necessary tools
+
+- `python` (2 or 3)
+- `ansible`
+
+
```

### Comparing `obsah-0.0.2/LICENSE` & `obsah-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `obsah-0.0.2/setup.py` & `obsah-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,48 +32,60 @@
         package_data.extend(files)
     os.chdir(oldcwd)
     return package_data
 
 
 setup(
     name='obsah',
-    version='0.0.2',
+    version='0.0.3',
+    license='GPL-2.0-only',
     description='packaging wrapper using ansible',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     url='https://github.com/theforeman/obsah',
     author='The Foreman Project',
     author_email='foreman-dev@googlegroups.com',
     zip_safe=False,
+    python_requires=">=2.7, <4, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*",
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
 
     keywords='ansible foreman packaging koji brew mock',
 
-    packages=find_packages(exclude=['contrib', 'docs', 'tests']),
+    packages=find_packages(exclude=['contrib', 'docs']),
 
-    install_requires=['ansible >= 2.5'],
+    install_requires=[
+        'ansible >= 2.5; python_version < "3.8"',
+        'ansible-core; python_version >= "3.8"',
+    ],
 
     extras_require={
         'argcomplete': ['argcomplete'],
     },
 
     package_data={
         'obsah': find_package_data('obsah', 'data'),
     },
 
     entry_points={
         'console_scripts': [
             'obsah=obsah:main',
         ],
     },
+
+    project_urls={
+        "Documentation": "https://obsah.readthedocs.io/en/latest/",
+        "Source": "https://github.com/theforeman/obsah",
+    },
 )
```

### Comparing `obsah-0.0.2/obsah/__init__.py` & `obsah-0.0.3/obsah/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,17 @@
         Whether this playbook takes a target argument.
 
         This is determined by a hosts: targets inside the playbook
         """
         with open(self.path) as playbook_file:
             plays = yaml.safe_load(playbook_file.read())
 
-        return any(self.application_config.target_name() in play['hosts'] for play in plays)
+        target_names = set(self.application_config.target_names())
+
+        return any(len(target_names.intersection(play.get('hosts', []))) > 0 for play in plays)
 
     @property
     def playbook_variables(self):
         """
         The playbook variables that should be exposed to the user
 
         This is extracted from the metadata.
@@ -179,14 +181,21 @@
     @staticmethod
     def target_name():
         """
         Return the name of the target in the playbook if the playbook takes a parameter.
         """
         return 'packages'
 
+    @classmethod
+    def target_names(cls):
+        """
+        Return the names of the targets in the playbook if the playbook takes parameters.
+        """
+        return [cls.target_name()]
+
     @staticmethod
     def metadata_name():
         """
         Return the name of the metadata file.
         """
         return 'metadata.obsah.yaml'
 
@@ -247,15 +256,14 @@
         from ansible.inventory.manager import InventoryManager # pylint: disable=all
         from ansible.parsing.dataloader import DataLoader # pylint: disable=all
         ansible_loader = DataLoader()
         ansible_inventory = InventoryManager(loader=ansible_loader,
                                              sources=inventory_path)
         targets = list(ansible_inventory.hosts.keys())
         targets.extend(ansible_inventory.groups.keys())
-        targets.extend(['all'])
     return targets
 
 
 def obsah_argument_parser(application_config=ApplicationConfig, playbooks=None, targets=None):
     """
     Construct an argument parser with the given actions and target choices.
     """
```

### Comparing `obsah-0.0.2/obsah.egg-info/PKG-INFO` & `obsah-0.0.3/obsah.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 Metadata-Version: 2.1
 Name: obsah
-Version: 0.0.2
+Version: 0.0.3
 Summary: packaging wrapper using ansible
 Home-page: https://github.com/theforeman/obsah
 Author: The Foreman Project
 Author-email: foreman-dev@googlegroups.com
-License: UNKNOWN
-Description: # obsah - easily build CLI applications using ansible playbooks
-        
-        [![Documentation Status](https://readthedocs.org/projects/obsah/badge/?version=latest)](https://obsah.readthedocs.io/en/latest/)
-        
-        `obsah` is an Ansible wrapper that will help you to build CLI applications by writing Ansible playbooks.
-        
-        ## necessary tools
-        
-        - `python` (2 or 3)
-        - `ansible`
-        
+License: GPL-2.0-only
+Project-URL: Documentation, https://obsah.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/theforeman/obsah
 Keywords: ansible foreman packaging koji brew mock
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=2.7, <4, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
 Provides-Extra: argcomplete
+License-File: LICENSE
+
+# obsah - easily build CLI applications using ansible playbooks
+
+[![Documentation Status](https://readthedocs.org/projects/obsah/badge/?version=latest)](https://obsah.readthedocs.io/en/latest/)
+
+`obsah` is an Ansible wrapper that will help you to build CLI applications by writing Ansible playbooks.
+
+## necessary tools
+
+- `python` (2 or 3)
+- `ansible`
+
+
```

