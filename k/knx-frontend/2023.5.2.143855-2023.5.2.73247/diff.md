# Comparing `tmp/knx_frontend-2023.5.2.143855.tar.gz` & `tmp/knx_frontend-2023.5.2.73247.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knx_frontend-2023.5.2.143855.tar", last modified: Tue May  2 15:15:53 2023, max compression
+gzip compressed data, was "knx_frontend-2023.5.2.73247.tar", last modified: Tue May  2 07:58:45 2023, max compression
```

## Comparing `knx_frontend-2023.5.2.143855.tar` & `knx_frontend-2023.5.2.73247.tar`

### file list

```diff
@@ -1,105 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:53.280518 knx_frontend-2023.5.2.143855/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-02 15:11:38.000000 knx_frontend-2023.5.2.143855/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-02 15:11:38.000000 knx_frontend-2023.5.2.143855/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-02 15:15:53.280518 knx_frontend-2023.5.2.143855/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-02 15:11:38.000000 knx_frontend-2023.5.2.143855/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 15:11:55.000000 knx_frontend-2023.5.2.143855/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:53.260518 knx_frontend-2023.5.2.143855/knx_frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/entrypoint-5e4e4dd9.js
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/entrypoint-5e4e4dd9.js.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:53.272518 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/
--rw-r--r--   0 runner    (1001) docker     (123)    40762 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/0af2eb52.js
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/0af2eb52.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    37070 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/0e40d3e9.js
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/0e40d3e9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/0e40d3e9.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    61102 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/4fa1e58d.js
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/4fa1e58d.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13782 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/4fa1e58d.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/749bbd9b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/749bbd9b.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    96196 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/789523e2.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/789523e2.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/789523e2.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/78cd9069.js
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/78cd9069.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/78cd9069.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    18672 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/9080a47b.js
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/9080a47b.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/94794678.js
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/94794678.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)   106486 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/dade42d6.js
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/dade42d6.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/dade42d6.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/ea4e1a95.js
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/ea4e1a95.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/ea4e1a95.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    92699 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/ecca0abf.js
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/ecca0abf.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/ecca0abf.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)  2629940 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/entrypoint-4e598fff.js
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/entrypoint-4e598fff.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   463935 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/entrypoint-4e598fff.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)   231161 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/f0618551.js
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/f0618551.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    41600 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/f0618551.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    47097 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/fc280d00.js
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/fc280d00.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/fc280d00.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:53.280518 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/00e63187.js
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/00e63187.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/00e63187.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    62850 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/230a12b6.js
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/230a12b6.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/230a12b6.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    42152 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/230a12b6.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    48281 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/525c6b8e.js
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/525c6b8e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/525c6b8e.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/525c6b8e.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    63350 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/679a99d6.js
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/679a99d6.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/679a99d6.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    29225 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/679a99d6.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   149257 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/81f2e6ee.js
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/81f2e6ee.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26866 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/81f2e6ee.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    74314 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/81f2e6ee.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/9f79b138.js
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/9f79b138.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-05-02 15:14:22.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/9f79b138.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4a1271f.js
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4a1271f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4a1271f.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    50269 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4b8554f.js
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4b8554f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4b8554f.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    21463 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4b8554f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/c1cea011.js
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/c1cea011.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/c1cea011.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    33490 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/d5e44388.js
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/d5e44388.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/d5e44388.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/e8fee43e.js
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/e8fee43e.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/e9d6c77f.js
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/e9d6c77f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/e9d6c77f.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)   495718 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/entrypoint-5e4e4dd9.js
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/entrypoint-5e4e4dd9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   104670 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/entrypoint-5e4e4dd9.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)   157621 2023-05-02 15:14:21.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/entrypoint-5e4e4dd9.js.map
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 15:14:22.000000 knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:44.000000 knx_frontend-2023.5.2.143855/knx_frontend/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:53.260518 knx_frontend-2023.5.2.143855/knx_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-02 15:15:52.000000 knx_frontend-2023.5.2.143855/knx_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-02 15:15:53.000000 knx_frontend-2023.5.2.143855/knx_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:15:52.000000 knx_frontend-2023.5.2.143855/knx_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 15:15:53.000000 knx_frontend-2023.5.2.143855/knx_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-02 15:11:38.000000 knx_frontend-2023.5.2.143855/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:15:53.280518 knx_frontend-2023.5.2.143855/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:58:45.576756 knx_frontend-2023.5.2.73247/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-02 07:54:55.000000 knx_frontend-2023.5.2.73247/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-02 07:54:55.000000 knx_frontend-2023.5.2.73247/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-02 07:58:45.576756 knx_frontend-2023.5.2.73247/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-02 07:54:55.000000 knx_frontend-2023.5.2.73247/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 07:55:05.000000 knx_frontend-2023.5.2.73247/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:58:45.544756 knx_frontend-2023.5.2.73247/knx_frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-02 07:57:47.000000 knx_frontend-2023.5.2.73247/knx_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-02 07:57:47.000000 knx_frontend-2023.5.2.73247/knx_frontend/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-02 07:57:47.000000 knx_frontend-2023.5.2.73247/knx_frontend/entrypoint-5baef557.js
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-02 07:57:47.000000 knx_frontend-2023.5.2.73247/knx_frontend/entrypoint-5baef557.js.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:58:45.560756 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/
+-rw-r--r--   0 runner    (1001) docker     (123)    40762 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/0af2eb52.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/0af2eb52.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    37070 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/0e40d3e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/0e40d3e9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/0e40d3e9.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    61102 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/4fa1e58d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/4fa1e58d.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13782 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/4fa1e58d.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/749bbd9b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/749bbd9b.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    96196 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/789523e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/789523e2.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/789523e2.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/78cd9069.js
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/78cd9069.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/78cd9069.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    18672 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/9080a47b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/9080a47b.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/94794678.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/94794678.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    92707 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/bd85fc7a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/bd85fc7a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/bd85fc7a.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   106486 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/dade42d6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/dade42d6.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/dade42d6.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/ea4e1a95.js
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/ea4e1a95.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/ea4e1a95.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  2629940 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/entrypoint-48b69fdd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/entrypoint-48b69fdd.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   463924 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/entrypoint-48b69fdd.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   231161 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/f0618551.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/f0618551.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    41600 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/f0618551.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    47097 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/fc280d00.js
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/fc280d00.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/fc280d00.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 07:57:46.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:58:45.576756 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/00e63187.js
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/00e63187.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/00e63187.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    62850 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/230a12b6.js
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/230a12b6.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/230a12b6.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42152 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/230a12b6.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    48281 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/525c6b8e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/525c6b8e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/525c6b8e.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/525c6b8e.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   149257 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/81f2e6ee.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/81f2e6ee.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26866 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/81f2e6ee.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    74314 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/81f2e6ee.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    63358 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/9cd92628.js
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/9cd92628.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/9cd92628.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/9cd92628.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/9f79b138.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/9f79b138.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/9f79b138.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4a1271f.js
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4a1271f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4a1271f.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    50269 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4b8554f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4b8554f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4b8554f.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    21463 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4b8554f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/c1cea011.js
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/c1cea011.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/c1cea011.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    33490 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/d5e44388.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/d5e44388.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/d5e44388.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/e8fee43e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/e8fee43e.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/e9d6c77f.js
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/e9d6c77f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/e9d6c77f.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   495718 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/entrypoint-5baef557.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/entrypoint-5baef557.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   104726 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/entrypoint-5baef557.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   157621 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/entrypoint-5baef557.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 07:57:28.000000 knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:58:45.576756 knx_frontend-2023.5.2.73247/knx_frontend/knx_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-02 07:58:44.000000 knx_frontend-2023.5.2.73247/knx_frontend/knx_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-02 07:58:45.000000 knx_frontend-2023.5.2.73247/knx_frontend/knx_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:58:44.000000 knx_frontend-2023.5.2.73247/knx_frontend/knx_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-02 07:58:45.000000 knx_frontend-2023.5.2.73247/knx_frontend/knx_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-02 07:54:55.000000 knx_frontend-2023.5.2.73247/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 07:58:45.576756 knx_frontend-2023.5.2.73247/setup.cfg
```

### Comparing `knx_frontend-2023.5.2.143855/LICENSE` & `knx_frontend-2023.5.2.73247/LICENSE`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/PKG-INFO` & `knx_frontend-2023.5.2.73247/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: knx_frontend
-Version: 2023.5.2.143855
+Version: 2023.5.2.73247
 Summary: KNX panel for Home Assistant
-Author-email: Marvin Wichmann <me@marvin-wichmann.de>, Matthias Alphart <farmio@alphart.net>
+Author-email: Marvin Wichmann <me@marvin-wichmann.de>
 License: MIT License
-Project-URL: Repository, https://github.com/XKNX/knx-frontend.git
+Project-URL: homepage, https://github.com/XKNX/knx-frontend
 Keywords: Home Assistant,KNX
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KNX UI
```

