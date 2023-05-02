# Comparing `tmp/zope.security-6.1.tar.gz` & `tmp/zope.security-6.2a1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.security-6.1.tar", last modified: Wed Jan 18 07:48:20 2023, max compression
+gzip compressed data, was "zope.security-6.2a1.dev0.tar", last modified: Thu Apr 20 06:20:43 2023, max compression
```

## Comparing `zope.security-6.1.tar` & `zope.security-6.2a1.dev0.tar`

### file list

```diff
@@ -1,121 +1,102 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.164555 zope.security-6.1/
--rw-r--r--   0 jens       (501) staff       (20)      587 2023-01-15 09:49:35.000000 zope.security-6.1/.coveragerc
--rwxr-xr-x   0 jens       (501) staff       (20)     1918 2023-01-15 09:49:35.000000 zope.security-6.1/.manylinux-install.sh
--rwxr-xr-x   0 jens       (501) staff       (20)      509 2023-01-15 09:49:35.000000 zope.security-6.1/.manylinux.sh
--rw-r--r--   0 jens       (501) staff       (20)    20113 2023-01-18 07:34:58.000000 zope.security-6.1/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      799 2023-01-15 09:49:35.000000 zope.security-6.1/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       32 2023-01-03 12:45:40.000000 zope.security-6.1/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2023-01-03 12:45:40.000000 zope.security-6.1/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      422 2023-01-15 09:49:35.000000 zope.security-6.1/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)    22926 2023-01-18 07:48:20.164631 zope.security-6.1/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     1290 2023-01-03 12:45:40.000000 zope.security-6.1/README.rst
--rw-r--r--   0 jens       (501) staff       (20)     1792 2023-01-15 09:49:35.000000 zope.security-6.1/appveyor.yml
--rw-r--r--   0 jens       (501) staff       (20)      546 2023-01-16 14:43:05.000000 zope.security-6.1/buildout.cfg
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.151597 zope.security-6.1/docs/
--rw-r--r--   0 jens       (501) staff       (20)     5588 2023-01-03 12:45:40.000000 zope.security-6.1/docs/Makefile
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.147601 zope.security-6.1/docs/_build/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.151742 zope.security-6.1/docs/_build/doctest/
--rw-r--r--   0 jens       (501) staff       (20)     1490 2023-01-17 09:36:28.000000 zope.security-6.1/docs/_build/doctest/output.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.147644 zope.security-6.1/docs/_build/html/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.152887 zope.security-6.1/docs/_build/html/_sources/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.155243 zope.security-6.1/docs/_build/html/_sources/api/
--rw-r--r--   0 jens       (501) staff       (20)      110 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/api/adapter.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    23089 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/api/checker.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     5103 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/api/decorator.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      122 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/api/interfaces.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      122 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/api/management.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      134 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/api/metaconfigure.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     3332 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/api/permission.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      130 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/api/protectclass.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     1003 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/api/proxy.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      138 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/api/simplepolicies.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      110 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/api/testing.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     2258 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/api/zcml.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       28 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/changes.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     8157 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/example.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    10645 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/hacking.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      631 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     4334 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/narr.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    14695 2023-01-03 12:45:40.000000 zope.security-6.1/docs/_build/html/_sources/proxy.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.156935 zope.security-6.1/docs/api/
--rw-r--r--   0 jens       (501) staff       (20)      110 2023-01-03 12:45:40.000000 zope.security-6.1/docs/api/adapter.rst
--rw-r--r--   0 jens       (501) staff       (20)    23089 2023-01-03 12:45:40.000000 zope.security-6.1/docs/api/checker.rst
--rw-r--r--   0 jens       (501) staff       (20)     5103 2023-01-03 12:45:40.000000 zope.security-6.1/docs/api/decorator.rst
--rw-r--r--   0 jens       (501) staff       (20)      122 2023-01-03 12:45:40.000000 zope.security-6.1/docs/api/interfaces.rst
--rw-r--r--   0 jens       (501) staff       (20)      122 2023-01-03 12:45:40.000000 zope.security-6.1/docs/api/management.rst
--rw-r--r--   0 jens       (501) staff       (20)      134 2023-01-03 12:45:40.000000 zope.security-6.1/docs/api/metaconfigure.rst
--rw-r--r--   0 jens       (501) staff       (20)     3332 2023-01-03 12:45:40.000000 zope.security-6.1/docs/api/permission.rst
--rw-r--r--   0 jens       (501) staff       (20)      130 2023-01-03 12:45:40.000000 zope.security-6.1/docs/api/protectclass.rst
--rw-r--r--   0 jens       (501) staff       (20)     1003 2023-01-03 12:45:40.000000 zope.security-6.1/docs/api/proxy.rst
--rw-r--r--   0 jens       (501) staff       (20)      138 2023-01-03 12:45:40.000000 zope.security-6.1/docs/api/simplepolicies.rst
--rw-r--r--   0 jens       (501) staff       (20)      110 2023-01-03 12:45:40.000000 zope.security-6.1/docs/api/testing.rst
--rw-r--r--   0 jens       (501) staff       (20)     2258 2023-01-03 12:45:40.000000 zope.security-6.1/docs/api/zcml.rst
--rw-r--r--   0 jens       (501) staff       (20)       28 2023-01-03 12:45:40.000000 zope.security-6.1/docs/changes.rst
--rw-r--r--   0 jens       (501) staff       (20)     9154 2023-01-03 12:45:40.000000 zope.security-6.1/docs/conf.py
--rw-r--r--   0 jens       (501) staff       (20)     8157 2023-01-03 12:45:40.000000 zope.security-6.1/docs/example.rst
--rw-r--r--   0 jens       (501) staff       (20)    10645 2023-01-03 12:45:40.000000 zope.security-6.1/docs/hacking.rst
--rw-r--r--   0 jens       (501) staff       (20)      631 2023-01-03 12:45:40.000000 zope.security-6.1/docs/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     5108 2023-01-03 12:45:40.000000 zope.security-6.1/docs/make.bat
--rw-r--r--   0 jens       (501) staff       (20)     4334 2023-01-03 12:45:40.000000 zope.security-6.1/docs/narr.rst
--rw-r--r--   0 jens       (501) staff       (20)    14695 2023-01-03 12:45:40.000000 zope.security-6.1/docs/proxy.rst
--rw-r--r--   0 jens       (501) staff       (20)      122 2023-01-03 12:45:40.000000 zope.security-6.1/rtd.txt
--rw-r--r--   0 jens       (501) staff       (20)      594 2023-01-18 07:48:20.165342 zope.security-6.1/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     6687 2023-01-18 07:35:09.000000 zope.security-6.1/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.147940 zope.security-6.1/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.157074 zope.security-6.1/src/zope/
--rw-r--r--   0 jens       (501) staff       (20)       56 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.160919 zope.security-6.1/src/zope/security/
--rw-r--r--   0 jens       (501) staff       (20)     1009 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     1684 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/_compat.py
--rw-r--r--   0 jens       (501) staff       (20)      997 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/_definitions.py
--rw-r--r--   0 jens       (501) staff       (20)    26676 2023-01-18 07:34:11.000000 zope.security-6.1/src/zope/security/_proxy.c
--rw-r--r--   0 jens       (501) staff       (20)    18340 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/_zope_security_checker.c
--rw-r--r--   0 jens       (501) staff       (20)     4955 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/adapter.py
--rw-r--r--   0 jens       (501) staff       (20)    36314 2023-01-18 07:34:11.000000 zope.security-6.1/src/zope/security/checker.py
--rw-r--r--   0 jens       (501) staff       (20)      639 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/configure.zcml
--rw-r--r--   0 jens       (501) staff       (20)     3159 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/decorator.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.161265 zope.security-6.1/src/zope/security/examples/
--rw-r--r--   0 jens       (501) staff       (20)     8769 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/examples/sandbox.py
--rw-r--r--   0 jens       (501) staff       (20)     6305 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/examples/sandbox_security.py
--rw-r--r--   0 jens       (501) staff       (20)      892 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/i18n.py
--rw-r--r--   0 jens       (501) staff       (20)    13752 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)     5115 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/management.py
--rw-r--r--   0 jens       (501) staff       (20)     1964 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/meta.zcml
--rw-r--r--   0 jens       (501) staff       (20)     8318 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/metaconfigure.py
--rw-r--r--   0 jens       (501) staff       (20)     6862 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/metadirectives.py
--rw-r--r--   0 jens       (501) staff       (20)     3531 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/permission.py
--rw-r--r--   0 jens       (501) staff       (20)     1019 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/permissions.zcml
--rw-r--r--   0 jens       (501) staff       (20)     3504 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/protectclass.py
--rw-r--r--   0 jens       (501) staff       (20)    13836 2023-01-18 07:34:11.000000 zope.security-6.1/src/zope/security/proxy.py
--rw-r--r--   0 jens       (501) staff       (20)     2750 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/simplepolicies.py
--rw-r--r--   0 jens       (501) staff       (20)     3209 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/testing.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.164239 zope.security-6.1/src/zope/security/tests/
--rw-r--r--   0 jens       (501) staff       (20)      589 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)      856 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/exampleclass.py
--rw-r--r--   0 jens       (501) staff       (20)     1560 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/module.py
--rw-r--r--   0 jens       (501) staff       (20)      707 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/redefineperms.zcml
--rw-r--r--   0 jens       (501) staff       (20)    18656 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_adapter.py
--rw-r--r--   0 jens       (501) staff       (20)    87497 2023-01-18 07:34:11.000000 zope.security-6.1/src/zope/security/tests/test_checker.py
--rw-r--r--   0 jens       (501) staff       (20)     1373 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_compile_flags.py
--rw-r--r--   0 jens       (501) staff       (20)     6087 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_decorator.py
--rw-r--r--   0 jens       (501) staff       (20)     1675 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_location.py
--rw-r--r--   0 jens       (501) staff       (20)     7424 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_management.py
--rw-r--r--   0 jens       (501) staff       (20)    30575 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_metaconfigure.py
--rw-r--r--   0 jens       (501) staff       (20)     7816 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_permission.py
--rw-r--r--   0 jens       (501) staff       (20)     5544 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_protectclass.py
--rw-r--r--   0 jens       (501) staff       (20)    65358 2023-01-16 14:43:05.000000 zope.security-6.1/src/zope/security/tests/test_proxy.py
--rw-r--r--   0 jens       (501) staff       (20)     2799 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_simpleinteraction.py
--rw-r--r--   0 jens       (501) staff       (20)     4863 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_simplepolicies.py
--rw-r--r--   0 jens       (501) staff       (20)     2760 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_testing.py
--rw-r--r--   0 jens       (501) staff       (20)     8016 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_zcml.py
--rw-r--r--   0 jens       (501) staff       (20)    21828 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/tests/test_zcml_functest.py
--rw-r--r--   0 jens       (501) staff       (20)     3981 2023-01-03 12:45:40.000000 zope.security-6.1/src/zope/security/zcml.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-18 07:48:20.158008 zope.security-6.1/src/zope.security.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)    22926 2023-01-18 07:48:20.000000 zope.security-6.1/src/zope.security.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     3339 2023-01-18 07:48:20.000000 zope.security-6.1/src/zope.security.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-01-18 07:48:20.000000 zope.security-6.1/src/zope.security.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)        5 2023-01-18 07:48:20.000000 zope.security-6.1/src/zope.security.egg-info/namespace_packages.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-01-03 14:40:42.000000 zope.security-6.1/src/zope.security.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)      368 2023-01-18 07:48:20.000000 zope.security-6.1/src/zope.security.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)        5 2023-01-18 07:48:20.000000 zope.security-6.1/src/zope.security.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     1612 2023-01-16 14:43:05.000000 zope.security-6.1/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.534636 zope.security-6.2a1.dev0/
+-rw-r--r--   0 mac        (513) staff       (20)      587 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/.coveragerc
+-rwxr-xr-x   0 mac        (513) staff       (20)     2182 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/.manylinux-install.sh
+-rwxr-xr-x   0 mac        (513) staff       (20)      509 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/.manylinux.sh
+-rw-r--r--   0 mac        (513) staff       (20)    20556 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      799 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      452 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)    23376 2023-04-20 06:20:43.534803 zope.security-6.2a1.dev0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1290 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1958 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/appveyor.yml
+-rw-r--r--   0 mac        (513) staff       (20)      546 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/buildout.cfg
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.512626 zope.security-6.2a1.dev0/docs/
+-rw-r--r--   0 mac        (513) staff       (20)     5588 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/Makefile
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.516872 zope.security-6.2a1.dev0/docs/api/
+-rw-r--r--   0 mac        (513) staff       (20)      110 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/adapter.rst
+-rw-r--r--   0 mac        (513) staff       (20)    23089 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/checker.rst
+-rw-r--r--   0 mac        (513) staff       (20)     5103 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/decorator.rst
+-rw-r--r--   0 mac        (513) staff       (20)      122 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/interfaces.rst
+-rw-r--r--   0 mac        (513) staff       (20)      122 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/management.rst
+-rw-r--r--   0 mac        (513) staff       (20)      134 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/metaconfigure.rst
+-rw-r--r--   0 mac        (513) staff       (20)     3332 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/permission.rst
+-rw-r--r--   0 mac        (513) staff       (20)      130 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/protectclass.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1003 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/proxy.rst
+-rw-r--r--   0 mac        (513) staff       (20)      138 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/simplepolicies.rst
+-rw-r--r--   0 mac        (513) staff       (20)      110 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/testing.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2258 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/zcml.rst
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/changes.rst
+-rw-r--r--   0 mac        (513) staff       (20)     9154 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/conf.py
+-rw-r--r--   0 mac        (513) staff       (20)     8157 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/example.rst
+-rw-r--r--   0 mac        (513) staff       (20)    10645 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/hacking.rst
+-rw-r--r--   0 mac        (513) staff       (20)      631 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)     5108 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/make.bat
+-rw-r--r--   0 mac        (513) staff       (20)     4334 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/narr.rst
+-rw-r--r--   0 mac        (513) staff       (20)    14695 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/proxy.rst
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.503250 zope.security-6.2a1.dev0/include/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.503389 zope.security-6.2a1.dev0/include/zope.proxy/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.503526 zope.security-6.2a1.dev0/include/zope.proxy/zope/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.517207 zope.security-6.2a1.dev0/include/zope.proxy/zope/proxy/
+-rw-r--r--   0 mac        (513) staff       (20)     1457 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/include/zope.proxy/zope/proxy/proxy.h
+-rw-r--r--   0 mac        (513) staff       (20)      122 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/rtd.txt
+-rw-r--r--   0 mac        (513) staff       (20)      595 2023-04-20 06:20:43.535422 zope.security-6.2a1.dev0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     5837 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.504062 zope.security-6.2a1.dev0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.517536 zope.security-6.2a1.dev0/src/zope/
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.527111 zope.security-6.2a1.dev0/src/zope/security/
+-rw-r--r--   0 mac        (513) staff       (20)     1009 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     1684 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/_compat.py
+-rw-r--r--   0 mac        (513) staff       (20)      997 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/_definitions.py
+-rw-r--r--   0 mac        (513) staff       (20)    26688 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/_proxy.c
+-rw-r--r--   0 mac        (513) staff       (20)    18340 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/_zope_security_checker.c
+-rw-r--r--   0 mac        (513) staff       (20)     4955 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/adapter.py
+-rw-r--r--   0 mac        (513) staff       (20)    36314 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/checker.py
+-rw-r--r--   0 mac        (513) staff       (20)      639 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/configure.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     3159 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/decorator.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.527771 zope.security-6.2a1.dev0/src/zope/security/examples/
+-rw-r--r--   0 mac        (513) staff       (20)     8769 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/examples/sandbox.py
+-rw-r--r--   0 mac        (513) staff       (20)     6305 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/examples/sandbox_security.py
+-rw-r--r--   0 mac        (513) staff       (20)      892 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/i18n.py
+-rw-r--r--   0 mac        (513) staff       (20)    13752 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     5115 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/management.py
+-rw-r--r--   0 mac        (513) staff       (20)     1964 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/meta.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     8318 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/metaconfigure.py
+-rw-r--r--   0 mac        (513) staff       (20)     6862 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/metadirectives.py
+-rw-r--r--   0 mac        (513) staff       (20)     3531 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/permission.py
+-rw-r--r--   0 mac        (513) staff       (20)     1019 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/permissions.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     3504 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/protectclass.py
+-rw-r--r--   0 mac        (513) staff       (20)    13815 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/proxy.py
+-rw-r--r--   0 mac        (513) staff       (20)     2750 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/simplepolicies.py
+-rw-r--r--   0 mac        (513) staff       (20)     3209 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/testing.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.534317 zope.security-6.2a1.dev0/src/zope/security/tests/
+-rw-r--r--   0 mac        (513) staff       (20)      589 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      856 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/exampleclass.py
+-rw-r--r--   0 mac        (513) staff       (20)     1560 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/module.py
+-rw-r--r--   0 mac        (513) staff       (20)      707 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/redefineperms.zcml
+-rw-r--r--   0 mac        (513) staff       (20)    18656 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_adapter.py
+-rw-r--r--   0 mac        (513) staff       (20)    87468 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_checker.py
+-rw-r--r--   0 mac        (513) staff       (20)     1373 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_compile_flags.py
+-rw-r--r--   0 mac        (513) staff       (20)     6087 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_decorator.py
+-rw-r--r--   0 mac        (513) staff       (20)     1675 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_location.py
+-rw-r--r--   0 mac        (513) staff       (20)     7424 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_management.py
+-rw-r--r--   0 mac        (513) staff       (20)    30575 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_metaconfigure.py
+-rw-r--r--   0 mac        (513) staff       (20)     7816 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_permission.py
+-rw-r--r--   0 mac        (513) staff       (20)     5544 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_protectclass.py
+-rw-r--r--   0 mac        (513) staff       (20)    65397 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_proxy.py
+-rw-r--r--   0 mac        (513) staff       (20)     2799 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_simpleinteraction.py
+-rw-r--r--   0 mac        (513) staff       (20)     4863 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_simplepolicies.py
+-rw-r--r--   0 mac        (513) staff       (20)     2760 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_testing.py
+-rw-r--r--   0 mac        (513) staff       (20)     8016 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_zcml.py
+-rw-r--r--   0 mac        (513) staff       (20)    21828 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_zcml_functest.py
+-rw-r--r--   0 mac        (513) staff       (20)     3981 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/zcml.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.519863 zope.security-6.2a1.dev0/src/zope.security.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)    23376 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     2525 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      368 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1666 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/tox.ini
```

### Comparing `zope.security-6.1/.coveragerc` & `zope.security-6.2a1.dev0/.coveragerc`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/.manylinux-install.sh` & `zope.security-6.2a1.dev0/.manylinux-install.sh`

 * *Files 7% similar despite different names*

