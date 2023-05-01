# Comparing `tmp/pure_interface-7.0.2.tar.gz` & `tmp/pure_interface-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Source\pure_interface\dist\.tmp-g_2wb4tl\pure_interface-7.0.2.tar", last modified: Mon May  1 21:19:49 2023, max compression
+gzip compressed data, was "D:\Source\pure_interface\dist\.tmp-_a_hks6u\pure_interface-7.1.0.tar", last modified: Mon May  1 21:58:03 2023, max compression
```

## Comparing `pure_interface-7.0.2.tar` & `pure_interface-7.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 21:19:49.815589 pure_interface-7.0.2/
--rw-rw-rw-   0        0        0     1070 2021-09-21 22:43:47.000000 pure_interface-7.0.2/LICENSE
--rw-rw-rw-   0        0        0    34872 2023-05-01 21:19:49.815589 pure_interface-7.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    33904 2023-04-27 23:17:43.000000 pure_interface-7.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 21:19:49.787813 pure_interface-7.0.2/pure_interface/
--rw-rw-rw-   0        0        0      617 2023-05-01 21:17:43.000000 pure_interface-7.0.2/pure_interface/__init__.py
--rw-rw-rw-   0        0        0     7884 2023-03-01 20:08:43.000000 pure_interface-7.0.2/pure_interface/adaption.py
--rw-rw-rw-   0        0        0     2167 2023-03-01 20:08:43.000000 pure_interface-7.0.2/pure_interface/data_classes.py
--rw-rw-rw-   0        0        0     8441 2023-04-27 23:17:43.000000 pure_interface-7.0.2/pure_interface/delegation.py
--rw-rw-rw-   0        0        0      372 2023-03-01 20:08:43.000000 pure_interface-7.0.2/pure_interface/errors.py
--rw-rw-rw-   0        0        0    33634 2023-05-01 21:16:47.000000 pure_interface-7.0.2/pure_interface/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-01 21:19:49.793583 pure_interface-7.0.2/pure_interface.egg-info/
--rw-rw-rw-   0        0        0    34872 2023-05-01 21:19:49.000000 pure_interface-7.0.2/pure_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      821 2023-05-01 21:19:49.000000 pure_interface-7.0.2/pure_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 21:19:49.000000 pure_interface-7.0.2/pure_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-01 21:19:49.000000 pure_interface-7.0.2/pure_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2021-09-21 22:43:47.000000 pure_interface-7.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1088 2023-05-01 21:19:49.816587 pure_interface-7.0.2/setup.cfg
--rw-rw-rw-   0        0        0       43 2021-09-21 22:43:47.000000 pure_interface-7.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 21:19:49.813588 pure_interface-7.0.2/tests/
--rw-rw-rw-   0        0        0     3843 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_adapt_args_anno.py
--rw-rw-rw-   0        0        0     2871 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_adapt_args_no_anno.py
--rw-rw-rw-   0        0        0    12205 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_adaption.py
--rw-rw-rw-   0        0        0     1022 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_dataclass_support.py
--rw-rw-rw-   0        0        0     8954 2023-05-01 21:04:02.000000 pure_interface-7.0.2/tests/test_delegate.py
--rw-rw-rw-   0        0        0     5935 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_func_sigs3.py
--rw-rw-rw-   0        0        0    11757 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_function_sigs.py
--rw-rw-rw-   0        0        0     1051 2023-05-01 21:06:52.000000 pure_interface-7.0.2/tests/test_generic_support.py
--rw-rw-rw-   0        0        0    16459 2023-05-01 21:18:53.000000 pure_interface-7.0.2/tests/test_implementation_checks.py
--rw-rw-rw-   0        0        0     2803 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_inheritance.py
--rw-rw-rw-   0        0        0     4040 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_isinstance.py
--rw-rw-rw-   0        0        0     2346 2023-03-01 20:08:43.000000 pure_interface-7.0.2/tests/test_meta_classes.py
--rw-rw-rw-   0        0        0     2877 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_module_funcs.py
--rw-rw-rw-   0        0        0     3364 2023-03-01 20:08:43.000000 pure_interface-7.0.2/tests/test_no_content_checks.py
--rw-rw-rw-   0        0        0     2071 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_tracker.py
--rw-rw-rw-   0        0        0      514 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_versions_in_sync.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:58:03.589988 pure_interface-7.1.0/
+-rw-rw-rw-   0        0        0     1070 2021-09-21 22:43:47.000000 pure_interface-7.1.0/LICENSE
+-rw-rw-rw-   0        0        0    34895 2023-05-01 21:58:03.589988 pure_interface-7.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    33927 2023-05-01 21:55:51.000000 pure_interface-7.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 21:58:03.559726 pure_interface-7.1.0/pure_interface/
+-rw-rw-rw-   0        0        0      617 2023-05-01 21:55:58.000000 pure_interface-7.1.0/pure_interface/__init__.py
+-rw-rw-rw-   0        0        0     7884 2023-03-01 20:08:43.000000 pure_interface-7.1.0/pure_interface/adaption.py
+-rw-rw-rw-   0        0        0     2167 2023-03-01 20:08:43.000000 pure_interface-7.1.0/pure_interface/data_classes.py
+-rw-rw-rw-   0        0        0     8522 2023-05-01 21:45:26.000000 pure_interface-7.1.0/pure_interface/delegation.py
+-rw-rw-rw-   0        0        0      372 2023-03-01 20:08:43.000000 pure_interface-7.1.0/pure_interface/errors.py
+-rw-rw-rw-   0        0        0    33634 2023-05-01 21:16:47.000000 pure_interface-7.1.0/pure_interface/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:58:03.564727 pure_interface-7.1.0/pure_interface.egg-info/
+-rw-rw-rw-   0        0        0    34895 2023-05-01 21:58:03.000000 pure_interface-7.1.0/pure_interface.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      821 2023-05-01 21:58:03.000000 pure_interface-7.1.0/pure_interface.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 21:58:03.000000 pure_interface-7.1.0/pure_interface.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-01 21:58:03.000000 pure_interface-7.1.0/pure_interface.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2021-09-21 22:43:47.000000 pure_interface-7.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1088 2023-05-01 21:58:03.591989 pure_interface-7.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       43 2021-09-21 22:43:47.000000 pure_interface-7.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:58:03.588989 pure_interface-7.1.0/tests/
+-rw-rw-rw-   0        0        0     3843 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_adapt_args_anno.py
+-rw-rw-rw-   0        0        0     2871 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_adapt_args_no_anno.py
+-rw-rw-rw-   0        0        0    12205 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_adaption.py
+-rw-rw-rw-   0        0        0     1022 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_dataclass_support.py
+-rw-rw-rw-   0        0        0     9280 2023-05-01 21:50:19.000000 pure_interface-7.1.0/tests/test_delegate.py
+-rw-rw-rw-   0        0        0     5935 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_func_sigs3.py
+-rw-rw-rw-   0        0        0    11757 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_function_sigs.py
+-rw-rw-rw-   0        0        0     1051 2023-05-01 21:06:52.000000 pure_interface-7.1.0/tests/test_generic_support.py
+-rw-rw-rw-   0        0        0    16459 2023-05-01 21:18:53.000000 pure_interface-7.1.0/tests/test_implementation_checks.py
+-rw-rw-rw-   0        0        0     2803 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_inheritance.py
+-rw-rw-rw-   0        0        0     4040 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_isinstance.py
+-rw-rw-rw-   0        0        0     2346 2023-03-01 20:08:43.000000 pure_interface-7.1.0/tests/test_meta_classes.py
+-rw-rw-rw-   0        0        0     2877 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_module_funcs.py
+-rw-rw-rw-   0        0        0     3364 2023-03-01 20:08:43.000000 pure_interface-7.1.0/tests/test_no_content_checks.py
+-rw-rw-rw-   0        0        0     2071 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_tracker.py
+-rw-rw-rw-   0        0        0      514 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_versions_in_sync.py
```

### Comparing `pure_interface-7.0.2/LICENSE` & `pure_interface-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/PKG-INFO` & `pure_interface-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_interface
-Version: 7.0.2
+Version: 7.1.0
 Summary: A Python interface library that disallows function body content on interfaces and supports adaption.
 Home-page: https://github.com/seequent/pure_interface
 Download-URL: https://pypi.org/project/pure-interface/
 Author: Tim Mitchell
 Author-email: tim.mitchell@seequent.com
 License: MIT
 Keywords: abc interface adapt adaption mapper structural typing dataclass
