# Comparing `tmp/ruamel.yaml.string-0.1.0.tar.gz` & `tmp/ruamel.yaml.string-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruamel.yaml.string-0.1.0.tar", last modified: Wed Dec  8 07:38:31 2021, max compression
+gzip compressed data, was "ruamel.yaml.string-0.1.1.tar", last modified: Tue May  2 05:35:55 2023, max compression
```

## Comparing `ruamel.yaml.string-0.1.0.tar` & `ruamel.yaml.string-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,15 @@
-drwxr-xr-x   0 anthon    (1000) anthon    (1000)        0 2021-12-08 07:38:31.500748 ruamel.yaml.string-0.1.0/
-drwxr-xr-x   0 anthon    (1000) anthon    (1000)        0 2021-12-08 07:38:31.500748 ruamel.yaml.string-0.1.0/.ruamel/
--rw-r--r--   0 anthon    (1000) anthon    (1000)       63 2021-12-08 07:38:31.000000 ruamel.yaml.string-0.1.0/.ruamel/__init__.py
-drwxr-xr-x   0 anthon    (1000) anthon    (1000)        0 2021-12-08 07:38:31.500748 ruamel.yaml.string-0.1.0/.ruamel/yaml/
--rw-r--r--   0 anthon    (1000) anthon    (1000)       63 2021-12-08 07:38:31.000000 ruamel.yaml.string-0.1.0/.ruamel/yaml/__init__.py
--rw-r--r--   0 anthon    (1000) anthon    (1000)     1116 2021-12-08 07:38:30.000000 ruamel.yaml.string-0.1.0/LICENSE
--rw-r--r--   0 anthon    (1000) anthon    (1000)     2296 2021-12-08 07:38:31.500748 ruamel.yaml.string-0.1.0/PKG-INFO
--rw-r--r--   0 anthon    (1000) anthon    (1000)     1632 2021-12-08 07:38:30.000000 ruamel.yaml.string-0.1.0/README.rst
--rw-r--r--   0 anthon    (1000) anthon    (1000)      631 2021-12-08 06:57:10.000000 ruamel.yaml.string-0.1.0/__init__.py
--rw-r--r--   0 anthon    (1000) anthon    (1000)      488 2021-12-08 07:24:45.000000 ruamel.yaml.string-0.1.0/__plug_in__.py
-drwxr-xr-x   0 anthon    (1000) anthon    (1000)        0 2021-12-08 07:38:31.500748 ruamel.yaml.string-0.1.0/ruamel.yaml.string.egg-info/
--rw-r--r--   0 anthon    (1000) anthon    (1000)     2296 2021-12-08 07:38:31.000000 ruamel.yaml.string-0.1.0/ruamel.yaml.string.egg-info/PKG-INFO
--rw-r--r--   0 anthon    (1000) anthon    (1000)      373 2021-12-08 07:38:31.000000 ruamel.yaml.string-0.1.0/ruamel.yaml.string.egg-info/SOURCES.txt
--rw-r--r--   0 anthon    (1000) anthon    (1000)        1 2021-12-08 07:38:31.000000 ruamel.yaml.string-0.1.0/ruamel.yaml.string.egg-info/dependency_links.txt
--rw-r--r--   0 anthon    (1000) anthon    (1000)       19 2021-12-08 07:38:31.000000 ruamel.yaml.string-0.1.0/ruamel.yaml.string.egg-info/namespace_packages.txt
--rw-r--r--   0 anthon    (1000) anthon    (1000)       21 2021-12-08 07:38:31.000000 ruamel.yaml.string-0.1.0/ruamel.yaml.string.egg-info/requires.txt
--rw-r--r--   0 anthon    (1000) anthon    (1000)        7 2021-12-08 07:38:31.000000 ruamel.yaml.string-0.1.0/ruamel.yaml.string.egg-info/top_level.txt
--rw-r--r--   0 anthon    (1000) anthon    (1000)       38 2021-12-08 07:38:31.500748 ruamel.yaml.string-0.1.0/setup.cfg
--rw-rw-r--   0 anthon    (1000) anthon    (1000)    35813 2021-12-08 07:38:30.000000 ruamel.yaml.string-0.1.0/setup.py
+drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-05-02 05:35:55.532289 ruamel.yaml.string-0.1.1/
+-rw-r--r--   0 anthon    (1000) users      (500)     1121 2023-05-02 05:35:55.000000 ruamel.yaml.string-0.1.1/LICENSE
+-rw-r--r--   0 anthon    (1000) users      (500)     2400 2023-05-02 05:35:55.532150 ruamel.yaml.string-0.1.1/PKG-INFO
+-rw-r--r--   0 anthon    (1000) users      (500)     1756 2023-05-02 05:35:55.000000 ruamel.yaml.string-0.1.1/README.rst
+-rw-r--r--   0 anthon    (1000) users      (500)      656 2023-05-02 05:34:58.000000 ruamel.yaml.string-0.1.1/__init__.py
+-rw-r--r--   0 anthon    (1000) users      (500)      601 2022-03-19 08:14:42.000000 ruamel.yaml.string-0.1.1/__plug_in__.py
+drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-05-02 05:35:55.531946 ruamel.yaml.string-0.1.1/ruamel.yaml.string.egg-info/
+-rw-r--r--   0 anthon    (1000) users      (500)     2400 2023-05-02 05:35:55.000000 ruamel.yaml.string-0.1.1/ruamel.yaml.string.egg-info/PKG-INFO
+-rw-r--r--   0 anthon    (1000) users      (500)      318 2023-05-02 05:35:55.000000 ruamel.yaml.string-0.1.1/ruamel.yaml.string.egg-info/SOURCES.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        1 2023-05-02 05:35:55.000000 ruamel.yaml.string-0.1.1/ruamel.yaml.string.egg-info/dependency_links.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        1 2023-05-02 05:35:55.000000 ruamel.yaml.string-0.1.1/ruamel.yaml.string.egg-info/not-zip-safe
+-rw-r--r--   0 anthon    (1000) users      (500)       21 2023-05-02 05:35:55.000000 ruamel.yaml.string-0.1.1/ruamel.yaml.string.egg-info/requires.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        7 2023-05-02 05:35:55.000000 ruamel.yaml.string-0.1.1/ruamel.yaml.string.egg-info/top_level.txt
+-rw-r--r--   0 anthon    (1000) users      (500)       38 2023-05-02 05:35:55.532324 ruamel.yaml.string-0.1.1/setup.cfg
+-rw-rw-r--   0 anthon    (1000) users      (500)    33421 2023-05-02 05:35:55.000000 ruamel.yaml.string-0.1.1/setup.py
```

### Comparing `ruamel.yaml.string-0.1.0/LICENSE` & `ruamel.yaml.string-0.1.1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
  The MIT License (MIT)
 