```diff
@@ -24,33 +24,40 @@
 ls -ld /cache/pip
 
 # We need some libraries because we build wheels from scratch:
 yum -y install libffi-devel
 
 tox_env_map() {
     case $1 in
+        *"cp312"*) echo 'py312';;
         *"cp37"*) echo 'py37';;
         *"cp38"*) echo 'py38';;
         *"cp39"*) echo 'py39';;
         *"cp310"*) echo 'py310';;
         *"cp311"*) echo 'py311';;
         *) echo 'py';;
     esac
 }
 
 # Compile wheels
 for PYBIN in /opt/python/*/bin; do
     if \
+       [[ "${PYBIN}" == *"cp312"* ]] || \
        [[ "${PYBIN}" == *"cp311"* ]] || \
        [[ "${PYBIN}" == *"cp37"* ]] || \
        [[ "${PYBIN}" == *"cp38"* ]] || \
        [[ "${PYBIN}" == *"cp39"* ]] || \
        [[ "${PYBIN}" == *"cp310"* ]] ; then
-        "${PYBIN}/pip" install -e /io/
-        "${PYBIN}/pip" wheel /io/ -w wheelhouse/
+        if [[ "${PYBIN}" == *"cp312"* ]] ; then
+            "${PYBIN}/pip" install --pre -e /io/
+            "${PYBIN}/pip" wheel /io/ --pre -w wheelhouse/
+        else
+            "${PYBIN}/pip" install -e /io/
+            "${PYBIN}/pip" wheel /io/ -w wheelhouse/
+        fi
         if [ `uname -m` == 'aarch64' ]; then
           cd /io/
           ${PYBIN}/pip install tox
           TOXENV=$(tox_env_map "${PYBIN}")
           ${PYBIN}/tox -e ${TOXENV}
           cd ..
         fi
```

