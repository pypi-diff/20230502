# Comparing `tmp/fresco-3.2.0.tar.gz` & `tmp/fresco-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fresco-3.2.0.tar", last modified: Sun Apr 16 17:05:39 2023, max compression
+gzip compressed data, was "fresco-3.3.0.tar", last modified: Tue May  2 14:38:24 2023, max compression
```

## Comparing `fresco-3.2.0.tar` & `fresco-3.3.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:05:39.020991 fresco-3.2.0/
--rw-r--r--   0 oliver    (1001) wheel        (0)    20107 2023-04-16 17:02:23.000000 fresco-3.2.0/CHANGELOG.rst
--rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-04-16 17:02:22.000000 fresco-3.2.0/LICENSE.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)       50 2023-04-16 17:02:22.000000 fresco-3.2.0/MANIFEST.in
--rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-04-16 17:05:39.021103 fresco-3.2.0/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)      822 2023-04-16 17:02:22.000000 fresco-3.2.0/README.rst
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:05:39.012626 fresco-3.2.0/fresco/
--rw-r--r--   0 oliver    (1001) wheel        (0)      917 2023-04-16 17:05:34.000000 fresco-3.2.0/fresco/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7055 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/cookie.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    26509 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/core.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3232 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/decorators.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4410 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4171 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/middleware.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    13004 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/multidict.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10272 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/options.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    27071 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/request.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3339 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/requestcontext.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    37099 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/response.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10176 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/routeargs.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    57738 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/routing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2513 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/static.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    11016 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/subrequests.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:05:39.016820 fresco-3.2.0/fresco/tests/
--rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1871 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/fixtures.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2171 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_cookie.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    34019 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_core.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1480 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_decorators.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      973 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3137 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_middleware.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7565 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_multidict.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8603 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_options.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    16389 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_request.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3115 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_requestcontext.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8934 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_response.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8162 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_routeargs.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    36812 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_routing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4686 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_static.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7909 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_subrequests.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:05:39.018308 fresco-3.2.0/fresco/tests/util/
--rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10570 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/form_data.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1117 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/test_common.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10803 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/test_http.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1492 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/test_security.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7643 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/test_urls.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3038 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/test_wsgi.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      106 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/types.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      347 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/typing.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:05:39.020805 fresco-3.2.0/fresco/util/
--rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1609 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/cache.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1258 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/common.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     5484 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/contentencodings.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1383 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/file.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    22126 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/http.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1289 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/io.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      370 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/object.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1058 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/security.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2309 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/textproc.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     9195 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/urls.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    12970 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/wsgi.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:05:39.013444 fresco-3.2.0/fresco.egg-info/
--rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-04-16 17:05:38.000000 fresco-3.2.0/fresco.egg-info/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)     1476 2023-04-16 17:05:38.000000 fresco-3.2.0/fresco.egg-info/SOURCES.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-04-16 17:05:38.000000 fresco-3.2.0/fresco.egg-info/dependency_links.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-04-16 17:05:38.000000 fresco-3.2.0/fresco.egg-info/top_level.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)      795 2023-04-16 17:05:39.021821 fresco-3.2.0/setup.cfg
--rw-r--r--   0 oliver    (1001) wheel        (0)      634 2023-04-16 17:02:22.000000 fresco-3.2.0/setup.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:38:24.318645 fresco-3.3.0/
+-rw-r--r--   0 oliver    (1001) wheel        (0)    20513 2023-05-02 14:35:11.000000 fresco-3.3.0/CHANGELOG.rst
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-05-02 14:35:09.000000 fresco-3.3.0/LICENSE.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)       50 2023-05-02 14:35:09.000000 fresco-3.3.0/MANIFEST.in
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-05-02 14:38:24.318758 fresco-3.3.0/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)      822 2023-05-02 14:35:09.000000 fresco-3.3.0/README.rst
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:38:24.310052 fresco-3.3.0/fresco/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3520 2023-05-02 14:38:20.000000 fresco-3.3.0/fresco/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7055 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/cookie.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    26551 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/core.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3232 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/decorators.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4410 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4173 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/middleware.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    13362 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/multidict.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    13614 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/options.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    27071 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/request.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3504 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/requestcontext.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    37078 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/response.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10176 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/routeargs.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    57738 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/routing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2513 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/static.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11025 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/subrequests.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:38:24.314384 fresco-3.3.0/fresco/tests/
+-rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1871 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/fixtures.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2171 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_cookie.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    34019 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_core.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1480 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_decorators.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      973 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3137 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_middleware.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7565 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_multidict.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10868 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_options.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    16389 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_request.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3115 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_requestcontext.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     8934 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_response.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     8162 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_routeargs.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    36812 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_routing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4686 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_static.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7909 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_subrequests.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:38:24.315889 fresco-3.3.0/fresco/tests/util/
+-rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10570 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/form_data.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1117 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/test_common.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10803 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/test_http.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1492 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/test_security.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7643 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/test_urls.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3038 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/test_wsgi.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      106 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/types.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      347 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/typing.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:38:24.318452 fresco-3.3.0/fresco/util/
+-rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1609 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/cache.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1258 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/common.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     5484 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/contentencodings.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1383 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/file.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    22175 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/http.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1289 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/io.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      370 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/object.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1058 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/security.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2309 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/textproc.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9195 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/urls.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    12970 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/wsgi.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:38:24.310894 fresco-3.3.0/fresco.egg-info/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-05-02 14:38:24.000000 fresco-3.3.0/fresco.egg-info/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1476 2023-05-02 14:38:24.000000 fresco-3.3.0/fresco.egg-info/SOURCES.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-05-02 14:38:24.000000 fresco-3.3.0/fresco.egg-info/dependency_links.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-05-02 14:38:24.000000 fresco-3.3.0/fresco.egg-info/top_level.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)      795 2023-05-02 14:38:24.319366 fresco-3.3.0/setup.cfg
+-rw-r--r--   0 oliver    (1001) wheel        (0)      634 2023-05-02 14:35:09.000000 fresco-3.3.0/setup.py
```

### Comparing `fresco-3.2.0/CHANGELOG.rst` & `fresco-3.3.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+3.3.0 (released 2023-05-02)
+---------------------------
+
+- Options: fresco.options.Options can now take a list of paths as its first argument
+- Options: tags can now be specified with environment variable substitutions
+  (eg "{FOO}" would load files tagged with the current value of the 'FOO'
+  environment variable)
+- Options: add ``fresco.options.list_from_str`` and ``fresco.options.dict_from_options``
 
 3.2.0 (released 2023-04-16)
 ---------------------------
 
 - Bugfix: fixed cases where the close methods of WSGI content iterators were
   not called, notably when using subrequests
 - Bugfix: fix ``ResourceWarnings`` caused by unclosed temporary files