@@ -557,15 +557,15 @@
         def foo(self):
             return self.impl.foo * 2
 
         def bar(self, baz):
             return 'my bar'
 
 However, attempting to set an instance attribute as an override will just set the attribute on the underlying delegate
-instead.  If you want to override using an instance attribute, first define it as a class attribute::
+instead.  If you want to override an interface attribute using an instance attribute, first define it as a class attribute::
 
     class MyDelegate(Delegate, IFoo):
         pi_attr_delegates = {'impl': IFoo}
         foo = None  # prevents delegation of foo to `impl`
 
         def __init__(self, impl):
             self.impl = impl
```

### Comparing `pure_interface-7.0.2/README.rst` & `pure_interface-7.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -535,15 +535,15 @@
         def foo(self):
             return self.impl.foo * 2
 
         def bar(self, baz):
             return 'my bar'
 
 However, attempting to set an instance attribute as an override will just set the attribute on the underlying delegate
-instead.  If you want to override using an instance attribute, first define it as a class attribute::
+instead.  If you want to override an interface attribute using an instance attribute, first define it as a class attribute::
 
     class MyDelegate(Delegate, IFoo):
         pi_attr_delegates = {'impl': IFoo}
         foo = None  # prevents delegation of foo to `impl`
 
         def __init__(self, impl):
             self.impl = impl