- Copyright (c) 2021 Anthon van der Neut, Ruamel bvba
+ Copyright (c) 2021-2023 Anthon van der Neut, Ruamel bvba
 
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `ruamel.yaml.string-0.1.0/PKG-INFO` & `ruamel.yaml.string-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: ruamel.yaml.string
-Version: 0.1.0
+Version: 0.1.1
 Summary: add dump_to_string/dumps method that returns YAML document as string
 Home-page: https://sourceforge.net/p/ruamel-yaml-string/code/ci/default/tree
 Author: Anthon van der Neut
 Author-email: a.van.der.neut@ruamel.eu
 License: MIT
 Keywords: yaml 1.2 dump python string
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 ruamel.yaml.string
 ==================
 
+:version:       0.1.1
+:updated:       2023-05-02
+
 This plug-in adds a method ``dump_to_string`` (and its equivalent ``dumps``)
 to the ``ruamel.yaml.YAML`` instance that returns the document as
 a Python ``string``.
 
 Installation
 ============
 
@@ -34,15 +36,15 @@
 
 This module is dependent on ``ruamel.yaml``, so you do not have to explicitly
 make your module depending on both.
 
 Usage
 =====
 
-::
+.. code:: python
 
   import ruamel.yaml
 
   yaml = ruamel.yaml.YAML(typ=['rt', 'string'])
   data  = dict(abc=42, help=['on', 'its', 'way'])
   print('retval', yaml.dump_to_string(data))
   print('>>>> done')
@@ -53,35 +55,36 @@
   help:
   - on
   - its
   - way
   >>>> done
 
 
-Please note that there is no final newline added to the bytes
-array returned, and that the ``>>>> done`` is on the next line is caused by
+Please note that there is no final newline added to the string
+that is returned. That the ``>>>> done`` is on the next line is caused by
 the `print()` function adding a newline by default. (This is different
 from using PyYAML's `dump`, as e.g. the output of various ``print dump(data)`` 
 examples in the documentation (2021) fail to clearly show the double newline at the
 end of the examples output. It is similar to `json.dumps(data, indent=2)` that returns
 a string without final newline.)
 
 Alternatively the
 first call to ``print`` could be::
 
-  print('retval', yaml.dump_to_bytes(data, add_final_eol=True).decode('utf-8'), end='')
+  print('retval', yaml.dump_to_string(data, add_final_eol=True), end='')
 
 with the same effect.
 
-`.dump_to_bytes()` can be shortened to `.dumpb()`
+`.dump_to_string()` can be shortened to `.dumps()`
 
 *Directly writing to ``sys.stdout`` using ``yaml.dump(data, sys.stdout)`` is 
 much more efficient than ``print``-ing the result of ``yaml.dumps(data)``*
 
 
 ChangeLog
 =========
 
-NEXT:
-  - initial plug-in version
-
+0.1.1 (2023-05-02):
+  - typing added and readme corrections
 
+0.1.0 (2022-03-17):
+  - initial plug-in version
```