```

### Comparing `fresco-3.2.0/LICENSE.txt` & `fresco-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/PKG-INFO` & `fresco-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fresco
-Version: 3.2.0
+Version: 3.3.0
 Summary: A Web/WSGI micro-framework
 Home-page: https://ollycope.com/software/fresco/latest/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: wsgi web www framework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fresco-3.2.0/README.rst` & `fresco-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/cookie.py` & `fresco-3.3.0/fresco/cookie.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/core.py` & `fresco-3.3.0/fresco/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,17 +147,17 @@
         return "<%s %s>" % (
             clsname,
             ("\n" + " " * (len(clsname) + 2)).join(str(r) for r in self.__routes__),
         )
 
     def get_response(
         self,
-        request,
-        path,
-        method,
+        request: Request,
+        path: str,
+        method: str,
         currentcontext=context.currentcontext,
         normpath=normpath,
     ):
         ctx = currentcontext()
         ctx["app"] = self
         environ = request.environ
         environ["fresco.app"] = self
@@ -260,15 +260,15 @@
         # Is the URL just missing a trailing '/'?
         if not path or path[-1] != "/":
             for _ in self.get_methods(request, path + "/"):
                 return Response.unrestricted_redirect_permanent(path + "/")
 
         return Response.not_found()
 
-    def view(self, request=None) -> Response:
+    def view(self, request: t.Optional[Request] = None) -> Response:
         request = request or context.request
         try:
             path = request.path_info
         except ResponseException as e:
             response = e.response
         else:
             response = self.get_response(request, path, request.method)
```

### Comparing `fresco-3.2.0/fresco/decorators.py` & `fresco-3.3.0/fresco/decorators.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/exceptions.py` & `fresco-3.3.0/fresco/exceptions.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/middleware.py` & `fresco-3.3.0/fresco/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 #
-__all__ = "XForwarded"
+__all__ = ["XForwarded"]
 
 
 class XForwarded(object):
     """\
     Modify the WSGI environment so that the X_FORWARDED_* headers are observed
     and generated URIs are correct in a proxied environment.
```

### Comparing `fresco-3.2.0/fresco/multidict.py` & `fresco-3.3.0/fresco/multidict.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,20 +12,32 @@
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 #
 """
 An order preserving multidict implementation
 """
 from collections.abc import MutableMapping
+from collections.abc import Mapping
 from itertools import repeat
+import typing as t
 from typing import Any
 from typing import Dict
 from typing import Set
 
 
+if t.TYPE_CHECKING:
+    from typeshed import SupportsKeysAndGetItem
+else:
+    SupportsKeysAndGetItem = Mapping
+
+SupportsKeysAndGetItemOrIterable = t.Union[
+    SupportsKeysAndGetItem, t.Iterable[t.Tuple[Any, Any]]
+]
+
+
 class MultiDict(MutableMapping):
     """
     Dictionary-like object that supports multiple values per key. Insertion
     order is preserved.
 
     Synopsis:
 
@@ -40,17 +52,21 @@
         >>> d.getlist('b')
         [3]
         >>> list(d.allitems())
         [('a', 1), ('a', 2), ('b', 3)]
 
     """
 
+    _dict: Dict[Any, Any]
+    _order: t.List[Any]
     setdefault = MutableMapping.setdefault
 
-    def __init__(self, *args, **kwargs):
+    def __init__(
+        self, mapping_or_iterable: SupportsKeysAndGetItemOrIterable = tuple(), **kwargs
+    ):
         """
         MultiDicts can be constructed in the following ways:
 
             1. From a sequence of ``(key, value)`` pairs:
 
                 >>> from fresco.multidict import MultiDict
                 >>> MultiDict([('a', 1), ('a', 2)])  # doctest: +ELLIPSIS
@@ -72,21 +88,17 @@
             4. From keyword arguments:
 
                 >>> from fresco.multidict import MultiDict
                 >>> MultiDict(a=1)  # doctest: +ELLIPSIS
                 MultiDict(...)
 
         """
-        if len(args) > 1:
-            raise TypeError(
-                "%s expected at most 2 arguments, got %d"
-                % (self.__class__.__name__, 1 + len(args))
-            )
-        self.clear()
-        self.update(*args, **kwargs)
+        self._order = []
+        self._dict = {}
+        self._update(mapping_or_iterable, True, kwargs)
 
     def __getitem__(self, key):
         """
         Return the first item associated with ``key``:
 
             >>> d = MultiDict([('a', 1), ('a', 2)])
             >>> d['a']
@@ -285,15 +297,15 @@
         except (KeyError, IndexError):
             if args:
                 return args[0]
             raise KeyError(key)
         self._order.remove((key, value))
         return value
 
-    def popitem(self):
+    def popitem(self) -> t.Tuple[Any, Any]:
         """
         Return and remove a ``(key, value)`` pair from the dictionary.
 
         The item popped is always the most recently added key and the first
         value associated with it:
 
             >>> d = MultiDict([('a', 1), ('a', 2), ('b', 3)])
@@ -310,15 +322,25 @@
         """
         try:
             key = self._order[-1][0]
         except IndexError:
             raise KeyError("popitem(): dictionary is empty")
         return key, self.pop(key)
 
