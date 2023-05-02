# Comparing `tmp/mothertongues-0.18.20230410.tar.gz` & `tmp/mothertongues-0.18.20230502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mothertongues-0.18.20230410.tar", last modified: Mon Apr 10 20:00:44 2023, max compression
+gzip compressed data, was "mothertongues-0.18.20230502.tar", last modified: Tue May  2 20:13:30 2023, max compression
```

## Comparing `mothertongues-0.18.20230410.tar` & `mothertongues-0.18.20230502.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.272616 mothertongues-0.18.20230410/
--rw-r--r--   0 pinea      (502) staff       (20)    34523 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/LICENSE
--rw-r--r--   0 pinea      (502) staff       (20)      392 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/MANIFEST.in
--rw-r--r--   0 pinea      (502) staff       (20)     5178 2023-04-10 20:00:44.272427 mothertongues-0.18.20230410/PKG-INFO
--rw-r--r--   0 pinea      (502) staff       (20)     4835 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/README.md
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.241843 mothertongues-0.18.20230410/mothertongues.egg-info/
--rw-r--r--   0 pinea      (502) staff       (20)     5178 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mothertongues.egg-info/PKG-INFO
--rw-r--r--   0 pinea      (502) staff       (20)     5248 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mothertongues.egg-info/SOURCES.txt
--rw-r--r--   0 pinea      (502) staff       (20)        1 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mothertongues.egg-info/dependency_links.txt
--rw-r--r--   0 pinea      (502) staff       (20)       64 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mothertongues.egg-info/entry_points.txt
--rw-r--r--   0 pinea      (502) staff       (20)        1 2023-03-10 00:49:13.000000 mothertongues-0.18.20230410/mothertongues.egg-info/not-zip-safe
--rw-r--r--   0 pinea      (502) staff       (20)      205 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mothertongues.egg-info/requires.txt
--rw-r--r--   0 pinea      (502) staff       (20)        4 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mothertongues.egg-info/top_level.txt
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.243375 mothertongues-0.18.20230410/mtd/
--rw-r--r--   0 pinea      (502) staff       (20)     1113 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)       79 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/app.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.244226 mothertongues-0.18.20230410/mtd/buildtools/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/buildtools/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     2121 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/buildtools/swagger-pre.json
--rw-r--r--   0 pinea      (502) staff       (20)     1555 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/buildtools/swagger.json
--rw-r--r--   0 pinea      (502) staff       (20)     2151 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/buildtools/write_static.py
--rw-r--r--   0 pinea      (502) staff       (20)    13677 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/cli.py
--rw-r--r--   0 pinea      (502) staff       (20)     9751 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/dictionary.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.244430 mothertongues-0.18.20230410/mtd/exceptions/
--rw-r--r--   0 pinea      (502) staff       (20)     3900 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/exceptions/__init__.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.245059 mothertongues-0.18.20230410/mtd/languages/
--rw-r--r--   0 pinea      (502) staff       (20)     4206 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/languages/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     2647 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/languages/config_schema.json
--rw-r--r--   0 pinea      (502) staff       (20)     6106 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/languages/manifest_schema.json
--rw-r--r--   0 pinea      (502) staff       (20)     1044 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/languages/suites.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.247450 mothertongues-0.18.20230410/mtd/parsers/
--rw-r--r--   0 pinea      (502) staff       (20)     2089 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1564 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/csv_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)      917 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/dict_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     2011 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/gsheet_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     6481 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/json_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1329 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/pkl_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1623 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/psv_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1654 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/request_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1610 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/tsv_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     7676 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/utils.py
--rw-r--r--   0 pinea      (502) staff       (20)     2993 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/xlsx_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     4675 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/xml_parser.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.248037 mothertongues-0.18.20230410/mtd/processors/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/processors/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     2366 2023-04-10 19:59:43.000000 mothertongues-0.18.20230410/mtd/processors/sorter.py
--rw-r--r--   0 pinea      (502) staff       (20)    13166 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/processors/transducer.py
--rw-r--r--   0 pinea      (502) staff       (20)     2085 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/processors/validator.py
--rw-r--r--   0 pinea      (502) staff       (20)     2754 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/resources.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.248661 mothertongues-0.18.20230410/mtd/static/
--rw-r--r--   0 pinea      (502) staff       (20)      332 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1270 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/active.sites.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.248906 mothertongues-0.18.20230410/mtd/static/assets/
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.249077 mothertongues-0.18.20230410/mtd/static/assets/icon/
--rw-r--r--   0 pinea      (502) staff       (20)     1981 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/assets/icon/favicon.ico
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.249415 mothertongues-0.18.20230410/mtd/static/assets/js/
--rw-r--r--   0 pinea      (502) staff       (20)      293 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/assets/js/config-danish.js
--rw-r--r--   0 pinea      (502) staff       (20)     1195 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/assets/js/dict_cached-danish.js
--rw-r--r--   0 pinea      (502) staff       (20)      266 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/assets/manifest.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.249975 mothertongues-0.18.20230410/mtd/static/css/
--rw-r--r--   0 pinea      (502) staff       (20)     4049 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/css/custom.css
--rw-r--r--   0 pinea      (502) staff       (20)     7797 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/css/normalize.css
--rw-r--r--   0 pinea      (502) staff       (20)    11452 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/css/skeleton.css
--rw-r--r--   0 pinea      (502) staff       (20)      266 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/manifest.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.254371 mothertongues-0.18.20230410/mtd/static/swagger-ui/
--rw-r--r--   0 pinea      (502) staff       (20)      445 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/swagger-ui/favicon-16x16.png
--rw-r--r--   0 pinea      (502) staff       (20)     1141 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/swagger-ui/favicon-32x32.png
--rw-r--r--   0 pinea      (502) staff       (20)  1547890 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/swagger-ui/swagger-ui-bundle.js
--rw-r--r--   0 pinea      (502) staff       (20)   475131 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/swagger-ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 pinea      (502) staff       (20)   153816 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/swagger-ui/swagger-ui.css
--rw-r--r--   0 pinea      (502) staff       (20)     1455 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/swagger.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.256327 mothertongues-0.18.20230410/mtd/templates/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/templates/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1524 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/templates/apidocs.html
--rw-r--r--   0 pinea      (502) staff       (20)     2097 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/templates/dictionary.html
--rw-r--r--   0 pinea      (502) staff       (20)     3795 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/templates/index.html
--rw-r--r--   0 pinea      (502) staff       (20)   100235 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/templates/stats.html
--rw-r--r--   0 pinea      (502) staff       (20)     9074 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/templates/validator.html
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.260249 mothertongues-0.18.20230410/mtd/tests/
--rw-r--r--   0 pinea      (502) staff       (20)     4548 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/__init__.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.261407 mothertongues-0.18.20230410/mtd/tests/integration/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/integration/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)      764 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/integration/config_test.json
--rw-r--r--   0 pinea      (502) staff       (20)     3535 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/integration/test_api_resources.py
--rw-r--r--   0 pinea      (502) staff       (20)     2551 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/integration/test_basic_integration.py
--rw-r--r--   0 pinea      (502) staff       (20)     3515 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/integration/test_cli.py
--rw-r--r--   0 pinea      (502) staff       (20)      132 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/integration/test_swagger_integration.py
--rw-r--r--   0 pinea      (502) staff       (20)      465 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/log.py
--rw-r--r--   0 pinea      (502) staff       (20)     2795 2023-03-09 23:35:38.000000 mothertongues-0.18.20230410/mtd/tests/run.py
--rw-r--r--   0 pinea      (502) staff       (20)     4691 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_cli.py
--rw-r--r--   0 pinea      (502) staff       (20)     1053 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_csv_parser.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.261837 mothertongues-0.18.20230410/mtd/tests/test_data/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/__init__.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.262308 mothertongues-0.18.20230410/mtd/tests/test_data/csv/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/csv/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1244 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/csv/data.csv
--rw-r--r--   0 pinea      (502) staff       (20)     2190 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/csv/manifest.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.263506 mothertongues-0.18.20230410/mtd/tests/test_data/json/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)       54 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/bad.json
--rw-r--r--   0 pinea      (502) staff       (20)     2687 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/data.json
--rw-r--r--   0 pinea      (502) staff       (20)     1363 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/data_reduced.json
--rw-r--r--   0 pinea      (502) staff       (20)     1766 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/dict_manifest.json
--rw-r--r--   0 pinea      (502) staff       (20)     1798 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/manifest.json
--rw-r--r--   0 pinea      (502) staff       (20)       39 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/missing.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.263994 mothertongues-0.18.20230410/mtd/tests/test_data/pkl/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/pkl/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1185 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/pkl/data.pkl
--rw-r--r--   0 pinea      (502) staff       (20)     1798 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/pkl/manifest.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.264561 mothertongues-0.18.20230410/mtd/tests/test_data/psv/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/psv/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1244 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/psv/data.psv
--rw-r--r--   0 pinea      (502) staff       (20)     2190 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/psv/manifest.json
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test.log
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.265803 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)      488 2023-03-09 23:36:58.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/config_0.json
--rw-r--r--   0 pinea      (502) staff       (20)      488 2023-03-09 23:36:58.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/config_1.json
--rw-r--r--   0 pinea      (502) staff       (20)      398 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/config_2_minimal.json
--rw-r--r--   0 pinea      (502) staff       (20)      153 2023-03-09 23:36:58.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/dictionaries.txt
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/test.log
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.267705 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)       40 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_composite.json
--rw-r--r--   0 pinea      (502) staff       (20)       71 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_counter_feeding.yaml
--rw-r--r--   0 pinea      (502) staff       (20)        7 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_feeding.csv
--rw-r--r--   0 pinea      (502) staff       (20)        7 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_intermediate_transducer.csv
--rw-r--r--   0 pinea      (502) staff       (20)        8 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_length_transducer.csv
--rw-r--r--   0 pinea      (502) staff       (20)       95 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_length_transducer.yaml
--rw-r--r--   0 pinea      (502) staff       (20)        3 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_transducer.csv
--rw-r--r--   0 pinea      (502) staff       (20)       53 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_transducer.json
--rw-r--r--   0 pinea      (502) staff       (20)       53 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_transducer.yaml
--rw-r--r--   0 pinea      (502) staff       (20)        4 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_transducer_2.csv
--rw-r--r--   0 pinea      (502) staff       (20)       54 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_transducer_2.yaml
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.268126 mothertongues-0.18.20230410/mtd/tests/test_data/tsv/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/tsv/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1244 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/tsv/data.tsv
--rw-r--r--   0 pinea      (502) staff       (20)     2190 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/tsv/manifest.json
--rw-r--r--   0 pinea      (502) staff       (20)     1812 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/whitespace_manifest.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.269065 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     4473 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/data.xlsx
--rw-r--r--   0 pinea      (502) staff       (20)     2199 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/manifest.json
--rw-r--r--   0 pinea      (502) staff       (20)     2199 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/manifest.xlsx
--rw-r--r--   0 pinea      (502) staff       (20)     2151 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/manifest_alternate.json
--rw-r--r--   0 pinea      (502) staff       (20)     7324 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/missing_sheet_data.xlsx
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.269842 mothertongues-0.18.20230410/mtd/tests/test_data/xml/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xml/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)    10291 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xml/data.xml
--rw-r--r--   0 pinea      (502) staff       (20)     9274 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xml/data_reduced.xml
--rw-r--r--   0 pinea      (502) staff       (20)     1901 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xml/manifest.json
--rw-r--r--   0 pinea      (502) staff       (20)     1108 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data_configuration_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1693 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_dict_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     2292 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_dictionary.py
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_formatted_export.py
--rw-r--r--   0 pinea      (502) staff       (20)     1643 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_json_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1069 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_pkl_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1008 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_psv_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_raw_export.py
--rw-r--r--   0 pinea      (502) staff       (20)     3682 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_request_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     2702 2023-04-10 19:59:43.000000 mothertongues-0.18.20230410/mtd/tests/test_sorter.py
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_swagger_spec.py
--rw-r--r--   0 pinea      (502) staff       (20)     9180 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_transducer.py
--rw-r--r--   0 pinea      (502) staff       (20)     1008 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_tsv_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)      992 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_validator.py
--rw-r--r--   0 pinea      (502) staff       (20)     2115 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_xlsx_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1298 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_xml_parser.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.272058 mothertongues-0.18.20230410/mtd/transducers/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)      183 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/circumflex_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)       36 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/combining_comma.csv
--rw-r--r--   0 pinea      (502) staff       (20)       42 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/combining_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)      941 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/config.yaml
--rw-r--r--   0 pinea      (502) staff       (20)        6 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/digraph_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)       55 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/dot_below_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)       87 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/hacek_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)       64 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/macron_lowline_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)       40 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)        5 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/slurpy_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)        6 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/slurpy_to_line_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)      115 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/underline_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)       29 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mtd/version.py
--rw-r--r--   0 pinea      (502) staff       (20)     2556 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/views.py
--rw-r--r--   0 pinea      (502) staff       (20)      205 2023-02-04 19:46:13.000000 mothertongues-0.18.20230410/requirements.txt
--rw-r--r--   0 pinea      (502) staff       (20)       38 2023-04-10 20:00:44.272664 mothertongues-0.18.20230410/setup.cfg
--rw-r--r--   0 pinea      (502) staff       (20)     1214 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/setup.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.741388 mothertongues-0.18.20230502/
+-rw-r--r--   0 pinea      (502) staff       (20)    34523 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/LICENSE
+-rw-r--r--   0 pinea      (502) staff       (20)      392 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/MANIFEST.in
+-rw-r--r--   0 pinea      (502) staff       (20)     5198 2023-05-02 20:13:30.741245 mothertongues-0.18.20230502/PKG-INFO
+-rw-r--r--   0 pinea      (502) staff       (20)     4835 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/README.md
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.715096 mothertongues-0.18.20230502/mothertongues.egg-info/
+-rw-r--r--   0 pinea      (502) staff       (20)     5198 2023-05-02 20:13:30.000000 mothertongues-0.18.20230502/mothertongues.egg-info/PKG-INFO
+-rw-r--r--   0 pinea      (502) staff       (20)     5248 2023-05-02 20:13:30.000000 mothertongues-0.18.20230502/mothertongues.egg-info/SOURCES.txt
+-rw-r--r--   0 pinea      (502) staff       (20)        1 2023-05-02 20:13:30.000000 mothertongues-0.18.20230502/mothertongues.egg-info/dependency_links.txt
+-rw-r--r--   0 pinea      (502) staff       (20)       89 2023-05-02 20:13:30.000000 mothertongues-0.18.20230502/mothertongues.egg-info/entry_points.txt
+-rw-r--r--   0 pinea      (502) staff       (20)        1 2023-05-02 20:13:30.000000 mothertongues-0.18.20230502/mothertongues.egg-info/not-zip-safe
+-rw-r--r--   0 pinea      (502) staff       (20)      211 2023-05-02 20:13:30.000000 mothertongues-0.18.20230502/mothertongues.egg-info/requires.txt
+-rw-r--r--   0 pinea      (502) staff       (20)        4 2023-05-02 20:13:30.000000 mothertongues-0.18.20230502/mothertongues.egg-info/top_level.txt
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.715906 mothertongues-0.18.20230502/mtd/
+-rw-r--r--   0 pinea      (502) staff       (20)     1113 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)       79 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/app.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.716533 mothertongues-0.18.20230502/mtd/buildtools/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/buildtools/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2121 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/buildtools/swagger-pre.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1555 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/buildtools/swagger.json
+-rw-r--r--   0 pinea      (502) staff       (20)     2151 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/buildtools/write_static.py
+-rw-r--r--   0 pinea      (502) staff       (20)    13677 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/cli.py
+-rw-r--r--   0 pinea      (502) staff       (20)     9751 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/dictionary.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.716655 mothertongues-0.18.20230502/mtd/exceptions/
+-rw-r--r--   0 pinea      (502) staff       (20)     3900 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/exceptions/__init__.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.717138 mothertongues-0.18.20230502/mtd/languages/
+-rw-r--r--   0 pinea      (502) staff       (20)     4206 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/languages/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2647 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/languages/config_schema.json
+-rw-r--r--   0 pinea      (502) staff       (20)     6106 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/languages/manifest_schema.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1044 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/languages/suites.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.719087 mothertongues-0.18.20230502/mtd/parsers/
+-rw-r--r--   0 pinea      (502) staff       (20)     2089 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/parsers/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1564 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/parsers/csv_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)      947 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/parsers/dict_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2011 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/parsers/gsheet_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     5960 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/parsers/json_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1359 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/parsers/pkl_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1623 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/parsers/psv_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1654 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/parsers/request_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1610 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/parsers/tsv_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     7677 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/parsers/utils.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2993 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/parsers/xlsx_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     4675 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/parsers/xml_parser.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.719666 mothertongues-0.18.20230502/mtd/processors/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/processors/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2366 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/processors/sorter.py
+-rw-r--r--   0 pinea      (502) staff       (20)    13166 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/processors/transducer.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2085 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/processors/validator.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2754 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/resources.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.720323 mothertongues-0.18.20230502/mtd/static/
+-rw-r--r--   0 pinea      (502) staff       (20)      332 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1270 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/active.sites.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.720565 mothertongues-0.18.20230502/mtd/static/assets/
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.720936 mothertongues-0.18.20230502/mtd/static/assets/icon/
+-rw-r--r--   0 pinea      (502) staff       (20)     1981 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/assets/icon/favicon.ico
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.721544 mothertongues-0.18.20230502/mtd/static/assets/js/
+-rw-r--r--   0 pinea      (502) staff       (20)      293 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/assets/js/config-danish.js
+-rw-r--r--   0 pinea      (502) staff       (20)     1195 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/assets/js/dict_cached-danish.js
+-rw-r--r--   0 pinea      (502) staff       (20)      266 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/assets/manifest.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.722346 mothertongues-0.18.20230502/mtd/static/css/
+-rw-r--r--   0 pinea      (502) staff       (20)     4049 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/css/custom.css
+-rw-r--r--   0 pinea      (502) staff       (20)     7797 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/css/normalize.css
+-rw-r--r--   0 pinea      (502) staff       (20)    11452 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/css/skeleton.css
+-rw-r--r--   0 pinea      (502) staff       (20)      266 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/manifest.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.726218 mothertongues-0.18.20230502/mtd/static/swagger-ui/
+-rw-r--r--   0 pinea      (502) staff       (20)      445 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/swagger-ui/favicon-16x16.png
+-rw-r--r--   0 pinea      (502) staff       (20)     1141 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/swagger-ui/favicon-32x32.png
+-rw-r--r--   0 pinea      (502) staff       (20)  1547890 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/swagger-ui/swagger-ui-bundle.js
+-rw-r--r--   0 pinea      (502) staff       (20)   475131 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/swagger-ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 pinea      (502) staff       (20)   153816 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/swagger-ui/swagger-ui.css
+-rw-r--r--   0 pinea      (502) staff       (20)     1455 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/static/swagger.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.727964 mothertongues-0.18.20230502/mtd/templates/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/templates/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1524 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/templates/apidocs.html
+-rw-r--r--   0 pinea      (502) staff       (20)     2097 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/templates/dictionary.html
+-rw-r--r--   0 pinea      (502) staff       (20)     3795 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/templates/index.html
+-rw-r--r--   0 pinea      (502) staff       (20)   100235 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/templates/stats.html
+-rw-r--r--   0 pinea      (502) staff       (20)     9074 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/templates/validator.html
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.731101 mothertongues-0.18.20230502/mtd/tests/
+-rw-r--r--   0 pinea      (502) staff       (20)     4548 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/__init__.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.732099 mothertongues-0.18.20230502/mtd/tests/integration/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/integration/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)      764 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/integration/config_test.json
+-rw-r--r--   0 pinea      (502) staff       (20)     3535 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/integration/test_api_resources.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2551 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/integration/test_basic_integration.py
+-rw-r--r--   0 pinea      (502) staff       (20)     3515 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/integration/test_cli.py
+-rw-r--r--   0 pinea      (502) staff       (20)      132 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/integration/test_swagger_integration.py
+-rw-r--r--   0 pinea      (502) staff       (20)      465 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/log.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2795 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/run.py
+-rw-r--r--   0 pinea      (502) staff       (20)     4691 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_cli.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1053 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_csv_parser.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.732567 mothertongues-0.18.20230502/mtd/tests/test_data/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/__init__.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.733051 mothertongues-0.18.20230502/mtd/tests/test_data/csv/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/csv/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1244 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/csv/data.csv
+-rw-r--r--   0 pinea      (502) staff       (20)     2190 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/csv/manifest.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.734024 mothertongues-0.18.20230502/mtd/tests/test_data/json/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/json/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)       54 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/json/bad.json
+-rw-r--r--   0 pinea      (502) staff       (20)     2687 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/json/data.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1363 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/json/data_reduced.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1766 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/json/dict_manifest.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1798 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/json/manifest.json
+-rw-r--r--   0 pinea      (502) staff       (20)       39 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/json/missing.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.734400 mothertongues-0.18.20230502/mtd/tests/test_data/pkl/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/pkl/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1185 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/pkl/data.pkl
+-rw-r--r--   0 pinea      (502) staff       (20)     1798 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/pkl/manifest.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.734767 mothertongues-0.18.20230502/mtd/tests/test_data/psv/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/psv/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1244 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/psv/data.psv
+-rw-r--r--   0 pinea      (502) staff       (20)     2190 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/psv/manifest.json
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/test.log
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.735715 mothertongues-0.18.20230502/mtd/tests/test_data/test_dictionary/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/test_dictionary/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)      488 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/test_dictionary/config_0.json
+-rw-r--r--   0 pinea      (502) staff       (20)      488 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/test_dictionary/config_1.json
+-rw-r--r--   0 pinea      (502) staff       (20)      398 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/test_dictionary/config_2_minimal.json
+-rw-r--r--   0 pinea      (502) staff       (20)      153 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/test_dictionary/dictionaries.txt
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/test_dictionary/test.log
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.737350 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)       40 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/test_composite.json
+-rw-r--r--   0 pinea      (502) staff       (20)       71 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/test_counter_feeding.yaml
+-rw-r--r--   0 pinea      (502) staff       (20)        7 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/test_feeding.csv
+-rw-r--r--   0 pinea      (502) staff       (20)        7 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/test_intermediate_transducer.csv
+-rw-r--r--   0 pinea      (502) staff       (20)        8 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/test_length_transducer.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       95 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/test_length_transducer.yaml
+-rw-r--r--   0 pinea      (502) staff       (20)        3 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/test_transducer.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       53 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/test_transducer.json
+-rw-r--r--   0 pinea      (502) staff       (20)       53 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/test_transducer.yaml
+-rw-r--r--   0 pinea      (502) staff       (20)        4 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/test_transducer_2.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       54 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/transducers/test_transducer_2.yaml
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.737796 mothertongues-0.18.20230502/mtd/tests/test_data/tsv/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/tsv/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1244 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/tsv/data.tsv
+-rw-r--r--   0 pinea      (502) staff       (20)     2190 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/tsv/manifest.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1812 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/whitespace_manifest.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.738681 mothertongues-0.18.20230502/mtd/tests/test_data/xlsx/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/xlsx/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     4473 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/xlsx/data.xlsx
+-rw-r--r--   0 pinea      (502) staff       (20)     2199 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/xlsx/manifest.json
+-rw-r--r--   0 pinea      (502) staff       (20)     2199 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/xlsx/manifest.xlsx
+-rw-r--r--   0 pinea      (502) staff       (20)     2151 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/xlsx/manifest_alternate.json
+-rw-r--r--   0 pinea      (502) staff       (20)     7324 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/xlsx/missing_sheet_data.xlsx
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.739275 mothertongues-0.18.20230502/mtd/tests/test_data/xml/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/xml/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)    10291 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/xml/data.xml
+-rw-r--r--   0 pinea      (502) staff       (20)     9274 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/xml/data_reduced.xml
+-rw-r--r--   0 pinea      (502) staff       (20)     1901 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data/xml/manifest.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1108 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_data_configuration_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1693 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_dict_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2292 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_dictionary.py
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_formatted_export.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1643 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_json_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1069 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_pkl_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1008 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_psv_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_raw_export.py
+-rw-r--r--   0 pinea      (502) staff       (20)     3682 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_request_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2697 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_sorter.py
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_swagger_spec.py
+-rw-r--r--   0 pinea      (502) staff       (20)     9175 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_transducer.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1008 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_tsv_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)      992 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_validator.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2115 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_xlsx_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1298 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/tests/test_xml_parser.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-05-02 20:13:30.741041 mothertongues-0.18.20230502/mtd/transducers/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)      183 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/circumflex_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       36 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/combining_comma.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       42 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/combining_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)      941 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/config.yaml
+-rw-r--r--   0 pinea      (502) staff       (20)        6 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/digraph_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       55 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/dot_below_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       87 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/hacek_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       64 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/macron_lowline_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       40 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)        5 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/slurpy_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)        6 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/slurpy_to_line_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)      115 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/transducers/underline_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       29 2023-05-02 20:13:30.000000 mothertongues-0.18.20230502/mtd/version.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2556 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/mtd/views.py
+-rw-r--r--   0 pinea      (502) staff       (20)      211 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/requirements.txt
+-rw-r--r--   0 pinea      (502) staff       (20)       38 2023-05-02 20:13:30.741431 mothertongues-0.18.20230502/setup.cfg
+-rw-r--r--   0 pinea      (502) staff       (20)     1214 2023-04-17 01:22:23.000000 mothertongues-0.18.20230502/setup.py
```

### Comparing `mothertongues-0.18.20230410/LICENSE` & `mothertongues-0.18.20230502/LICENSE`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/PKG-INFO` & `mothertongues-0.18.20230502/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mothertongues
-Version: 0.18.20230410
+Version: 0.18.20230502
 Summary: Mother Tongues Dictionaries dictionary creation tool
 Home-page: https://github.com/roedoejet/mothertongues
 Author: Aidan Pine
 Author-email: info@mothertongues.org
 License: AGPL-3.0
+Platform: UNKNOWN
 Requires-Python: >=3.6.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mother Tongues Dictionaries (MTD)
 
 [![Coverage Status](https://coveralls.io/repos/github/roedoejet/mothertongues/badge.svg?branch=master)](https://coveralls.io/github/roedoejet/mothertongues?branch=master)
@@ -86,7 +87,9 @@
 [@markturin](https://github.com/markturin).
 [@eddieantonio](https://github.com/eddieantonio).
 [@kavonjon](https://github.com/kavonjon).
 
 ## License
 
 [AGPL-3 © Aidan Pine.](LICENSE)
+
+
```