### Comparing `ruamel.yaml.string-0.1.0/README.rst` & `ruamel.yaml.string-0.1.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 
 ruamel.yaml.string
 ==================
 
+:version:       0.1.1
+:updated:       2023-05-02
+
 This plug-in adds a method ``dump_to_string`` (and its equivalent ``dumps``)
 to the ``ruamel.yaml.YAML`` instance that returns the document as
 a Python ``string``.
 
 Installation
 ============
 
@@ -15,15 +18,15 @@
 
 This module is dependent on ``ruamel.yaml``, so you do not have to explicitly
 make your module depending on both.
 
 Usage
 =====
 
-::
+.. code:: python
 
   import ruamel.yaml
 
   yaml = ruamel.yaml.YAML(typ=['rt', 'string'])
   data  = dict(abc=42, help=['on', 'its', 'way'])
   print('retval', yaml.dump_to_string(data))
   print('>>>> done')
@@ -34,33 +37,36 @@
   help:
   - on
   - its
   - way
   >>>> done
 
 
-Please note that there is no final newline added to the bytes
-array returned, and that the ``>>>> done`` is on the next line is caused by
+Please note that there is no final newline added to the string
+that is returned. That the ``>>>> done`` is on the next line is caused by
 the `print()` function adding a newline by default. (This is different
 from using PyYAML's `dump`, as e.g. the output of various ``print dump(data)`` 
 examples in the documentation (2021) fail to clearly show the double newline at the
 end of the examples output. It is similar to `json.dumps(data, indent=2)` that returns
 a string without final newline.)
 
 Alternatively the
 first call to ``print`` could be::
 
-  print('retval', yaml.dump_to_bytes(data, add_final_eol=True).decode('utf-8'), end='')
+  print('retval', yaml.dump_to_string(data, add_final_eol=True), end='')
 
 with the same effect.
 
-`.dump_to_bytes()` can be shortened to `.dumpb()`
+`.dump_to_string()` can be shortened to `.dumps()`
 
 *Directly writing to ``sys.stdout`` using ``yaml.dump(data, sys.stdout)`` is 
 much more efficient than ``print``-ing the result of ``yaml.dumps(data)``*
 
 
 ChangeLog
 =========
 