```

### Comparing `pure_interface-7.0.2/pure_interface/__init__.py` & `pure_interface-7.1.0/pure_interface/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 from .delegation import Delegate
 
 try:
     from .data_classes import dataclass
 except ImportError:
     pass
 
-__version__ = '7.0.2'
+__version__ = '7.1.0'
```

### Comparing `pure_interface-7.0.2/pure_interface/adaption.py` & `pure_interface-7.1.0/pure_interface/adaption.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/pure_interface/data_classes.py` & `pure_interface-7.1.0/pure_interface/data_classes.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/pure_interface/delegation.py` & `pure_interface-7.1.0/pure_interface/delegation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import division, absolute_import, print_function
 
 import operator
 
+import pure_interface
 from .errors import InterfaceError
 from .interface import get_interface_names, type_is_interface, get_type_interfaces, InterfaceType
 
 _composed_types_map = {}
 _letters = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ'
 
 
@@ -119,31 +120,31 @@
 
         def i_have_attribute(attrib):
             for klass in non_interface_bases:
                 if attrib in klass.__dict__:
                     return True
             return False
 
-        for delegate, attr_list in cls.pi_attr_delegates.items():
+        for delegate, attr_list in cls.__dict__.get('pi_attr_delegates', {}).items():
             if isinstance(attr_list, type):
                 attr_list = list(get_interface_names(attr_list))
             if delegate in cls.pi_attr_mapping:
                 raise ValueError(f'Delegate {delegate} is in pi_attr_map')
             for attr in attr_list:
                 if attr in cls.pi_attr_mapping:
                     raise ValueError(f'{attr} in pi_attr_map and handled by delegate {delegate}')
                 if i_have_attribute(attr):
                     continue
                 dotted_name = f'{delegate}.{attr}'
                 setattr(cls, attr, _Delegated(dotted_name))
-        for attr, dotted_name in cls.pi_attr_mapping.items():
+        for attr, dotted_name in cls.__dict__.get('pi_attr_mapping', {}).items():
             if not i_have_attribute(attr):
                 setattr(cls, attr, _Delegated(dotted_name))
-        if cls.pi_attr_fallback:
-            fallback = cls.pi_attr_fallback
+        fallback = cls.__dict__.get('pi_attr_fallback', None)
+        if fallback is not None:
             for interface in get_type_interfaces(cls):
                 interface_names = get_interface_names(interface)
                 for attr in interface_names:
                     if not i_have_attribute(attr):
                         dotted_name = f'{fallback}.{attr}'
                         setattr(cls, attr, _Delegated(dotted_name))
```

### Comparing `pure_interface-7.0.2/pure_interface/interface.py` & `pure_interface-7.1.0/pure_interface/interface.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/pure_interface.egg-info/PKG-INFO` & `pure_interface-7.1.0/pure_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-interface
-Version: 7.0.2
+Version: 7.1.0
 Summary: A Python interface library that disallows function body content on interfaces and supports adaption.
 Home-page: https://github.com/seequent/pure_interface
 Download-URL: https://pypi.org/project/pure-interface/
 Author: Tim Mitchell
 Author-email: tim.mitchell@seequent.com
 License: MIT
 Keywords: abc interface adapt adaption mapper structural typing dataclass
@@ -557,15 +557,15 @@
         def foo(self):
             return self.impl.foo * 2
 
         def bar(self, baz):
             return 'my bar'
 
 However, attempting to set an instance attribute as an override will just set the attribute on the underlying delegate