-    def update(self, *args, **kwargs):
+    @t.overload
+    def update(
+        self, mapping_or_iterable: SupportsKeysAndGetItem, /, **kwargs: Any
+    ) -> None:
+        ...
+
+    @t.overload
+    def update(self, /, **kwargs: Any) -> None:
+        ...
+
+    def update(self, mapping_or_iterable=tuple(), **kwargs):
         r"""
         Update the MultiDict from another MultiDict, regular dictionary or a
         iterable of ``(key, value)`` pairs. New keys overwrite old keys - use
         :meth:`extend` if you want new keys to be added to old keys.
 
         Updating from another MultiDict:
 
@@ -345,66 +367,61 @@
         or keyword arguments:
 
                 >>> d = MultiDict([('name', 'eric'),\
                 ...                ('occupation', 'lumberjack')])
                 >>> d.update(mood='okay')
 
         """
-        if len(args) > 1:
-            raise TypeError("expected at most 1 argument, got %d" % (1 + len(args),))
-        if args:
-            other = args[0]
-        else:
-            other = []
-        return self._update(other, True, **kwargs)
+        self._update(mapping_or_iterable, True, kwargs)
 
-    def extend(self, *args, **kwargs):
+    def extend(
+        self, mapping_or_iterable: SupportsKeysAndGetItemOrIterable = tuple(), **kwargs
+    ):
         """
         Extend the MultiDict with another MultiDict, regular dictionary or a
         iterable of ``(key, value)`` pairs. This is similar to :meth:`update`
         except that new keys are added to old keys.
         """
-        if len(args) > 1:
-            raise TypeError("expected at most 1 argument, got %d", (1 + len(args),))
-        if args:
-            other = args[0]
-        else:
-            other = []
-        return self._update(other, False, **kwargs)
+        return self._update(mapping_or_iterable, False, kwargs)
 
-    def _update(self, *args, **kwargs):
+    def _update(
+        self,
+        other: SupportsKeysAndGetItemOrIterable,
+        replace: bool,
+        extra_kwargs: Dict[Any, Any],
+    ):
         """
         Update the MultiDict from another object and optionally kwargs.
 
         :param other: the other MultiDict, dict, or iterable (first positional
                       arg)
         :param replace: if ``True``, entries will replace rather than extend
                         existing entries (second positional arg)
         """
-        other, replace = args
-
         if isinstance(other, self.__class__):
             items = list(other.allitems())
-        elif isinstance(other, dict):
+        elif isinstance(other, Mapping):
             items = list(other.items())
         else:
             items = list(other)
 
-        if kwargs:
-            items += list(kwargs.items())
+        if extra_kwargs:
+            items += list(extra_kwargs.items())
 
         if replace:
             replaced = {k for k, v in items if k in self._dict}
             self._order = [(k, v) for (k, v) in self._order if k not in replaced]
             for key in replaced:
                 self._dict[key] = []
 
+        setdefault = self._dict.setdefault
+        append_order = self._order.append
         for k, v in items:
-            self._dict.setdefault(k, []).append(v)
-            self._order.append((k, v))
+            setdefault(k, []).append(v)
+            append_order((k, v))
 
     def __repr__(self):
         """
         ``__repr__`` representation of object
         """
         return "%s(%r)" % (self.__class__.__name__, list(self.allitems()))
 
@@ -424,8 +441,8 @@
         return isinstance(other, MultiDict) and self._order == other._order
 
     def __ne__(self, other):
         return not (self == other)
 
     def clear(self):
         self._order = []
-        self._dict: Dict[Any, Any] = {}
+        self._dict = {}
```

### Comparing `fresco-3.2.0/fresco/options.py` & `fresco-3.3.0/fresco/options.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 #
 import inspect
 import json
 import logging
+import typing as t
 import os
 import re
 from decimal import Decimal
 from pathlib import Path
 from socket import gethostname
 from typing import Any
 from typing import Callable
@@ -27,14 +28,16 @@
 from typing import List
 from typing import Mapping
 from typing import Sequence
 from typing import Union
 
 from fresco.exceptions import OptionsLoadedException
 
+__all__ = ["Options"]
+
 logger = logging.getLogger(__name__)
 
 
 class Options(dict):
     """\
     Options dictionary. An instance of this is attached to each
     :class:`fresco.core.FrescoApp` instance, as a central store for
@@ -68,85 +71,122 @@
             self._loaded_callbacks.append(fn)
         return fn
 
     def do_loaded_callbacks(self):
         for func in self._loaded_callbacks:
             func(self)
 
+    def trigger_onload(self):
+        """
+        Mark the options object as having loaded and call any registered
+        onload callbacks
+        """
+        if self._is_loaded:
+            raise OptionsLoadedException("Options have already been loaded")
+        self.do_loaded_callbacks()
+        self.__dict__["_is_loaded"] = True
+
     def copy(self):
         return self.__class__(super().copy())
 
     def load(
         self,
-        sources: str,
+        sources: t.Union[str, t.Iterable[t.Union[Path, str]]],
         tags: Sequence[str] = [],
         use_environ=False,
         strict=True,
         dir=None,
+        trigger_onload=True,
     ):
         """
         Find all files matching glob pattern ``sources`` and populates the
         options object from those with matching filenames containing ``tags``.
 