### Comparing `mothertongues-0.18.20230410/README.md` & `mothertongues-0.18.20230502/README.md`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mothertongues.egg-info/PKG-INFO` & `mothertongues-0.18.20230502/mothertongues.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mothertongues
-Version: 0.18.20230410
+Version: 0.18.20230502
 Summary: Mother Tongues Dictionaries dictionary creation tool
 Home-page: https://github.com/roedoejet/mothertongues
 Author: Aidan Pine
 Author-email: info@mothertongues.org
 License: AGPL-3.0
+Platform: UNKNOWN
 Requires-Python: >=3.6.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mother Tongues Dictionaries (MTD)
 
 [![Coverage Status](https://coveralls.io/repos/github/roedoejet/mothertongues/badge.svg?branch=master)](https://coveralls.io/github/roedoejet/mothertongues?branch=master)
@@ -86,7 +87,9 @@
 [@markturin](https://github.com/markturin).
 [@eddieantonio](https://github.com/eddieantonio).
 [@kavonjon](https://github.com/kavonjon).
 
 ## License
 
 [AGPL-3 © Aidan Pine.](LICENSE)
+
+
```

### Comparing `mothertongues-0.18.20230410/mothertongues.egg-info/SOURCES.txt` & `mothertongues-0.18.20230502/mothertongues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/__init__.py` & `mothertongues-0.18.20230502/mtd/__init__.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/buildtools/swagger-pre.json` & `mothertongues-0.18.20230502/mtd/buildtools/swagger-pre.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/buildtools/swagger.json` & `mothertongues-0.18.20230502/mtd/buildtools/swagger.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/buildtools/write_static.py` & `mothertongues-0.18.20230502/mtd/buildtools/write_static.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/cli.py` & `mothertongues-0.18.20230502/mtd/cli.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/dictionary.py` & `mothertongues-0.18.20230502/mtd/dictionary.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/exceptions/__init__.py` & `mothertongues-0.18.20230502/mtd/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/languages/__init__.py` & `mothertongues-0.18.20230502/mtd/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/languages/config_schema.json` & `mothertongues-0.18.20230502/mtd/languages/config_schema.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/languages/manifest_schema.json` & `mothertongues-0.18.20230502/mtd/languages/manifest_schema.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/languages/suites.py` & `mothertongues-0.18.20230502/mtd/languages/suites.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/parsers/__init__.py` & `mothertongues-0.18.20230502/mtd/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/parsers/csv_parser.py` & `mothertongues-0.18.20230502/mtd/parsers/csv_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/parsers/dict_parser.py` & `mothertongues-0.18.20230502/mtd/parsers/dict_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 class Parser(JsonParser):
     '''
     Parse data for MTD. location (jsonpath) specifies location of data
 
     :param ResourceManifest manifest: Manifest for parser
     '''
     def __init__(self, manifest: ResourceManifest, resource: Union[dict, list]):
+        self.path_cache = {}
         self.manifest = manifest
         self.resource = resource
         if "location" in self.manifest:
             self.resource = resolve_pointer(self.resource, self.manifest['location'])
-        self.entry_template = self.manifest['targets']
+        self.entry_template = self.manifest['targets']
```

### Comparing `mothertongues-0.18.20230410/mtd/parsers/gsheet_parser.py` & `mothertongues-0.18.20230502/mtd/parsers/gsheet_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/parsers/json_parser.py` & `mothertongues-0.18.20230502/mtd/parsers/json_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,113 +3,100 @@
 import pandas as pd
 from mtd.exceptions import SchemaValidationError
 from mtd.parsers.utils import BaseParser
 from mtd.languages import MANIFEST_SCHEMA
 from jsonschema.exceptions import ValidationError
 from mtd.parsers.utils import ResourceManifest
 from typing import Dict, List, Union
-from jsonpath_rw import parse as json_parse
+from jsonpath_ng import parse as json_parse
 from tqdm import tqdm
-import multiprocessing as mp
 
 class Parser(BaseParser):
     '''
     Parse data for MTD. location (jsonpath) specifies location of data
 
     :param ResourceManifest manifest: Manifest for parser
     :param (str or json) resource_path: JSON or path to JSON
     '''
     def __init__(self, manifest: ResourceManifest, resource_path: Union[str, dict, list]):
         self.manifest = manifest
+        self.path_cache = {}
         try:
             if isinstance(resource_path, str):
                 with open(resource_path, encoding='utf8') as f:
                     self.resource = json.load(f)
             elif isinstance(resource_path, (dict, list)):
                 self.resource = resource_path
         except ValueError:
             raise SchemaValidationError('json', resource_path)
         if "location" in self.manifest:
             self.resource = resolve_pointer(self.resource, self.manifest['location'])
         self.entry_template = self.manifest['targets']
 
+    def get_matcher(self, path: str):
+        if path not in self.path_cache:
+            self.path_cache[path] = json_parse(path)
+        return self.path_cache[path]
+
     def getValueFromJsonPath(self, entry: dict, path: str):
-        jsonpath_expr = json_parse(path)
+        jsonpath_expr = self.get_matcher(path)
         result = jsonpath_expr.find(entry)
         if not result:
             result = ''
         return result
 
-    def chunks(self, l, n):
-        """Yield successive n-sized chunks from l."""
-        if not n:
-            n = 1
-        for i in range(0, len(l), n):
-            yield l[i:i + n]
-        
-    def resolve_targets(self):
-        ''' This function chunks the resource into equal chunks for each available core.
-            A 5000 entry corpus ran in 34 seconds compared with 103. TODO: This should still be faster...
-        '''
-        pool = mp.Pool(mp.cpu_count())
-        chunked = self.chunks(self.resource, int(len(self.resource) / mp.cpu_count()))
-        chunk_list = pool.map(self.resolve_targets_m, chunked)
-        pool.close()
-        return [item for sublist in chunk_list for item in sublist]
-
-    def resolve_targets_m(self, resource) -> List[dict]:
+    def resolve_targets(self) -> List[dict]:
         return [
             self.fill_entry_template(
                 self.entry_template, entry, self.getValueFromJsonPath
             )
-            for entry in tqdm(resource)
+            for entry in tqdm(self.resource)
         ]
 
     def fill_listof_entry_template(self, listof_dict: dict, entry, convert_function) -> list:
         listof = [match for match in convert_function(entry, listof_dict['listof'])]
         if not listof:
             return listof
         new_els = []
         if isinstance(listof_dict['value'], dict) and "listof" in listof_dict['value']:
             listof_dict['listof'] = listof_dict['value']['listof']
             listof_dict['value'] = listof_dict['value']['value']
             for el in listof:
-                json_expr = json_parse(f"{el.full_path}")
+                json_expr = self.get_matcher(f"{el.full_path}")
                 items = [match.value for match in json_expr.find(entry)][0]
                 for item in items:
                     i = items.index(item)
-                    item_json_expr = json_parse(f"{json_expr}.[{i}]")
+                    item_json_expr = self.get_matcher(f"{json_expr}.[{i}]")
                     new_entry = [match.value for match in item_json_expr.find(entry)]
                     el = self.fill_listof_entry_template(listof_dict, new_entry, convert_function)
                     new_els.append(el)
         elif isinstance(listof_dict['value'], dict):
             items = [match.value for match in listof][0]
             if isinstance(items, dict):
                 items = [items]
             json_expr = listof[0].full_path
             for el in items:
                 i = items.index(el)
                 new_el = {}
-                for k,v in listof_dict['value'].items():
-                    new_json_expr = json_parse(f"{json_expr}.[{i}].[{v.strip()}]")
+                for k, v in listof_dict['value'].items():
+                    new_json_expr = self.get_matcher(f"{json_expr}.[{i}].[{v.strip()}]")
                     new_el[k] = self.validate_type(k, [match.value for match in new_json_expr.find(entry)])
                 new_els.append(new_el)
         else:
             for el in listof:
-                json_expr = json_parse(f"{el.full_path}")
+                json_expr = self.get_matcher(f"{el.full_path}")
                 items = [match.value for match in json_expr.find(entry)][0]
                 for item in items:
                     i = items.index(item)
-                    new_json_expr = json_parse(f"{json_expr}.[{i}]")
+                    new_json_expr = self.get_matcher(f"{json_expr}.[{i}]")
                     new_el = [match.value for match in new_json_expr.find(entry)][0]
                     new_els.append(new_el)
 
         return new_els
 
-    
     def fill_entry_template(self, entry_template: dict, entry, convert_function) -> dict:
         '''This recursive function "fills in" the data according to the resource manifest. This is a slight modification from the one used by all parsers.
 
         Args:
             :param dict entry_template: The template for an entry. Keys are preserved, values are usually paths in the resource to data (JSONPath, XPath or Cell coordinates etc)
             :param any entry: The actual word/entry to extract some data from. This could be a row, or json dict or any piece of nested data from the data resource.
             :param function convert_function: A function that takes an entry and a path and returns the "filled in" object
@@ -130,14 +117,14 @@
                 new_lemma[k] = new_v
             else:
                 try:
                     new_lemma[k] = self.validate_type(k, convert_function(entry, v.strip()))
                 except:
                     breakpoint()
         return new_lemma
-    
+
     def parse(self) -> Dict[str, Union[dict, pd.DataFrame]]:
         try:
             data = self.resolve_targets()
             return {"manifest": self.manifest, "data": pd.DataFrame(data)}
         except JsonPointerException as e:
             raise e
```

### Comparing `mothertongues-0.18.20230410/mtd/parsers/pkl_parser.py` & `mothertongues-0.18.20230502/mtd/parsers/pkl_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 import pandas as pd
 from mtd.exceptions import SchemaValidationError
 from mtd.parsers.json_parser import Parser as JsonParser
 from mtd.languages import MANIFEST_SCHEMA
 from jsonschema.exceptions import ValidationError
 from mtd.parsers.utils import ResourceManifest
 from typing import Dict, List, Union
-from jsonpath_rw import parse as json_parse
+from jsonpath_ng import parse as json_parse
 import pickle
 
 class Parser(JsonParser):
     '''
     Parse data for MTD. location (jsonpath) specifies location of data
 
     :param ResourceManifest manifest: Manifest for parser
     :param (str or json) resource_path: Dict or path to pkl
     '''
     def __init__(self, manifest: ResourceManifest, resource_path: Union[str, dict, list]):
+        self.path_cache = {}
         self.manifest = manifest
         try:
             if isinstance(resource_path, str):
                 with open(resource_path, 'rb') as f:
                     self.resource = pickle.load(f)
             elif isinstance(resource_path, (dict, list)):
                 self.resource = resource_path
         except ValueError:
             raise SchemaValidationError('json', resource_path)
         if "location" in self.manifest:
             self.resource = resolve_pointer(self.resource, self.manifest['location'])
-        self.entry_template = self.manifest['targets']
+        self.entry_template = self.manifest['targets']
```

### Comparing `mothertongues-0.18.20230410/mtd/parsers/psv_parser.py` & `mothertongues-0.18.20230502/mtd/parsers/psv_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/parsers/request_parser.py` & `mothertongues-0.18.20230502/mtd/parsers/request_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/parsers/tsv_parser.py` & `mothertongues-0.18.20230502/mtd/parsers/tsv_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/parsers/utils.py` & `mothertongues-0.18.20230502/mtd/parsers/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from mtd.languages import MANIFEST_SCHEMA
 from urllib.parse import urlparse
 import json
 from jsonschema import validate
 from jsonschema.exceptions import ValidationError
 from mtd.tests import logger
 from typing import Dict, List, Union
-from jsonpath_rw import jsonpath, parse as json_parse
+from jsonpath_ng import jsonpath, parse as json_parse
 import requests
 import os
 
 class ResourceManifest():
     '''A manifest file for a given resource.
 
        Resources in this case are lexical resources. They can be in any format supported by MTD and the resources
@@ -158,15 +158,15 @@
                     try:
                         new_lemma[k] = self.validate_type(k, convert_function(entry, v.strip()))
                     except:
                         new_lemma[k] = v.strip()
         return new_lemma
     
     def validate_type(self, k, v):
-        '''Some parsers like lxml and jsonpath_rw return lists when the data manifest does not specify a list, this corrects that.
+        '''Some parsers like lxml and jsonpath_ng return lists when the data manifest does not specify a list, this corrects that.
         '''
         if type(v) == list and len(v) > 0 and type(v[0]) == jsonpath.DatumInContext:
             v = v[0].value
         if isinstance(v, list) and len(v) == 1 and self.return_manifest_key_type(k, self.manifest.manifest) != list:
             return v[0]
         else:
-            return v
+            return v
```

### Comparing `mothertongues-0.18.20230410/mtd/parsers/xlsx_parser.py` & `mothertongues-0.18.20230502/mtd/parsers/xlsx_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/parsers/xml_parser.py` & `mothertongues-0.18.20230502/mtd/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/processors/sorter.py` & `mothertongues-0.18.20230502/mtd/processors/sorter.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/processors/transducer.py` & `mothertongues-0.18.20230502/mtd/processors/transducer.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/processors/validator.py` & `mothertongues-0.18.20230502/mtd/processors/validator.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/resources.py` & `mothertongues-0.18.20230502/mtd/resources.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/static/active.sites.json` & `mothertongues-0.18.20230502/mtd/static/active.sites.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/static/assets/icon/favicon.ico` & `mothertongues-0.18.20230502/mtd/static/assets/icon/favicon.ico`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/static/assets/js/dict_cached-danish.js` & `mothertongues-0.18.20230502/mtd/static/assets/js/dict_cached-danish.js`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/static/css/custom.css` & `mothertongues-0.18.20230502/mtd/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/static/css/normalize.css` & `mothertongues-0.18.20230502/mtd/static/css/normalize.css`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/static/css/skeleton.css` & `mothertongues-0.18.20230502/mtd/static/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/static/swagger-ui/favicon-32x32.png` & `mothertongues-0.18.20230502/mtd/static/swagger-ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/static/swagger-ui/swagger-ui-bundle.js` & `mothertongues-0.18.20230502/mtd/static/swagger-ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/static/swagger-ui/swagger-ui-standalone-preset.js` & `mothertongues-0.18.20230502/mtd/static/swagger-ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/static/swagger-ui/swagger-ui.css` & `mothertongues-0.18.20230502/mtd/static/swagger-ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/static/swagger.json` & `mothertongues-0.18.20230502/mtd/static/swagger.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/templates/apidocs.html` & `mothertongues-0.18.20230502/mtd/templates/apidocs.html`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/templates/dictionary.html` & `mothertongues-0.18.20230502/mtd/templates/dictionary.html`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/templates/index.html` & `mothertongues-0.18.20230502/mtd/templates/index.html`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/templates/stats.html` & `mothertongues-0.18.20230502/mtd/templates/stats.html`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/templates/validator.html` & `mothertongues-0.18.20230502/mtd/templates/validator.html`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/__init__.py` & `mothertongues-0.18.20230502/mtd/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/integration/config_test.json` & `mothertongues-0.18.20230502/mtd/tests/integration/config_test.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/integration/test_api_resources.py` & `mothertongues-0.18.20230502/mtd/tests/integration/test_api_resources.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/integration/test_basic_integration.py` & `mothertongues-0.18.20230502/mtd/tests/integration/test_basic_integration.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/integration/test_cli.py` & `mothertongues-0.18.20230502/mtd/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/run.py` & `mothertongues-0.18.20230502/mtd/tests/run.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_cli.py` & `mothertongues-0.18.20230502/mtd/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_csv_parser.py` & `mothertongues-0.18.20230502/mtd/tests/test_csv_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/csv/data.csv` & `mothertongues-0.18.20230502/mtd/tests/test_data/csv/data.csv`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/csv/manifest.json` & `mothertongues-0.18.20230502/mtd/tests/test_data/csv/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/json/data.json` & `mothertongues-0.18.20230502/mtd/tests/test_data/json/data.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/json/data_reduced.json` & `mothertongues-0.18.20230502/mtd/tests/test_data/json/data_reduced.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/json/dict_manifest.json` & `mothertongues-0.18.20230502/mtd/tests/test_data/json/dict_manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/json/manifest.json` & `mothertongues-0.18.20230502/mtd/tests/test_data/json/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/pkl/data.pkl` & `mothertongues-0.18.20230502/mtd/tests/test_data/pkl/data.pkl`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/pkl/manifest.json` & `mothertongues-0.18.20230502/mtd/tests/test_data/pkl/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/psv/data.psv` & `mothertongues-0.18.20230502/mtd/tests/test_data/psv/data.psv`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/psv/manifest.json` & `mothertongues-0.18.20230502/mtd/tests/test_data/psv/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/tsv/data.tsv` & `mothertongues-0.18.20230502/mtd/tests/test_data/tsv/data.tsv`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/tsv/manifest.json` & `mothertongues-0.18.20230502/mtd/tests/test_data/tsv/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/whitespace_manifest.json` & `mothertongues-0.18.20230502/mtd/tests/test_data/whitespace_manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/data.xlsx` & `mothertongues-0.18.20230502/mtd/tests/test_data/xlsx/data.xlsx`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/manifest.json` & `mothertongues-0.18.20230502/mtd/tests/test_data/xlsx/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/manifest.xlsx` & `mothertongues-0.18.20230502/mtd/tests/test_data/xlsx/manifest.xlsx`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/manifest_alternate.json` & `mothertongues-0.18.20230502/mtd/tests/test_data/xlsx/manifest_alternate.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/missing_sheet_data.xlsx` & `mothertongues-0.18.20230502/mtd/tests/test_data/xlsx/missing_sheet_data.xlsx`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/xml/data.xml` & `mothertongues-0.18.20230502/mtd/tests/test_data/xml/data.xml`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/xml/data_reduced.xml` & `mothertongues-0.18.20230502/mtd/tests/test_data/xml/data_reduced.xml`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data/xml/manifest.json` & `mothertongues-0.18.20230502/mtd/tests/test_data/xml/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_data_configuration_parser.py` & `mothertongues-0.18.20230502/mtd/tests/test_data_configuration_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_dict_parser.py` & `mothertongues-0.18.20230502/mtd/tests/test_dict_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_dictionary.py` & `mothertongues-0.18.20230502/mtd/tests/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_json_parser.py` & `mothertongues-0.18.20230502/mtd/tests/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_pkl_parser.py` & `mothertongues-0.18.20230502/mtd/tests/test_pkl_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_psv_parser.py` & `mothertongues-0.18.20230502/mtd/tests/test_psv_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_request_parser.py` & `mothertongues-0.18.20230502/mtd/tests/test_request_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_sorter.py` & `mothertongues-0.18.20230502/mtd/tests/test_sorter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import TestCase
 from mtd.processors.sorter import ArbSorter
 from string import ascii_lowercase
 from pandas import DataFrame
-from pandas.util.testing import assert_frame_equal
+from pandas.testing import assert_frame_equal
 
 
 class SorterTest(TestCase):
     def setUp(self):
         self.english_alphabet = list(ascii_lowercase)
         self.danish_alphabet = self.english_alphabet + ["æ", "ø", "å"]
```

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_transducer.py` & `mothertongues-0.18.20230502/mtd/tests/test_transducer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest import main, TestCase
 from mtd.processors.transducer import Transducer
 from pandas import DataFrame
-from pandas.util.testing import assert_frame_equal
+from pandas.testing import assert_frame_equal
 import os
 import mtd.tests.test_data.transducers as test_transducers_path
 import mtd.transducers as transducers_path
 from mtd.exceptions import TransducerNotFoundError, TransducerSourceNotFoundError
 from js2py import eval_js
 
 class TransducerTest(TestCase):
```

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_tsv_parser.py` & `mothertongues-0.18.20230502/mtd/tests/test_tsv_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_validator.py` & `mothertongues-0.18.20230502/mtd/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_xlsx_parser.py` & `mothertongues-0.18.20230502/mtd/tests/test_xlsx_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/tests/test_xml_parser.py` & `mothertongues-0.18.20230502/mtd/tests/test_xml_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/transducers/config.yaml` & `mothertongues-0.18.20230502/mtd/transducers/config.yaml`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/mtd/views.py` & `mothertongues-0.18.20230502/mtd/views.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20230410/setup.py` & `mothertongues-0.18.20230502/setup.py`

 * *Files identical despite different names*