-instead.  If you want to override using an instance attribute, first define it as a class attribute::
+instead.  If you want to override an interface attribute using an instance attribute, first define it as a class attribute::
 
     class MyDelegate(Delegate, IFoo):
         pi_attr_delegates = {'impl': IFoo}
         foo = None  # prevents delegation of foo to `impl`
 
         def __init__(self, impl):
             self.impl = impl
```

### Comparing `pure_interface-7.0.2/pure_interface.egg-info/SOURCES.txt` & `pure_interface-7.1.0/pure_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/setup.cfg` & `pure_interface-7.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7572 655f 696e 7465 7266 6163   = pure_interfac
-00000020: 650d 0a76 6572 7369 6f6e 203d 2037 2e30  e..version = 7.0
-00000030: 2e32 0d0a 6465 7363 7269 7074 696f 6e20  .2..description 
+00000020: 650d 0a76 6572 7369 6f6e 203d 2037 2e31  e..version = 7.1
+00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
 00000040: 3d20 4120 5079 7468 6f6e 2069 6e74 6572  = A Python inter
 00000050: 6661 6365 206c 6962 7261 7279 2074 6861  face library tha
 00000060: 7420 6469 7361 6c6c 6f77 7320 6675 6e63  t disallows func
 00000070: 7469 6f6e 2062 6f64 7920 636f 6e74 656e  tion body conten
 00000080: 7420 6f6e 2069 6e74 6572 6661 6365 7320  t on interfaces 
 00000090: 616e 6420 7375 7070 6f72 7473 2061 6461  and supports ada
 000000a0: 7074 696f 6e2e 0d0a 6b65 7977 6f72 6473  ption...keywords
```

### Comparing `pure_interface-7.0.2/tests/test_adapt_args_anno.py` & `pure_interface-7.1.0/tests/test_adapt_args_anno.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_adapt_args_no_anno.py` & `pure_interface-7.1.0/tests/test_adapt_args_no_anno.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_adaption.py` & `pure_interface-7.1.0/tests/test_adaption.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_dataclass_support.py` & `pure_interface-7.1.0/tests/test_dataclass_support.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_delegate.py` & `pure_interface-7.1.0/tests/test_delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,19 @@
         self.impl = impl
 
 
 class DSubFallback(DFallback, ISubTalker):
     pass
 
 
+class DSubFallback2(DFallback, ISubTalker):
+    pi_attr_fallback = 'impl'
+
+
+
 class DAttrMap(delegation.Delegate, IPoint):
     pi_attr_mapping = {'x': 'a.x',
                        'y': 'b.y',
                        'to_str': 'b.to_str',
                        }
 
     def __init__(self, a, b):
@@ -283,16 +288,21 @@
         self.assertEqual(4, d3.y)
         self.assertEqual('1, 4', d3.to_str())
         d3.y = 8  # delegates to p
         self.assertEqual(4, p.y)
         self.assertEqual(3, d3.z)
 
     def test_delegate_subclass_fallback(self):
-        """Fallback delegates are used for subclass interface attributes too."""
-        d = DSubFallback(Talker())
+        """Check fallback delegates are not used for subclass interface attributes too."""
+        with self.assertRaises(TypeError):
+            DSubFallback(Talker())  # no implementation of chat
+
+    def test_delegate_subclass_fallback2(self):
+        """Check subclass fallbacks are used for missing attributes."""
+        d = DSubFallback2(Talker())
         self.assertEqual('chat', d.chat())
 
 
 class CompositionTest(unittest.TestCase):
 
     def test_type_composition(self):
         a = Point(1, 2)
```

### Comparing `pure_interface-7.0.2/tests/test_func_sigs3.py` & `pure_interface-7.1.0/tests/test_func_sigs3.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_function_sigs.py` & `pure_interface-7.1.0/tests/test_function_sigs.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_generic_support.py` & `pure_interface-7.1.0/tests/test_generic_support.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_implementation_checks.py` & `pure_interface-7.1.0/tests/test_implementation_checks.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_inheritance.py` & `pure_interface-7.1.0/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_isinstance.py` & `pure_interface-7.1.0/tests/test_isinstance.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_meta_classes.py` & `pure_interface-7.1.0/tests/test_meta_classes.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_module_funcs.py` & `pure_interface-7.1.0/tests/test_module_funcs.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_no_content_checks.py` & `pure_interface-7.1.0/tests/test_no_content_checks.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_tracker.py` & `pure_interface-7.1.0/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.2/tests/test_versions_in_sync.py` & `pure_interface-7.1.0/tests/test_versions_in_sync.py`

 * *Files identical despite different names*