### Comparing `zope.security-6.1/CHANGES.rst` & `zope.security-6.2a1.dev0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 =========
  Changes
 =========
 
+6.2a1.dev0 (2023-04-20)
+-----------------------
+
+- Make ``next()`` on C proxies call ``__next__`` rather than ``next`` (see
+  PEP 3114), and drop support for the Python 2 ``next`` method name from
+  pure-Python proxies.
+
+- Drop using ``setup_requires`` due to constant problems on GHA.
+
+- Add preliminary support for Python 3.12 as of 3.12a7 -- even though there are
+  currently tests breaking, so please do not consider it fully supported.
+
+
 6.1 (2023-01-18)
 ================
 
 - Remove more proxying code for names that no longer exist in Python 3.
   (`#92 <https://github.com/zopefoundation/zope.security/issues/92>`_)
```

### Comparing `zope.security-6.1/CONTRIBUTING.md` & `zope.security-6.2a1.dev0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/LICENSE.txt` & `zope.security-6.2a1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/PKG-INFO` & `zope.security-6.2a1.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.security
-Version: 6.1
+Version: 6.2a1.dev0
 Summary: Zope Security Framework
 Home-page: http://github.com/zopefoundation/zope.security
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://zopesecurity.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.security/issues
@@ -67,14 +67,27 @@
 Documentation is available at https://zopesecurity.readthedocs.io/
 
 
 =========
  Changes
 =========
 