-        :param sources: glob pattern or glob patterns separated by ";"
-        :param tags: a list of tags to look for in file names. If a filename
-                     contains multiple tags, all the tags in the filename must
-                     match for it to be loaded.
+        :param sources:
+            one or more glob patterns separated by ";",
+            or a list of glob patterns
+
+        :param tags:
+            a list of tags to look for in file names.
+
         :param use_environ: if true, environment variables matching previously
                             loaded keys will be loaded into the options object.
                             This happens after all files have been processed.
         :param strict: if true, the first file loaded is assumed to contain
                        all available option keys. Any new key found in a later
                        file will raise an error.
 
         Files may be in python (``.py``), json (``.json``), TOML (``.toml``)
         format. Any other files will be interpreted as simple lists of
         ```key=value`` pairs.
 
-        Tags in filenames should be delimited with periods, eg ".env.production.py". For
-        For example the filename ``setttings.dev.local.ini`` would be
-        considered to have the tags, ``('dev', 'local')``
-
-        The string '{hostname}' can be included as part of a tag name: it will
-        be substituted for the current host's name with dots replaced by
-        underscores.
+        Tags in filenames are delimited with periods,
+        for example ".env.production.py".
+        The filename ``setttings.dev.local.ini`` would be
+        considered to have the tags ``('dev', 'local')``
+
+        Where filename contain multiple tags, all tags must match for the file
+        to be loaded.
+
+        Tag names may contain the names of environment variable surrounded by
+        braces, for example ``{USER}``. These will be substituted for the
+        environment variable's value, with any dots or path separators replaced
+        by underscores.
+
+        The special variable ``{hostname}`` will be substituted for the current
+        host's name with dots replaced by underscores.
 
         Files with the suffix ".sample" are unconditionally excluded.
 
         Files are loaded in the order specified by ``tags``, then in filename
         order. Environment variables, if requested, are loaded last.
 
         Example::
 
             opts = Options()
-            opts.load(Options(), ".env*", ["dev", "host-{hostname}", "local"])
+            opts.load(".env*", ["dev", "host-{hostname}", "local"])
 
         Would load options from files named ``.env``, ``.env.json``, ``.env.dev.py``
         and ``.env.local.py.``
 
         """
         if self._is_loaded:
             raise OptionsLoadedException("Options have already been loaded")
-        hostname = gethostname().replace(".", "_")
+
+        tag_substitutions = os.environ.copy()
+        tag_substitutions["hostname"] = gethostname()
+        tag_substitutions = {
+            k: v.replace(".", "_").replace(os.pathsep, "_")
+            for k, v in tag_substitutions.items()
+        }
+
         candidates: List[Path] = []
         if dir is None:
             dir = Path(".")
         else:
             dir = Path(dir)
 
-        for source in sources.split(";"):
-            sourcepath = dir / Path(source.strip())
+        if isinstance(sources, str):
+            sources = [s.strip() for s in sources.split(";")]
+        for source in sources:
+            sourcepath = dir / Path(source)
             candidates.extend(
                 p
                 for p in sourcepath.parent.glob(sourcepath.name)
                 if p.suffix.lower() != ".sample"
             )
 
         if tags:
-            tags = [t.format(hostname=hostname) for t in tags]
+            subbed_tags = []
+            for tag in tags:
+                try:
+                    subbed_tags.append(tag.format(**tag_substitutions))
+                except KeyError:
+                    pass
+            tags = subbed_tags
             tagged_sources = []
             for p in candidates:
                 candidate_tags = [t for t in str(p.name).split(".") if t][1:]
                 if len(candidate_tags) == 0:
                     tagged_sources.append((candidate_tags, p))
                 else:
                     # Ignore the final tag if it matches a common config file
@@ -212,16 +252,17 @@
                 )
 
             if use_environ:
                 for k in self:
                     if k in os.environ:
                         self[k] = parse_value(self, os.environ[k])
 
-        self.do_loaded_callbacks()
-        self.__dict__["_is_loaded"] = True
+        if trigger_onload:
+            self.do_loaded_callbacks()
+            self.__dict__["_is_loaded"] = True
         return self
 
     def update_from_file(self, path, load_all=False):
         """
         Update the instance with any symbols found in the python source file at
         `path`.
 
@@ -252,17 +293,19 @@
         else:
             self.update(
                 (k, v) for k, v in d.items() if isinstance(k, str) and k and k[0] != "_"
             )
 
     def update_from_object(self, ob, load_all=False):
         """
-        Update the instance with any symbols listed in object `ob`
-        :param load_all: If true private symbols will also be loaded into the
-                         options object.
+        Update the instance with any symbols found in object ``ob``.
+
+        :param load_all:
+            If true private symbols will also be loaded into the options
+            object.
         """
         self.update_from_dict(dict(inspect.getmembers(ob)), load_all)
 
 
 def parse_value(
     options: Mapping,
     v: str,
@@ -294,7 +337,74 @@
 
     options = dict(options)
     values = {}
     for k, v in pairs:
         k = k.strip()
         values[k] = options[k] = parse_value(options, v)
     return values
+
+
+def list_from_str(s, separator=","):
+    """
+    Return the value of ``s`` split into a list of times by ``separator``.
+    Spaces around items will be stripped.
+    """
+    if isinstance(s, str):
+        if not s.strip():
+            return []
+        return [item.strip() for item in s.split(",")]
+    raise TypeError(f"Expected string, got {s!r}")
+
+
+def dict_from_options(
+    prefix: str, options: t.Mapping[str, Any], recursive: bool = False
+) -> t.Dict[str, Any]:
+    """
+    Create a dictionary containing all items in ``options`` whose keys start
+    with ``prefix``, with that prefix stripped.
+
+    Example:
+
+        >>> from fresco.options import Options, dict_from_options
+        >>> options = Options(
+        ...      {"DATABASE_HOST": "127.0.0.1", "DATABASE_USER": "scott"}
+        ... )
+        >>> dict_from_options("DATABASE_", options)
+        {'HOST': '127.0.0.1', 'USER': 'scott'}
+
+    If ``recursive`` is True, a recursive splitting will be
+    applied. The last character of ``prefix`` will be used as the separator,
+    for example::
+
+        >>> from fresco.options import dict_from_options
+        >>> options = Options(
+        ...      {
+        ...          "DATABASE_DEV_HOST": "127.0.0.1",
+        ...          "DATABASE_DEV_USER": "scott",
+        ...          "DATABASE_PROD_HOST": "192.168.0.78",
+        ...          "DATABASE_PROD_HOST": "tiger",
+        ...      }
+        ... )
+        >>> dict_from_options("DATABASE_", options, recursive=True)
+        {'DEV': {'HOST': '127.0.0.1', ...}, 'PROD': {'HOST', ...}}
+
+    """
+
+    prefixlen = len(prefix)
+    d = {k[prefixlen:]: v for k, v in options.items() if k.startswith(prefix)}
+
+    def recursive_split(d: t.Mapping[str, Any], sep: str) -> t.Dict[str, Any]:
+        d_: t.Dict[str, Any] = {}
+        for k in d:
+            if sep in k:
+                ks = k.split(sep)
+                subdict = d_
+                for subkey in ks[:-1]:
+                    subdict = subdict.setdefault(subkey, {})
+                subdict[ks[-1]] = d[k]
+            else:
+                d_[k] = d[k]
+        return d_
+
+    if recursive:
+        return recursive_split(d, prefix[-1])
+    return d
```

