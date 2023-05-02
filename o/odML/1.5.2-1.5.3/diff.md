# Comparing `tmp/odML-1.5.2.tar.gz` & `tmp/odML-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odML-1.5.2.tar", last modified: Mon Dec  6 09:38:17 2021, max compression
+gzip compressed data, was "odML-1.5.3.tar", last modified: Wed Apr 19 17:54:31 2023, max compression
```

## Comparing `odML-1.5.2.tar` & `odML-1.5.3.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.706331 odML-1.5.2/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    34888 2021-11-02 09:01:52.000000 odML-1.5.2/CHANGELOG.md
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     1635 2021-11-02 09:01:52.000000 odML-1.5.2/LICENSE
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      132 2020-02-18 13:54:57.000000 odML-1.5.2/MANIFEST.in
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     6018 2021-12-06 09:38:17.706331 odML-1.5.2/PKG-INFO
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     5213 2021-06-21 12:40:25.000000 odML-1.5.2/README.md
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.698331 odML-1.5.2/odML.egg-info/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     6018 2021-12-06 09:38:17.000000 odML-1.5.2/odML.egg-info/PKG-INFO
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     3653 2021-12-06 09:38:17.000000 odML-1.5.2/odML.egg-info/SOURCES.txt
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)        1 2021-12-06 09:38:17.000000 odML-1.5.2/odML.egg-info/dependency_links.txt
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      197 2021-12-06 09:38:17.000000 odML-1.5.2/odML.egg-info/entry_points.txt
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)       63 2021-12-06 09:38:17.000000 odML-1.5.2/odML.egg-info/requires.txt
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)        5 2021-12-06 09:38:17.000000 odML-1.5.2/odML.egg-info/top_level.txt
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.698331 odML-1.5.2/odml/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     4394 2021-11-02 09:01:52.000000 odML-1.5.2/odml/__init__.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    23748 2020-05-14 06:39:54.000000 odML-1.5.2/odml/base.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     5936 2020-05-14 06:39:54.000000 odML-1.5.2/odml/doc.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     9258 2021-06-21 12:40:25.000000 odML-1.5.2/odml/dtypes.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     2140 2021-06-21 12:40:25.000000 odML-1.5.2/odml/fileio.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     5249 2021-06-21 12:40:25.000000 odML-1.5.2/odml/format.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      729 2021-12-06 09:37:56.000000 odML-1.5.2/odml/info.json
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      401 2020-01-17 15:05:51.000000 odML-1.5.2/odml/info.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    36784 2021-06-21 12:40:25.000000 odML-1.5.2/odml/property.py
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.698331 odML-1.5.2/odml/rdf/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)        0 2020-01-17 15:05:51.000000 odML-1.5.2/odml/rdf/__init__.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     8407 2020-02-12 14:19:51.000000 odML-1.5.2/odml/rdf/fuzzy_finder.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    12209 2020-05-14 06:39:54.000000 odML-1.5.2/odml/rdf/query_creator.py
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.698331 odML-1.5.2/odml/resources/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    37003 2020-01-17 15:05:51.000000 odML-1.5.2/odml/resources/odml-ontology.ttl
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     2182 2020-01-17 15:05:51.000000 odML-1.5.2/odml/resources/section_subclasses.yaml
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.698331 odML-1.5.2/odml/scripts/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)        0 2019-11-07 11:50:53.000000 odML-1.5.2/odml/scripts/__init__.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     4528 2021-06-21 12:40:25.000000 odML-1.5.2/odml/scripts/odml_convert.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     5568 2021-06-21 12:40:25.000000 odML-1.5.2/odml/scripts/odml_to_rdf.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     3582 2019-11-07 11:50:53.000000 odML-1.5.2/odml/scripts/odml_view.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    32926 2020-08-12 13:06:11.000000 odML-1.5.2/odml/section.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     5954 2021-06-21 12:40:25.000000 odML-1.5.2/odml/templates.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     4202 2021-06-21 12:40:25.000000 odML-1.5.2/odml/terminology.py
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.702331 odML-1.5.2/odml/tools/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      187 2020-01-17 15:05:51.000000 odML-1.5.2/odml/tools/__init__.py
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.702331 odML-1.5.2/odml/tools/converters/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      140 2020-01-17 15:05:51.000000 odML-1.5.2/odml/tools/converters/__init__.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     8017 2021-06-21 12:40:25.000000 odML-1.5.2/odml/tools/converters/format_converter.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    20161 2021-06-21 12:40:25.000000 odML-1.5.2/odml/tools/converters/version_converter.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    13494 2020-05-14 06:39:54.000000 odML-1.5.2/odml/tools/dict_parser.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     1431 2020-02-12 14:19:51.000000 odML-1.5.2/odml/tools/doc_inherit.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     2138 2020-02-12 14:19:51.000000 odML-1.5.2/odml/tools/dumper.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    12624 2021-06-21 12:40:25.000000 odML-1.5.2/odml/tools/odmlparser.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     1427 2020-05-14 06:39:54.000000 odML-1.5.2/odml/tools/parser_utils.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    22710 2021-10-18 17:28:45.000000 odML-1.5.2/odml/tools/rdf_converter.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      478 2020-05-14 06:39:54.000000 odML-1.5.2/odml/tools/version_converter.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    34074 2021-06-21 12:40:25.000000 odML-1.5.2/odml/tools/xmlparser.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     2232 2020-05-14 06:39:54.000000 odML-1.5.2/odml/util.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    21621 2021-06-21 12:40:25.000000 odML-1.5.2/odml/validation.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)       38 2021-12-06 09:38:17.706331 odML-1.5.2/setup.cfg
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     2379 2021-11-02 09:01:52.000000 odML-1.5.2/setup.py
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.702331 odML-1.5.2/test/
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.706331 odML-1.5.2/test/resources/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    10839 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/example.odml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     1877 2019-09-27 09:19:35.000000 odML-1.5.2/test/resources/ignore_errors.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      102 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/invalid_root.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      170 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/invalid_version.json
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      114 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/invalid_version.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      119 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/invalid_version.yaml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      134 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/local_repository_file_v1.0.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      134 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/local_repository_file_v1.1.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)       85 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/missing_root.json
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)       20 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/missing_root.yaml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      139 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/missing_version.json
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)       96 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/missing_version.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)       85 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/missing_version.yaml
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.698331 odML-1.5.2/test/resources/scripts/
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.706331 odML-1.5.2/test/resources/scripts/odml_convert/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     2888 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_convert/conversion_example_A.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     2888 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_convert/conversion_example_B.xml
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.706331 odML-1.5.2/test/resources/scripts/odml_convert/test_broken/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)        0 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_convert/test_broken/empty.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      471 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_convert/test_broken/invalid_xml.xml
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.706331 odML-1.5.2/test/resources/scripts/odml_convert/test_recursive/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      723 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_convert/test_recursive/conversion_example_sub_root.xml
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.706331 odML-1.5.2/test/resources/scripts/odml_convert/test_recursive/sub/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      723 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_convert/test_recursive/sub/conversion_example_sub_sub.xml
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.706331 odML-1.5.2/test/resources/scripts/odml_to_rdf/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    10249 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_to_rdf/example_A.doi.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    10249 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_to_rdf/example_B.doi.xml
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.706331 odML-1.5.2/test/resources/scripts/odml_to_rdf/test_invalid/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      471 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_to_rdf/test_invalid/invalid.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      105 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_to_rdf/test_invalid/not_odml.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)       10 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_to_rdf/test_invalid/not_xml.md
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.706331 odML-1.5.2/test/resources/scripts/odml_to_rdf/test_recursive/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    10249 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_to_rdf/test_recursive/example_sub_root.doi.xml
-drwxrwxr-x   0 msonntag  (1001) msonntag  (1001)        0 2021-12-06 09:38:17.706331 odML-1.5.2/test/resources/scripts/odml_to_rdf/test_recursive/sub/
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    10249 2020-08-12 13:06:32.000000 odML-1.5.2/test/resources/scripts/odml_to_rdf/test_recursive/sub/example_sub.doi.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    15534 2020-05-14 06:39:54.000000 odML-1.5.2/test/resources/validation_dtypes.json
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     6778 2020-05-14 06:39:54.000000 odML-1.5.2/test/resources/validation_dtypes.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     6102 2020-05-14 06:39:54.000000 odML-1.5.2/test/resources/validation_dtypes.yaml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      567 2020-05-14 06:39:54.000000 odML-1.5.2/test/resources/validation_section.json
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      412 2020-05-14 06:39:54.000000 odML-1.5.2/test/resources/validation_section.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      314 2020-05-14 06:39:54.000000 odML-1.5.2/test/resources/validation_section.yaml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     1013 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/version_conversion.json
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      551 2019-09-16 13:45:33.000000 odML-1.5.2/test/resources/version_conversion.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      355 2019-09-16 13:49:18.000000 odML-1.5.2/test/resources/version_conversion.yaml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    11209 2019-10-21 14:39:39.000000 odML-1.5.2/test/resources/version_conversion_int.json
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     5462 2019-10-21 14:39:39.000000 odML-1.5.2/test/resources/version_conversion_int.xml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     4553 2019-10-21 14:39:39.000000 odML-1.5.2/test/resources/version_conversion_int.yaml
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)      458 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_bugs.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    11606 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_doc.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     5943 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_doc_integration.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     7994 2021-06-21 12:40:25.000000 odML-1.5.2/test/test_dtypes.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    19011 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_dtypes_integration.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     2117 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_dumper.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     1450 2021-06-21 12:40:25.000000 odML-1.5.2/test/test_fileio.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     1302 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_find_section.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     5763 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_format_converter.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     3552 2021-06-21 12:40:25.000000 odML-1.5.2/test/test_infer_type.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     3229 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_iterators.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     1689 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_links.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     7201 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_parser_json.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    12328 2021-06-21 12:40:25.000000 odML-1.5.2/test/test_parser_odml.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     1566 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_parser_xml.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     6445 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_parser_yaml.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    47981 2020-08-12 13:06:32.000000 odML-1.5.2/test/test_property.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     7970 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_property_integration.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     5657 2021-10-18 17:28:54.000000 odML-1.5.2/test/test_rdf_reader.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    20519 2020-08-12 13:06:32.000000 odML-1.5.2/test/test_rdf_writer.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    11901 2021-06-21 12:40:25.000000 odML-1.5.2/test/test_samplefile.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     3295 2020-08-12 13:06:32.000000 odML-1.5.2/test/test_script_odml_convert.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     3333 2020-08-12 13:06:32.000000 odML-1.5.2/test/test_script_odml_to_rdf.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    44893 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_section.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    11768 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_section_integration.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     4520 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_terminology.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     2520 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_util.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    18797 2020-08-12 13:06:11.000000 odML-1.5.2/test/test_validation.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     4543 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_validation_integration.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)    35866 2021-06-21 12:40:25.000000 odML-1.5.2/test/test_version_converter.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     2966 2020-05-14 06:39:54.000000 odML-1.5.2/test/test_version_converter_integration.py
--rw-rw-r--   0 msonntag  (1001) msonntag  (1001)     3216 2021-06-21 12:40:25.000000 odML-1.5.2/test/test_xml_writer.py
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.295595 odML-1.5.3/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    35439 2023-04-19 17:29:42.000000 odML-1.5.3/CHANGELOG.md
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     1635 2023-02-22 09:18:24.000000 odML-1.5.3/LICENSE
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      132 2021-06-16 13:44:43.000000 odML-1.5.3/MANIFEST.in
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     6004 2023-04-19 17:54:31.295595 odML-1.5.3/PKG-INFO
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     5218 2023-04-19 17:29:42.000000 odML-1.5.3/README.md
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.283595 odML-1.5.3/odML.egg-info/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     6004 2023-04-19 17:54:31.000000 odML-1.5.3/odML.egg-info/PKG-INFO
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     3653 2023-04-19 17:54:31.000000 odML-1.5.3/odML.egg-info/SOURCES.txt
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)        1 2023-04-19 17:54:31.000000 odML-1.5.3/odML.egg-info/dependency_links.txt
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      196 2023-04-19 17:54:31.000000 odML-1.5.3/odML.egg-info/entry_points.txt
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)       46 2023-04-19 17:54:31.000000 odML-1.5.3/odML.egg-info/requires.txt
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)        5 2023-04-19 17:54:31.000000 odML-1.5.3/odML.egg-info/top_level.txt
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.287595 odML-1.5.3/odml/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     4394 2023-04-19 17:29:42.000000 odML-1.5.3/odml/__init__.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    23748 2021-06-16 13:44:43.000000 odML-1.5.3/odml/base.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     5936 2021-06-16 13:44:43.000000 odML-1.5.3/odml/doc.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     9258 2023-02-22 09:18:24.000000 odML-1.5.3/odml/dtypes.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     2140 2023-02-22 09:18:24.000000 odML-1.5.3/odml/fileio.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     5249 2023-02-22 09:18:24.000000 odML-1.5.3/odml/format.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      730 2023-04-19 17:54:15.000000 odML-1.5.3/odml/info.json
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      401 2021-06-16 13:44:43.000000 odML-1.5.3/odml/info.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    36784 2023-02-22 09:18:24.000000 odML-1.5.3/odml/property.py
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.287595 odML-1.5.3/odml/rdf/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)        0 2021-06-16 13:44:43.000000 odML-1.5.3/odml/rdf/__init__.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     8407 2021-06-16 13:44:43.000000 odML-1.5.3/odml/rdf/fuzzy_finder.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    12209 2021-06-16 13:44:43.000000 odML-1.5.3/odml/rdf/query_creator.py
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.287595 odML-1.5.3/odml/resources/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    37003 2021-06-16 13:44:43.000000 odML-1.5.3/odml/resources/odml-ontology.ttl
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     2182 2021-06-16 13:44:43.000000 odML-1.5.3/odml/resources/section_subclasses.yaml
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.287595 odML-1.5.3/odml/scripts/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)        0 2021-06-16 13:44:43.000000 odML-1.5.3/odml/scripts/__init__.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     4528 2023-02-22 09:18:24.000000 odML-1.5.3/odml/scripts/odml_convert.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     5568 2023-02-22 09:18:24.000000 odML-1.5.3/odml/scripts/odml_to_rdf.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     3582 2021-06-16 13:44:43.000000 odML-1.5.3/odml/scripts/odml_view.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    32926 2023-02-22 09:18:24.000000 odML-1.5.3/odml/section.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     5954 2023-02-22 09:18:24.000000 odML-1.5.3/odml/templates.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     4202 2023-02-22 09:18:24.000000 odML-1.5.3/odml/terminology.py
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.287595 odML-1.5.3/odml/tools/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      187 2021-06-16 13:44:43.000000 odML-1.5.3/odml/tools/__init__.py
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.287595 odML-1.5.3/odml/tools/converters/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      140 2021-06-16 13:44:43.000000 odML-1.5.3/odml/tools/converters/__init__.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     8017 2023-02-22 09:18:24.000000 odML-1.5.3/odml/tools/converters/format_converter.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    20161 2023-02-22 09:18:24.000000 odML-1.5.3/odml/tools/converters/version_converter.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    13494 2021-06-16 13:44:43.000000 odML-1.5.3/odml/tools/dict_parser.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     1431 2021-06-16 13:44:43.000000 odML-1.5.3/odml/tools/doc_inherit.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     2138 2021-06-16 13:44:43.000000 odML-1.5.3/odml/tools/dumper.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    12624 2023-02-22 09:18:24.000000 odML-1.5.3/odml/tools/odmlparser.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     1427 2021-06-16 13:44:43.000000 odML-1.5.3/odml/tools/parser_utils.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    24401 2023-04-19 17:29:42.000000 odML-1.5.3/odml/tools/rdf_converter.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      478 2021-06-16 13:44:43.000000 odML-1.5.3/odml/tools/version_converter.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    34074 2023-02-22 09:18:24.000000 odML-1.5.3/odml/tools/xmlparser.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     2232 2021-06-16 13:44:43.000000 odML-1.5.3/odml/util.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    21621 2023-02-22 09:18:24.000000 odML-1.5.3/odml/validation.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)       38 2023-04-19 17:54:31.295595 odML-1.5.3/setup.cfg
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     2591 2023-04-17 10:03:16.000000 odML-1.5.3/setup.py
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.291595 odML-1.5.3/test/
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.295595 odML-1.5.3/test/resources/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    10839 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/example.odml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     1877 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/ignore_errors.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      102 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/invalid_root.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      170 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/invalid_version.json
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      114 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/invalid_version.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      119 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/invalid_version.yaml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      134 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/local_repository_file_v1.0.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      134 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/local_repository_file_v1.1.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)       85 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/missing_root.json
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)       20 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/missing_root.yaml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      139 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/missing_version.json
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)       96 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/missing_version.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)       85 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/missing_version.yaml
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.283595 odML-1.5.3/test/resources/scripts/
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.295595 odML-1.5.3/test/resources/scripts/odml_convert/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     2888 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_convert/conversion_example_A.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     2888 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_convert/conversion_example_B.xml
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.295595 odML-1.5.3/test/resources/scripts/odml_convert/test_broken/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)        0 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_convert/test_broken/empty.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      471 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_convert/test_broken/invalid_xml.xml
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.295595 odML-1.5.3/test/resources/scripts/odml_convert/test_recursive/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      723 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_convert/test_recursive/conversion_example_sub_root.xml
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.295595 odML-1.5.3/test/resources/scripts/odml_convert/test_recursive/sub/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      723 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_convert/test_recursive/sub/conversion_example_sub_sub.xml
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.295595 odML-1.5.3/test/resources/scripts/odml_to_rdf/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    10249 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_to_rdf/example_A.doi.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    10249 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_to_rdf/example_B.doi.xml
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.295595 odML-1.5.3/test/resources/scripts/odml_to_rdf/test_invalid/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      471 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_to_rdf/test_invalid/invalid.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      105 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_to_rdf/test_invalid/not_odml.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)       10 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_to_rdf/test_invalid/not_xml.md
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.295595 odML-1.5.3/test/resources/scripts/odml_to_rdf/test_recursive/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    10249 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_to_rdf/test_recursive/example_sub_root.doi.xml
+drwxrwxr-x   0 msonntag  (1000) msonntag  (1000)        0 2023-04-19 17:54:31.295595 odML-1.5.3/test/resources/scripts/odml_to_rdf/test_recursive/sub/
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    10249 2023-02-22 09:18:24.000000 odML-1.5.3/test/resources/scripts/odml_to_rdf/test_recursive/sub/example_sub.doi.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    15534 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/validation_dtypes.json
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     6778 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/validation_dtypes.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     6102 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/validation_dtypes.yaml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      567 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/validation_section.json
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      412 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/validation_section.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      314 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/validation_section.yaml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     1013 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/version_conversion.json
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      551 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/version_conversion.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      355 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/version_conversion.yaml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    11209 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/version_conversion_int.json
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     5462 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/version_conversion_int.xml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     4553 2021-06-16 13:44:43.000000 odML-1.5.3/test/resources/version_conversion_int.yaml
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)      458 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_bugs.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    11606 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_doc.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     5943 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_doc_integration.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     7994 2023-02-22 09:18:24.000000 odML-1.5.3/test/test_dtypes.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    19011 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_dtypes_integration.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     2117 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_dumper.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     1450 2023-02-22 09:18:24.000000 odML-1.5.3/test/test_fileio.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     1302 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_find_section.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     5763 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_format_converter.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     3552 2023-02-22 09:18:24.000000 odML-1.5.3/test/test_infer_type.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     3229 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_iterators.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     1689 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_links.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     7201 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_parser_json.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    12328 2023-02-22 09:18:24.000000 odML-1.5.3/test/test_parser_odml.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     1566 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_parser_xml.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     6445 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_parser_yaml.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    47981 2023-02-22 09:18:24.000000 odML-1.5.3/test/test_property.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     7970 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_property_integration.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     6089 2023-04-17 10:03:16.000000 odML-1.5.3/test/test_rdf_reader.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    19770 2023-04-17 10:03:16.000000 odML-1.5.3/test/test_rdf_writer.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    11901 2023-02-22 09:18:24.000000 odML-1.5.3/test/test_samplefile.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     3295 2023-02-22 09:18:24.000000 odML-1.5.3/test/test_script_odml_convert.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     3333 2023-02-22 09:18:24.000000 odML-1.5.3/test/test_script_odml_to_rdf.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    44893 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_section.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    11768 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_section_integration.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     4520 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_terminology.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     2520 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_util.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    18797 2023-02-22 09:18:24.000000 odML-1.5.3/test/test_validation.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     4543 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_validation_integration.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)    35866 2023-02-22 09:18:24.000000 odML-1.5.3/test/test_version_converter.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     2966 2021-06-16 13:44:43.000000 odML-1.5.3/test/test_version_converter_integration.py
+-rw-rw-r--   0 msonntag  (1000) msonntag  (1000)     3216 2023-02-22 09:18:24.000000 odML-1.5.3/test/test_xml_writer.py
```

### Comparing `odML-1.5.2/CHANGELOG.md` & `odML-1.5.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 # Changelog
 
 Used to document all changes from previous releases and collect changes 
 until the next release.
 
 