-NEXT:
+0.1.1 (2023-05-02):
+  - typing added and readme corrections
+
+0.1.0 (2022-03-17):
   - initial plug-in version
```

### Comparing `ruamel.yaml.string-0.1.0/__init__.py` & `ruamel.yaml.string-0.1.1/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # coding: utf-8
 
 _package_data = dict(
     full_package_name='ruamel.yaml.string',
-    version_info=(0, 1, 0),
-    __version__='0.1.0',
+    version_info=(0, 1, 1),
+    __version__='0.1.1',
+    version_timestamp='2023-05-02 07:34:58',
     author='Anthon van der Neut',
     author_email='a.van.der.neut@ruamel.eu',
     description='add dump_to_string/dumps method that returns YAML document as string',
     entry_points=None,
     license='MIT',
     since=2021,
-    universal=True,
     keywords='yaml 1.2 dump python string',
     nested=True,
     install_requires=['ruamel.yaml>=0.17.17'],
     python_requires='>=3',
     tox=dict(env='3'),
 )
```

### Comparing `ruamel.yaml.string-0.1.0/ruamel.yaml.string.egg-info/PKG-INFO` & `ruamel.yaml.string-0.1.1/ruamel.yaml.string.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: ruamel.yaml.string
-Version: 0.1.0
+Version: 0.1.1
 Summary: add dump_to_string/dumps method that returns YAML document as string
 Home-page: https://sourceforge.net/p/ruamel-yaml-string/code/ci/default/tree
 Author: Anthon van der Neut
 Author-email: a.van.der.neut@ruamel.eu
 License: MIT
 Keywords: yaml 1.2 dump python string
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 ruamel.yaml.string
 ==================
 
+:version:       0.1.1
+:updated:       2023-05-02
+
 This plug-in adds a method ``dump_to_string`` (and its equivalent ``dumps``)
 to the ``ruamel.yaml.YAML`` instance that returns the document as
 a Python ``string``.
 
 Installation
 ============
 
@@ -34,15 +36,15 @@
 
 This module is dependent on ``ruamel.yaml``, so you do not have to explicitly
 make your module depending on both.
 
 Usage
 =====
 
-::
+.. code:: python
 
   import ruamel.yaml
 
   yaml = ruamel.yaml.YAML(typ=['rt', 'string'])
   data  = dict(abc=42, help=['on', 'its', 'way'])
   print('retval', yaml.dump_to_string(data))
   print('>>>> done')
@@ -53,35 +55,36 @@
   help:
   - on
   - its
   - way
   >>>> done
 
 
-Please note that there is no final newline added to the bytes
-array returned, and that the ``>>>> done`` is on the next line is caused by
+Please note that there is no final newline added to the string
+that is returned. That the ``>>>> done`` is on the next line is caused by
 the `print()` function adding a newline by default. (This is different
 from using PyYAML's `dump`, as e.g. the output of various ``print dump(data)`` 
 examples in the documentation (2021) fail to clearly show the double newline at the
 end of the examples output. It is similar to `json.dumps(data, indent=2)` that returns
 a string without final newline.)
 
 Alternatively the
 first call to ``print`` could be::
 
-  print('retval', yaml.dump_to_bytes(data, add_final_eol=True).decode('utf-8'), end='')
+  print('retval', yaml.dump_to_string(data, add_final_eol=True), end='')
 
 with the same effect.
 
-`.dump_to_bytes()` can be shortened to `.dumpb()`
+`.dump_to_string()` can be shortened to `.dumps()`
 
 *Directly writing to ``sys.stdout`` using ``yaml.dump(data, sys.stdout)`` is 
 much more efficient than ``print``-ing the result of ``yaml.dumps(data)``*
 
 
 ChangeLog
 =========
 
-NEXT:
-  - initial plug-in version
-
+0.1.1 (2023-05-02):
+  - typing added and readme corrections
 
+0.1.0 (2022-03-17):
+  - initial plug-in version
```

### Comparing `ruamel.yaml.string-0.1.0/setup.py` & `ruamel.yaml.string-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 # # header
 # coding: utf-8