### Comparing `fresco-3.2.0/fresco/request.py` & `fresco-3.3.0/fresco/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         Return the contents of submitted form data
 
         This will return the ``POST`` or ``PUT`` data when available, otherwise
         querystring (``GET``)  data. Querystring data is always available via
         the ``query`` property.
         """
         if self._form is None:
-            if self.environ["REQUEST_METHOD"] in ("PUT", "POST"):
+            if self.environ["REQUEST_METHOD"] in {"PUT", "POST"}:
                 items, close = parse_post(
                     self.environ,
                     self.environ["wsgi.input"],
                     self.charset,
                     self.MAX_SIZE,
                     self.MAX_MULTIPART_SIZE,
                     ie_workaround=self.IE_CONTENT_DISPOSITION_WORKAROUND,
```

### Comparing `fresco-3.2.0/fresco/requestcontext.py` & `fresco-3.3.0/fresco/requestcontext.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 #
 from collections import defaultdict
 from threading import get_ident
 from typing import Any
 from typing import Dict
-from typing import List
+import typing as t
 
-__all__ = "context", "RequestContext"
+__all__ = ["context", "RequestContext"]
+
+ContextDict = t.Dict[str, Any]
+ContextStack = t.List[ContextDict]
 
 
 class RequestContext(object):
-    """\
+    """
     A local storage class that maintains different values for each request
     context in which it is used.
 
     Requires an ``ident_func`` that returns a hashable identifier that will
     give a different value per request. In a threaded environment this would be
     ``threading.get_ident``. If using a different execution model, a different
     strategy would need to be found.
@@ -38,54 +41,58 @@
     - ``view_self``: the instance of the current class based view if
       applicable, otherwise ``None``.
     - ``request``: the current :class:`~fresco.request.Request` object.
     """
 
     __slots__ = ["_contexts", "_ident_func"]
 
-    def __init__(self, ident_func=get_ident, setattr=object.__setattr__):
-        c: Dict[Any, List] = defaultdict(list)
+    def __init__(
+        self,
+        ident_func: t.Callable[[], t.Any] = get_ident,
+        setattr=object.__setattr__
+    ):
+        c: Dict[Any, ContextStack] = defaultdict(list)
         c[ident_func()] = [{}]
         setattr(self, "_contexts", c)
         setattr(self, "_ident_func", ident_func)
 
-    def push(self, **bindnames):
+    def push(self, **bindnames: t.Any):
         self._contexts[self._ident_func()].append(bindnames)
 
     def pop(self):
         ident = self._ident_func()
         ctx = self._contexts[ident]
         ctx.pop()
         if not ctx:
             del self._contexts[ident]
 
-    def currentcontext(self):
+    def currentcontext(self) -> ContextDict:
         return self._contexts[self._ident_func()][-1]
 
     def __getattr__(self, item):
         try:
             return self._contexts[self._ident_func()][-1][item]
         except (KeyError, IndexError):
             raise AttributeError(item)
 
-    def __setattr__(self, item, ob):
+    def __setattr__(self, item: str, ob: t.Any):
         self._contexts[self._ident_func()][-1][item] = ob
 
     def __delattr__(self, item):
         try:
             del self._contexts[self._ident_func()][-1][item]
         except KeyError:
             raise AttributeError(item)
 
     # Emulate dictionary access methods
     __getitem__ = __getattr__
     __setitem__ = __setattr__
     __delitem__ = __delattr__
 
-    def get(self, item, default=None):
+    def get(self, item: str, default=None):
         return self.currentcontext().get(item, default)
 
     def __repr__(self):
         return "<%s localdepth=%d; total=%d; current=%r>" % (
             self.__class__.__name__,
             len(self._contexts[self._ident_func()]),
             sum(len(ctx) for ctx in self._contexts.values()),
```

### Comparing `fresco-3.2.0/fresco/response.py` & `fresco-3.3.0/fresco/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     "x_ua_compatible": "X-UA-Compatible",
 }
 
 default_charset = "UTF-8"
 
 
 def encoder(stream, charset):
-    r"""\
+    """
     Encode a response iterator using the given character set.
     """
     if charset is None:
         charset = default_charset
 
     for chunk in stream:
         if not isinstance(chunk, bytes):
@@ -322,15 +322,15 @@
                 addheader((h, str(item)))
         else:
             addheader((h, str(val)))
     return hs
 
 
 class Response(object):
-    """\
+    """
     Model an HTTP response
     """
 
     default_content_type = "text/html; charset=UTF-8"
 
     def __init__(
         self,
@@ -496,30 +496,30 @@
             responder.status,
             headers=responder.headers,
             passthrough=True,
             onclose=[close] if close is not None else [],
         )
 
     def get_headers(self, name):
-        """\
+        """
         Return the list of headers set with the given name.
 
         Synopsis::
 
             >>> r = Response(set_cookie = ['cookie1', 'cookie2'])
             >>> r.get_headers('set-cookie')
             ['cookie1', 'cookie2']
 
         """
         return [
             value for header, value in self.headers if header.lower() == name.lower()
         ]
 
     def get_header(self, name, default=""):
-        """\
+        """
         Return the concatenated values of the named header(s) or ``default`` if
         the header has not been set.
 
         As specified in RFC2616 (section 4.2), multiple headers will be
         combined using a single comma.
 
         Example usage::
@@ -543,39 +543,39 @@
             >>> Response(status=200).status_code
             200
         """
         return int(self.status.split(" ", 1)[0])
 
     @property
     def content_type(self):
-        """\
+        """
         Return the value of the ``Content-Type`` header if set, otherwise
         ``None``.
         """
         for key, val in self.headers:
             if key.lower() == "content-type":
                 return val
         return None
 
     def add_header(self, name, value, make_header_name=make_header_name):
-        """\
+        """
         Return a new response object with the given additional header.
 
         Synopsis::
 
             >>> r = Response(content_type='text/plain')
             >>> r.headers
             [('Content-Type', 'text/plain')]
             >>> r.add_header('Cache-Control', 'no-cache').headers
             [('Content-Type', 'text/plain'), ('Cache-Control', 'no-cache')]
         """
         return self.replace(headers=(self.headers + [(make_header_name(name), value)]))
 
     def add_headers(self, headers=[], **kwheaders):