+# Version 1.5.3
+
+## Support rdflib version 6+
+
+The rdflib upgrade from version 5.0.0 to 6+ introduced breaking changes 
+in the rdflib library. This update fixes these breaks without changing 
+functionality, unpins the rdflib version and defaults to the latest
+version on install.
+
+## Dropping official support for Python 3.5 and 3.6
+
+The introduction of the rdflib 6+ library restricts the
+Python support for 3.7+.
+
+It is still possible to install odml with a Python version <=3.6, 
+but these versions are no longer tested and officially supported.
+
+
 # Version 1.5.2
 
 ## Pinning rdflib version to 5.0.0 until further notice
 
 Due to major breaking changes introduced in the upgrade of
 rdflib 5.0.0 to 6.0.0, the rdflib version is pinned to 5.0.0
 until the breaking code has been fixed.
```

### Comparing `odML-1.5.2/LICENSE` & `odML-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/PKG-INFO` & `odML-1.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: odML
-Version: 1.5.2
+Version: 1.5.3
 Summary: open metadata Markup Language
 Home-page: https://github.com/G-Node/python-odml
 Author: Hagen Fritsch, Jan Grewe, Christian Kellner, Achilleas Koutsou, Michael Sonntag, Lyuba Zehl
 Author-email: dev@g-node.org
 License: BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![gh actions tests](https://github.com/G-Node/python-odml/workflows/run-tests/badge.svg?branch=master)](https://github.com/G-Node/python-odml/actions)
@@ -94,15 +93,15 @@
 
 For details regarding the introduced changes please check the [github
 release notes](https://github.com/G-Node/python-odml/releases).
 
 
 # Dependencies
 
-* Python 3.6+
+* Python 3.7+
 * Python packages:
 
   * lxml (version 3.7.2)
   * yaml (version >= 5.1)
   * rdflib (version >=4.2.2)
 
 * These packages will be downloaded and installed automatically if the ```pip```
@@ -118,15 +117,17 @@
 
   * libxml2-dev
   * libxslt1-dev
   * lib32z1-dev
 
 ## Previous Python versions
 
-Python 2 has reached end of life. We will not keep any future versions of odml Python 2 compatible and will completely drop support for Python 2 with August 2020. We also recommend using a Python version >= 3.6. If a Python version < 3.6 is a requirement, the following dependency needs to be installed as well:
+Python 2 has reached end of life. Current and future versions of odml are not Python 2 compatible. We removed support 
+for Python 2 in August 2020 with version 1.5.2. We also recommend using a Python version >= 3.7. If a 
+Python version < 3.7 is a requirement, the following dependency needs to be installed as well:
 
 * pip install
   * enum34 (version 0.4.4)
 * apt install
   * python-enum
 
 # Building from source
@@ -162,9 +163,7 @@
 # Bugs & Questions
 
 Should you find a behaviour that is likely a bug, please file a bug report at
 [the github bug tracker](https://github.com/G-Node/python-odml/issues).
 
 If you have questions regarding the use of the library, feel free to join the
 [#gnode](http://webchat.freenode.net?channels=%23gnode) IRC channel on freenode.
-
-
```

### Comparing `odML-1.5.2/README.md` & `odML-1.5.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 For details regarding the introduced changes please check the [github
 release notes](https://github.com/G-Node/python-odml/releases).
 
 
 # Dependencies
 
-* Python 3.6+
+* Python 3.7+
 * Python packages:
 
   * lxml (version 3.7.2)
   * yaml (version >= 5.1)
   * rdflib (version >=4.2.2)
 
 * These packages will be downloaded and installed automatically if the ```pip```
@@ -97,15 +97,17 @@
 
   * libxml2-dev
   * libxslt1-dev
   * lib32z1-dev
 
 ## Previous Python versions
 
-Python 2 has reached end of life. We will not keep any future versions of odml Python 2 compatible and will completely drop support for Python 2 with August 2020. We also recommend using a Python version >= 3.6. If a Python version < 3.6 is a requirement, the following dependency needs to be installed as well:
+Python 2 has reached end of life. Current and future versions of odml are not Python 2 compatible. We removed support 
+for Python 2 in August 2020 with version 1.5.2. We also recommend using a Python version >= 3.7. If a 
+Python version < 3.7 is a requirement, the following dependency needs to be installed as well:
 
 * pip install
   * enum34 (version 0.4.4)
 * apt install
   * python-enum
 
 # Building from source
```

### Comparing `odML-1.5.2/odML.egg-info/PKG-INFO` & `odML-1.5.3/odML.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: odML
-Version: 1.5.2
+Version: 1.5.3
 Summary: open metadata Markup Language
 Home-page: https://github.com/G-Node/python-odml
 Author: Hagen Fritsch, Jan Grewe, Christian Kellner, Achilleas Koutsou, Michael Sonntag, Lyuba Zehl
 Author-email: dev@g-node.org
 License: BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![gh actions tests](https://github.com/G-Node/python-odml/workflows/run-tests/badge.svg?branch=master)](https://github.com/G-Node/python-odml/actions)
@@ -94,15 +93,15 @@
 
 For details regarding the introduced changes please check the [github
 release notes](https://github.com/G-Node/python-odml/releases).
 
 
 # Dependencies
 
-* Python 3.6+
+* Python 3.7+
 * Python packages:
 
   * lxml (version 3.7.2)
   * yaml (version >= 5.1)
   * rdflib (version >=4.2.2)
 
 * These packages will be downloaded and installed automatically if the ```pip```
@@ -118,15 +117,17 @@
 
   * libxml2-dev
   * libxslt1-dev
   * lib32z1-dev
 
 ## Previous Python versions
 
-Python 2 has reached end of life. We will not keep any future versions of odml Python 2 compatible and will completely drop support for Python 2 with August 2020. We also recommend using a Python version >= 3.6. If a Python version < 3.6 is a requirement, the following dependency needs to be installed as well:
+Python 2 has reached end of life. Current and future versions of odml are not Python 2 compatible. We removed support 
+for Python 2 in August 2020 with version 1.5.2. We also recommend using a Python version >= 3.7. If a 
+Python version < 3.7 is a requirement, the following dependency needs to be installed as well:
 
 * pip install
   * enum34 (version 0.4.4)
 * apt install
   * python-enum
 
 # Building from source
@@ -162,9 +163,7 @@
 # Bugs & Questions
 
 Should you find a behaviour that is likely a bug, please file a bug report at
 [the github bug tracker](https://github.com/G-Node/python-odml/issues).
 
 If you have questions regarding the use of the library, feel free to join the
 [#gnode](http://webchat.freenode.net?channels=%23gnode) IRC channel on freenode.
-
-
```

### Comparing `odML-1.5.2/odML.egg-info/SOURCES.txt` & `odML-1.5.3/odML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/__init__.py` & `odML-1.5.3/odml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # Monkey patch formatting 'warnings' messages for the whole module.
 warnings.formatwarning = _format_warning
 
 if _python_version.major < 3:
     msg = "Python 2 has reached end of live."
     msg += "\n\todML support for Python 2 has been dropped."
     warnings.warn(msg, category=DeprecationWarning, stacklevel=2)
-elif _python_version.major == 3 and _python_version.minor < 6:
+elif _python_version.major == 3 and _python_version.minor < 7:
     msg = "The '%s' package is not tested with your Python version. " % __name__
     msg += "\n\tPlease consider upgrading to the latest Python distribution."
     warnings.warn(msg)
 
 __version__ = VERSION
```

### Comparing `odML-1.5.2/odml/base.py` & `odML-1.5.3/odml/base.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/doc.py` & `odML-1.5.3/odml/doc.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/dtypes.py` & `odML-1.5.3/odml/dtypes.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/fileio.py` & `odML-1.5.3/odml/fileio.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/format.py` & `odML-1.5.3/odml/format.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/info.json` & `odML-1.5.3/odml/info.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8428571428571429%*

 * *Differences: {"'CLASSIFIERS'": "{insert: [(5, 'Programming Language :: Python :: 3.10')], delete: [2]}",*

 * * "'COPYRIGHT'": "'(c) 2011-2023, German Neuroinformatics Node'",*

 * * "'VERSION'": "'1.5.3'"}*

```diff
@@ -1,19 +1,19 @@
 {
     "AUTHOR": "Hagen Fritsch, Jan Grewe, Christian Kellner, Achilleas Koutsou, Michael Sonntag, Lyuba Zehl",
     "CLASSIFIERS": [
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License"
     ],
     "CONTACT": "dev@g-node.org",
-    "COPYRIGHT": "(c) 2011-2021, German Neuroinformatics Node",
+    "COPYRIGHT": "(c) 2011-2023, German Neuroinformatics Node",
     "FORMAT_VERSION": "1.1",
     "HOMEPAGE": "https://github.com/G-Node/python-odml",
-    "VERSION": "1.5.2"
+    "VERSION": "1.5.3"
 }
```

### Comparing `odML-1.5.2/odml/property.py` & `odML-1.5.3/odml/property.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/rdf/fuzzy_finder.py` & `odML-1.5.3/odml/rdf/fuzzy_finder.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/rdf/query_creator.py` & `odML-1.5.3/odml/rdf/query_creator.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/resources/odml-ontology.ttl` & `odML-1.5.3/odml/resources/odml-ontology.ttl`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/resources/section_subclasses.yaml` & `odML-1.5.3/odml/resources/section_subclasses.yaml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/scripts/odml_convert.py` & `odML-1.5.3/odml/scripts/odml_convert.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/scripts/odml_to_rdf.py` & `odML-1.5.3/odml/scripts/odml_to_rdf.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/scripts/odml_view.py` & `odML-1.5.3/odml/scripts/odml_view.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/section.py` & `odML-1.5.3/odml/section.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/templates.py` & `odML-1.5.3/odml/templates.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/terminology.py` & `odML-1.5.3/odml/terminology.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/tools/converters/format_converter.py` & `odML-1.5.3/odml/tools/converters/format_converter.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/tools/converters/version_converter.py` & `odML-1.5.3/odml/tools/converters/version_converter.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/tools/dict_parser.py` & `odML-1.5.3/odml/tools/dict_parser.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/tools/doc_inherit.py` & `odML-1.5.3/odml/tools/doc_inherit.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/tools/dumper.py` & `odML-1.5.3/odml/tools/dumper.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/tools/odmlparser.py` & `odML-1.5.3/odml/tools/odmlparser.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/tools/parser_utils.py` & `odML-1.5.3/odml/tools/parser_utils.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/tools/rdf_converter.py` & `odML-1.5.3/odml/tools/rdf_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,30 +5,45 @@
 
 import os
 import string
 import uuid
 import warnings
 
 from io import StringIO
+
+from rdflib import __version__ as rdflib_version
 from rdflib import Graph, Literal, URIRef
 from rdflib.graph import Seq
+try:
+    from rdflib.container import Seq as CollSeq
+except ImportError as exc:
+    # annoy people to upgrade their rdflib version but still support the usage
+    print("deprecated rdflib version. Please upgrade to the latest version.")
 from rdflib.namespace import XSD, RDF, RDFS
 
 import yaml
 
 import odml
 
 from ..format import Format, Document, Section, Property
 from ..info import FORMAT_VERSION, INSTALL_PATH
 from .dict_parser import DictReader
 from .parser_utils import ParserException, RDF_CONVERSION_FORMATS
 
 ODML_NS = Format.namespace()
 
 
+def rdflib_version_major():
+    version_split = rdflib_version.split(".")
+    if len(version_split) < 3 or not version_split[0].isdigit():
+        print("Could not parse rdflib version %s" % rdflib_version)
+        return 0
+    return int(version_split[0])
+
+
 def load_rdf_subclasses():
     """
     load_rdf_subclasses loads odml section types to RDF Section subclass types
     mappings from a file and returns the mapping as a dictionary.
     Will return an empty dictionary, if the Subclasses file cannot be loaded.
 
     :return: Dictionary of the form {'Section type': 'RDF class type'}
@@ -129,24 +144,31 @@
         self.graph.add((parent_node, rdf_predicate, seq))
 
         # rdflib so far does not respect RDF:li item order in RDF:Seq on
         # loading so we have to use custom numbered Node elements for now.
         # Once rdflib upgrades this should be reversed to RDF:li again!
         # see https://github.com/RDFLib/rdflib/issues/280
         # -- keep until supported
-        # bag = URIRef(ODML_NS + str(uuid.uuid4()))
-        # self.graph.add((bag, RDF.type, RDF.Bag))
-        # self.graph.add((curr_node, fmt.rdf_map(k), bag))
-        # for curr_val in values:
-        #     self.graph.add((bag, RDF.li, Literal(curr_val)))
-        counter = 1
-        for curr_val in values:
-            custom_predicate = "%s_%s" % (str(RDF), counter)
-            self.graph.add((seq, URIRef(custom_predicate), Literal(curr_val)))
-            counter = counter + 1
+        #bag = URIRef(ODML_NS + str(uuid.uuid4()))
+        #self.graph.add((bag, RDF.type, RDF.Bag))
+        #self.graph.add((parent_node, rdf_predicate, bag))
+        #for curr_val in values:
+        #    self.graph.add((bag, RDF.li, Literal(curr_val)))
+        if rdflib_version_major() >= 6:
+            seq_list = []
+            for curr_val in values:
+                seq_list.append(Literal(curr_val))
+            _ = CollSeq(self.graph, seq, seq_list)
+        else:
+            # manually create and use the value blank nodes order
+            counter = 1
+            for curr_val in values:
+                custom_predicate = "%s_%s" % (str(RDF), counter)
+                self.graph.add((seq, URIRef(custom_predicate), Literal(curr_val)))
+                counter = counter + 1
 
     def save_odml_list(self, parent_node, rdf_predicate, odml_list):
         """
         save_odml_list adds all odml elements in a list to the current
         parent node and handles all child items via save_element.
 
         :param parent_node: current parent node in the RDF graph.
@@ -345,17 +367,21 @@
             if k in self.section_subclasses:
                 msg = "RDFWriter custom subclasses: Key '%s' already exists. " % k
                 msg += "Value '%s' replaces default value '%s'." % (val, self.section_subclasses[k])
                 warnings.warn(msg, stacklevel=2)
             self.section_subclasses[k] = val
 
     def __str__(self):
+        if rdflib_version_major() >= 6:
+            return self.convert_to_rdf().serialize(format='turtle')
         return self.convert_to_rdf().serialize(format='turtle').decode("utf-8")
 
     def __unicode__(self):
+        if rdflib_version_major() >= 6:
+            return self.convert_to_rdf().serialize(format='turtle')
         return self.convert_to_rdf().serialize(format='turtle').decode("utf-8")
 
     def get_rdf_str(self, rdf_format="turtle"):
         """
         Convert the current odML content of the parser to a common RDF graph
         and return the graph as a string object in the specified RDF format.
 
@@ -366,14 +392,16 @@
         :return: string object
         """
         if rdf_format not in RDF_CONVERSION_FORMATS:
             msg = "odml.RDFWriter.get_rdf_str: Format for output files is incorrect."
             msg = "%s Please choose from the list: %s" % (msg, list(RDF_CONVERSION_FORMATS))
             raise ValueError(msg)
 
+        if rdflib_version_major() >= 6:
+            return self.convert_to_rdf().serialize(format=rdf_format)
         return self.convert_to_rdf().serialize(format=rdf_format).decode("utf-8")
 
     def write_file(self, filename, rdf_format="turtle"):
         """
         Convert the current odML content of the parser to a common RDF graph
         and write the resulting graph to an output file using the provided
         RDF output format.
@@ -512,26 +540,34 @@
         """
         prop_attrs = {}
         for attr in Property.rdf_map_items:
             elems = list(self.graph.objects(subject=prop_uri, predicate=attr[1]))
             if attr[0] == "value" and elems:
                 prop_attrs[attr[0]] = []
 
-                # rdflib does not respect order with RDF.li items yet, see comment above
-                # support both RDF.li and rdf:_nnn for now.
-                # Remove rdf:_nnn once rdflib respects RDF.li order in an RDF.Seq obj.
-                values = list(self.graph.objects(subject=elems[0], predicate=RDF.li))
-                if values:
-                    for curr_val in values:
-                        prop_attrs[attr[0]].append(curr_val.toPython())
-                else:
-                    # rdf:__nnn part
+                if rdflib_version_major() >= 6:
+                    # rdflib version 6.x.x+ should support rdf:_nnn only, RDF.li
+                    # are not supported; reverse import the blank node values;
+                    # hopefully in the correct order.
                     val_seq = Seq(graph=self.graph, subject=elems[0])
                     for seq_item in val_seq:
                         prop_attrs[attr[0]].append(seq_item.toPython())
+                else:
+                    # rdflib does not respect order with RDF.li items yet, see comment above
+                    # support both RDF.li and rdf:_nnn for now.
+                    # Remove rdf:_nnn once rdflib respects RDF.li order in an RDF.Seq obj.
+                    values = list(self.graph.objects(subject=elems[0], predicate=RDF.li))
+                    if values:
+                        for curr_val in values:
+                            prop_attrs[attr[0]].append(curr_val.toPython())
+                    else:
+                        # rdf:__nnn part
+                        val_seq = Seq(graph=self.graph, subject=elems[0])
+                        for seq_item in val_seq:
+                            prop_attrs[attr[0]].append(seq_item.toPython())
 
             elif attr[0] == "id":
                 prop_attrs[attr[0]] = prop_uri.split("#", 1)[1]
             elif elems:
                 prop_attrs[attr[0]] = str(elems[0].toPython())
 
         self._check_mandatory_attrs(prop_attrs)
```

### Comparing `odML-1.5.2/odml/tools/xmlparser.py` & `odML-1.5.3/odml/tools/xmlparser.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/util.py` & `odML-1.5.3/odml/util.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/odml/validation.py` & `odML-1.5.3/odml/validation.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/setup.py` & `odML-1.5.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,21 +27,26 @@
     'odml.tools',
     'odml.tools.converters'
 ]
 
 with open('README.md') as f:
     description_text = f.read()
 
-# pyparsing needs to be pinned to 2.4.7 for the time being. setup install fetches a pre-release
-# package that currently results in issues with the rdflib library.
-install_req = ["lxml", "pyyaml>=5.1", "rdflib==5.0.0", "docopt", "pathlib", "pyparsing==2.4.7"]
-
-# owlrl depends on rdflib - the pinned version should be removed once the version pin has also been
-# removed from rdflib. Also needs to be updated in requirements-test.txt
-tests_req = ["pytest", "owlrl==5.2.3", "requests"]
+install_req = ["docopt", "lxml", "pathlib", "pyyaml>=5.1", "rdflib>=6.0.0"]
+# owlrl depends on rdflib; update any changes in requirements-test.txt as well.
+tests_req = ["owlrl", "pytest", "requests"]
+
+# Keep support for for Python versions below 3.7; relevant for the
+# rdflib usage; rdflib >= 6 does not support Python versions below 3.7.
+if _python_version.minor <= 6:
+    # pyparsing needs to be pinned to 2.4.7 due to issues with the rdflib 5.0.0 library.
+    install_req = ["docopt", "lxml", "pathlib", "pyyaml>=5.1", "rdflib==5.0.0", "pyparsing==2.4.7"]
+
+    # owlrl depends on rdflib and needs to be pinned to a corresponding version.
+    tests_req = ["owlrl==5.2.3", "pytest", "requests"]
 
 setup(
     name='odML',
     version=VERSION,
     description='open metadata Markup Language',
     author=AUTHOR,
     author_email=CONTACT,
@@ -62,11 +67,11 @@
 )
 
 # Make this the last thing people read after a setup.py install
 if _python_version.major < 3:
     msg = "Python 2 has reached end of live."
     msg += "\n\todML support for Python 2 has been dropped."
     print(msg)
-elif _python_version.major == 3 and _python_version.minor < 6:
+elif _python_version.major == 3 and _python_version.minor < 7:
     msg = "\n\nThis package is not tested with your Python version. "
     msg += "\n\tPlease consider upgrading to the latest Python distribution."
     print(msg)
```

### Comparing `odML-1.5.2/test/resources/example.odml` & `odML-1.5.3/test/resources/example.odml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/ignore_errors.xml` & `odML-1.5.3/test/resources/ignore_errors.xml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/scripts/odml_convert/conversion_example_A.xml` & `odML-1.5.3/test/resources/scripts/odml_convert/conversion_example_A.xml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/scripts/odml_convert/conversion_example_B.xml` & `odML-1.5.3/test/resources/scripts/odml_convert/conversion_example_B.xml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/scripts/odml_convert/test_recursive/conversion_example_sub_root.xml` & `odML-1.5.3/test/resources/scripts/odml_convert/test_recursive/conversion_example_sub_root.xml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/scripts/odml_convert/test_recursive/sub/conversion_example_sub_sub.xml` & `odML-1.5.3/test/resources/scripts/odml_convert/test_recursive/sub/conversion_example_sub_sub.xml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/scripts/odml_to_rdf/example_A.doi.xml` & `odML-1.5.3/test/resources/scripts/odml_to_rdf/example_A.doi.xml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/scripts/odml_to_rdf/example_B.doi.xml` & `odML-1.5.3/test/resources/scripts/odml_to_rdf/example_B.doi.xml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/scripts/odml_to_rdf/test_recursive/example_sub_root.doi.xml` & `odML-1.5.3/test/resources/scripts/odml_to_rdf/test_recursive/example_sub_root.doi.xml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/scripts/odml_to_rdf/test_recursive/sub/example_sub.doi.xml` & `odML-1.5.3/test/resources/scripts/odml_to_rdf/test_recursive/sub/example_sub.doi.xml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/validation_dtypes.json` & `odML-1.5.3/test/resources/validation_dtypes.json`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/validation_dtypes.xml` & `odML-1.5.3/test/resources/validation_dtypes.xml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/validation_dtypes.yaml` & `odML-1.5.3/test/resources/validation_dtypes.yaml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/validation_section.json` & `odML-1.5.3/test/resources/validation_section.json`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/version_conversion.json` & `odML-1.5.3/test/resources/version_conversion.json`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/version_conversion.xml` & `odML-1.5.3/test/resources/version_conversion.xml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/version_conversion_int.json` & `odML-1.5.3/test/resources/version_conversion_int.json`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/version_conversion_int.xml` & `odML-1.5.3/test/resources/version_conversion_int.xml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/resources/version_conversion_int.yaml` & `odML-1.5.3/test/resources/version_conversion_int.yaml`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_doc.py` & `odML-1.5.3/test/test_doc.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_doc_integration.py` & `odML-1.5.3/test/test_doc_integration.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_dtypes.py` & `odML-1.5.3/test/test_dtypes.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_dtypes_integration.py` & `odML-1.5.3/test/test_dtypes_integration.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_dumper.py` & `odML-1.5.3/test/test_dumper.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_fileio.py` & `odML-1.5.3/test/test_fileio.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_find_section.py` & `odML-1.5.3/test/test_find_section.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_format_converter.py` & `odML-1.5.3/test/test_format_converter.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_infer_type.py` & `odML-1.5.3/test/test_infer_type.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_iterators.py` & `odML-1.5.3/test/test_iterators.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_links.py` & `odML-1.5.3/test/test_links.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_parser_json.py` & `odML-1.5.3/test/test_parser_json.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_parser_odml.py` & `odML-1.5.3/test/test_parser_odml.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_parser_xml.py` & `odML-1.5.3/test/test_parser_xml.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_parser_yaml.py` & `odML-1.5.3/test/test_parser_yaml.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_property.py` & `odML-1.5.3/test/test_property.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_property_integration.py` & `odML-1.5.3/test/test_property_integration.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_rdf_reader.py` & `odML-1.5.3/test/test_rdf_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import unittest
 
 from rdflib import Literal
 
 from odml import Property, Section, Document
 from odml.format import Format
-from odml.tools.rdf_converter import RDFWriter, RDFReader
+from odml.tools.rdf_converter import RDFWriter, RDFReader, rdflib_version_major
 from odml.tools.parser_utils import ParserException
 
 ODMLNS = Format.namespace()
 
 
 class TestRDFReader(unittest.TestCase):
 
@@ -111,25 +111,33 @@
         Test if ParserError is thrown if mandatory attributes are missing for section.
         """
         rdf_writer = RDFWriter([self.doc])
         rdf_writer.convert_to_rdf()
         for rdf_sec in rdf_writer.graph.subjects(predicate=ODMLNS.hasName, object=Literal("sec1")):
             rdf_writer.graph.remove((rdf_sec, ODMLNS.hasName, Literal("sec1")))
 
-        new_graph = rdf_writer.graph.serialize(format="turtle").decode("utf-8")
+        # support both >=6.0.0 and <6.0.0 versions of rdflib for the time being
+        if rdflib_version_major() < 6:
+            new_graph = rdf_writer.graph.serialize(format="turtle").decode("utf-8")
+        else:
+            new_graph = rdf_writer.graph.serialize(format="turtle")
 
         with self.assertRaises(ParserException):
             RDFReader().from_string(new_graph, "turtle")
 
     def test_mandatory_attrs_property(self):
         """
         Test if ParserError is thrown if mandatory attributes are missing for section.
         """
         rdf_writer = RDFWriter([self.doc])
         rdf_writer.convert_to_rdf()
         for rdf_sec in rdf_writer.graph.subjects(predicate=ODMLNS.hasName, object=Literal("prop1")):
             rdf_writer.graph.remove((rdf_sec, ODMLNS.hasName, Literal("prop1")))
 
-        new_graph = rdf_writer.graph.serialize(format="turtle").decode("utf-8")
+        # support both >=6.0.0 and <6.0.0 versions of rdflib for the time being
+        if rdflib_version_major() < 6:
+            new_graph = rdf_writer.graph.serialize(format="turtle").decode("utf-8")
+        else:
+            new_graph = rdf_writer.graph.serialize(format="turtle")
 
         with self.assertRaises(ParserException):
             RDFReader().from_string(new_graph, "turtle")
```

### Comparing `odML-1.5.2/test/test_rdf_writer.py` & `odML-1.5.3/test/test_rdf_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,48 +124,33 @@
         doc = parse("""
             s1[t1]
             """)
 
         rdf_writer = RDFWriter([doc])
         rdf_writer.convert_to_rdf()
 
-        check = rdf_writer.graph.subject_objects(predicate=RDF.li)
-        self.assertEqual(len(list(check)), 0)
-
         check = rdf_writer.graph.subject_objects(predicate=URIRef("%s_1" % str(RDF)))
         self.assertEqual(len(list(check)), 0)
 
         doc = parse("""
             s1[t1]
             - p1
             """)
 
         rdf_writer = RDFWriter([doc])
         rdf_writer.convert_to_rdf()
 
-        check = rdf_writer.graph.subjects(predicate=RDF.li, object=Literal("val"))
-        self.assertEqual(len(list(check)), 0)
-
         check = rdf_writer.graph.subjects(predicate=URIRef("%s_1" % str(RDF)),
                                           object=Literal("val"))
         self.assertEqual(len(list(check)), 1)
 
         doc.sections[0].properties[0].append("val2")
         rdf_writer = RDFWriter([doc])
         rdf_writer.convert_to_rdf()
 
-        check = rdf_writer.graph.subject_objects(predicate=RDF.li)
-        self.assertEqual(len(list(check)), 0)
-
-        check = rdf_writer.graph.subjects(predicate=RDF.li, object=Literal("val"))
-        self.assertEqual(len(list(check)), 0)
-
-        check = rdf_writer.graph.subjects(predicate=RDF.li, object=Literal("val2"))
-        self.assertEqual(len(list(check)), 0)
-
         check = rdf_writer.graph.subjects(predicate=URIRef("%s_1" % str(RDF)),
                                           object=Literal("val"))
         self.assertEqual(len(list(check)), 1)
 
         check = rdf_writer.graph.subjects(predicate=URIRef("%s_2" % str(RDF)),
                                           object=Literal("val2"))
         self.assertEqual(len(list(check)), 1)
@@ -177,17 +162,14 @@
              - p1
              - p2
              """)
 
         rdf_writer = RDFWriter([doc])
         rdf_writer.convert_to_rdf()
 
-        check = rdf_writer.graph.subjects(predicate=RDF.li, object=Literal("val"))
-        self.assertEqual(len(list(check)), 0)
-
         check = rdf_writer.graph.subjects(predicate=URIRef("%s_1" % str(RDF)),
                                           object=Literal("val"))
         self.assertEqual(len(list(check)), 3)
 
     def test_section_subclass(self):
         file_path = os.path.join(odml.__path__[0], 'resources', 'section_subclasses.yaml')
         with open(file_path, "r") as subclass_file:
```

### Comparing `odML-1.5.2/test/test_samplefile.py` & `odML-1.5.3/test/test_samplefile.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_script_odml_convert.py` & `odML-1.5.3/test/test_script_odml_convert.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_script_odml_to_rdf.py` & `odML-1.5.3/test/test_script_odml_to_rdf.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_section.py` & `odML-1.5.3/test/test_section.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_section_integration.py` & `odML-1.5.3/test/test_section_integration.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_terminology.py` & `odML-1.5.3/test/test_terminology.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_util.py` & `odML-1.5.3/test/test_util.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_validation.py` & `odML-1.5.3/test/test_validation.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_validation_integration.py` & `odML-1.5.3/test/test_validation_integration.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_version_converter.py` & `odML-1.5.3/test/test_version_converter.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_version_converter_integration.py` & `odML-1.5.3/test/test_version_converter_integration.py`

 * *Files identical despite different names*

### Comparing `odML-1.5.2/test/test_xml_writer.py` & `odML-1.5.3/test/test_xml_writer.py`

 * *Files identical despite different names*