-# dd: 20200903
-
-from __future__ import print_function, absolute_import, division, unicode_literals
+# dd: 20230418
 
 # # __init__.py parser
 
 import sys
 import os
 import datetime
-import traceback
+from textwrap import dedent
 
 sys.path = [path for path in sys.path if path not in [os.getcwd(), ""]]
 import platform  # NOQA
 from _ast import *  # NOQA
 from ast import parse  # NOQA
 
 from setuptools import setup, Extension, Distribution  # NOQA
 from setuptools.command import install_lib  # NOQA
 from setuptools.command.sdist import sdist as _sdist  # NOQA
 
-try:
-    from setuptools.namespaces import Installer as NameSpaceInstaller # NOQA
-except ImportError:
-    msg = ('You should use the latest setuptools. The namespaces.py file that this setup.py'
-           ' uses was added in setuptools 28.7.0 (Oct 2016)')
-    print(msg)
-    sys.exit()
+# try:
+#     from setuptools.namespaces import Installer as NameSpaceInstaller # NOQA
+# except ImportError:
+#     msg = ('You should use the latest setuptools. The namespaces.py file that this setup.py'
+#            ' uses was added in setuptools 28.7.0 (Oct 2016)')
+#     print(msg)
+#     sys.exit()
 
 if __name__ != '__main__':
     raise NotImplementedError('should never include setup.py')
 
 # # definitions
 
 full_package_name = None
@@ -274,16 +272,15 @@
                 alt_files.append(x)
         return alt_files
 
 
 class MySdist(_sdist):
     def initialize_options(self):
         _sdist.initialize_options(self)
-        # see pep 527, new uploads should be tar.gz or .zip
-        # fmt = getattr(self, 'tarfmt',  None)
+        # failed expiriment, see pep 527, new uploads should be tar.gz or .zip
         # because of unicode_literals
         # self.formats = fmt if fmt else [b'bztar'] if sys.version_info < (3, ) else ['bztar']
         dist_base = os.environ.get('PYDISTBASE')
         fpn = getattr(getattr(self, 'nsp', self), 'full_package_name', None)
         if fpn and dist_base:
             print('setting  distdir {}/{}'.format(dist_base, fpn))
             self.dist_dir = os.path.join(dist_base, fpn)
@@ -313,16 +310,16 @@
     def __init__(self, pkg_data):
         assert isinstance(pkg_data, dict)
         self._pkg_data = pkg_data
         self.full_package_name = self.pn(self._pkg_data['full_package_name'])
         self._split = None
         self.depth = self.full_package_name.count('.')
         self.nested = self._pkg_data.get('nested', False)
-        if self.nested:
-            NameSpaceInstaller.install_namespaces = lambda x: None
+        # if self.nested:
+        #     NameSpaceInstaller.install_namespaces = lambda x: None
         self.command = None
         self.python_version()
         self._pkg = [None, None]  # required and pre-installable packages
         if sys.argv[0] == 'setup.py' and sys.argv[1] == 'install':
             debug('calling setup.py', sys.argv)
             if '-h' in sys.argv:
                 pass
@@ -383,17 +380,14 @@
         if skip:
             # this interferes with output checking
             # print('skipping sub-packages:', ', '.join(skip))
             pass
         return self._split
 
     @property
-    def namespace_packages(self):
-        return self.split[: self.depth]
-
     def namespace_directories(self, depth=None):
         """return list of directories where the namespace should be created /
         can be found
         """
         res = []
         for index, d in enumerate(self.split[:depth]):
             # toplevel gets a dot
@@ -406,31 +400,19 @@
     def package_dir(self):
         d = {
             # don't specify empty dir, clashes with package_data spec
             self.full_package_name: '.'
         }
         if 'extra_packages' in self._pkg_data:
             return d