-        """\
+        """
         Return a new response object with the given additional headers.
 
         Synopsis::
 
             >>> r = Response(content_type='text/plain')
             >>> r.headers
             [('Content-Type', 'text/plain')]
@@ -583,15 +583,15 @@
             ...     cache_control='no-cache',
             ... ).headers
             [('Content-Type', 'text/plain'), ('Cache-Control', 'no-cache')]
         """
         return self.replace(headers=make_headers(self.headers + headers, kwheaders))
 
     def remove_headers(self, *headers):
-        """\
+        """
         Return a new response object with the named headers removed.
 
         Synopsis::
 
             >>> r = Response(content_type='text/plain',
             ...              cache_control='no-cache')
             >>> r.headers
@@ -613,15 +613,15 @@
         path="/",
         secure=None,
         domain=None,
         comment=None,
         httponly=False,
         samesite="Lax",
     ):
-        """\
+        """
         Return a new response object with the given cookie added.
 
         Synopsis::
 
             >>> r = Response(content_type='text/plain')
             >>> r.headers
             [('Content-Type', 'text/plain')]
@@ -716,15 +716,15 @@
             status,
             headers,
             onclose=onclose,
             content_iterator=content_iterator,
         )
 
     def buffered(self):
-        """\
+        """
         Return a new response object with the content buffered into a list.
         This will also generate a content-length header.
 
         Example usage::
 
             >>> def generate_content():
             ...     yield "one two "
@@ -752,15 +752,15 @@
                 if mo:
                     return mo.group(1)
                 break
         return default_charset
 
     @classmethod
     def not_found(cls, request=None):
-        """\
+        """
         Return an HTTP not found response (404).
 
         Synopsis::
 
             >>> def view():
             ...     return Response.not_found()
             ...
@@ -820,15 +820,15 @@
         Return an HTTP unauthorized response (401) with a WWW-Authenticate
         header set for HTTP Basic authentication..
         """
         return cls.unauthorized(authenticate=f'Basic realm="{realm}"')
 
     @classmethod
     def forbidden(cls, message="Sorry, access is denied"):
-        """\
+        """
         Return an HTTP forbidden response (403).
 
         Synopsis::
 
             >>> def view():
             ...     return Response.forbidden()
             ...
@@ -836,15 +836,15 @@
         return cls(
             "<html>\n<body>\n<h1>%s</h1>\n</body>\n</html>" % (message,),
             status=STATUS_FORBIDDEN,
         )
 
     @classmethod
     def bad_request(cls, request=None):
-        """\
+        """
         Return an HTTP bad request response.
 
         Synopsis::
 
             >>> def view():
             ...     return Response.bad_request()
             ...
@@ -859,15 +859,15 @@
                 "</body>"
                 "</html>"
             ],
         )
 
     @classmethod
     def length_required(cls, request=None):
-        """\
+        """
         Return an HTTP Length Required response (411).
 
         Synopsis::
 
             >>> def view():
             ...     return Response.length_required()
             ...
@@ -882,30 +882,30 @@
                 "</body>"
                 "</html>"
             ],
         )
 
     @classmethod
     def payload_too_large(cls, request=None):
-        """\
+        """
         Return an HTTP Payload Too Large response (413)::
 
             >>> response = Response.payload_too_large()
 
         """
         return cls(
             status=STATUS_PAYLOAD_TOO_LARGE,
             content=["<html><body><h1>Payload Too Large</h1></body></html>"],
         )
 
     request_entity_too_large = payload_too_large
 
     @classmethod
     def method_not_allowed(cls, valid_methods):
-        """\
+        """
         Return an HTTP method not allowed response (405)::
 
             >>> from fresco import context
             >>> def view():
             ...     if context.request.method == 'POST':
             ...         return Response.method_not_allowed(('POST', ))
             ...
@@ -919,15 +919,15 @@
             status=STATUS_METHOD_NOT_ALLOWED,
             allow=",".join(valid_methods),
             content=["<html><body><h1>Method not allowed</h1></body></html>"],
         )
 
     @classmethod
     def internal_server_error(cls):
-        """\
+        """
         Return an HTTP internal server error response (500).
 
         Synopsis::
 
             >>> def view():
             ...     return Response.internal_server_error()
             ...
@@ -940,15 +940,15 @@
             content=["<html><body><h1>Internal Server Error</h1></body></html>"],
         )
 
     @classmethod
     def unrestricted_redirect(
         cls, location, request=None, status=STATUS_FOUND, **kwargs
     ):
-        """\
+        """
         Return an HTTP redirect reponse (30x).
 
         :param location: The redirect location or a view specification.
         :param status: HTTP status code for the redirect, default is
                        ``STATUS_FOUND`` (temporary redirect)
         :param kwargs: kwargs to be passed to :func:`fresco.core.urlfor` to
                        construct the redirect URL
@@ -1056,15 +1056,16 @@
         :param status: HTTP status code for the redirect, default is
                        ``STATUS_FOUND`` (temporary redirect)
         :param fallback: a fallback URL to be used for the redirect in the case
                          that ``location`` is considered unsafe
         :param kwargs: kwargs to be passed to :func:`fresco.core.urlfor` to
                        construct the redirect URL, or the fallback in the case
                        that ``location`` is already a qualified URL.
-        Synopsis:
+
+        Synopsis::
 
             >>> def view():
             ...   return Response.redirect("/new-location")
             ...
 
         The location argument is interpreted as for
         :meth:`~fresco.response.Response.unrestricted_redirect`
@@ -1080,41 +1081,41 @@
             return cls.unrestricted_redirect(url, status=status, **kwargs)
         if fallback:
             return fallback
         raise ValueError("Unsafe URL")
 
     @classmethod
     def redirect_permanent(cls, *args, **kwargs):
-        """\
+        """
         Return an HTTP permanent redirect reponse.
 
         :param location: the URI of the new location. If relative this will be
                          converted to an absolute URL based on the current
                          request.
 
         """
         kwargs["status"] = STATUS_MOVED_PERMANENTLY
         return cls.redirect(*args, **kwargs)
 
     @classmethod
     def redirect_temporary(cls, *args, **kwargs):