### Comparing `knx_frontend-2023.5.2.143855/README.md` & `knx_frontend-2023.5.2.73247/README.md`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/0af2eb52.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/0af2eb52.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/0af2eb52.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/0af2eb52.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/0e40d3e9.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/0e40d3e9.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/0e40d3e9.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/0e40d3e9.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/4fa1e58d.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/4fa1e58d.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/4fa1e58d.js.LICENSE.txt` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/4fa1e58d.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/4fa1e58d.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/4fa1e58d.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/749bbd9b.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/749bbd9b.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/749bbd9b.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/749bbd9b.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/789523e2.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/789523e2.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/789523e2.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/789523e2.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/78cd9069.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/78cd9069.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/78cd9069.js.LICENSE.txt` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/78cd9069.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/78cd9069.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/78cd9069.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/9080a47b.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/9080a47b.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/9080a47b.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/9080a47b.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/94794678.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/94794678.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/94794678.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/94794678.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/dade42d6.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/dade42d6.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/dade42d6.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/dade42d6.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/ea4e1a95.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/ea4e1a95.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/ea4e1a95.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/ea4e1a95.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/ecca0abf.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/bd85fc7a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see ecca0abf.js.LICENSE.txt */
+/*! For license information please see bd85fc7a.js.LICENSE.txt */
 "use strict";
 (self.webpackChunkknx_frontend = self.webpackChunkknx_frontend || []).push([
     [428], {
         87428: function(e, t, r) {
             r.r(t), r.d(t, {
                 KNXOverview: function() {
                     return Lt
@@ -3197,15 +3197,15 @@
                                 this.loadKnxInfo()
                             }
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
                                 var e, t, r, n, o;
-                                return this.knxInfo ? (0, i.dy)(it || (it = bt(['\n      <div class="columns">\n        <ha-card class="knx-info" header="KNX Information">\n          <div class="card-content knx-info-section">\n            <div class="knx-content-row">\n              <div>XKNX Version</div>\n              <div>', '</div>\n            </div>\n\n            <div class="knx-content-row">\n              <div>KNX Frontend Version</div>\n              <div>', '</div>\n            </div>\n\n            <div class="knx-content-row">\n              <div>', "</div>\n              <div>", '</div>\n            </div>\n\n            <div class="knx-content-row">\n              <div>', "</div>\n              <div>", '</div>\n            </div>\n\n            <div class="knx-bug-report">\n              <div>', '</div>\n              <ul>\n                <li>\n                  <a href="https://github.com/XKNX/knx-frontend/issues" target="_blank"\n                    >', '</a\n                  >\n                </li>\n                <li>\n                  <a href="https://github.com/XKNX/xknxproject/issues" target="_blank"\n                    >', '</a\n                  >\n                </li>\n                <li>\n                  <a href="https://github.com/XKNX/xknx/issues" target="_blank"\n                    >', "</a\n                  >\n                </li>\n              </ul>\n            </div>\n          </div>\n        </ha-card>\n        ", '\n        <ha-card\n          class="knx-info"\n          .header=', '\n        >\n          <div class="knx-project-description">\n            ', '\n          </div>\n          <div class="knx-content-row">\n            <ha-file-upload\n              .hass=', '\n              accept=".knxproj"\n              .icon=', "\n              .label=", "\n              .value=", "\n              .uploading=", "\n              @file-picked=", '\n            ></ha-file-upload>\n          </div>\n          <div class="knx-content-row">\n            <ha-selector-text\n              .hass=', "\n              .value=", "\n              .label=", "\n              .selector=", "\n              .required=", "\n              @value-changed=", '\n            >\n            </ha-selector-text>\n          </div>\n          <div class="knx-content-button">\n            <ha-button @click=', " .disabled=", "\n              >", "</ha-button\n            >\n          </div>\n        </ha-card>\n      </div>\n    "])), null === (e = this.knxInfo) || void 0 === e ? void 0 : e.version, "2023.5.2.143855", (0, ft.N)(this.hass.language, "overview_connected_to_bus"), null !== (t = this.knxInfo) && void 0 !== t && t.connected ? "Yes" : "No", (0, ft.N)(this.hass.language, "overview_individual_address"), null === (r = this.knxInfo) || void 0 === r ? void 0 : r.current_address, (0, ft.N)(this.hass.language, "overview_issue_tracker"), (0, ft.N)(this.hass.language, "overview_issue_tracker_knx_frontend"), (0, ft.N)(this.hass.language, "overview_issue_tracker_xknxproject"), (0, ft.N)(this.hass.language, "overview_issue_tracker_xknx"), null !== (n = this.knxInfo) && void 0 !== n && n.project ? this._projectCard(this.knxInfo.project) : i.Ld, (0, ft.N)(this.hass.language, "overview_project_file_header"), (0, ft.N)(this.hass.language, "overview_project_upload_description"), this.hass, "M14,2H6A2,2 0 0,0 4,4V20A2,2 0 0,0 6,22H18A2,2 0 0,0 20,20V8L14,2M13.5,16V19H10.5V16H8L12,12L16,16H13.5M13,9V3.5L18.5,9H13Z", (0, ft.N)(this.hass.language, "overview_project_file"), null === (o = this._projectFile) || void 0 === o ? void 0 : o.name, this._uploading, this._filePicked, this.hass, this._projectPassword || "", (0, ft.N)(this.hass.language, "overview_project_password"), {
+                                return this.knxInfo ? (0, i.dy)(it || (it = bt(['\n      <div class="columns">\n        <ha-card class="knx-info" header="KNX Information">\n          <div class="card-content knx-info-section">\n            <div class="knx-content-row">\n              <div>XKNX Version</div>\n              <div>', '</div>\n            </div>\n\n            <div class="knx-content-row">\n              <div>KNX Frontend Version</div>\n              <div>', '</div>\n            </div>\n\n            <div class="knx-content-row">\n              <div>', "</div>\n              <div>", '</div>\n            </div>\n\n            <div class="knx-content-row">\n              <div>', "</div>\n              <div>", '</div>\n            </div>\n\n            <div class="knx-bug-report">\n              <div>', '</div>\n              <ul>\n                <li>\n                  <a href="https://github.com/XKNX/knx-frontend/issues" target="_blank"\n                    >', '</a\n                  >\n                </li>\n                <li>\n                  <a href="https://github.com/XKNX/knx-frontend/issues" target="_blank"\n                    >', '</a\n                  >\n                </li>\n                <li>\n                  <a href="https://github.com/XKNX/knx-frontend/issues" target="_blank"\n                    >', "</a\n                  >\n                </li>\n              </ul>\n            </div>\n          </div>\n        </ha-card>\n        ", '\n        <ha-card\n          class="knx-info"\n          .header=', '\n        >\n          <div class="knx-project-description">\n            ', '\n          </div>\n          <div class="knx-content-row">\n            <ha-file-upload\n              .hass=', '\n              accept=".knxproj"\n              .icon=', "\n              .label=", "\n              .value=", "\n              .uploading=", "\n              @file-picked=", '\n            ></ha-file-upload>\n          </div>\n          <div class="knx-content-row">\n            <ha-selector-text\n              .hass=', "\n              .value=", "\n              .label=", "\n              .selector=", "\n              .required=", "\n              @value-changed=", '\n            >\n            </ha-selector-text>\n          </div>\n          <div class="knx-content-button">\n            <ha-button @click=', " .disabled=", "\n              >", "</ha-button\n            >\n          </div>\n        </ha-card>\n      </div>\n    "])), null === (e = this.knxInfo) || void 0 === e ? void 0 : e.version, "2023.5.2.73247", (0, ft.N)(this.hass.language, "overview_connected_to_bus"), null !== (t = this.knxInfo) && void 0 !== t && t.connected ? "Yes" : "No", (0, ft.N)(this.hass.language, "overview_individual_address"), null === (r = this.knxInfo) || void 0 === r ? void 0 : r.current_address, (0, ft.N)(this.hass.language, "overview_issue_tracker"), (0, ft.N)(this.hass.language, "overview_issue_tracker_knx_frontend"), (0, ft.N)(this.hass.language, "overview_issue_tracker_xknxproject"), (0, ft.N)(this.hass.language, "overview_issue_tracker_xknx"), null !== (n = this.knxInfo) && void 0 !== n && n.project ? this._projectCard(this.knxInfo.project) : i.Ld, (0, ft.N)(this.hass.language, "overview_project_file_header"), (0, ft.N)(this.hass.language, "overview_project_upload_description"), this.hass, "M14,2H6A2,2 0 0,0 4,4V20A2,2 0 0,0 6,22H18A2,2 0 0,0 20,20V8L14,2M13.5,16V19H10.5V16H8L12,12L16,16H13.5M13,9V3.5L18.5,9H13Z", (0, ft.N)(this.hass.language, "overview_project_file"), null === (o = this._projectFile) || void 0 === o ? void 0 : o.name, this._uploading, this._filePicked, this.hass, this._projectPassword || "", (0, ft.N)(this.hass.language, "overview_project_password"), {
                                     text: {
                                         multiline: !1,
                                         type: "password"
                                     }
                                 }, !1, this._passwordChanged, this._uploadFile, this._uploading || !this._projectFile, (0, ft.N)(this.hass.language, "overview_project_upload")) : (0, i.dy)(nt || (nt = bt(["Loading..."])))
                             }
                         }, {
```

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/entrypoint-4e598fff.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/entrypoint-48b69fdd.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see entrypoint-4e598fff.js.LICENSE.txt */ ! function() {
+/*! For license information please see entrypoint-48b69fdd.js.LICENSE.txt */ ! function() {
     var e, t, r, n, o = {
             47715: function(e, t, r) {
                 "use strict";
                 r.d(t, {
                     i: function() {
                         return n
                     }
@@ -49052,15 +49052,15 @@
                 return a.f[r](e, t), t
             }), []))
         }, a.u = function(e) {
             return {
                 95: "94794678",
                 182: "9080a47b",
                 384: "749bbd9b",
-                428: "ecca0abf",
+                428: "bd85fc7a",
                 442: "78cd9069",
                 525: "f0618551",
                 582: "789523e2",
                 588: "4fa1e58d",
                 663: "0e40d3e9",
                 813: "0af2eb52",
                 837: "dade42d6",
```

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/entrypoint-4e598fff.js.LICENSE.txt` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/entrypoint-48b69fdd.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/f0618551.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/f0618551.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/f0618551.js.LICENSE.txt` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/f0618551.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/f0618551.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/f0618551.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/fc280d00.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/fc280d00.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_es5/fc280d00.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_es5/fc280d00.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/00e63187.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/00e63187.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/00e63187.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/00e63187.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/230a12b6.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/230a12b6.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/230a12b6.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/230a12b6.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/230a12b6.js.map` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/230a12b6.js.map`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/525c6b8e.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/525c6b8e.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/525c6b8e.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/525c6b8e.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/525c6b8e.js.map` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/525c6b8e.js.map`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/679a99d6.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/9cd92628.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 679a99d6.js.LICENSE.txt */
+/*! For license information please see 9cd92628.js.LICENSE.txt */
 "use strict";
 (self.webpackChunkknx_frontend = self.webpackChunkknx_frontend || []).push([
     [428], {
         7428: (e, t, r) => {
             r.r(t), r.d(t, {
                 KNXOverview: () => ge
             });
@@ -143,15 +143,15 @@
                             var t = this.toElementDescriptor(e);
                             return this.disallowProperty(e, "finisher", "An element descriptor"), this.disallowProperty(e, "extras", "An element descriptor"), t
                         }), this)
                     },
                     toElementDescriptor: function(e) {
                         var t = String(e.kind);
                         if ("method" !== t && "field" !== t) throw new TypeError('An element descriptor\'s .kind property must be either "method" or "field", but a decorator created an element descriptor with .kind "' + t + '"');
-                        var r = f(e.key),
+                        var r = u(e.key),
                             i = String(e.placement);
                         if ("static" !== i && "prototype" !== i && "own" !== i) throw new TypeError('An element descriptor\'s .placement property must be one of "static", "prototype" or "own", but a decorator created an element descriptor with .placement "' + i + '"');
                         var n = e.descriptor;
                         this.disallowProperty(e, "elements", "An element descriptor");
                         var o = {
                             kind: t,
                             key: r,
@@ -159,15 +159,15 @@
                             descriptor: Object.assign({}, n)
                         };
                         return "field" !== t ? this.disallowProperty(e, "initializer", "A method descriptor") : (this.disallowProperty(n, "get", "The property descriptor of a field descriptor"), this.disallowProperty(n, "set", "The property descriptor of a field descriptor"), this.disallowProperty(n, "value", "The property descriptor of a field descriptor"), o.initializer = e.initializer), o
                     },
                     toElementFinisherExtras: function(e) {
                         return {
                             element: this.toElementDescriptor(e),
-                            finisher: u(e, "finisher"),
+                            finisher: f(e, "finisher"),
                             extras: this.toElementDescriptors(e.extras)
                         }
                     },
                     fromClassDescriptor: function(e) {
                         var t = {
                             kind: "class",
                             elements: e.map(this.fromElementDescriptor, this)
@@ -177,15 +177,15 @@
                             configurable: !0
                         }), t
                     },
                     toClassDescriptor: function(e) {
                         var t = String(e.kind);
                         if ("class" !== t) throw new TypeError('A class descriptor\'s .kind property must be "class", but a decorator created a class descriptor with .kind "' + t + '"');
                         this.disallowProperty(e, "key", "A class descriptor"), this.disallowProperty(e, "placement", "A class descriptor"), this.disallowProperty(e, "descriptor", "A class descriptor"), this.disallowProperty(e, "initializer", "A class descriptor"), this.disallowProperty(e, "extras", "A class descriptor");
-                        var r = u(e, "finisher");
+                        var r = f(e, "finisher");
                         return {
                             elements: this.toElementDescriptors(e.elements),
                             finisher: r
                         }
                     },
                     runClassFinishers: function(e, t) {
                         for (var r = 0; r < t.length; r++) {
@@ -201,15 +201,15 @@
                         if (void 0 !== e[t]) throw new TypeError(r + " can't have a ." + t + " property.")
                     }
                 };
                 return e
             }
 
             function l(e) {
-                var t, r = f(e.key);
+                var t, r = u(e.key);
                 "method" === e.kind ? t = {
                     value: e.value,
                     writable: !0,
                     configurable: !0,
                     enumerable: !1
                 } : "get" === e.kind ? t = {
                     get: e.value,
@@ -241,21 +241,21 @@
                 return e.decorators && e.decorators.length
             }
 
             function p(e) {
                 return void 0 !== e && !(void 0 === e.value && void 0 === e.writable)
             }
 
-            function u(e, t) {
+            function f(e, t) {
                 var r = e[t];
                 if (void 0 !== r && "function" != typeof r) throw new TypeError("Expected '" + t + "' to be a function");
                 return r
             }
 
-            function f(e) {
+            function u(e) {
                 var t = function(e, t) {
                     if ("object" != typeof e || null === e) return e;
                     var r = e[Symbol.toPrimitive];
                     if (void 0 !== r) {
                         var i = r.call(e, t || "default");
                         if ("object" != typeof i) return i;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
@@ -270,17 +270,17 @@
                 for (var r = 0, i = new Array(t); r < t; r++) i[r] = e[r];
                 return i
             }! function(e, t, r, i) {
                 var n = s();
                 if (i)
                     for (var o = 0; o < i.length; o++) n = i[o](n);
                 var a = t((function(e) {
-                        n.initializeInstanceElements(e, u.elements)
+                        n.initializeInstanceElements(e, f.elements)
                     }), r),
-                    u = n.decorateClass(function(e) {
+                    f = n.decorateClass(function(e) {
                         for (var t = [], r = function(e) {
                                 return "method" === e.kind && e.key === o.key && e.placement === o.placement
                             }, i = 0; i < e.length; i++) {
                             var n, o = e[i];
                             if ("method" === o.kind && (n = t.find(r)))
                                 if (p(o.descriptor) || p(n.descriptor)) {
                                     if (c(o) || c(n)) throw new ReferenceError("Duplicated methods (" + o.key + ") can't be decorated.");
@@ -292,15 +292,15 @@
                                     }
                                     d(o, n)
                                 }
                             else t.push(o)
                         }
                         return t
                     }(a.d.map(l)), e);
-                n.initializeClassElements(a.F, u.elements), n.runClassFinishers(a.F, u.finishers)
+                n.initializeClassElements(a.F, f.elements), n.runClassFinishers(a.F, f.finishers)
             }([(0, n.Mo)("ha-button")], (function(e, t) {
                 return {
                     F: class extends t {
                         constructor(...t) {
                             super(...t), e(this)
                         }
                     },
@@ -1830,15 +1830,15 @@
                                 static: [],
                                 prototype: [],
                                 own: []
                             };
                         if (e.forEach((function(e) {
                                 this.addElementPlacement(e, n)
                             }), this), e.forEach((function(e) {
-                                if (!fe(e)) return r.push(e);
+                                if (!ue(e)) return r.push(e);
                                 var t = this.decorateElement(e, n);
                                 r.push(t.element), r.push.apply(r, t.extras), i.push.apply(i, t.finishers)
                             }), this), !t) return {
                             elements: r,
                             finishers: i
                         };
                         var o = this.decorateConstructor(r, t);
@@ -2000,19 +2000,19 @@
                     key: r,
                     placement: e.static ? "static" : "field" === e.kind ? "own" : "prototype",
                     descriptor: t
                 };
                 return e.decorators && (i.decorators = e.decorators), "field" === e.kind && (i.initializer = e.value), i
             }
 
-            function ue(e, t) {
+            function fe(e, t) {
                 void 0 !== e.descriptor.get ? t.descriptor.get = e.descriptor.get : t.descriptor.set = e.descriptor.set
             }
 
-            function fe(e) {
+            function ue(e) {
                 return e.decorators && e.decorators.length
             }
 
             function he(e) {
                 return void 0 !== e && !(void 0 === e.value && void 0 === e.writable)
             }
 
@@ -2052,22 +2052,22 @@
                     s = n.decorateClass(function(e) {
                         for (var t = [], r = function(e) {
                                 return "method" === e.kind && e.key === o.key && e.placement === o.placement
                             }, i = 0; i < e.length; i++) {
                             var n, o = e[i];
                             if ("method" === o.kind && (n = t.find(r)))
                                 if (he(o.descriptor) || he(n.descriptor)) {
-                                    if (fe(o) || fe(n)) throw new ReferenceError("Duplicated methods (" + o.key + ") can't be decorated.");
+                                    if (ue(o) || ue(n)) throw new ReferenceError("Duplicated methods (" + o.key + ") can't be decorated.");
                                     n.descriptor = o.descriptor
                                 } else {
-                                    if (fe(o)) {
-                                        if (fe(n)) throw new ReferenceError("Decorators can't be placed on different accessors with for the same property (" + o.key + ").");
+                                    if (ue(o)) {
+                                        if (ue(n)) throw new ReferenceError("Decorators can't be placed on different accessors with for the same property (" + o.key + ").");
                                         n.decorators = o.decorators
                                     }
-                                    ue(o, n)
+                                    fe(o, n)
                                 }
                             else t.push(o)
                         }
                         return t
                     }(a.d.map(pe)), e);
                 return n.initializeClassElements(a.F, s.elements), n.runClassFinishers(a.F, s.finishers)
             }([(0, n.Mo)("knx-overview")], (function(e, t) {
@@ -2130,15 +2130,15 @@
             <div class="knx-content-row">
               <div>XKNX Version</div>
               <div>${null===(e=this.knxInfo)||void 0===e?void 0:e.version}</div>
             </div>
 
             <div class="knx-content-row">
               <div>KNX Frontend Version</div>
-              <div>${"2023.5.2.143855"}</div>
+              <div>${"2023.5.2.73247"}</div>
             </div>
 
             <div class="knx-content-row">
               <div>${(0,le.N)(this.hass.language,"overview_connected_to_bus")}</div>
               <div>${null!==(t=this.knxInfo)&&void 0!==t&&t.connected?"Yes":"No"}</div>
             </div>
 
@@ -2152,20 +2152,20 @@
               <ul>
                 <li>
                   <a href="https://github.com/XKNX/knx-frontend/issues" target="_blank"
                     >${(0,le.N)(this.hass.language,"overview_issue_tracker_knx_frontend")}</a
                   >
                 </li>
                 <li>
-                  <a href="https://github.com/XKNX/xknxproject/issues" target="_blank"
+                  <a href="https://github.com/XKNX/knx-frontend/issues" target="_blank"
                     >${(0,le.N)(this.hass.language,"overview_issue_tracker_xknxproject")}</a
                   >
                 </li>
                 <li>
-                  <a href="https://github.com/XKNX/xknx/issues" target="_blank"
+                  <a href="https://github.com/XKNX/knx-frontend/issues" target="_blank"
                     >${(0,le.N)(this.hass.language,"overview_issue_tracker_xknx")}</a
                   >
                 </li>
               </ul>
             </div>
           </div>
         </ha-card>
@@ -2411,8 +2411,8 @@
                         }
                     }]
                 }
             }), i.oi)
         }
     }
 ]);
-//# sourceMappingURL=679a99d6.js.map
+//# sourceMappingURL=9cd92628.js.map
```

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/679a99d6.js.map` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/9cd92628.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8968253968253969%*

 * *Differences: {"'file'": "'9cd92628.js'",*

 * * "'sourcesContent'": '{insert: [(5, \'import { mdiFileUpload } from "@mdi/js";\\nimport { css, '*

 * *                     'nothing, html, LitElement, TemplateResult } from "lit";\\nimport { '*

 * *                     'customElement, property, state } from "lit/decorators";\\n\\nimport '*

 * *                     '"@ha/components/ha-button-menu";\\nimport "@ha/components/ha-card";\\nimport '*

 * *                     '"@ha/layouts/ha-app-layout";\\nimport "@ha/layouts/hass-subpage";\\nimport '*

 * *     […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "679a99d6.js",
+    "file": "9cd92628.js",
     "mappings": ";;;;;;;AAgBA;AC8BA;;;;AAKA;;;AAIA;AAKA;AACA;AACA;AACA;AACA;;;;AAIA;;AAIA;;AAEA;;;;AAKA;AACA;;AAEA;AAEA;;;;;AAKA;AACA;;;AAGA;;;;;AAMA;AACA;AApGA;;AAwGA;;AAGA;;;;AAOA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA+GA;AC1JA;AACA;AACA;AACA;AACA;AACA;;AAGA;AAGA;;AAeA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AAEA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACtDA;ACzBA;AACA;AACA;AACA;AACA;;AAEA;AACA;;AAEA;;AAEA;;AAIA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AAIA;AACA;;AAEA;;AAGA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;AA0CA;;;;;;AC9DA;;;;;ACrDA;;;;AD8DA;AACA;;;;AAIA;AACA;;;;AAIA;;;;AAIA;;;;;AAKA;;;;;AAKA;;;;;;;AAOA;;;AAGA;;;AAGA;;;;AAIA;;;AAGA;AACA;AACA;AACA;;;;;AAKA;AACA;AACA;AACA;AACA;AACA;;;;;AAKA;AACA;;;;;AAjFA;;;AA6FA;;;;AAIA;AACA;;;AAGA;AACA;;;AAGA;AACA;;;;;;AAMA;AACA;AACA;;;;AAKA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA4JA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://knx-frontend/./homeassistant-frontend/src/components/ha-button.ts",
         "webpack://knx-frontend/./homeassistant-frontend/src/components/ha-file-upload.ts",
         "webpack://knx-frontend/mwc-textarea-base.ts",
@@ -14,12 +14,12 @@
     ],
     "sourcesContent": [
         "import { Button } from \"@material/mwc-button\";\nimport { css } from \"lit\";\nimport { customElement } from \"lit/decorators\";\nimport { styles } from \"@material/mwc-button/styles.css\";\n\n@customElement(\"ha-button\")\nexport class HaButton extends Button {\n  static override styles = [\n    styles,\n    css`\n      ::slotted([slot=\"icon\"]) {\n        margin-inline-start: 0px;\n        margin-inline-end: 8px;\n        direction: var(--direction);\n      }\n    `,\n  ];\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-button\": HaButton;\n  }\n}\n",
         "import { styles } from \"@material/mwc-textfield/mwc-textfield.css\";\nimport { mdiClose } from \"@mdi/js\";\nimport { css, html, LitElement, PropertyValues, TemplateResult } from \"lit\";\nimport { customElement, property, query, state } from \"lit/decorators\";\nimport { classMap } from \"lit/directives/class-map\";\nimport { fireEvent } from \"../common/dom/fire_event\";\nimport { HomeAssistant } from \"../types\";\nimport \"./ha-circular-progress\";\nimport \"./ha-icon-button\";\n\ndeclare global {\n  interface HASSDomEvents {\n    \"file-picked\": { files: FileList };\n  }\n}\n\n@customElement(\"ha-file-upload\")\nexport class HaFileUpload extends LitElement {\n  @property({ attribute: false }) public hass?: HomeAssistant;\n\n  @property() public accept!: string;\n\n  @property() public icon?: string;\n\n  @property() public label!: string;\n\n  @property() public value: string | TemplateResult | null = null;\n\n  @property({ type: Boolean }) private uploading = false;\n\n  @property({ type: Boolean, attribute: \"auto-open-file-dialog\" })\n  private autoOpenFileDialog = false;\n\n  @state() private _drag = false;\n\n  @query(\"#input\") private _input?: HTMLInputElement;\n\n  protected firstUpdated(changedProperties: PropertyValues) {\n    super.firstUpdated(changedProperties);\n    if (this.autoOpenFileDialog) {\n      this._openFilePicker();\n    }\n  }\n\n  public render(): TemplateResult {\n    return html`\n      ${this.uploading\n        ? html`<ha-circular-progress\n            alt=\"Uploading\"\n            size=\"large\"\n            active\n          ></ha-circular-progress>`\n        : html`\n            <label\n              for=\"input\"\n              class=\"mdc-text-field mdc-text-field--filled ${classMap({\n                \"mdc-text-field--focused\": this._drag,\n                \"mdc-text-field--with-leading-icon\": Boolean(this.icon),\n                \"mdc-text-field--with-trailing-icon\": Boolean(this.value),\n              })}\"\n              @drop=${this._handleDrop}\n              @dragenter=${this._handleDragStart}\n              @dragover=${this._handleDragStart}\n              @dragleave=${this._handleDragEnd}\n              @dragend=${this._handleDragEnd}\n            >\n              <span class=\"mdc-text-field__ripple\"></span>\n              <span\n                class=\"mdc-floating-label ${this.value || this._drag\n                  ? \"mdc-floating-label--float-above\"\n                  : \"\"}\"\n                id=\"label\"\n                >${this.label}</span\n              >\n              ${this.icon\n                ? html`<span\n                    class=\"mdc-text-field__icon mdc-text-field__icon--leading\"\n                  >\n                    <ha-icon-button\n                      @click=${this._openFilePicker}\n                      .path=${this.icon}\n                    ></ha-icon-button>\n                  </span>`\n                : \"\"}\n              <div class=\"value\">${this.value}</div>\n              <input\n                id=\"input\"\n                type=\"file\"\n                class=\"mdc-text-field__input file\"\n                accept=${this.accept}\n                @change=${this._handleFilePicked}\n                aria-labelledby=\"label\"\n              />\n              ${this.value\n                ? html`<span\n                    class=\"mdc-text-field__icon mdc-text-field__icon--trailing\"\n                  >\n                    <ha-icon-button\n                      slot=\"suffix\"\n                      @click=${this._clearValue}\n                      .label=${this.hass?.localize(\"ui.common.close\") ||\n                      \"close\"}\n                      .path=${mdiClose}\n                    ></ha-icon-button>\n                  </span>`\n                : \"\"}\n              <span\n                class=\"mdc-line-ripple ${this._drag\n                  ? \"mdc-line-ripple--active\"\n                  : \"\"}\"\n              ></span>\n            </label>\n          `}\n    `;\n  }\n\n  private _openFilePicker() {\n    this._input?.click();\n  }\n\n  private _handleDrop(ev: DragEvent) {\n    ev.preventDefault();\n    ev.stopPropagation();\n    if (ev.dataTransfer?.files) {\n      fireEvent(this, \"file-picked\", { files: ev.dataTransfer.files });\n    }\n    this._drag = false;\n  }\n\n  private _handleDragStart(ev: DragEvent) {\n    ev.preventDefault();\n    ev.stopPropagation();\n    this._drag = true;\n  }\n\n  private _handleDragEnd(ev: DragEvent) {\n    ev.preventDefault();\n    ev.stopPropagation();\n    this._drag = false;\n  }\n\n  private _handleFilePicked(ev) {\n    fireEvent(this, \"file-picked\", { files: ev.target.files });\n  }\n\n  private _clearValue(ev: Event) {\n    ev.preventDefault();\n    this.value = null;\n    fireEvent(this, \"change\");\n  }\n\n  static get styles() {\n    return [\n      styles,\n      css`\n        :host {\n          display: block;\n        }\n        .mdc-text-field--filled {\n          height: auto;\n          padding-top: 16px;\n          cursor: pointer;\n        }\n        .mdc-text-field--filled.mdc-text-field--with-trailing-icon {\n          padding-top: 28px;\n        }\n        .mdc-text-field:not(.mdc-text-field--disabled) .mdc-text-field__icon {\n          color: var(--secondary-text-color);\n        }\n        .mdc-text-field--filled.mdc-text-field--with-trailing-icon\n          .mdc-text-field__icon {\n          align-self: flex-end;\n        }\n        .mdc-text-field__icon--leading {\n          margin-bottom: 12px;\n          inset-inline-start: initial;\n          inset-inline-end: 0px;\n          direction: var(--direction);\n        }\n        .mdc-text-field--filled .mdc-floating-label--float-above {\n          transform: scale(0.75);\n          top: 8px;\n        }\n        .mdc-floating-label {\n          inset-inline-start: 16px !important;\n          inset-inline-end: initial !important;\n          direction: var(--direction);\n        }\n        .mdc-text-field--filled .mdc-floating-label {\n          inset-inline-start: 48px !important;\n          inset-inline-end: initial !important;\n          direction: var(--direction);\n        }\n        .dragged:before {\n          position: var(--layout-fit_-_position);\n          top: var(--layout-fit_-_top);\n          right: var(--layout-fit_-_right);\n          bottom: var(--layout-fit_-_bottom);\n          left: var(--layout-fit_-_left);\n          background: currentColor;\n          content: \"\";\n          opacity: var(--dark-divider-opacity);\n          pointer-events: none;\n          border-radius: 4px;\n        }\n        .value {\n          width: 100%;\n        }\n        input.file {\n          display: none;\n        }\n        img {\n          max-width: 100%;\n          max-height: 125px;\n        }\n        ha-icon-button {\n          --mdc-icon-button-size: 24px;\n          --mdc-icon-size: 20px;\n        }\n        ha-circular-progress {\n          display: block;\n          text-align-last: center;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-file-upload\": HaFileUpload;\n  }\n}\n",
         "/**\n * @license\n * Copyright 2019 Google LLC\n * SPDX-License-Identifier: Apache-2.0\n */\n\n// Style preference for leading underscores.\n// tslint:disable:strip-private-property-underscore\n\n\nimport {TextAreaCharCounter, TextFieldBase, TextFieldInputMode, TextFieldType} from '@material/mwc-textfield/mwc-textfield-base.js';\nimport {ComplexAttributeConverter, html, TemplateResult} from 'lit';\nimport {property, query} from 'lit/decorators.js';\nimport {classMap} from 'lit/directives/class-map.js';\nimport {ifDefined} from 'lit/directives/if-defined.js';\nimport {live} from 'lit/directives/live.js';\n\nexport {TextAreaCharCounter, TextFieldInputMode, TextFieldType};\n\nconst booleanOrStringConverter: ComplexAttributeConverter<boolean|string> = {\n  fromAttribute(value) {\n    if (value === null) {\n      return false;\n    } else if (value === '') {\n      return true;\n    }\n\n    return value;\n  },\n  toAttribute(value) {\n    if (typeof value === 'boolean') {\n      return value ? '' : null;\n    }\n\n    return value;\n  }\n};\n\n/** @soyCompatible */\nexport abstract class TextAreaBase extends TextFieldBase {\n  @query('textarea') protected override formElement!: HTMLInputElement;\n\n  @property({type: Number}) rows = 2;\n\n  @property({type: Number}) cols = 20;\n\n  @property({converter: booleanOrStringConverter})\n  override charCounter: boolean|TextAreaCharCounter = false;\n\n  /** @soyTemplate */\n  override render(): TemplateResult {\n    const shouldRenderCharCounter = this.charCounter && this.maxLength !== -1;\n    const shouldRenderInternalCharCounter =\n        shouldRenderCharCounter && this.charCounter === 'internal';\n    const shouldRenderExternalCharCounter =\n        shouldRenderCharCounter && !shouldRenderInternalCharCounter;\n    const shouldRenderHelperText = !!this.helper || !!this.validationMessage ||\n        shouldRenderExternalCharCounter;\n\n    /** @classMap */\n    const classes = {\n      'mdc-text-field--disabled': this.disabled,\n      'mdc-text-field--no-label': !this.label,\n      'mdc-text-field--filled': !this.outlined,\n      'mdc-text-field--outlined': this.outlined,\n      'mdc-text-field--end-aligned': this.endAligned,\n      'mdc-text-field--with-internal-counter': shouldRenderInternalCharCounter,\n    };\n\n    return html`\n      <label class=\"mdc-text-field mdc-text-field--textarea ${\n        classMap(classes)}\">\n        ${this.renderRipple()}\n        ${this.outlined ? this.renderOutline() : this.renderLabel()}\n        ${this.renderInput()}\n        ${this.renderCharCounter(shouldRenderInternalCharCounter)}\n        ${this.renderLineRipple()}\n      </label>\n      ${\n        this.renderHelperText(\n            shouldRenderHelperText, shouldRenderExternalCharCounter)}\n    `;\n  }\n\n  /** @soyTemplate */\n  protected override renderInput(): TemplateResult {\n    const ariaLabelledbyOrUndef = !!this.label ? 'label' : undefined;\n    const minOrUndef = this.minLength === -1 ? undefined : this.minLength;\n    const maxOrUndef = this.maxLength === -1 ? undefined : this.maxLength;\n    const autocapitalizeOrUndef = this.autocapitalize ?\n        (this.autocapitalize as 'off' | 'none' | 'on' | 'sentences' | 'words' |\n         'characters' | 'off' | 'none' | 'on' | 'sentences' | 'words' |\n         'characters') :\n        undefined;\n\n    return html`\n      <textarea\n          aria-labelledby=${ifDefined(ariaLabelledbyOrUndef)}\n          class=\"mdc-text-field__input\"\n          .value=\"${live(this.value) as unknown as string}\"\n          rows=\"${this.rows}\"\n          cols=\"${this.cols}\"\n          ?disabled=\"${this.disabled}\"\n          placeholder=\"${this.placeholder}\"\n          ?required=\"${this.required}\"\n          ?readonly=\"${this.readOnly}\"\n          minlength=\"${ifDefined(minOrUndef)}\"\n          maxlength=\"${ifDefined(maxOrUndef)}\"\n          name=\"${ifDefined(this.name === '' ? undefined : this.name)}\"\n          inputmode=\"${ifDefined(this.inputMode)}\"\n          autocapitalize=\"${ifDefined(autocapitalizeOrUndef)}\"\n          @input=\"${this.handleInputChange}\"\n          @blur=\"${this.onInputBlur}\">\n      </textarea>`;\n  }\n}\n",
         "import { TextAreaBase } from \"@material/mwc-textarea/mwc-textarea-base\";\nimport { styles as textfieldStyles } from \"@material/mwc-textfield/mwc-textfield.css\";\nimport { styles as textareaStyles } from \"@material/mwc-textarea/mwc-textarea.css\";\nimport { css, PropertyValues } from \"lit\";\nimport { customElement, property } from \"lit/decorators\";\n\n@customElement(\"ha-textarea\")\nexport class HaTextArea extends TextAreaBase {\n  @property({ type: Boolean, reflect: true }) autogrow = false;\n\n  firstUpdated() {\n    super.firstUpdated();\n\n    this.setAttribute(\"dir\", document.dir);\n  }\n\n  updated(changedProperties: PropertyValues) {\n    super.updated(changedProperties);\n    if (this.autogrow && changedProperties.has(\"value\")) {\n      this.mdcRoot.dataset.value = this.value + '=\\u200B\"'; // add a zero-width space to correctly wrap\n    }\n  }\n\n  static override styles = [\n    textfieldStyles,\n    textareaStyles,\n    css`\n      :host([autogrow]) .mdc-text-field {\n        position: relative;\n        min-height: 74px;\n        min-width: 178px;\n        max-height: 200px;\n      }\n      :host([autogrow]) .mdc-text-field:after {\n        content: attr(data-value);\n        margin-top: 23px;\n        margin-bottom: 9px;\n        line-height: 1.5rem;\n        min-height: 42px;\n        padding: 0px 32px 0 16px;\n        letter-spacing: var(\n          --mdc-typography-subtitle1-letter-spacing,\n          0.009375em\n        );\n        visibility: hidden;\n        white-space: pre-wrap;\n      }\n      :host([autogrow]) .mdc-text-field__input {\n        position: absolute;\n        height: calc(100% - 32px);\n      }\n      :host([autogrow]) .mdc-text-field.mdc-text-field--no-label:after {\n        margin-top: 16px;\n        margin-bottom: 16px;\n      }\n      :host([dir=\"rtl\"]) .mdc-floating-label {\n        right: 16px;\n        left: initial;\n      }\n    `,\n  ];\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-textarea\": HaTextArea;\n  }\n}\n",
         "import { mdiEye, mdiEyeOff } from \"@mdi/js\";\nimport { css, CSSResultGroup, html, LitElement } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport { fireEvent } from \"../../common/dom/fire_event\";\nimport { StringSelector } from \"../../data/selector\";\nimport { HomeAssistant } from \"../../types\";\nimport \"../ha-icon-button\";\nimport \"../ha-textarea\";\nimport \"../ha-textfield\";\n\n@customElement(\"ha-selector-text\")\nexport class HaTextSelector extends LitElement {\n  @property() public hass!: HomeAssistant;\n\n  @property() public value?: any;\n\n  @property() public name?: string;\n\n  @property() public label?: string;\n\n  @property() public placeholder?: string;\n\n  @property() public helper?: string;\n\n  @property() public selector!: StringSelector;\n\n  @property({ type: Boolean }) public disabled = false;\n\n  @property({ type: Boolean }) public required = true;\n\n  @state() private _unmaskedPassword = false;\n\n  protected render() {\n    if (this.selector.text?.multiline) {\n      return html`<ha-textarea\n        .name=${this.name}\n        .label=${this.label}\n        .placeholder=${this.placeholder}\n        .value=${this.value || \"\"}\n        .helper=${this.helper}\n        helperPersistent\n        .disabled=${this.disabled}\n        @input=${this._handleChange}\n        autocapitalize=\"none\"\n        .autocomplete=${this.selector.text?.autocomplete}\n        spellcheck=\"false\"\n        .required=${this.required}\n        autogrow\n      ></ha-textarea>`;\n    }\n    return html`<ha-textfield\n        .name=${this.name}\n        .value=${this.value || \"\"}\n        .placeholder=${this.placeholder || \"\"}\n        .helper=${this.helper}\n        helperPersistent\n        .disabled=${this.disabled}\n        .type=${this._unmaskedPassword ? \"text\" : this.selector.text?.type}\n        @input=${this._handleChange}\n        .label=${this.label || \"\"}\n        .suffix=${this.selector.text?.type === \"password\"\n          ? // reserve some space for the icon.\n            html`<div style=\"width: 24px\"></div>`\n          : this.selector.text?.suffix}\n        .required=${this.required}\n        .autocomplete=${this.selector.text?.autocomplete}\n      ></ha-textfield>\n      ${this.selector.text?.type === \"password\"\n        ? html`<ha-icon-button\n            toggles\n            .label=${`${this._unmaskedPassword ? \"Hide\" : \"Show\"} password`}\n            @click=${this._toggleUnmaskedPassword}\n            .path=${this._unmaskedPassword ? mdiEyeOff : mdiEye}\n          ></ha-icon-button>`\n        : \"\"}`;\n  }\n\n  private _toggleUnmaskedPassword(): void {\n    this._unmaskedPassword = !this._unmaskedPassword;\n  }\n\n  private _handleChange(ev) {\n    let value = ev.target.value;\n    if (this.value === value) {\n      return;\n    }\n    if (value === \"\" && !this.required) {\n      value = undefined;\n    }\n\n    fireEvent(this, \"value-changed\", { value });\n  }\n\n  static get styles(): CSSResultGroup {\n    return css`\n      :host {\n        display: block;\n        position: relative;\n      }\n      ha-textarea,\n      ha-textfield {\n        width: 100%;\n      }\n      ha-icon-button {\n        position: absolute;\n        top: 10px;\n        right: 10px;\n        --mdc-icon-button-size: 36px;\n        --mdc-icon-size: 20px;\n        color: var(--secondary-text-color);\n        inset-inline-start: initial;\n        inset-inline-end: 10px;\n        direction: var(--direction);\n      }\n    `;\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-selector-text\": HaTextSelector;\n  }\n}\n",
-        "import { mdiFileUpload } from \"@mdi/js\";\nimport { css, nothing, html, LitElement, TemplateResult } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\n\nimport \"@ha/components/ha-button-menu\";\nimport \"@ha/components/ha-card\";\nimport \"@ha/layouts/ha-app-layout\";\nimport \"@ha/layouts/hass-subpage\";\nimport \"@ha/components/ha-button\";\nimport \"@ha/components/ha-file-upload\";\nimport \"@ha/components/ha-selector/ha-selector-text\";\nimport { uploadFile } from \"@ha/data/file_upload\";\nimport { extractApiErrorMessage } from \"@ha/data/hassio/common\";\nimport { showAlertDialog } from \"@ha/dialogs/generic/show-dialog-box\";\nimport { HomeAssistant } from \"@ha/types\";\n\nimport { getKnxInfo, processProjectFile, removeProjectFile } from \"../services/websocket.service\";\nimport { KNXInfo, KNXProjectInfo } from \"../types/websocket\";\nimport { localize } from \"../localize/localize\";\nimport { KNXLogger } from \"../tools/knx-logger\";\nimport { VERSION } from \"../version\";\n\nconst logger = new KNXLogger(\"overview\");\n\n@customElement(\"knx-overview\")\nexport class KNXOverview extends LitElement {\n  @property({ type: Object }) public hass!: HomeAssistant;\n\n  @property({ type: Boolean, reflect: true }) public narrow!: boolean;\n\n  @state() private knxInfo: KNXInfo | null = null;\n\n  @state() private _projectPassword?: string;\n\n  @state() private _uploading = false;\n\n  @state() private _projectFile?: File;\n\n  protected firstUpdated() {\n    this.loadKnxInfo();\n  }\n\n  protected render(): TemplateResult | void {\n    if (!this.knxInfo) {\n      return html`Loading...`;\n    }\n\n    return html`\n      <div class=\"columns\">\n        <ha-card class=\"knx-info\" header=\"KNX Information\">\n          <div class=\"card-content knx-info-section\">\n            <div class=\"knx-content-row\">\n              <div>XKNX Version</div>\n              <div>${this.knxInfo?.version}</div>\n            </div>\n\n            <div class=\"knx-content-row\">\n              <div>KNX Frontend Version</div>\n              <div>${VERSION}</div>\n            </div>\n\n            <div class=\"knx-content-row\">\n              <div>${localize(this.hass!.language, \"overview_connected_to_bus\")}</div>\n              <div>${this.knxInfo?.connected ? \"Yes\" : \"No\"}</div>\n            </div>\n\n            <div class=\"knx-content-row\">\n              <div>${localize(this.hass!.language, \"overview_individual_address\")}</div>\n              <div>${this.knxInfo?.current_address}</div>\n            </div>\n\n            <div class=\"knx-bug-report\">\n              <div>${localize(this.hass!.language, \"overview_issue_tracker\")}</div>\n              <ul>\n                <li>\n                  <a href=\"https://github.com/XKNX/knx-frontend/issues\" target=\"_blank\"\n                    >${localize(this.hass!.language, \"overview_issue_tracker_knx_frontend\")}</a\n                  >\n                </li>\n                <li>\n                  <a href=\"https://github.com/XKNX/xknxproject/issues\" target=\"_blank\"\n                    >${localize(this.hass!.language, \"overview_issue_tracker_xknxproject\")}</a\n                  >\n                </li>\n                <li>\n                  <a href=\"https://github.com/XKNX/xknx/issues\" target=\"_blank\"\n                    >${localize(this.hass!.language, \"overview_issue_tracker_xknx\")}</a\n                  >\n                </li>\n              </ul>\n            </div>\n          </div>\n        </ha-card>\n        ${this.knxInfo?.project ? this._projectCard(this.knxInfo.project) : nothing}\n        <ha-card\n          class=\"knx-info\"\n          .header=${localize(this.hass!.language, \"overview_project_file_header\")}\n        >\n          <div class=\"knx-project-description\">\n            ${localize(this.hass!.language, \"overview_project_upload_description\")}\n          </div>\n          <div class=\"knx-content-row\">\n            <ha-file-upload\n              .hass=${this.hass}\n              accept=\".knxproj\"\n              .icon=${mdiFileUpload}\n              .label=${localize(this.hass!.language, \"overview_project_file\")}\n              .value=${this._projectFile?.name}\n              .uploading=${this._uploading}\n              @file-picked=${this._filePicked}\n            ></ha-file-upload>\n          </div>\n          <div class=\"knx-content-row\">\n            <ha-selector-text\n              .hass=${this.hass}\n              .value=${this._projectPassword || \"\"}\n              .label=${localize(this.hass!.language, \"overview_project_password\")}\n              .selector=${{ text: { multiline: false, type: \"password\" } }}\n              .required=${false}\n              @value-changed=${this._passwordChanged}\n            >\n            </ha-selector-text>\n          </div>\n          <div class=\"knx-content-button\">\n            <ha-button @click=${this._uploadFile} .disabled=${this._uploading || !this._projectFile}\n              >${localize(this.hass!.language, \"overview_project_upload\")}</ha-button\n            >\n          </div>\n        </ha-card>\n      </div>\n    `;\n  }\n\n  private _projectCard(projectInfo: KNXProjectInfo) {\n    return html`\n      <ha-card\n        class=\"knx-info\"\n        .header=${localize(this.hass!.language, \"overview_project_data_header\")}\n      >\n        <div class=\"card-content knx-info-section\">\n          <div class=\"knx-content-row\">\n            <div>${localize(this.hass!.language, \"overview_project_data_name\")}</div>\n            <div>${projectInfo.name}</div>\n          </div>\n          <div class=\"knx-content-row\">\n            <div>${localize(this.hass!.language, \"overview_project_data_last_modified\")}</div>\n            <div>${new Date(projectInfo.last_modified).toUTCString()}</div>\n          </div>\n          <div class=\"knx-content-row\">\n            <div>${localize(this.hass!.language, \"overview_project_data_tool_version\")}</div>\n            <div>${projectInfo.tool_version}</div>\n          </div>\n        </div>\n        <div class=\"knx-delete-project-button\">\n          <ha-button\n            class=\"knx-warning\"\n            @click=${this._removeProject}\n            .disabled=${this._uploading || !this.knxInfo?.project}\n            >${localize(this.hass!.language, \"overview_project_delete\")}</ha-button\n          >\n        </div>\n      </ha-card>\n    `;\n  }\n\n  private loadKnxInfo() {\n    getKnxInfo(this.hass).then(\n      (knxInfo) => {\n        this.knxInfo = knxInfo;\n        this.requestUpdate();\n      },\n      (err) => {\n        logger.error(\"getKnxInfo\", err);\n      }\n    );\n  }\n\n  private _filePicked(ev) {\n    this._projectFile = ev.detail.files[0];\n  }\n\n  private _passwordChanged(ev) {\n    this._projectPassword = ev.detail.value;\n  }\n\n  private async _uploadFile(_ev) {\n    const file = this._projectFile;\n    if (typeof file === \"undefined\") {\n      return;\n    }\n\n    let error: Error | undefined;\n    this._uploading = true;\n    try {\n      const project_file_id = await uploadFile(this.hass, file);\n      await processProjectFile(this.hass, project_file_id, this._projectPassword || \"\");\n    } catch (err: any) {\n      error = err;\n      showAlertDialog(this, {\n        title: \"Upload failed\",\n        text: extractApiErrorMessage(err),\n        confirmText: \"ok\",\n      });\n    } finally {\n      if (!error) {\n        this._projectFile = undefined;\n        this._projectPassword = undefined;\n      }\n      this._uploading = false;\n      this.loadKnxInfo();\n    }\n  }\n\n  private async _removeProject(_ev) {\n    try {\n      await removeProjectFile(this.hass);\n    } catch (err: any) {\n      showAlertDialog(this, {\n        title: \"Deletion failed\",\n        text: extractApiErrorMessage(err),\n        confirmText: \"ok\",\n      });\n    } finally {\n      this.loadKnxInfo();\n    }\n  }\n\n  static get styles() {\n    return css`\n      .columns {\n        display: flex;\n        justify-content: center;\n      }\n\n      .columns > ha-card {\n        min-width: 400px;\n      }\n\n      @media screen and (max-width: 1500px) {\n        .columns {\n          flex-direction: column;\n        }\n\n        .columns > ha-card {\n          width: 96.5%;\n        }\n\n        .knx-delete-project-button {\n          top: 20px;\n        }\n\n        .knx-info {\n          margin-right: 8px;\n          max-width: 96.5%;\n        }\n      }\n\n      @media screen and (min-width: 1501px) {\n        .knx-info {\n          max-width: 400px;\n        }\n      }\n\n      .knx-info {\n        margin-left: 8px;\n        margin-top: 8px;\n      }\n\n      .knx-info-section {\n        display: flex;\n        flex-direction: column;\n      }\n\n      .knx-content-row {\n        display: flex;\n        flex-direction: row;\n        justify-content: space-between;\n      }\n\n      .knx-content-row > div:nth-child(2) {\n        margin-left: 1rem;\n      }\n\n      .knx-content-button {\n        display: flex;\n        flex-direction: row-reverse;\n        justify-content: space-between;\n      }\n\n      .knx-warning {\n        --mdc-theme-primary: var(--error-color);\n      }\n\n      .knx-project-description {\n        margin-top: -8px;\n        padding: 0px 16px 16px;\n      }\n\n      .knx-delete-project-button {\n        position: absolute;\n        bottom: 0;\n        right: 0;\n      }\n\n      .knx-bug-report {\n        margin-top: 20px;\n      }\n\n      .knx-bug-report > ul > li > a {\n        text-decoration: none;\n        color: var(--mdc-theme-primary);\n      }\n\n      ha-file-upload,\n      ha-selector-text {\n        width: 100%;\n        margin: 0 8px 8px;\n      }\n    `;\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"knx-overview\": KNXOverview;\n  }\n}\n",
-        "export const VERSION = \"2023.5.2.143855\";\n"
+        "import { mdiFileUpload } from \"@mdi/js\";\nimport { css, nothing, html, LitElement, TemplateResult } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\n\nimport \"@ha/components/ha-button-menu\";\nimport \"@ha/components/ha-card\";\nimport \"@ha/layouts/ha-app-layout\";\nimport \"@ha/layouts/hass-subpage\";\nimport \"@ha/components/ha-button\";\nimport \"@ha/components/ha-file-upload\";\nimport \"@ha/components/ha-selector/ha-selector-text\";\nimport { uploadFile } from \"@ha/data/file_upload\";\nimport { extractApiErrorMessage } from \"@ha/data/hassio/common\";\nimport { showAlertDialog } from \"@ha/dialogs/generic/show-dialog-box\";\nimport { HomeAssistant } from \"@ha/types\";\n\nimport { getKnxInfo, processProjectFile, removeProjectFile } from \"../services/websocket.service\";\nimport { KNXInfo, KNXProjectInfo } from \"../types/websocket\";\nimport { localize } from \"../localize/localize\";\nimport { KNXLogger } from \"../tools/knx-logger\";\nimport { VERSION } from \"../version\";\n\nconst logger = new KNXLogger(\"overview\");\n\n@customElement(\"knx-overview\")\nexport class KNXOverview extends LitElement {\n  @property({ type: Object }) public hass!: HomeAssistant;\n\n  @property({ type: Boolean, reflect: true }) public narrow!: boolean;\n\n  @state() private knxInfo: KNXInfo | null = null;\n\n  @state() private _projectPassword?: string;\n\n  @state() private _uploading = false;\n\n  @state() private _projectFile?: File;\n\n  protected firstUpdated() {\n    this.loadKnxInfo();\n  }\n\n  protected render(): TemplateResult | void {\n    if (!this.knxInfo) {\n      return html`Loading...`;\n    }\n\n    return html`\n      <div class=\"columns\">\n        <ha-card class=\"knx-info\" header=\"KNX Information\">\n          <div class=\"card-content knx-info-section\">\n            <div class=\"knx-content-row\">\n              <div>XKNX Version</div>\n              <div>${this.knxInfo?.version}</div>\n            </div>\n\n            <div class=\"knx-content-row\">\n              <div>KNX Frontend Version</div>\n              <div>${VERSION}</div>\n            </div>\n\n            <div class=\"knx-content-row\">\n              <div>${localize(this.hass!.language, \"overview_connected_to_bus\")}</div>\n              <div>${this.knxInfo?.connected ? \"Yes\" : \"No\"}</div>\n            </div>\n\n            <div class=\"knx-content-row\">\n              <div>${localize(this.hass!.language, \"overview_individual_address\")}</div>\n              <div>${this.knxInfo?.current_address}</div>\n            </div>\n\n            <div class=\"knx-bug-report\">\n              <div>${localize(this.hass!.language, \"overview_issue_tracker\")}</div>\n              <ul>\n                <li>\n                  <a href=\"https://github.com/XKNX/knx-frontend/issues\" target=\"_blank\"\n                    >${localize(this.hass!.language, \"overview_issue_tracker_knx_frontend\")}</a\n                  >\n                </li>\n                <li>\n                  <a href=\"https://github.com/XKNX/knx-frontend/issues\" target=\"_blank\"\n                    >${localize(this.hass!.language, \"overview_issue_tracker_xknxproject\")}</a\n                  >\n                </li>\n                <li>\n                  <a href=\"https://github.com/XKNX/knx-frontend/issues\" target=\"_blank\"\n                    >${localize(this.hass!.language, \"overview_issue_tracker_xknx\")}</a\n                  >\n                </li>\n              </ul>\n            </div>\n          </div>\n        </ha-card>\n        ${this.knxInfo?.project ? this._projectCard(this.knxInfo.project) : nothing}\n        <ha-card\n          class=\"knx-info\"\n          .header=${localize(this.hass!.language, \"overview_project_file_header\")}\n        >\n          <div class=\"knx-project-description\">\n            ${localize(this.hass!.language, \"overview_project_upload_description\")}\n          </div>\n          <div class=\"knx-content-row\">\n            <ha-file-upload\n              .hass=${this.hass}\n              accept=\".knxproj\"\n              .icon=${mdiFileUpload}\n              .label=${localize(this.hass!.language, \"overview_project_file\")}\n              .value=${this._projectFile?.name}\n              .uploading=${this._uploading}\n              @file-picked=${this._filePicked}\n            ></ha-file-upload>\n          </div>\n          <div class=\"knx-content-row\">\n            <ha-selector-text\n              .hass=${this.hass}\n              .value=${this._projectPassword || \"\"}\n              .label=${localize(this.hass!.language, \"overview_project_password\")}\n              .selector=${{ text: { multiline: false, type: \"password\" } }}\n              .required=${false}\n              @value-changed=${this._passwordChanged}\n            >\n            </ha-selector-text>\n          </div>\n          <div class=\"knx-content-button\">\n            <ha-button @click=${this._uploadFile} .disabled=${this._uploading || !this._projectFile}\n              >${localize(this.hass!.language, \"overview_project_upload\")}</ha-button\n            >\n          </div>\n        </ha-card>\n      </div>\n    `;\n  }\n\n  private _projectCard(projectInfo: KNXProjectInfo) {\n    return html`\n      <ha-card\n        class=\"knx-info\"\n        .header=${localize(this.hass!.language, \"overview_project_data_header\")}\n      >\n        <div class=\"card-content knx-info-section\">\n          <div class=\"knx-content-row\">\n            <div>${localize(this.hass!.language, \"overview_project_data_name\")}</div>\n            <div>${projectInfo.name}</div>\n          </div>\n          <div class=\"knx-content-row\">\n            <div>${localize(this.hass!.language, \"overview_project_data_last_modified\")}</div>\n            <div>${new Date(projectInfo.last_modified).toUTCString()}</div>\n          </div>\n          <div class=\"knx-content-row\">\n            <div>${localize(this.hass!.language, \"overview_project_data_tool_version\")}</div>\n            <div>${projectInfo.tool_version}</div>\n          </div>\n        </div>\n        <div class=\"knx-delete-project-button\">\n          <ha-button\n            class=\"knx-warning\"\n            @click=${this._removeProject}\n            .disabled=${this._uploading || !this.knxInfo?.project}\n            >${localize(this.hass!.language, \"overview_project_delete\")}</ha-button\n          >\n        </div>\n      </ha-card>\n    `;\n  }\n\n  private loadKnxInfo() {\n    getKnxInfo(this.hass).then(\n      (knxInfo) => {\n        this.knxInfo = knxInfo;\n        this.requestUpdate();\n      },\n      (err) => {\n        logger.error(\"getKnxInfo\", err);\n      }\n    );\n  }\n\n  private _filePicked(ev) {\n    this._projectFile = ev.detail.files[0];\n  }\n\n  private _passwordChanged(ev) {\n    this._projectPassword = ev.detail.value;\n  }\n\n  private async _uploadFile(_ev) {\n    const file = this._projectFile;\n    if (typeof file === \"undefined\") {\n      return;\n    }\n\n    let error: Error | undefined;\n    this._uploading = true;\n    try {\n      const project_file_id = await uploadFile(this.hass, file);\n      await processProjectFile(this.hass, project_file_id, this._projectPassword || \"\");\n    } catch (err: any) {\n      error = err;\n      showAlertDialog(this, {\n        title: \"Upload failed\",\n        text: extractApiErrorMessage(err),\n        confirmText: \"ok\",\n      });\n    } finally {\n      if (!error) {\n        this._projectFile = undefined;\n        this._projectPassword = undefined;\n      }\n      this._uploading = false;\n      this.loadKnxInfo();\n    }\n  }\n\n  private async _removeProject(_ev) {\n    try {\n      await removeProjectFile(this.hass);\n    } catch (err: any) {\n      showAlertDialog(this, {\n        title: \"Deletion failed\",\n        text: extractApiErrorMessage(err),\n        confirmText: \"ok\",\n      });\n    } finally {\n      this.loadKnxInfo();\n    }\n  }\n\n  static get styles() {\n    return css`\n      .columns {\n        display: flex;\n        justify-content: center;\n      }\n\n      .columns > ha-card {\n        min-width: 400px;\n      }\n\n      @media screen and (max-width: 1500px) {\n        .columns {\n          flex-direction: column;\n        }\n\n        .columns > ha-card {\n          width: 96.5%;\n        }\n\n        .knx-delete-project-button {\n          top: 20px;\n        }\n\n        .knx-info {\n          margin-right: 8px;\n          max-width: 96.5%;\n        }\n      }\n\n      @media screen and (min-width: 1501px) {\n        .knx-info {\n          max-width: 400px;\n        }\n      }\n\n      .knx-info {\n        margin-left: 8px;\n        margin-top: 8px;\n      }\n\n      .knx-info-section {\n        display: flex;\n        flex-direction: column;\n      }\n\n      .knx-content-row {\n        display: flex;\n        flex-direction: row;\n        justify-content: space-between;\n      }\n\n      .knx-content-row > div:nth-child(2) {\n        margin-left: 1rem;\n      }\n\n      .knx-content-button {\n        display: flex;\n        flex-direction: row-reverse;\n        justify-content: space-between;\n      }\n\n      .knx-warning {\n        --mdc-theme-primary: var(--error-color);\n      }\n\n      .knx-project-description {\n        margin-top: -8px;\n        padding: 0px 16px 16px;\n      }\n\n      .knx-delete-project-button {\n        position: absolute;\n        bottom: 0;\n        right: 0;\n      }\n\n      .knx-bug-report {\n        margin-top: 20px;\n      }\n\n      .knx-bug-report > ul > li > a {\n        text-decoration: none;\n        color: var(--mdc-theme-primary);\n      }\n\n      ha-file-upload,\n      ha-selector-text {\n        width: 100%;\n        margin: 0 8px 8px;\n      }\n    `;\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"knx-overview\": KNXOverview;\n  }\n}\n",
+        "export const VERSION = \"2023.5.2.73247\";\n"
     ],
     "version": 3
 }
```

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/81f2e6ee.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/81f2e6ee.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/81f2e6ee.js.LICENSE.txt` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/81f2e6ee.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/81f2e6ee.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/81f2e6ee.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/81f2e6ee.js.map` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/81f2e6ee.js.map`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/9f79b138.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/9f79b138.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/9f79b138.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/9f79b138.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/9f79b138.js.map` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/9f79b138.js.map`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4a1271f.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4a1271f.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4a1271f.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4a1271f.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4b8554f.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4b8554f.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4b8554f.js.LICENSE.txt` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4b8554f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4b8554f.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4b8554f.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/b4b8554f.js.map` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/b4b8554f.js.map`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/c1cea011.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/c1cea011.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/c1cea011.js.LICENSE.txt` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/c1cea011.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/c1cea011.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/c1cea011.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/d5e44388.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/d5e44388.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/d5e44388.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/d5e44388.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/d5e44388.js.map` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/d5e44388.js.map`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/e8fee43e.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/e8fee43e.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/e8fee43e.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/e8fee43e.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/e9d6c77f.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/e9d6c77f.js`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/e9d6c77f.js.gz` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/e9d6c77f.js.gz`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/entrypoint-5e4e4dd9.js` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/entrypoint-5baef557.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see entrypoint-5e4e4dd9.js.LICENSE.txt */
+/*! For license information please see entrypoint-5baef557.js.LICENSE.txt */
 (() => {
     var e, t, r, i, n = {
             7715: (e, t, r) => {
                 "use strict";
                 r.d(t, {
                     i: () => i
                 });
@@ -12566,15 +12566,15 @@
     }, s.d = (e, t) => {
         for (var r in t) s.o(t, r) && !s.o(e, r) && Object.defineProperty(e, r, {
             enumerable: !0,
             get: t[r]
         })
     }, s.f = {}, s.e = e => Promise.all(Object.keys(s.f).reduce(((t, r) => (s.f[r](e, t), t)), [])), s.u = e => ({
         182: "e8fee43e",
-        428: "679a99d6",
+        428: "9cd92628",
         442: "c1cea011",
         503: "b4a1271f",
         525: "81f2e6ee",
         582: "525c6b8e",
         588: "b4b8554f",
         663: "e9d6c77f",
         686: "00e63187",
@@ -18234,8 +18234,8 @@
                 }]
             }
         }), Me);
         const Vt = document.createElement("style");
         Vt.innerHTML = "\nbody {\n  font-family: Roboto, sans-serif;\n  -moz-osx-font-smoothing: grayscale;\n  -webkit-font-smoothing: antialiased;\n  font-weight: 400;\n  margin: 0;\n  padding: 0;\n  height: 100vh;\n}\n@media (prefers-color-scheme: dark) {\n  body {\n    background-color: #111111;\n    color: #e1e1e1;\n  }\n}\n", document.head.appendChild(Vt)
     })()
 })();
-//# sourceMappingURL=entrypoint-5e4e4dd9.js.map
+//# sourceMappingURL=entrypoint-5baef557.js.map
```

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/entrypoint-5e4e4dd9.js.LICENSE.txt` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/entrypoint-5baef557.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend/frontend_latest/entrypoint-5e4e4dd9.js.map` & `knx_frontend-2023.5.2.73247/knx_frontend/frontend_latest/entrypoint-5baef557.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'file'": "'entrypoint-5baef557.js'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "entrypoint-5e4e4dd9.js",
+    "file": "entrypoint-5baef557.js",
     "mappings": ";;;AA0DA;AACA;;AAEA;;;AAIA;AACA;AACA;AAEA;;;AAkBA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;;AAGA;;;AASA;;AAGA;;;AAkBA;AACA;AACA;AACA;AACA;;;;;AAKA;AACA;AACA;AACA;AACA;;;;;AAKA;AACA;AACA;AACA;AACA;;AAGA;;;;ACnGA;;ACvBA;AACA;AACA;;AAGA;;ACaA;;AAEA;;AAwBA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;AAKA;;ACtDA;AACA;AACA;AACA;;AAEA;;AAKA;;;;;;;;;;;;AAgBA;;AChBA;;AAEA;;AAEA;AAEA;;;;;;;;;;;;;;;AA2EA;;ACrHA;;;;;;;AAOA;;AAGA;;;;;;;;;;;;;;;;;AAqBA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AC2GA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AClDA;;ACnDA;;AAGA;AACA;AACA;;AAEA;AAGA;;AAEA;;;AAGA;;AAGA;AACA;;;;AAIA;;;AAGA;;;;AAKA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA2FA;;;;;;;;;;;;ACHA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAwFA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAgGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAAA;;;;;;;;;;;;;;;;;AAmBA;;;;;;;;;;ACrQA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;;;AAGA;AACA;;;;;AAOA;;;AAIA;;AAMA;AAEA;ACuEA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACgNA;;;;;;;;;;;;;;;;;;;;;AC9TA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AC2TA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AC3RA;;;;;AC7HA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACgGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACkHA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACrJA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACqGA;;AC1IA;;;AAKA;;AAEA;;;;;AAKA;;;;;AAKA;AAEA;;;AAGA;;;;;AAOA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAsFA;ACvIA;AAEA;;AAGA;AACA;;AAEA;;AAGA;AACA;;;AAGA;;AAGA;;AAEA;AACA;;;;AAKA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAgDA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACkBA;AC5FA;AAGA;;AAGA;AACA;;AAEA;;AAGA;AACA;;;;;;;AAQA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAwCA;;;;AC7BA;AACA;;;;;AAKA;AACA;;;AAGA;;;AAGA;;;;;;AAMA;AACA;AACA;AACA;;AA7BA;;;;AAgDA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://knx-frontend/mwc-circular-progress-base.ts",
         "webpack://knx-frontend/./homeassistant-frontend/src/components/ha-circular-progress.ts",
         "webpack://knx-frontend/./homeassistant-frontend/src/components/ha-icon-button-arrow-prev.ts",
```

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend.egg-info/PKG-INFO` & `knx_frontend-2023.5.2.73247/knx_frontend/knx_frontend.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: knx-frontend
-Version: 2023.5.2.143855
+Version: 2023.5.2.73247
 Summary: KNX panel for Home Assistant
-Author-email: Marvin Wichmann <me@marvin-wichmann.de>, Matthias Alphart <farmio@alphart.net>
+Author-email: Marvin Wichmann <me@marvin-wichmann.de>
 License: MIT License
-Project-URL: Repository, https://github.com/XKNX/knx-frontend.git
+Project-URL: homepage, https://github.com/XKNX/knx-frontend
 Keywords: Home Assistant,KNX
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KNX UI
```

### Comparing `knx_frontend-2023.5.2.143855/knx_frontend.egg-info/SOURCES.txt` & `knx_frontend-2023.5.2.73247/knx_frontend/knx_frontend.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,16 @@
 MANIFEST.in
 README.md
 VERSION
 pyproject.toml
 setup.cfg
 knx_frontend/__init__.py
 knx_frontend/constants.py
-knx_frontend/entrypoint-5e4e4dd9.js
-knx_frontend/entrypoint-5e4e4dd9.js.gz
-knx_frontend/py.typed
-knx_frontend.egg-info/PKG-INFO
-knx_frontend.egg-info/SOURCES.txt
-knx_frontend.egg-info/dependency_links.txt
-knx_frontend.egg-info/top_level.txt
+knx_frontend/entrypoint-5baef557.js
+knx_frontend/entrypoint-5baef557.js.gz
 knx_frontend/frontend_es5/0af2eb52.js
 knx_frontend/frontend_es5/0af2eb52.js.gz
 knx_frontend/frontend_es5/0e40d3e9.js
 knx_frontend/frontend_es5/0e40d3e9.js.LICENSE.txt
 knx_frontend/frontend_es5/0e40d3e9.js.gz
 knx_frontend/frontend_es5/4fa1e58d.js
 knx_frontend/frontend_es5/4fa1e58d.js.LICENSE.txt
@@ -29,26 +24,26 @@
 knx_frontend/frontend_es5/78cd9069.js
 knx_frontend/frontend_es5/78cd9069.js.LICENSE.txt
 knx_frontend/frontend_es5/78cd9069.js.gz
 knx_frontend/frontend_es5/9080a47b.js
 knx_frontend/frontend_es5/9080a47b.js.gz
 knx_frontend/frontend_es5/94794678.js
 knx_frontend/frontend_es5/94794678.js.gz
+knx_frontend/frontend_es5/bd85fc7a.js
+knx_frontend/frontend_es5/bd85fc7a.js.LICENSE.txt
+knx_frontend/frontend_es5/bd85fc7a.js.gz
 knx_frontend/frontend_es5/dade42d6.js
 knx_frontend/frontend_es5/dade42d6.js.LICENSE.txt
 knx_frontend/frontend_es5/dade42d6.js.gz
 knx_frontend/frontend_es5/ea4e1a95.js
 knx_frontend/frontend_es5/ea4e1a95.js.LICENSE.txt
 knx_frontend/frontend_es5/ea4e1a95.js.gz
-knx_frontend/frontend_es5/ecca0abf.js
-knx_frontend/frontend_es5/ecca0abf.js.LICENSE.txt
-knx_frontend/frontend_es5/ecca0abf.js.gz
-knx_frontend/frontend_es5/entrypoint-4e598fff.js
-knx_frontend/frontend_es5/entrypoint-4e598fff.js.LICENSE.txt
-knx_frontend/frontend_es5/entrypoint-4e598fff.js.gz
+knx_frontend/frontend_es5/entrypoint-48b69fdd.js
+knx_frontend/frontend_es5/entrypoint-48b69fdd.js.LICENSE.txt
+knx_frontend/frontend_es5/entrypoint-48b69fdd.js.gz
 knx_frontend/frontend_es5/f0618551.js
 knx_frontend/frontend_es5/f0618551.js.LICENSE.txt
 knx_frontend/frontend_es5/f0618551.js.gz
 knx_frontend/frontend_es5/fc280d00.js
 knx_frontend/frontend_es5/fc280d00.js.LICENSE.txt
 knx_frontend/frontend_es5/fc280d00.js.gz
 knx_frontend/frontend_es5/manifest.json
@@ -59,22 +54,22 @@
 knx_frontend/frontend_latest/230a12b6.js.LICENSE.txt
 knx_frontend/frontend_latest/230a12b6.js.gz
 knx_frontend/frontend_latest/230a12b6.js.map
 knx_frontend/frontend_latest/525c6b8e.js
 knx_frontend/frontend_latest/525c6b8e.js.LICENSE.txt
 knx_frontend/frontend_latest/525c6b8e.js.gz
 knx_frontend/frontend_latest/525c6b8e.js.map
-knx_frontend/frontend_latest/679a99d6.js
-knx_frontend/frontend_latest/679a99d6.js.LICENSE.txt
-knx_frontend/frontend_latest/679a99d6.js.gz
-knx_frontend/frontend_latest/679a99d6.js.map
 knx_frontend/frontend_latest/81f2e6ee.js
 knx_frontend/frontend_latest/81f2e6ee.js.LICENSE.txt
 knx_frontend/frontend_latest/81f2e6ee.js.gz
 knx_frontend/frontend_latest/81f2e6ee.js.map
+knx_frontend/frontend_latest/9cd92628.js
+knx_frontend/frontend_latest/9cd92628.js.LICENSE.txt
+knx_frontend/frontend_latest/9cd92628.js.gz
+knx_frontend/frontend_latest/9cd92628.js.map
 knx_frontend/frontend_latest/9f79b138.js
 knx_frontend/frontend_latest/9f79b138.js.gz
 knx_frontend/frontend_latest/9f79b138.js.map
 knx_frontend/frontend_latest/b4a1271f.js
 knx_frontend/frontend_latest/b4a1271f.js.LICENSE.txt
 knx_frontend/frontend_latest/b4a1271f.js.gz
 knx_frontend/frontend_latest/b4b8554f.js
@@ -88,12 +83,16 @@
 knx_frontend/frontend_latest/d5e44388.js.gz
 knx_frontend/frontend_latest/d5e44388.js.map
 knx_frontend/frontend_latest/e8fee43e.js
 knx_frontend/frontend_latest/e8fee43e.js.gz
 knx_frontend/frontend_latest/e9d6c77f.js
 knx_frontend/frontend_latest/e9d6c77f.js.LICENSE.txt
 knx_frontend/frontend_latest/e9d6c77f.js.gz
-knx_frontend/frontend_latest/entrypoint-5e4e4dd9.js
-knx_frontend/frontend_latest/entrypoint-5e4e4dd9.js.LICENSE.txt
-knx_frontend/frontend_latest/entrypoint-5e4e4dd9.js.gz
-knx_frontend/frontend_latest/entrypoint-5e4e4dd9.js.map
-knx_frontend/frontend_latest/manifest.json
+knx_frontend/frontend_latest/entrypoint-5baef557.js
+knx_frontend/frontend_latest/entrypoint-5baef557.js.LICENSE.txt
+knx_frontend/frontend_latest/entrypoint-5baef557.js.gz
+knx_frontend/frontend_latest/entrypoint-5baef557.js.map
+knx_frontend/frontend_latest/manifest.json
+knx_frontend/knx_frontend.egg-info/PKG-INFO
+knx_frontend/knx_frontend.egg-info/SOURCES.txt
+knx_frontend/knx_frontend.egg-info/dependency_links.txt
+knx_frontend/knx_frontend.egg-info/top_level.txt
```

### Comparing `knx_frontend-2023.5.2.143855/pyproject.toml` & `knx_frontend-2023.5.2.73247/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [build-system]
-requires = ["setuptools~=62.3"]
+requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name         = "knx_frontend"
 license      = {text = "MIT License"}
 description  = "KNX panel for Home Assistant"
 keywords     = ["Home Assistant", "KNX"]
 readme       = "README.md"
 authors      = [
-    {name = "Marvin Wichmann", email = "me@marvin-wichmann.de"},
-    {name = "Matthias Alphart", email = "farmio@alphart.net"},
+    {name = "Marvin Wichmann", email = "me@marvin-wichmann.de"}
 ]
 requires-python = ">=3.9.0"
 dynamic = ["version"]
 
 [project.urls]
-Repository = "https://github.com/XKNX/knx-frontend.git"
+homepage = "https://github.com/XKNX/knx-frontend"
 
 [tool.setuptools.dynamic]
 version = {file = "VERSION"}
 
 [tool.setuptools.packages.find]
-include = ["knx_frontend*"]
+where = ["knx_frontend"]
 
 [tool.mypy]
 python_version = 3.9
 show_error_codes = true
 strict = true
```