-        if len(self.split) > 1:  # only if package namespace
-            d[self.split[0]] = self.namespace_directories(1)[0]
+        # if len(self.split) > 1:  # only if package namespace
+        #     d[self.split[0]] = self.namespace_directories(1)[0]
+        # print('d', d, os.getcwd())
         return d
 
-    def create_dirs(self):
-        """create the directories necessary for namespace packaging"""
-        directories = self.namespace_directories(self.depth)
-        if not directories:
-            return
-        if not os.path.exists(directories[0]):
-            for d in directories:
-                os.mkdir(d)
-                with open(os.path.join(d, '__init__.py'), 'w') as fp:
-                    fp.write(
-                        'import pkg_resources\n' 'pkg_resources.declare_namespace(__name__)\n'
-                    )
-
     def python_version(self):
         supported = self._pkg_data.get('supported')
         if supported is None:
             return
         if len(supported) == 1:
             minimum = supported[0]
         else:
@@ -714,15 +696,16 @@
                     pd[str(k)] = pd.pop(k)
             # for k in pd:
             #     pd[k] = [e.encode('utf-8') for e in pd[k]]  # de-unicode
         return pd
 
     @property
     def packages(self):
-        s = self.split
+        # s = self.split
+        s = [self._pkg_data['full_package_name']]
         # fixed this in package_data, the keys there must be non-unicode for py27
         # if sys.version_info < (3, 0):
         #     s = [x.encode('utf-8') for x in self.split]
         return s + self._pkg_data.get('extra_packages', [])
 
     @property
     def python_requires(self):
@@ -750,99 +733,29 @@
         try:
             plat = sys.argv.index('--plat-name')
             if 'win' in sys.argv[plat + 1]:
                 return None
         except ValueError:
             pass
         self._ext_modules = []
-        no_test_compile = False
+        no_test_compile = True
         if '--restructuredtext' in sys.argv:
             no_test_compile = True
         elif 'sdist' in sys.argv:
             no_test_compile = True
         if no_test_compile:
             for target in self._pkg_data.get('ext_modules', []):
                 ext = Extension(
                     self.pn(target['name']),
                     sources=[self.pn(x) for x in target['src']],
                     libraries=[self.pn(x) for x in target.get('lib')],
                 )
                 self._ext_modules.append(ext)
             return self._ext_modules
-
-        print('sys.argv', sys.argv)
-        import tempfile
-        import shutil
-        from textwrap import dedent
-
-        import distutils.sysconfig
-        import distutils.ccompiler
-        from distutils.errors import CompileError, LinkError
-
-        for target in self._pkg_data.get('ext_modules', []):  # list of dicts
-            ext = Extension(
-                self.pn(target['name']),
-                sources=[self.pn(x) for x in target['src']],
-                libraries=[self.pn(x) for x in target.get('lib')],
-            )
-            # debug('test1 in target', 'test' in target, target)
-            if 'test' not in target:  # no test, just hope it works
-                self._ext_modules.append(ext)
-                continue
-            if sys.version_info[:2] == (3, 4) and platform.system() == 'Windows':
-                # this is giving problems on appveyor, so skip
-                if 'FORCE_C_BUILD_TEST' not in os.environ:
-                    self._ext_modules.append(ext)
-                    continue
-            # write a temporary .c file to compile
-            c_code = dedent(target['test'])
-            try:
-                tmp_dir = tempfile.mkdtemp(prefix='tmp_ruamel_')
-                bin_file_name = 'test' + self.pn(target['name'])
-                file_name = os.path.join(tmp_dir, bin_file_name + '.c')
-                print('test compiling', file_name, '->', bin_file_name, end=' ')
-                with open(file_name, 'w') as fp:  # write source
-                    fp.write(c_code)
-                # and try to compile it
-                compiler = distutils.ccompiler.new_compiler()
-                assert isinstance(compiler, distutils.ccompiler.CCompiler)
-                # do any platform specific initialisations
-                distutils.sysconfig.customize_compiler(compiler)
-                # make sure you can reach header files because compile does change dir
-                compiler.add_include_dir(os.getcwd())
-                if sys.version_info < (3,):
-                    tmp_dir = tmp_dir.encode('utf-8')
-                # used to be a different directory, not necessary
-                compile_out_dir = tmp_dir
-                try:
-                    compiler.link_executable(
-                        compiler.compile([file_name], output_dir=compile_out_dir),
-                        bin_file_name,
-                        output_dir=tmp_dir,
-                        libraries=ext.libraries,
-                    )
-                except CompileError:
-                    debug('compile error:', file_name)
-                    print('compile error:', file_name)
-                    raise
-                except LinkError:
-                    debug('link error', file_name)
-                    print('link error', file_name)
-                    raise
-                print('OK')
-                self._ext_modules.append(ext)
-            except Exception as e:  # NOQA
-                debug('Exception:', e)
-                print('Exception:', e)
-                sys.exit(1)
-                if sys.version_info[:2] == (3, 4) and platform.system() == 'Windows':
-                    traceback.print_exc()
-            finally:
-                shutil.rmtree(tmp_dir)
-        return self._ext_modules
+        # this used to use distutils
 
     @property
     def test_suite(self):
         return self._pkg_data.get('test_suite')
 
     def wheel(self, kw, setup):
         """temporary add setup.cfg if creating a wheel to include LICENSE file
@@ -850,56 +763,98 @@
         """
         if 'bdist_wheel' not in sys.argv:
             return False
         file_name = 'setup.cfg'
         if os.path.exists(file_name):  # add it if not in there?
             return False
         with open(file_name, 'w') as fp:
-            if os.path.exists('LICENSE'):
-                fp.write('[metadata]\nlicense_file = LICENSE\n')
-            else:
-                print('\n\n>>>>>> LICENSE file not found <<<<<\n\n')
             if self._pkg_data.get('universal'):
                 fp.write('[bdist_wheel]\nuniversal = 1\n')
         try:
             setup(**kw)
         except Exception:
             raise
         finally:
             os.remove(file_name)
         return True
 
 
-# # call setup
+class TmpFiles:
+    def __init__(self, pkg_data, py_project=True, keep=False):
+        self._rm_after = []
+        self._pkg_data = pkg_data
+        self._py_project = py_project
+        self._bdist_wheel = 'bdist_wheel' in sys.argv
+        self._keep = keep
+
+    def __enter__(self):
+        self.bdist_wheel()
+        return
+        self.py_project()
+
+    def bdist_wheel(self):
+        """pyproject doesn't allow for universal, so use setup.cfg if necessary
+        """
+        file_name = 'setup.cfg'
+        if not self._bdist_wheel or os.path.exists(file_name):
+            return
+        if self._pkg_data.get('universal'):
+            self._rm_after.append(file_name)
+            with open(file_name, 'w') as fp:
+                fp.write('[bdist_wheel]\nuniversal = 1\n')
+
+    def py_project(self):
+        """
+        to prevent pip from complaining, or is it too late to create it from setup.py
+        """
+        file_name = 'pyproject.toml'
+        if not self._py_project or os.path.exists(file_name):
+            return
+        self._rm_after.append(file_name)
+        with open(file_name, 'w') as fp:
+            fp.write(dedent("""\
+            [build-system]
+            requires = ["setuptools", "wheel"]
+            # test
+            build-backend = "setuptools.build_meta"
+            """))
+
+    def __exit__(self, typ, value, traceback):
+        if self._keep:
+            return
+        for p in self._rm_after:
+            if not os.path.exists(p):
+                print('file {} already removed'.format(p))
+            else:
+                os.unlink(p)
+
+
+# call setup
 def main():
     dump_kw = '--dump-kw'
     if dump_kw in sys.argv:
         import wheel
-        import distutils
         import setuptools
+        import pip
 
         print('python:    ', sys.version)
+        print('pip:       ', pip.__version__)
         print('setuptools:', setuptools.__version__)
-        print('distutils: ', distutils.__version__)
         print('wheel:     ', wheel.__version__)
     nsp = NameSpacePackager(pkg_data)
     nsp.check()