+6.2a1.dev0 (2023-04-20)
+-----------------------
+
+- Make ``next()`` on C proxies call ``__next__`` rather than ``next`` (see
+  PEP 3114), and drop support for the Python 2 ``next`` method name from
+  pure-Python proxies.
+
+- Drop using ``setup_requires`` due to constant problems on GHA.
+
+- Add preliminary support for Python 3.12 as of 3.12a7 -- even though there are
+  currently tests breaking, so please do not consider it fully supported.
+
+
 6.1 (2023-01-18)
 ================
 
 - Remove more proxying code for names that no longer exist in Python 3.
   (`#92 <https://github.com/zopefoundation/zope.security/issues/92>`_)
```

### Comparing `zope.security-6.1/README.rst` & `zope.security-6.2a1.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/appveyor.yml` & `zope.security-6.2a1.dev0/appveyor.yml`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
   matrix:
     - python: 37-x64
     - python: 38-x64
     - python: 39-x64
     - python: 310-x64
     - python: 311-x64
+    # `multibuild` cannot install non-final versions as they are not on
+    # ftp.python.org, so we skip Python 3.11 until its final release:
+    # - python: 312-x64
 
 install:
   - "SET PYTHONVERSION=%PYTHON%"
   - "SET PATH=C:\\Python%PYTHON%;c:\\Python%PYTHON%\\scripts;%PATH%"
   - ps: |
       $env:PYTHON = "C:\\Python${env:PYTHON}"
       if (-not (Test-Path $env:PYTHON)) {
```