-        """\
+        """
         Return an HTTP permanent redirect reponse.
 
         :param location: the URI of the new location. If relative this will be
                          converted to an absolute URL based on the current
                          request.
 
         """
         kwargs["status"] = STATUS_FOUND
         return cls.redirect(*args, **kwargs)
 
     @classmethod
     def meta_refresh(cls, location, delay=1, request=None):
-        """\
+        """
         Return an HTML page containing a <meta http-equiv="refresh"> tag,
         causing the browser to redirect to the given location after ``delay``
         seconds.
 
         :param location: the URI of the new location. If relative this will be
                          converted to an absolute URL based on the current
                          request.
@@ -1168,15 +1169,15 @@
             status=status,
             headers=headers,
             content_type=content_type,
         )
 
 
 def dump_response(r, line_break=b"\r\n", encoding="UTF-8"):
-    """\
+    """
     Return a byte-string representation of the given response, as for a HTTP
     response.
     """
     output = []
     output.append(r.status.encode("ascii"))
     output.append(line_break)
     for k, v in sorted(r.headers):
```

### Comparing `fresco-3.2.0/fresco/routeargs.py` & `fresco-3.3.0/fresco/routeargs.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/routing.py` & `fresco-3.3.0/fresco/routing.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/static.py` & `fresco-3.3.0/fresco/static.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/subrequests.py` & `fresco-3.3.0/fresco/subrequests.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,20 +30,20 @@
       a full request context is constructed to emulate a request
       to the given path.
       The subrequest will invoke all middleware layers and application hooks.
 
     - **A callable**: a new subrequest context will be created and
       ``view(*args, **kwargs)`` will be called. Middleware and application
       hooks will not be called, and any
-      :class:`~fresco.routeargs.RouteArg`s  defined will not be resolved.
+      :class:`~fresco.routeargs.RouteArg` instances will not be resolved.
 
     - **Any other value**: the view function is looked up using the same
       route resolution rules as :meth:`~fresco.core.FrescoApp.urlfor`.
       Middleware and hooks will be skipped, but
-      :class:`~fresco.routeargs.RouteArg`s will be resolved.
+      :class:`~fresco.routeargs.RouteArg` instances will be resolved.
 
     If you pass in a view callable you can force RouteArgs to be resolved by
     specifying ``_resolve=True``.
 
     You can force a full request to be emulated by specifying ``_full=True``.
 
     Passing additional positional and keyword arguments has a different
```

### Comparing `fresco-3.2.0/fresco/tests/fixtures.py` & `fresco-3.3.0/fresco/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_cookie.py` & `fresco-3.3.0/fresco/tests/test_cookie.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_core.py` & `fresco-3.3.0/fresco/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_decorators.py` & `fresco-3.3.0/fresco/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_exceptions.py` & `fresco-3.3.0/fresco/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_middleware.py` & `fresco-3.3.0/fresco/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_multidict.py` & `fresco-3.3.0/fresco/tests/test_multidict.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_options.py` & `fresco-3.3.0/fresco/tests/test_options.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import pathlib
 import sys
 
 import pytest
 
 from fresco.options import Options
 from fresco.options import parse_key_value_pairs
+from fresco.options import dict_from_options
 
 
 class TestOptions(object):
     def test_options_dictionary_access(self):
         options = Options()
         options["x"] = 1
         assert options["x"] == 1
@@ -138,24 +139,32 @@
         assert parse_key_value_pairs({}, ["a=$x"]) == {"a": "$x"}
         assert parse_key_value_pairs({"x": 1}, ["a=${x}"]) == {"a": 1}
         assert parse_key_value_pairs({"x": 1}, ["a=$x"]) == {"a": 1}
         assert parse_key_value_pairs({}, ["a=1", "b=$a"]) == {"a": 1, "b": 1}
 
 
 class TestLoadOptions:
+
     def check_loadoptions(self, tmpdir, files, sources="*", tags=[], expected={}):
+        """
+        Write the files indicated in ``sources`` to the given temporary directory,
+
+        Create an Options object and populate it from the specified sources/tags.
+
+        Assert that the loaded options is equal to the value of ``expected``.
+        """
         t = pathlib.Path(tmpdir)
         for fname in files:
             with (t / fname).open("w", encoding="UTF-8") as f:
                 f.write(files[fname])
 
         @contextlib.contextmanager
         def optionsdir():
             def loadopts(sources="*", tags=[], strict=False, **kw):
-                return Options().load(str(sources), tags, strict=False, **kw)
+                return Options().load(sources, tags, strict=False, **kw)
 
             saved = os.getcwd()
             os.chdir(t)
             try:
                 yield loadopts
             finally:
                 os.chdir(saved)
@@ -209,18 +218,18 @@
             tmpdir,
             {"a.dev.txt": "a = dev", "a.local.txt": "a = local"},
         ) as loadopts:
             assert loadopts("*", ["dev", "local"]) == {"a": "local"}
             assert loadopts("*", ["local", "dev"]) == {"a": "dev"}
 
     def test_it_loads_from_os_environ(self, tmpdir):
-        with self.check_loadoptions(tmpdir, {"a.txt": "a = 1"}) as loadopts:
-            os.environ["a"] = "2"
-            assert loadopts("*", [], use_environ=False) == {"a": 1}
-            assert loadopts("*", [], use_environ=True) == {"a": 2}
+        with setenv(a="2"):
+            with self.check_loadoptions(tmpdir, {"a.txt": "a = 1"}) as loadopts:
+                assert loadopts("*", [], use_environ=False) == {"a": 1}
+                assert loadopts("*", [], use_environ=True) == {"a": 2}
 
     def test_it_calls_callbacks(self, tmpdir):
         with self.check_loadoptions(tmpdir, {"a.txt": "a = 1"}):
             options = Options()
             mock = Mock()
             options.onload(mock)
             options.load(str(pathlib.Path(tmpdir) / "*"))