-    nsp.create_dirs()
+    # nsp.create_dirs()
     MySdist.nsp = nsp
-    if pkg_data.get('tarfmt'):
-        MySdist.tarfmt = pkg_data.get('tarfmt')
-
     cmdclass = dict(install_lib=MyInstallLib, sdist=MySdist)
     if _bdist_wheel_available:
         MyBdistWheel.nsp = nsp
         cmdclass['bdist_wheel'] = MyBdistWheel
 
     kw = dict(
         name=nsp.full_package_name,
-        namespace_packages=nsp.namespace_packages,
         version=version_str,
         packages=nsp.packages,
         python_requires=nsp.python_requires,
         url=nsp.url,
         author=nsp.author,
         author_email=nsp.author_email,
         cmdclass=cmdclass,
@@ -910,52 +865,55 @@
         extras_require=nsp.extras_require,  # available since setuptools 18.0 / 2015-06
         license=nsp.license,
         classifiers=nsp.classifiers,
         keywords=nsp.keywords,
         package_data=nsp.package_data,
         ext_modules=nsp.ext_modules,
         test_suite=nsp.test_suite,
+        zip_safe=False,
     )
 
     if '--version' not in sys.argv and ('--verbose' in sys.argv or dump_kw in sys.argv):
         for k in sorted(kw):
             v = kw[k]
-            print('  "{0}": "{1}",'.format(k, v))
+            print('  "{0}": {1},'.format(k, repr(v)))
     # if '--record' in sys.argv:
     #     return
     if dump_kw in sys.argv:
         sys.argv.remove(dump_kw)
     try:
         with open('README.rst') as fp:
             kw['long_description'] = fp.read()
             kw['long_description_content_type'] = 'text/x-rst'
     except Exception:
         pass
 
-    if nsp.wheel(kw, setup):
-        return
-    for x in ['-c', 'egg_info', '--egg-base', 'pip-egg-info']:
-        if x not in sys.argv:
-            break
-    else:
-        # we're doing a tox setup install any starred package by searching up the source tree
-        # until you match your/package/name for your.package.name
-        for p in nsp.install_pre:
-            import subprocess
-
-            # search other source
-            setup_path = os.path.join(*p.split('.') + ['setup.py'])
-            try_dir = os.path.dirname(sys.executable)
-            while len(try_dir) > 1:
-                full_path_setup_py = os.path.join(try_dir, setup_path)
-                if os.path.exists(full_path_setup_py):
-                    pip = sys.executable.replace('python', 'pip')
-                    cmd = [pip, 'install', os.path.dirname(full_path_setup_py)]
-                    # with open('/var/tmp/notice', 'a') as fp:
-                    #     print('installing', cmd, file=fp)
-                    subprocess.check_output(cmd)
-                    break
-                try_dir = os.path.dirname(try_dir)
-    setup(**kw)
+    # if nsp.wheel(kw, setup):
+    #     return
+    with TmpFiles(pkg_data, keep=True):
+        for x in ['-c', 'egg_info', '--egg-base', 'pip-egg-info']:
+            if x not in sys.argv:
+                break
+        else:
+            # we're doing a tox setup install any starred package by searching up the
+            # source tree until you match your/package/name for your.package.name
+            for p in nsp.install_pre:
+                import subprocess
+
+                # search other source
+                setup_path = os.path.join(*p.split('.') + ['setup.py'])
+                try_dir = os.path.dirname(sys.executable)
+                while len(try_dir) > 1:
+                    full_path_setup_py = os.path.join(try_dir, setup_path)
+                    if os.path.exists(full_path_setup_py):
+                        pip = sys.executable.replace('python', 'pip')
+                        cmd = [pip, 'install', os.path.dirname(full_path_setup_py)]
+                        # with open('/var/tmp/notice', 'a') as fp:
+                        #     print('installing', cmd, file=fp)
+                        subprocess.check_output(cmd)
+                        break
+                    try_dir = os.path.dirname(try_dir)
+        setup(**kw)
+        print('done')
 
 
 main()
```