### Comparing `zope.security-6.1/buildout.cfg` & `zope.security-6.2a1.dev0/buildout.cfg`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/Makefile` & `zope.security-6.2a1.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/_build/html/_sources/api/checker.rst.txt` & `zope.security-6.2a1.dev0/docs/api/checker.rst`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/_build/html/_sources/api/decorator.rst.txt` & `zope.security-6.2a1.dev0/docs/api/decorator.rst`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/_build/html/_sources/api/permission.rst.txt` & `zope.security-6.2a1.dev0/docs/api/permission.rst`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/_build/html/_sources/api/proxy.rst.txt` & `zope.security-6.2a1.dev0/docs/api/proxy.rst`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/_build/html/_sources/api/zcml.rst.txt` & `zope.security-6.2a1.dev0/docs/api/zcml.rst`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/_build/html/_sources/example.rst.txt` & `zope.security-6.2a1.dev0/docs/example.rst`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/_build/html/_sources/hacking.rst.txt` & `zope.security-6.2a1.dev0/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/_build/html/_sources/index.rst.txt` & `zope.security-6.2a1.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/_build/html/_sources/narr.rst.txt` & `zope.security-6.2a1.dev0/docs/narr.rst`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/_build/html/_sources/proxy.rst.txt` & `zope.security-6.2a1.dev0/docs/proxy.rst`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/conf.py` & `zope.security-6.2a1.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/docs/make.bat` & `zope.security-6.2a1.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/setup.cfg` & `zope.security-6.2a1.dev0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	docs/_build/doctest/*
 	docs/_build/html/_sources/api/*
 
 [isort]
 force_single_line = True
 combine_as_imports = True
 sections = FUTURE,STDLIB,THIRDPARTY,ZOPE,FIRSTPARTY,LOCALFOLDER
-known_third_party = six, docutils, pkg_resources
+known_third_party = docutils, pkg_resources, pytz
 known_zope = 
 known_first_party = 
 default_section = ZOPE
 line_length = 79
 lines_after_imports = 2
 
 [egg_info]
```

### Comparing `zope.security-6.1/setup.py` & `zope.security-6.2a1.dev0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,43 +61,20 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
-# Include directories for C extensions
-# Sniff the location of the headers in the package distribution
-
-
-class ModuleHeaderDir:
-
-    def __init__(self, require_spec, where='../..'):
-        # By default, assume top-level pkg has the same name as the dist.
-        # Also assume that headers are located in the package dir, and
-        # are meant to be included as follows:
-        #    #include "module/header_name.h"
-        self._require_spec = require_spec
-        self._where = where
-
-    def __str__(self):
-        from pkg_resources import require
-        from pkg_resources import resource_filename
-        require(self._require_spec)
-        path = resource_filename(self._require_spec, self._where)
-        return os.path.abspath(path)
-
-
-include = [ModuleHeaderDir('zope.proxy')]
 
 codeoptimization = [
     Extension(
         "zope.security._proxy",
-        [os.path.join('src', 'zope', 'security', "_proxy.c")],
-        include_dirs=include,
+        include_dirs=[os.path.join('include', 'zope.proxy')],
+        sources=[os.path.join('src', 'zope', 'security', "_proxy.c")]
     ),
     Extension(
         "zope.security._zope_security_checker",
         [os.path.join('src', 'zope', 'security',
                       "_zope_security_checker.c")]
     ),
 ]
@@ -107,33 +84,31 @@
 # anti-optimizations (the C extension compatibility layer is known-slow,
 # and defeats JIT opportunities).
 py_impl = getattr(platform, 'python_implementation', lambda: None)
 is_pypy = py_impl() == 'PyPy'
 is_jython = 'java' in sys.platform
 
 if is_pypy or is_jython:
-    setup_requires = []
     ext_modules = []
 else:
-    setup_requires = ['zope.proxy >= 4.3.0']
     ext_modules = codeoptimization
 
 
 TESTS_REQUIRE = [
     'BTrees',
     'zope.component',
     'zope.configuration',
     'zope.location',
     'zope.testing',
     'zope.testrunner',
 ]
 
 
 setup(name='zope.security',
-      version='6.1',
+      version='6.2a1.dev0',
       author='Zope Foundation and Contributors',
       author_email='zope-dev@zope.org',
       description='Zope Security Framework',
       long_description=(
           read('README.rst')
           + '\n\n' +
           read('CHANGES.rst')
@@ -165,15 +140,14 @@
                             '/zope.security/issues'),
           'Sources': 'https://github.com/zopefoundation/zope.security',
       },
       license='ZPL 2.1',
       packages=find_packages('src'),
       package_dir={'': 'src'},
       namespace_packages=['zope'],
-      setup_requires=setup_requires,
       cmdclass={
           'build_ext': optional_build_ext,
       },
       ext_modules=ext_modules,
       python_requires='>=3.7',
       install_requires=[
           'setuptools',
```

### Comparing `zope.security-6.1/src/zope/security/__init__.py` & `zope.security-6.2a1.dev0/src/zope/security/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/_compat.py` & `zope.security-6.2a1.dev0/src/zope/security/_compat.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/_definitions.py` & `zope.security-6.2a1.dev0/src/zope/security/_definitions.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/_proxy.c` & `zope.security-6.2a1.dev0/src/zope/security/_proxy.c`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 DECLARE_STRING(__cmp__);
 DECLARE_STRING(__contains__);
 DECLARE_STRING(__delitem__);
 DECLARE_STRING(__getitem__);
 DECLARE_STRING(__hash__);
 DECLARE_STRING(__iter__);
 DECLARE_STRING(__len__);
-DECLARE_STRING(next);
+DECLARE_STRING(__next__);
 DECLARE_STRING(op_abs);
 DECLARE_STRING(op_add);
 DECLARE_STRING(op_and);
 DECLARE_STRING(op_divmod);
 DECLARE_STRING(op_float);
 DECLARE_STRING(op_floordiv);
 DECLARE_STRING(op_iadd);
@@ -347,15 +347,15 @@
 }
 
 static PyObject *
 proxy_iternext(SecurityProxy *self)
 {
   PyObject *result = NULL;
 
-  if (check(self, str_check_getattr, str_next) >= 0)
+  if (check(self, str_check_getattr, str___next__) >= 0)
     {
       result = PyIter_Next(self->proxy.proxy_object);
       PROXY_RESULT(self, result);
     }
   return result;
 }
 
@@ -874,15 +874,15 @@
   INIT_STRING(__cmp__);
   INIT_STRING(__contains__);
   INIT_STRING(__delitem__);
   INIT_STRING(__getitem__);
   INIT_STRING(__hash__);
   INIT_STRING(__iter__);
   INIT_STRING(__len__);
-  INIT_STRING(next);
+  INIT_STRING(__next__);
   INIT_STRING_OP(abs);
   INIT_STRING_OP(add);
   INIT_STRING_OP(and);
   INIT_STRING_OP(divmod);
   INIT_STRING_OP(float);
   INIT_STRING_OP(floordiv);
   INIT_STRING_OP(iadd);
```

### Comparing `zope.security-6.1/src/zope/security/_zope_security_checker.c` & `zope.security-6.2a1.dev0/src/zope/security/_zope_security_checker.c`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/adapter.py` & `zope.security-6.2a1.dev0/src/zope/security/adapter.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/checker.py` & `zope.security-6.2a1.dev0/src/zope/security/checker.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/configure.zcml` & `zope.security-6.2a1.dev0/src/zope/security/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/decorator.py` & `zope.security-6.2a1.dev0/src/zope/security/decorator.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/examples/sandbox.py` & `zope.security-6.2a1.dev0/src/zope/security/examples/sandbox.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/examples/sandbox_security.py` & `zope.security-6.2a1.dev0/src/zope/security/examples/sandbox_security.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/i18n.py` & `zope.security-6.2a1.dev0/src/zope/security/i18n.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/interfaces.py` & `zope.security-6.2a1.dev0/src/zope/security/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/management.py` & `zope.security-6.2a1.dev0/src/zope/security/management.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/meta.zcml` & `zope.security-6.2a1.dev0/src/zope/security/meta.zcml`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/metaconfigure.py` & `zope.security-6.2a1.dev0/src/zope/security/metaconfigure.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/metadirectives.py` & `zope.security-6.2a1.dev0/src/zope/security/metadirectives.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/permission.py` & `zope.security-6.2a1.dev0/src/zope/security/permission.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/permissions.zcml` & `zope.security-6.2a1.dev0/src/zope/security/permissions.zcml`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/protectclass.py` & `zope.security-6.2a1.dev0/src/zope/security/protectclass.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/proxy.py` & `zope.security-6.2a1.dev0/src/zope/security/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,14 @@
              # '__hash__',    # Unchecked in C proxy (rich comparison)
              # '__cmp__',     # Unchecked in C proxy
              '__getitem__',
              '__setitem__',
              '__delitem__',
              '__iter__',
              '__next__',
-             'next',
              '__contains__',
              '__neg__',
              '__pos__',
              '__abs__',
              '__invert__',
              '__complex__',
              '__int__',
```

### Comparing `zope.security-6.1/src/zope/security/simplepolicies.py` & `zope.security-6.2a1.dev0/src/zope/security/simplepolicies.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/testing.py` & `zope.security-6.2a1.dev0/src/zope/security/testing.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/__init__.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/exampleclass.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/exampleclass.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/module.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/module.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/redefineperms.zcml` & `zope.security-6.2a1.dev0/src/zope/security/tests/redefineperms.zcml`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_adapter.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_checker.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,16 +582,14 @@
                 try:
                     return self.items[self.index]
                 except IndexError:
                     raise StopIteration()
                 finally:
                     self.index += 1
 
-            next = __next__
-
             def __length_hint__(self):
                 self.hint_called = True
                 return self.hint
 
         # The hint is called on raw objects
         i = Iter()
         list(i)
```

### Comparing `zope.security-6.1/src/zope/security/tests/test_compile_flags.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_decorator.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_location.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_management.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_metaconfigure.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_metaconfigure.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_permission.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_protectclass.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_protectclass.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_proxy.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1486,15 +1486,17 @@
 class Checker:
 
     ok = 1
 
     unproxied_types = {str, }
 
     def check_getattr(self, _object, name):
-        if name not in ("foo", "next", "__class__", "__name__", "__module__"):
+        if name in ("__class__", "__name__", "__module__"):
+            return
+        if not self.ok or name not in ("__next__", "foo"):
             raise RuntimeError
 
     def check_setattr(self, _object, name):
         if name != "foo":
             raise RuntimeError
 
     def check(self, _object, _opname):
@@ -1531,15 +1533,14 @@
         return 42
 
     def __iter__(self):
         return self
 
     def __next__(self):
         return 42  # Infinite sequence
-    next = __next__
 
     def __len__(self):
         return 42
 
     def __contains__(self, x):
         return x == 42
 
@@ -1647,18 +1648,18 @@
         from zope.security.proxy import removeSecurityProxy
         self.assertEqual(removeSecurityProxy(iter(self.p)), self.x)
 
     def testIterFail(self):
         self.shouldFail(iter, self.p)
 
     def testNextOK(self):
-        self.assertEqual(self.p.next(), 42)
+        self.assertEqual(next(self.p), 42)
 
     def testNextFail(self):
-        self.shouldFail(self.p.next)
+        self.shouldFail(next, self.p)
 
     def testHashOK(self):
         self.assertEqual(hash(self.p), hash(self.x))
 
 #   def testHashFail(self):
 #       self.shouldFail(hash, self.p)
```

### Comparing `zope.security-6.1/src/zope/security/tests/test_simpleinteraction.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_simpleinteraction.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_simplepolicies.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_simplepolicies.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_testing.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_zcml.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_zcml.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/tests/test_zcml_functest.py` & `zope.security-6.2a1.dev0/src/zope/security/tests/test_zcml_functest.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope/security/zcml.py` & `zope.security-6.2a1.dev0/src/zope/security/zcml.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.1/src/zope.security.egg-info/PKG-INFO` & `zope.security-6.2a1.dev0/src/zope.security.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.security
-Version: 6.1
+Version: 6.2a1.dev0
 Summary: Zope Security Framework
 Home-page: http://github.com/zopefoundation/zope.security
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://zopesecurity.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.security/issues
@@ -67,14 +67,27 @@
 Documentation is available at https://zopesecurity.readthedocs.io/
 
 
 =========
  Changes
 =========
 
+6.2a1.dev0 (2023-04-20)
+-----------------------
+
+- Make ``next()`` on C proxies call ``__next__`` rather than ``next`` (see
+  PEP 3114), and drop support for the Python 2 ``next`` method name from
+  pure-Python proxies.
+
+- Drop using ``setup_requires`` due to constant problems on GHA.
+
+- Add preliminary support for Python 3.12 as of 3.12a7 -- even though there are
+  currently tests breaking, so please do not consider it fully supported.
+
+
 6.1 (2023-01-18)
 ================
 
 - Remove more proxying code for names that no longer exist in Python 3.
   (`#92 <https://github.com/zopefoundation/zope.security/issues/92>`_)
```

### Comparing `zope.security-6.1/src/zope.security.egg-info/SOURCES.txt` & `zope.security-6.2a1.dev0/src/zope.security.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -18,45 +18,27 @@
 docs/conf.py
 docs/example.rst
 docs/hacking.rst
 docs/index.rst
 docs/make.bat
 docs/narr.rst
 docs/proxy.rst
-docs/_build/doctest/output.txt
-docs/_build/html/_sources/changes.rst.txt
-docs/_build/html/_sources/example.rst.txt
-docs/_build/html/_sources/hacking.rst.txt
-docs/_build/html/_sources/index.rst.txt
-docs/_build/html/_sources/narr.rst.txt
-docs/_build/html/_sources/proxy.rst.txt
-docs/_build/html/_sources/api/adapter.rst.txt
-docs/_build/html/_sources/api/checker.rst.txt
-docs/_build/html/_sources/api/decorator.rst.txt
-docs/_build/html/_sources/api/interfaces.rst.txt
-docs/_build/html/_sources/api/management.rst.txt
-docs/_build/html/_sources/api/metaconfigure.rst.txt
-docs/_build/html/_sources/api/permission.rst.txt
-docs/_build/html/_sources/api/protectclass.rst.txt
-docs/_build/html/_sources/api/proxy.rst.txt
-docs/_build/html/_sources/api/simplepolicies.rst.txt
-docs/_build/html/_sources/api/testing.rst.txt
-docs/_build/html/_sources/api/zcml.rst.txt
 docs/api/adapter.rst
 docs/api/checker.rst
 docs/api/decorator.rst
 docs/api/interfaces.rst
 docs/api/management.rst
 docs/api/metaconfigure.rst
 docs/api/permission.rst
 docs/api/protectclass.rst
 docs/api/proxy.rst
 docs/api/simplepolicies.rst
 docs/api/testing.rst
 docs/api/zcml.rst
+include/zope.proxy/zope/proxy/proxy.h
 src/zope/__init__.py
 src/zope.security.egg-info/PKG-INFO
 src/zope.security.egg-info/SOURCES.txt
 src/zope.security.egg-info/dependency_links.txt
 src/zope.security.egg-info/namespace_packages.txt
 src/zope.security.egg-info/not-zip-safe
 src/zope.security.egg-info/requires.txt
```

### Comparing `zope.security-6.1/tox.ini` & `zope.security-6.2a1.dev0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 envlist =
     lint
     py37,py37-pure
     py38,py38-pure
     py39,py39-pure
     py310,py310-pure
     py311,py311-pure
+    py312,py312-pure
     pypy3
     docs
     coverage
     py37-watch, py311-watch
 
 [testenv]
 usedevelop = true
+pip_pre = py312: true
 deps =
+    Sphinx
 setenv =
     pure: PURE_PYTHON=1
     !pure-!pypy3: PURE_PYTHON=0
     ZOPE_INTERFACE_STRICT_IRO=1
     watch: ZOPE_WATCH_CHECKERS=1
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
```