@@ -228,7 +237,78 @@
 
     def test_it_sets_directory(self, tmpdir):
         with self.check_loadoptions(tmpdir, {"a.txt": "a = 1"}) as loadopts:
             with TemporaryDirectory() as tmpdir2:
                 os.chdir(tmpdir2)
                 assert loadopts("*") == {}
                 assert loadopts("*", dir=tmpdir) == {"a": 1}
+
+    def test_it_accepts_a_list_of_filespecs(self, tmpdir):
+        self.check_loadoptions(
+            tmpdir,
+            {"a.txt": "a=1", "b.txt": "b=1"},
+            sources=["a.*", "b.*"],
+            expected={"a": 1, "b": 1}
+        )
+
+    def test_it_substitutes_from_environment_variables(self, tmpdir):
+        with setenv(FOO="bar"):
+            self.check_loadoptions(
+                tmpdir,
+                {"a.txt": "a=1", "a.bar.txt": "a=2"},
+                tags=["{FOO}"],
+                expected={"a": 2}
+            )
+
+        with setenv(FOO="baz"):
+            self.check_loadoptions(
+                tmpdir,
+                {"a.txt": "a=1", "a.bar.txt": "a=2"},
+                tags=["{FOO}"],
+                expected={"a": 1}
+            )
+
+    def test_it_allows_missing_environment_variables(self, tmpdir):
+        assert "FOO" not in os.environ
+        self.check_loadoptions(
+            tmpdir,
+            {"a.txt": "a=1", "a.bar.txt": "a=2"},
+            tags=["{FOO}"],
+            expected={"a": 1}
+        )
+
+
+class TestDictFromOptions:
+
+    def test_it_splits_on_prefix(self):
+
+        options = Options(FOO_BAR=1, FOO_BAZ=2, FOO_BAR_BAZ=3, BAR=4)
+        assert dict_from_options("FOO_", options) == {"BAR": 1, "BAZ": 2, "BAR_BAZ": 3}
+
+    def test_it_splits_recursively(self):
+
+        options = Options(
+            A_A=1,
+            A_B_C_D=2,
+            A_B_E=3,
+            A_F_G_H=4,
+            A_I=5,
+            J_A=6,
+        )
+        assert dict_from_options("A_", options, recursive=True) == {
+            "A": 1,
+            "B": {"C": {"D": 2}, "E": 3},
+            "F": {"G": {"H": 4}},
+            "I": 5
+        }
+
+
+@contextlib.contextmanager
+def setenv(**kw):
+    saved = {k: os.environ[k] for k in kw if k in os.environ}
+    os.environ.update(kw)
+    yield os.environ
+    for k in kw:
+        if k in saved:
+            os.environ[k] = saved[k]
+        else:
+            del os.environ[k]
```

### Comparing `fresco-3.2.0/fresco/tests/test_request.py` & `fresco-3.3.0/fresco/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_requestcontext.py` & `fresco-3.3.0/fresco/tests/test_requestcontext.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_response.py` & `fresco-3.3.0/fresco/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_routeargs.py` & `fresco-3.3.0/fresco/tests/test_routeargs.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_routing.py` & `fresco-3.3.0/fresco/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_static.py` & `fresco-3.3.0/fresco/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/test_subrequests.py` & `fresco-3.3.0/fresco/tests/test_subrequests.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/util/form_data.py` & `fresco-3.3.0/fresco/tests/util/form_data.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/util/test_common.py` & `fresco-3.3.0/fresco/tests/util/test_common.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/util/test_http.py` & `fresco-3.3.0/fresco/tests/util/test_http.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/util/test_security.py` & `fresco-3.3.0/fresco/tests/util/test_security.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/util/test_urls.py` & `fresco-3.3.0/fresco/tests/util/test_urls.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/tests/util/test_wsgi.py` & `fresco-3.3.0/fresco/tests/util/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/util/cache.py` & `fresco-3.3.0/fresco/util/cache.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/util/common.py` & `fresco-3.3.0/fresco/util/common.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/util/contentencodings.py` & `fresco-3.3.0/fresco/util/contentencodings.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/util/file.py` & `fresco-3.3.0/fresco/util/file.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/util/http.py` & `fresco-3.3.0/fresco/util/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,15 @@
 
 
 def parse_querystring(
     data: str,
     charset: Optional[str] = None,
     strict: bool = False,
     keep_blank_values: bool = True,
+    unquote_plus=unquote_plus,
 ) -> List[Tuple[str, str]]:
     """
     Return ``(key, value)`` pairs from the given querystring::
 
         >>> list(parse_querystring('green%20eggs=ham;me=sam+i+am'))
         [('green eggs', 'ham'), ('me', 'sam i am')]
 
@@ -515,15 +516,15 @@
     The second iterator generates all remaining data.
 
     The first iterator must be exhausted before the second is iterated.
     The callable must only be called after the first iterator has been
     exhausted.
     """
     buf = b""
-    found = None
+    found: t.Optional[bool] = None
 
     def _found():
         if found is None:
             raise AssertionError("The first iterator was not exhausted")
         return found
 
     def read_upto():
```

### Comparing `fresco-3.2.0/fresco/util/io.py` & `fresco-3.3.0/fresco/util/io.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/util/security.py` & `fresco-3.3.0/fresco/util/security.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/util/textproc.py` & `fresco-3.3.0/fresco/util/textproc.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/util/urls.py` & `fresco-3.3.0/fresco/util/urls.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco/util/wsgi.py` & `fresco-3.3.0/fresco/util/wsgi.py`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/fresco.egg-info/PKG-INFO` & `fresco-3.3.0/fresco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fresco
-Version: 3.2.0
+Version: 3.3.0
 Summary: A Web/WSGI micro-framework
 Home-page: https://ollycope.com/software/fresco/latest/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: wsgi web www framework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fresco-3.2.0/fresco.egg-info/SOURCES.txt` & `fresco-3.3.0/fresco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/setup.cfg` & `fresco-3.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fresco-3.2.0/setup.py` & `fresco-3.3.0/setup.py`

 * *Files identical despite different names*

