# Comparing `tmp/nomenclature-iamc-0.8.tar.gz` & `tmp/nomenclature-iamc-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenclature-iamc-0.8.tar", last modified: Mon Jan  9 12:23:03 2023, max compression
+gzip compressed data, was "nomenclature-iamc-0.9.tar", last modified: Tue May  2 15:29:26 2023, max compression
```

## Comparing `nomenclature-iamc-0.8.tar` & `nomenclature-iamc-0.9.tar`

### file list

```diff
@@ -1,316 +1,322 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.410635 nomenclature-iamc-0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.422635 nomenclature-iamc-0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/.github/workflows/nightly.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/.stickler.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/DEVELOPING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.422635 nomenclature-iamc-0.8/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.422635 nomenclature-iamc-0.8/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.422635 nomenclature-iamc-0.8/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/_static/EU-logo-300x201.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)   172467 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/_static/iamc-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/_static/open_entrance-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.422635 nomenclature-iamc-0.8/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/_templates/navigation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.422635 nomenclature-iamc-0.8/doc/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/api/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/api/datastructuredefinition.rst
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/api/nomenclature.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/api/regionprocessor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.422635 nomenclature-iamc-0.8/doc/source/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/user_guide/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/user_guide/directory-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/user_guide/local-usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/user_guide/model-mapping.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/user_guide/model-registration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/user_guide/region.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/user_guide/variable.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/doc/source/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.426636 nomenclature-iamc-0.8/nomenclature/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/code.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.426636 nomenclature-iamc-0.8/nomenclature/error/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/error/codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/error/region.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/error/required_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/error/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.426636 nomenclature-iamc-0.8/nomenclature/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22216 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/processor/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/processor/required_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/processor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.426636 nomenclature-iamc-0.8/nomenclature/validation_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/validation_schemas/generic_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/validation_schemas/region_mapping_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/validation_schemas/region_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/validation_schemas/tag_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/nomenclature/validation_schemas/variable_schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.426636 nomenclature-iamc-0.8/nomenclature_iamc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-01-09 12:23:03.000000 nomenclature-iamc-0.8/nomenclature_iamc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-01-09 12:23:03.000000 nomenclature-iamc-0.8/nomenclature_iamc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 12:23:03.000000 nomenclature-iamc-0.8/nomenclature_iamc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-09 12:23:03.000000 nomenclature-iamc-0.8/nomenclature_iamc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-09 12:23:03.000000 nomenclature-iamc-0.8/nomenclature_iamc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-09 12:23:03.000000 nomenclature-iamc-0.8/nomenclature_iamc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/alias_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.410635 nomenclature-iamc-0.8/tests/data/check_aggregate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.410635 nomenclature-iamc-0.8/tests/data/check_aggregate/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/check_aggregate/components/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/check_aggregate/components/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/check_aggregate/components/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/check_aggregate/components/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.410635 nomenclature-iamc-0.8/tests/data/check_aggregate/components_dict/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/check_aggregate/components_dict/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/check_aggregate/components_dict/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/check_aggregate/components_dict/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/check_aggregate/components_dict/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.410635 nomenclature-iamc-0.8/tests/data/custom_dimension_nc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/custom_dimension_nc/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/custom_dimension_nc/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/custom_dimension_nc/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/custom_dimension_nc/scenario/scenarios.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/custom_dimension_nc/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/custom_dimension_nc/variable/tag_fuel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/custom_dimension_nc/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/duplicate_code_raises/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/duplicate_code_raises/bar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/duplicate_code_raises/foo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/duplicate_tag_raises/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/duplicate_tag_raises/tag_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/duplicate_tag_raises/tag_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.410635 nomenclature-iamc-0.8/tests/data/empty_definitions_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/empty_definitions_dir/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/empty_definitions_dir/definitions/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.410635 nomenclature-iamc-0.8/tests/data/end_whitespace/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.410635 nomenclature-iamc-0.8/tests/data/end_whitespace/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/end_whitespace/definitions/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/end_whitespace/definitions/scenario/scenarios.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/extras_nc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/extras_nc/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/extras_nc/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/extras_nc/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/extras_nc/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/failing_variable_codelist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/failing_variable_codelist/rename_arg_conflict/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/failing_variable_codelist/rename_arg_conflict/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/failing_variable_codelist/rename_arg_conflict/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/failing_variable_codelist/rename_undefined_target/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/failing_variable_codelist/rename_undefined_target/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/failing_variable_codelist/rename_undefined_target/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/failing_variable_codelist/unknown_weight/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/failing_variable_codelist/unknown_weight/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/failing_variable_codelist/unknown_weight/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/hidden_character/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/hidden_character/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/hidden_character/definitions/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/hidden_character/definitions/scenario/scenarios.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/invalid_yaml/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/invalid_yaml/foo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/multiple_unit_codelist/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/multiple_unit_codelist/variable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/non-default_dimensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/non-default_dimensions/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.430636 nomenclature-iamc-0.8/tests/data/non-default_dimensions/definitions/region/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_dimensions/definitions/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/non-default_dimensions/definitions/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_dimensions/definitions/scenario/scenarios.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/non-default_dimensions/definitions/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_dimensions/definitions/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/non-default_dimensions/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_dimensions/mappings/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_dimensions/mappings/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/non-default_dimensions_one_empty/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/non-default_dimensions_one_empty/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/non-default_dimensions_one_empty/definitions/empty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_dimensions_one_empty/definitions/empty/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/non-default_dimensions_one_empty/definitions/region/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_dimensions_one_empty/definitions/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/non-default_dimensions_one_empty/definitions/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_dimensions_one_empty/definitions/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/non-default_dimensions_one_empty/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_dimensions_one_empty/mappings/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_dimensions_one_empty/mappings/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/non-default_folders/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/non-default_folders/def/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/non-default_folders/def/region/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_folders/def/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/non-default_folders/def/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_folders/def/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/non-default_folders/map/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_folders/map/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/non-default_folders/map/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/norway_as_bool/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/norway_as_bool/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/region_aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_aggregation/illegal_mapping_conflict_regions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_aggregation/illegal_mapping_duplicate_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_aggregation/illegal_mapping_illegal_attribute.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_aggregation/illegal_mapping_invalid_format_dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_aggregation/illegal_mapping_model_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_aggregation/illegal_mapping_native_duplicate_key.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_aggregation/illegal_mapping_native_rename_key_conflict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_aggregation/illegal_mapping_native_rename_target_conflict_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_aggregation/illegal_mapping_native_rename_target_conflict_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_aggregation/working_mapping.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/region_codelist/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_codelist/region.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/region_processing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/region_processing/aggregate_only/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/aggregate_only/aggregate_only.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/region_processing/complete_processing/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/complete_processing/model_a.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/region_processing/complete_processing_list/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/complete_processing_list/model_a.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/region_processing/dsd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/region_processing/dsd/region/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/dsd/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/region_processing/dsd/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/dsd/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/region_processing/empty_aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/empty_aggregation/model_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/empty_aggregation/model_b.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.434636 nomenclature-iamc-0.8/tests/data/region_processing/no_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/no_mapping/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/region_processing/partial_aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/partial_aggregation/model_a.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/region_processing/rename_only/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/rename_only/model_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/rename_only/model_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/rename_only/model_c.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/region_processing/skip_aggregation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/region_processing/skip_aggregation/dsd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/region_processing/skip_aggregation/dsd/region/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/skip_aggregation/dsd/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/region_processing/skip_aggregation/dsd/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/skip_aggregation/dsd/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/region_processing/skip_aggregation/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/skip_aggregation/mappings/model_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/skip_aggregation/mappings/model_b.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.414635 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation/aggregate/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation/aggregate/aggregate_only.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation/dsd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation/dsd/region/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation/dsd/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation/dsd/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation/dsd/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation_rename/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation_rename/aggregate/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-09 12:22:52.000000 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation_rename/aggregate/aggregate_only.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation_rename/dsd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation_rename/dsd/region/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation_rename/dsd/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation_rename/dsd/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/region_processing/weighted_aggregation_rename/dsd/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/regionprocessor_duplicate/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/regionprocessor_duplicate/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/regionprocessor_duplicate/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/regionprocessor_exclude_region_overlap/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/regionprocessor_exclude_region_overlap/exclude_common_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/regionprocessor_exclude_region_overlap/exclude_native_overlap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/regionprocessor_not_defined/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/regionprocessor_not_defined/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/regionprocessor_not_defined/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/regionprocessor_unexpected_region/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/regionprocessor_unexpected_region/model_a.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/regionprocessor_working/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/regionprocessor_working/mapping_1.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/regionprocessor_working/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/required_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/required_data/definition/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/required_data/definition/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/required_data/definition/region/region.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/required_data/definition/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/required_data/definition/variable/variable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/required_data/required_data/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/required_data/required_data/requiredData.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/required_data/required_data/requiredData_apply_error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/required_data/required_data/requiredData_apply_working.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/required_data/required_data/requiredData_unknown_region.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/required_data/required_data/requiredData_unknown_unit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/required_data/required_data/requiredData_unknown_variable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.438636 nomenclature-iamc-0.8/tests/data/simple_codelist/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/simple_codelist/foo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/stray_tag/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/stray_tag/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/tests/data/stray_tag/definitions/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/stray_tag/definitions/variable/tag_fuel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/stray_tag/definitions/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/structure_validation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/structure_validation/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/tests/data/structure_validation/definitions/region/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/structure_validation/definitions/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/tests/data/structure_validation/definitions/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/structure_validation/definitions/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/tests/data/structure_validation/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/structure_validation/mappings/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/structure_validation/mappings/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/structure_validation_fails/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/structure_validation_fails/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/tests/data/structure_validation_fails/definitions/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/structure_validation_fails/definitions/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/tests/data/structure_validation_fails/definitions/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/structure_validation_fails/definitions/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/tests/data/structure_validation_fails/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/structure_validation_fails/mappings/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/structure_validation_fails/mappings/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/structure_validation_no_mappings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/structure_validation_no_mappings/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/tests/data/structure_validation_no_mappings/definitions/region/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/structure_validation_no_mappings/definitions/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/tests/data/structure_validation_no_mappings/definitions/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/structure_validation_no_mappings/definitions/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/tests/data/tagged_codelist/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/tagged_codelist/foo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/tagged_codelist/tag_sector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/tagged_codelist/tag_source.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.418635 nomenclature-iamc-0.8/tests/data/validation_nc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/tests/data/validation_nc/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/validation_nc/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:23:03.442636 nomenclature-iamc-0.8/tests/data/validation_nc/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/validation_nc/variable/tag_fuel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/validation_nc/variable/variables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/validation_nc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/validation_nc_duplicates.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/data/validation_nc_flat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/test_check_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/test_codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15491 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/test_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/test_definition_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/test_region_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/test_required_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-01-09 12:22:53.000000 nomenclature-iamc-0.8/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.464473 nomenclature-iamc-0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.476473 nomenclature-iamc-0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/.github/workflows/nightly.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/.stickler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/DEVELOPING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-02 15:29:26.500474 nomenclature-iamc-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.476473 nomenclature-iamc-0.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.476473 nomenclature-iamc-0.9/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.476473 nomenclature-iamc-0.9/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/_static/EU-logo-300x201.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)   172467 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/_static/iamc-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/_static/open_entrance-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.476473 nomenclature-iamc-0.9/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/_templates/navigation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.476473 nomenclature-iamc-0.9/doc/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/api/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/api/datastructuredefinition.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/api/nomenclature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/api/regionprocessor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.480473 nomenclature-iamc-0.9/doc/source/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/directory-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/local-usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/model-mapping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/model-registration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/region.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/variable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.480473 nomenclature-iamc-0.9/nomenclature/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.480473 nomenclature-iamc-0.9/nomenclature/error/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/error/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/error/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/error/required_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/error/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.480473 nomenclature-iamc-0.9/nomenclature/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/processor/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/processor/required_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/processor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.480473 nomenclature-iamc-0.9/nomenclature/validation_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/validation_schemas/generic_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/validation_schemas/region_mapping_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/validation_schemas/region_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/validation_schemas/tag_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/validation_schemas/variable_schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-02 15:29:26.000000 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-02 15:29:26.000000 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:29:26.000000 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 15:29:26.000000 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-02 15:29:26.000000 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 15:29:26.000000 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-02 15:29:26.500474 nomenclature-iamc-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.464473 nomenclature-iamc-0.9/tests/data/check_aggregate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.464473 nomenclature-iamc-0.9/tests/data/check_aggregate/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/check_aggregate/components/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/check_aggregate/components/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/check_aggregate/components/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/check_aggregate/components/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.464473 nomenclature-iamc-0.9/tests/data/check_aggregate/components_dict/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/check_aggregate/components_dict/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/check_aggregate/components_dict/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/check_aggregate/components_dict/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/check_aggregate/components_dict/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.464473 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/scenario/scenarios.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/variable/tag_fuel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/duplicate_code_raises/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/duplicate_code_raises/bar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/duplicate_code_raises/foo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/duplicate_tag_raises/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/duplicate_tag_raises/tag_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/duplicate_tag_raises/tag_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.464473 nomenclature-iamc-0.9/tests/data/empty_definitions_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/empty_definitions_dir/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/empty_definitions_dir/definitions/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/end_whitespace/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/end_whitespace/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/end_whitespace/definitions/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/end_whitespace/definitions/scenario/scenarios.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/extras_nc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/extras_nc/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/extras_nc/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/extras_nc/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/extras_nc/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/rename_arg_conflict/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/rename_arg_conflict/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/rename_arg_conflict/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/rename_undefined_target/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/rename_undefined_target/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/rename_undefined_target/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/unknown_weight/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/unknown_weight/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/unknown_weight/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/general_filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/general_filtering/basic_codelist.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/hidden_character/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/hidden_character/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/hidden_character/definitions/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/hidden_character/definitions/scenario/scenarios.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/invalid_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/invalid_yaml/foo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/multiple_unit_codelist/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/multiple_unit_codelist/variable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/non-default_dimensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/scenario/scenarios.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions/mappings/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions/mappings/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/empty/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/mappings/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/mappings/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/non-default_folders/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/non-default_folders/def/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_folders/def/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_folders/def/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_folders/def/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_folders/def/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_folders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_folders/map/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_folders/map/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/norway_as_bool/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/norway_as_bool/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_conflict_regions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_duplicate_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_illegal_attribute.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_invalid_format_dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_model_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_native_duplicate_key.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_native_rename_key_conflict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_native_rename_target_conflict_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_native_rename_target_conflict_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/working_mapping.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_codelist/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_codelist/region.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/aggregate_only/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/aggregate_only/aggregate_only.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/complete_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/complete_processing/model_a.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/complete_processing_list/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/complete_processing_list/model_a.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/region_processing/dsd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/dsd/region/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/dsd/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/dsd/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/dsd/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/empty_aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/empty_aggregation/model_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/empty_aggregation/model_b.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/no_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/no_mapping/.keep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/partial_aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/partial_aggregation/model_a.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/rename_only/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/rename_only/model_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/rename_only/model_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/rename_only/model_c.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/dsd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/dsd/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/dsd/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/dsd/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/dsd/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/mappings/model_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/mappings/model_b.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/aggregate/aggregate_only.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/dsd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/dsd/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/dsd/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/dsd/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/dsd/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/aggregate/aggregate_only.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/dsd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/dsd/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/dsd/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/dsd/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/dsd/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_to_filter_codelist/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_to_filter_codelist/region_filtering.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/regionprocessor_duplicate/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_duplicate/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_duplicate/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/regionprocessor_exclude_region_overlap/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_exclude_region_overlap/exclude_common_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_exclude_region_overlap/exclude_native_overlap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/regionprocessor_not_defined/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_not_defined/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_not_defined/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/regionprocessor_unexpected_region/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_unexpected_region/model_a.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/regionprocessor_working/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_working/mapping_1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_working/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/required_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/required_data/definition/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/required_data/definition/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/definition/region/region.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/required_data/definition/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/definition/variable/variable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/required_data/required_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/required_data/requiredData.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/required_data/requiredData_apply_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/required_data/requiredData_apply_working.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/required_data/requiredData_unknown_region.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/required_data/requiredData_unknown_unit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/required_data/requiredData_unknown_variable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/simple_codelist/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/simple_codelist/foo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/stray_tag/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/stray_tag/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/stray_tag/definitions/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/stray_tag/definitions/variable/tag_fuel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/stray_tag/definitions/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/structure_validation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/structure_validation/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation/definitions/region/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation/definitions/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation/definitions/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation/definitions/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation/mappings/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation/mappings/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/structure_validation_fails/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/structure_validation_fails/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation_fails/definitions/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation_fails/definitions/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation_fails/definitions/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation_fails/definitions/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation_fails/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation_fails/mappings/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation_fails/mappings/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/structure_validation_no_mappings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/structure_validation_no_mappings/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation_no_mappings/definitions/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation_no_mappings/definitions/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation_no_mappings/definitions/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation_no_mappings/definitions/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/tagged_codelist/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/tagged_codelist/foo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/tagged_codelist/tag_sector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/tagged_codelist/tag_source.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/validation_nc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/validation_nc/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/validation_nc/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc/variable/tag_fuel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc/variable/variables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc_duplicates.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc_flat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc_list_arg.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/variable_codelist_complex_attr/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/variable_codelist_complex_attr/variable_complex_attr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_check_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_definition_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_region_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_required_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_validation.py
```

### Comparing `nomenclature-iamc-0.8/.github/workflows/build-docs.yml` & `nomenclature-iamc-0.9/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/.github/workflows/nightly.yaml` & `nomenclature-iamc-0.9/.github/workflows/nightly.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/.github/workflows/publish.yaml` & `nomenclature-iamc-0.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/.github/workflows/pytest.yml` & `nomenclature-iamc-0.9/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/.gitignore` & `nomenclature-iamc-0.9/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 .cache
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
+# include xlsx files needed for testing
+!tests/data/*.xlsx
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `nomenclature-iamc-0.8/CITATION.cff` & `nomenclature-iamc-0.9/CITATION.cff`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/DEVELOPING.rst` & `nomenclature-iamc-0.9/DEVELOPING.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/LICENSE` & `nomenclature-iamc-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/PKG-INFO` & `nomenclature-iamc-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenclature-iamc
-Version: 0.8
+Version: 0.9
 Summary: Package for managing codelists & attributes for IAMC-format datasets
 Home-page: https://github.com/IAMconsortium/nomenclature
 Author: Scenario Services team, ECE program, IIASA
 Author-email: ece-scse@iiasa.ac.at
 License: APACHE-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nomenclature-iamc-0.8/README.md` & `nomenclature-iamc-0.9/README.md`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/Makefile` & `nomenclature-iamc-0.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/make.bat` & `nomenclature-iamc-0.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/_static/EU-logo-300x201.jpg` & `nomenclature-iamc-0.9/doc/source/_static/EU-logo-300x201.jpg`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/_static/iamc-logo.png` & `nomenclature-iamc-0.9/doc/source/_static/iamc-logo.png`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/_static/open_entrance-logo.png` & `nomenclature-iamc-0.9/doc/source/_static/open_entrance-logo.png`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/_templates/navigation.html` & `nomenclature-iamc-0.9/doc/source/_templates/navigation.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-<!-- this is a hard override because alabaster does not have an option
-     to set the tocdepth in the navigation sidebar,
-     see https://github.com/bitprophet/alabaster/issues/89 -->
-
-<h3>{{ _('Navigation') }}</h3>
-{{ toctree(maxdepth=4, includehidden=theme_sidebar_includehidden, collapse=theme_sidebar_collapse) }}
-{% if theme_extra_nav_links %}
-<hr />
-<ul>
-    {% for text, uri in theme_extra_nav_links.items() %}
-    <li class="toctree-l1"><a href="{{ uri }}">{{ text }}</a></li>
-    {% endfor %}
-</ul>
-{% endif %}
+<!-- this is a hard override because alabaster does not have an option
+     to set the tocdepth in the navigation sidebar,
+     see https://github.com/bitprophet/alabaster/issues/89 -->
+
+<h3>{{ _('Navigation') }}</h3>
+{{ toctree(maxdepth=2, includehidden=theme_sidebar_includehidden, collapse=theme_sidebar_collapse) }}
+{% if theme_extra_nav_links %}
+<hr />
+<ul>
+    {% for text, uri in theme_extra_nav_links.items() %}
+    <li class="toctree-l1"><a href="{{ uri }}">{{ text }}</a></li>
+    {% endfor %}
+</ul>
+{% endif %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 **** {{ _('Navigation') }} ****
-{{ toctree(maxdepth=4, includehidden=theme_sidebar_includehidden,
+{{ toctree(maxdepth=2, includehidden=theme_sidebar_includehidden,
 collapse=theme_sidebar_collapse) }} {% if theme_extra_nav_links %}
 ===============================================================================
     * {% for text, uri in theme_extra_nav_links.items() %}
     * {{_text_}}
     * {% endfor %}
 {% endif %}
```

### Comparing `nomenclature-iamc-0.8/doc/source/cli.rst` & `nomenclature-iamc-0.9/doc/source/cli.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/conf.py` & `nomenclature-iamc-0.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/index.rst` & `nomenclature-iamc-0.9/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/installation.rst` & `nomenclature-iamc-0.9/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/user_guide/codelist.rst` & `nomenclature-iamc-0.9/doc/source/user_guide/codelist.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/user_guide/directory-structure.rst` & `nomenclature-iamc-0.9/doc/source/user_guide/directory-structure.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/user_guide/local-usage.rst` & `nomenclature-iamc-0.9/doc/source/user_guide/local-usage.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/user_guide/model-mapping.rst` & `nomenclature-iamc-0.9/doc/source/user_guide/model-mapping.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/user_guide/model-registration.rst` & `nomenclature-iamc-0.9/doc/source/user_guide/model-registration.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/user_guide/variable.rst` & `nomenclature-iamc-0.9/doc/source/user_guide/variable.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/doc/source/user_guide.rst` & `nomenclature-iamc-0.9/doc/source/user_guide.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature/__init__.py` & `nomenclature-iamc-0.9/nomenclature/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature/cli.py` & `nomenclature-iamc-0.9/nomenclature/cli.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature/code.py` & `nomenclature-iamc-0.9/nomenclature/code.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import re
 from keyword import iskeyword
 from typing import Any, Dict, List, Optional, Set, Union
 
 from pydantic import BaseModel, Field, validator
 
 
@@ -67,18 +68,29 @@
     @property
     def tags(self):
         return re.findall("(?<={).*?(?=})", self.name)
 
     @property
     def flattened_dict(self):
         return {
-            **{k: v for k, v in self.dict().items() if k != "extra_attributes"},
+            **{
+                k: v
+                for k, v in self.dict(by_alias=True).items()
+                if k != "extra_attributes"
+            },
             **self.extra_attributes,
         }
 
+    @property
+    def flattened_dict_serialized(self):
+        return {
+            key: (json.dumps(value) if isinstance(value, (list, dict)) else value)
+            for key, value in self.flattened_dict.items()
+        }
+
     def replace_tag(self, tag: str, target: "Code") -> "Code":
         """Return a new instance with tag applied
 
         Parameters
         ----------
         tag : str
             Name of the tag
@@ -120,36 +132,80 @@
         if name not in self.__class__.named_attributes():
             self.extra_attributes[name] = value
         else:
             super().__setattr__(name, value)
 
 
 class VariableCode(Code):
-
     unit: Optional[Union[str, List[str]]] = Field(...)
     weight: Optional[str] = None
     region_aggregation: Optional[List[Dict[str, Dict]]] = Field(
         None, alias="region-aggregation"
     )
     skip_region_aggregation: Optional[bool] = Field(
         False, alias="skip-region-aggregation"
     )
     method: Optional[str] = None
     check_aggregate: Optional[bool] = Field(False, alias="check-aggregate")
     components: Optional[Union[List[str], List[Dict[str, List[str]]]]] = None
+    drop_negative_weights: Optional[bool] = None
 
     class Config:
         # this allows using both "check_aggregate" and "check-aggregate" for attribute
         # setting
         allow_population_by_field_name = True
 
+    @validator("region_aggregation", "components", "unit", pre=True)
+    def deserialize_json(cls, v):
+        try:
+            return json.loads(v) if isinstance(v, str) else v
+        except json.decoder.JSONDecodeError:
+            return v
+
     @property
     def units(self) -> List[Union[str, None]]:
         return self.unit if isinstance(self.unit, list) else [self.unit]
 
     @classmethod
     def named_attributes(cls) -> Set[str]:
         return (
             super()
             .named_attributes()
             .union(f.alias for f in cls.__dict__["__fields__"].values())
         )
+
+    @property
+    def pyam_agg_kwargs(self) -> Dict[str, Any]:
+        # return a dict of all not None pyam aggregation properties
+        return {
+            field: getattr(self, field)
+            for field in (
+                "weight",
+                "method",
+                "components",
+                "drop_negative_weights",
+            )
+            if getattr(self, field) is not None
+        }
+
+    @property
+    def agg_kwargs(self) -> Dict[str, Any]:
+        return (
+            {**self.pyam_agg_kwargs, **{"region_aggregation": self.region_aggregation}}
+            if self.region_aggregation is not None
+            else self.pyam_agg_kwargs
+        )
+
+
+class RegionCode(Code):
+    """A subclass of Code specified for regions
+
+    Attributes
+    ----------
+    name : str
+        Name of the RegionCode
+    hierarchy : str
+        Hierarchy of the RegionCode
+
+    """
+
+    hierarchy: str = None
```

### Comparing `nomenclature-iamc-0.8/nomenclature/codelist.py` & `nomenclature-iamc-0.9/nomenclature/codelist.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 from pathlib import Path
 from typing import ClassVar, Dict, List
 
 import pandas as pd
+import numpy as np
 import yaml
+import logging
 from jsonschema import validate
 from pyam.utils import write_sheet
 from pydantic import BaseModel, validator
 
-from nomenclature.code import Code, VariableCode
+from nomenclature.code import Code, VariableCode, RegionCode
 from nomenclature.error.codelist import DuplicateCodeError
 from nomenclature.error.variable import (
     MissingWeightError,
     VariableRenameArgError,
     VariableRenameTargetError,
 )
 
-# arguments of the method `pyam.IamDataFrame.aggregate_region`
-# required for checking validity of variable-CodeList-attributes
-PYAM_AGG_KWARGS = [
-    "components",
-    "method",
-    "weight",
-    "drop_negative_weights",
-]
 
 here = Path(__file__).parent.absolute()
 
 
 def read_validation_schema(i):
     with open(here / "validation_schemas" / f"{i}_schema.yaml", "r") as f:
         schema = yaml.safe_load(f)
@@ -114,15 +108,14 @@
         """
         return [c for c in items if c not in self.keys()]
 
     @classmethod
     def replace_tags(
         cls, code_list: List[Code], tag_name: str, tags: List[Code]
     ) -> List[Code]:
-
         _code_list: List[Code] = []
 
         for code in code_list:
             if "{" + tag_name + "}" in code.name:
                 _code_list.extend((code.replace_tag(tag_name, tag) for tag in tags))
             else:
                 _code_list.append(code)
@@ -239,27 +232,30 @@
         sheet_name : str
             Sheet name of `source`.
         col : str
             Column from `sheet_name` to use as codes.
         attrs : list, optional
             Columns from `sheet_name` to use as attributes.
         """
-        source = pd.read_excel(source, sheet_name=sheet_name)
+        codelist = pd.read_excel(source, sheet_name=sheet_name, usecols=[col] + attrs)
+
+        # replace nan with None
+        codelist = codelist.replace(np.nan, None)
 
         # check for duplicates in the codelist
-        duplicate_rows = source[col].duplicated(keep=False).values
+        duplicate_rows = codelist[col].duplicated(keep=False).values
         if any(duplicate_rows):
-            duplicates = source[duplicate_rows]
+            duplicates = codelist[duplicate_rows]
             # set index to equal the row numbers to simplify identifying the issue
             duplicates.index = pd.Index([i + 2 for i in duplicates.index])
             msg = f"Duplicate values in the codelist:\n{duplicates.head(20)}"
             raise ValueError(msg + ("\n..." if len(duplicates) > 20 else ""))
 
         # set `col` as index and cast all attribute-names to lowercase
-        codes = source[[col] + attrs].set_index(col)[attrs]
+        codes = codelist[[col] + attrs].set_index(col)[attrs]
         codes.rename(columns={c: str(c).lower() for c in codes.columns}, inplace=True)
         codes_di = codes.to_dict(orient="index")
         mapp = {
             title: cls.code_basis.from_dict({title: values})
             for title, values in codes_di.items()
         }
 
@@ -270,19 +266,24 @@
 
         Parameters
         ----------
         path : :class:`pathlib.Path` or str, optional
             Write to file path if not None, otherwise return as stream
         """
 
+        class Dumper(yaml.Dumper):
+            def increase_indent(self, flow=False, *args, **kwargs):
+                return super().increase_indent(flow=flow, indentless=False)
+
         # translate to list of nested dicts, replace None by empty field, write to file
         stream = (
             yaml.dump(
                 [{code: attrs} for code, attrs in self.codelist_repr().items()],
                 sort_keys=False,
+                Dumper=Dumper,
             )
             .replace(": null\n", ":\n")
             .replace(": nan\n", ":\n")
         )
 
         if path is not None:
             with open(path, "w") as file:
@@ -295,15 +296,17 @@
 
         Parameters
         ----------
         sort_by_code : bool, optional
             Sort the codelist before exporting to csv.
         """
         codelist = (
-            pd.DataFrame.from_dict(self.codelist_repr(), orient="index")
+            pd.DataFrame.from_dict(
+                self.codelist_repr(json_serialized=True), orient="index"
+            )
             .reset_index()
             .rename(columns={"index": self.name})
             .drop(columns="file")
         )
         if sort_by_code:
             codelist.sort_values(by=self.name, inplace=True)
         codelist.rename(
@@ -362,29 +365,68 @@
 
         write_sheet(excel_writer, sheet_name, self.to_pandas(sort_by_code))
 
         # close the file if `excel_writer` arg was a file name
         if close:
             excel_writer.close()
 
-    def codelist_repr(self) -> Dict:
+    def codelist_repr(self, json_serialized=False) -> Dict:
         """Cast a CodeList into corresponding dictionary"""
 
         nice_dict = {}
         for name, code in self.mapping.items():
+            code_dict = (
+                code.flattened_dict_serialized
+                if json_serialized
+                else code.flattened_dict
+            )
             code_dict = {
                 k: v
-                for k, v in code.flattened_dict.items()
+                for k, v in code_dict.items()
                 if (v is not None and k != "name") or k == "unit"
             }
 
             nice_dict[name] = code_dict
 
         return nice_dict
 
+    def filter(self, **kwargs) -> "CodeList":
+        """Filter a CodeList by any attribute-value pairs.
+
+        Parameters
+        ----------
+        **kwargs
+            Attribute-value mappings to be used for filtering.
+
+        Returns
+        -------
+        CodeList
+            CodeList with Codes that match attribute-value pairs.
+        """
+
+        # Returns True if code satisfies all filter parameters
+        def _match_attribute(code, kwargs):
+            return all(
+                hasattr(code, attribute) and getattr(code, attribute, None) == value
+                for attribute, value in kwargs.items()
+            )
+
+        filtered_codelist = CodeList(
+            name=self.name,
+            mapping={
+                code.name: code
+                for code in self.mapping.values()
+                if _match_attribute(code, kwargs)
+            },
+        )
+
+        if not filtered_codelist.mapping:
+            logging.warning("Formatted data is empty!")
+        return filtered_codelist
+
 
 class VariableCodeList(CodeList):
     """A subclass of CodeList specified for variables
 
     Attributes
     ----------
     name : str
@@ -397,87 +439,99 @@
     # class variables
     code_basis: ClassVar = VariableCode
     validation_schema: ClassVar[str] = "variable"
 
     @validator("mapping")
     def check_variable_region_aggregation_args(cls, v):
         """Check that any variable "region-aggregation" mappings are valid"""
-        items = [
-            (name, code)
-            for (name, code) in v.items()
-            if code.region_aggregation is not None
-        ]
 
-        for (name, code) in items:
-            # ensure that there no pyam-aggregation-kwargs and
-            conflict_args = [
-                i
-                for i, val in code.dict().items()
-                if i in PYAM_AGG_KWARGS and val is not None
-            ]
-            if conflict_args:
-                raise VariableRenameArgError(
-                    variable=name,
-                    file=code.file,
-                    args=conflict_args,
-                )
-
-            # ensure that mapped variables are defined in the nomenclature
-            invalid = []
-            for inst in code.region_aggregation:
-                invalid.extend(var for var in inst if var not in v)
-            if invalid:
-                raise VariableRenameTargetError(
-                    variable=name, file=code.file, target=invalid
-                )
+        for var in v.values():
+            # ensure that a variable does not have both individual
+            # pyam-aggregation-kwargs and a 'region-aggregation' attribute
+            if var.region_aggregation is not None:
+                if conflict_args := list(var.pyam_agg_kwargs.keys()):
+                    raise VariableRenameArgError(
+                        variable=var.name,
+                        file=var.file,
+                        args=conflict_args,
+                    )
+
+                # ensure that mapped variables are defined in the nomenclature
+                invalid = []
+                for inst in var.region_aggregation:
+                    invalid.extend(var for var in inst if var not in v)
+                if invalid:
+                    raise VariableRenameTargetError(
+                        variable=var.name, file=var.file, target=invalid
+                    )
         return v
 
     @validator("mapping")
     def check_weight_in_vars(cls, v):
-        # Check that all variables specified in 'weight' are present in the codelist
+        """Check that all variables specified in 'weight' are present in the codelist"""
         if missing_weights := [
-            (name, code.weight, code.file)
-            for name, code in v.items()
-            if code.weight is not None and code.weight not in v
+            (var.name, var.weight, var.file)
+            for var in v.values()
+            if var.weight is not None and var.weight not in v
         ]:
             raise MissingWeightError(
                 missing_weights="".join(
                     f"'{weight}' used for '{var}' in: {file}\n"
                     for var, weight, file in missing_weights
                 )
             )
         return v
 
     @validator("mapping")
     def cast_variable_components_args(cls, v):
         """Cast "components" list of dicts to a codelist"""
+
         # translate a list of single-key dictionaries to a simple dictionary
-        for name, code in v.items():
-            if code.components and isinstance(code.components[0], dict):
+        for var in v.values():
+            if var.components and isinstance(var.components[0], dict):
                 comp = {}
-                for val in code.components:
+                for val in var.components:
                     comp.update(val)
-                v[name].components = comp
+                v[var.name].components = comp
 
         return v
 
+    def vars_default_args(self, variables: List[str]) -> List[VariableCode]:
+        """return subset of variables which does not feature any special pyam
+        aggregation arguments and where skip_region_aggregation is False"""
+        return [
+            self[var]
+            for var in variables
+            if not self[var].agg_kwargs and not self[var].skip_region_aggregation
+        ]
+
+    def vars_kwargs(self, variables: List[str]) -> List[VariableCode]:
+        # return subset of variables which features special pyam aggregation arguments
+        # and where skip_region_aggregation is False
+        return [
+            self[var]
+            for var in variables
+            if self[var].agg_kwargs and not self[var].skip_region_aggregation
+        ]
+
 
 class RegionCodeList(CodeList):
     """A subclass of CodeList specified for regions
 
     Attributes
     ----------
     name : str
         Name of the RegionCodeList
     mapping : dict
-        Dictionary of `Code` objects
+        Dictionary of `RegionCode` objects
 
     """
 
     # class variable
+    code_basis: ClassVar = RegionCode
     validation_schema: ClassVar[str] = "region"
 
     @classmethod
     def from_directory(cls, name: str, path: Path, file_glob_pattern: str = "**/*"):
         """Initialize a RegionCodeList from a directory with codelist files
 
         Parameters
@@ -491,35 +545,82 @@
             files in all sub-folders)
 
         Returns
         -------
         RegionCodeList
 
         """
-        code_list: List[Code] = []
+        mapping: Dict[str, RegionCode] = {}
+        code_list: List[RegionCode] = []
 
         for yaml_file in (
             f
             for f in path.glob(file_glob_pattern)
             if f.suffix in {".yaml", ".yml"} and not f.name.startswith("tag_")
         ):
             with open(yaml_file, "r", encoding="utf-8") as stream:
                 _code_list = yaml.safe_load(stream)
 
-            # a "region" codelist assumes a top-level key to be used as attribute
+            # a "region" codelist assumes a top-level category to be used as attribute
             for top_level_cat in _code_list:
                 for top_key, _codes in top_level_cat.items():
                     for item in _codes:
-                        code = Code.from_dict(item)
+                        code = RegionCode.from_dict(item)
                         code.hierarchy = top_key
                         code.file = yaml_file.relative_to(path.parent).as_posix()
                         code_list.append(code)
 
         code_list = cls._parse_and_replace_tags(code_list, path, file_glob_pattern)
 
-        mapping: Dict[str, Code] = {}
+        mapping: Dict[str, RegionCode] = {}
         for code in code_list:
             if code.name in mapping:
                 raise DuplicateCodeError(name=name, code=code.name)
             mapping[code.name] = code
 
         return cls(name=name, mapping=mapping)
+
+    @property
+    def hierarchy(self) -> List[str]:
+        """Return the hierarchies defined in the RegionCodeList
+
+        Returns
+        -------
+        List[str]
+
+        """
+        return sorted(list(set(v.hierarchy for v in self.mapping.values())))
+
+    def filter(self, hierarchy: str) -> "RegionCodeList":
+        """Return a filtered RegionCodeList object
+
+        Parameters
+        ----------
+        hierarchy : str
+            String with filter parameter.
+
+        Raises
+        ------
+        ValueError
+            Provided hierarchy is not compatible with the given model.
+
+        Returns
+        -------
+        :class:'RegionCodeList'
+
+        Notes
+        -----
+        The following arguments are available for filtering:
+
+        - 'hierarchy': filter by the hierarchy of each region
+
+        """
+
+        mapping = {k: v for k, v in self.mapping.items() if v.hierarchy == hierarchy}
+        if mapping:
+            return RegionCodeList(name=self.name, mapping=mapping)
+        else:
+            msg: str = (
+                f"Filtered RegionCodeList is empty: hierarchy={hierarchy}\n"
+                "Use `RegionCodeList.hierarchy` method for available items."
+            )
+            raise ValueError(msg)
```

### Comparing `nomenclature-iamc-0.8/nomenclature/core.py` & `nomenclature-iamc-0.9/nomenclature/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,19 @@
     # perform validation and region-processing (optional)
     if processor is None:
         dsd.validate(df, dimensions=dimensions)
     else:
         if "region" in dimensions:
             dimensions.remove("region")
             dsd.validate(df, dimensions=dimensions)
-            df = processor.apply(df, dsd)
+            df = processor.apply(df)
             dsd.validate(df, dimensions=["region"])
         else:
             dsd.validate(df, dimensions=dimensions)
-            df = processor.apply(df, dsd)
+            df = processor.apply(df)
 
     # check consistency across the variable hierarchy
     error = dsd.check_aggregate(df)
     if error is not None:
         logger.error(f"These variables are not the sum of their components:\n{error}")
         raise ValueError("The validation failed. Please check the log for details.")
```

### Comparing `nomenclature-iamc-0.8/nomenclature/definition.py` & `nomenclature-iamc-0.9/nomenclature/definition.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature/error/region.py` & `nomenclature-iamc-0.9/nomenclature/error/region.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature/error/variable.py` & `nomenclature-iamc-0.9/nomenclature/error/variable.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature/processor/region.py` & `nomenclature-iamc-0.9/nomenclature/processor/region.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import logging
 from collections import Counter
 from pathlib import Path
-from typing import Dict, List, Optional, Set, Union
+from typing import Dict, List, Optional, Union
 
 import jsonschema
+import numpy as np
+import pandas as pd
 import pyam
 import pydantic
 import yaml
 from pyam import IamDataFrame
 from pyam.logging import adjust_log_level
 from pydantic import BaseModel, root_validator, validate_arguments, validator
 from pydantic.error_wrappers import ErrorWrapper
 from pydantic.types import DirectoryPath, FilePath
 
-from nomenclature.codelist import PYAM_AGG_KWARGS
+from nomenclature.codelist import RegionCodeList, VariableCodeList
 from nomenclature.definition import DataStructureDefinition
 from nomenclature.error.region import (
     ExcludeRegionOverlapError,
     ModelMappingCollisionError,
     RegionNameCollisionError,
     RegionNotDefinedError,
 )
 from nomenclature.processor.utils import get_relative_path
 
-AGG_KWARGS = PYAM_AGG_KWARGS + ["region_aggregation"]
-
 logger = logging.getLogger(__name__)
 
 here = Path(__file__).parent.absolute()
 
 
 class NativeRegion(BaseModel):
     """Define a model native region.
@@ -283,36 +283,59 @@
         # List of the common region names
         return [x.name for x in self.common_regions or []]
 
     @property
     def rename_mapping(self) -> Dict[str, str]:
         return {r.name: r.target_native_region for r in self.native_regions or []}
 
-    def validate_regions(self, dsd: DataStructureDefinition) -> None:
-        if hasattr(dsd, "region"):
-            # invalid = [c for c in self.all_regions if c not in dsd.region]
-            invalid = dsd.region.validate_items(self.all_regions)
-            if invalid:
-                raise RegionNotDefinedError(region=invalid, file=self.file)
+    def validate_regions(self, region_codelist: RegionCodeList) -> None:
+        if invalid := region_codelist.validate_items(self.all_regions):
+            raise RegionNotDefinedError(region=invalid, file=self.file)
+
+    def check_unexpected_regions(self, df: IamDataFrame) -> None:
+        # Raise error if a region in the input data is not used in the model mapping
+
+        if regions_not_found := set(df.region) - set(
+            self.model_native_region_names
+            + self.common_region_names
+            + [
+                const_reg
+                for comm_reg in self.common_regions or []
+                for const_reg in comm_reg.constituent_regions
+            ]
+            + (self.exclude_regions or [])
+        ):
+            raise ValueError(
+                f"Did not find region(s) {regions_not_found} in 'native_regions', "
+                "'common_regions' or 'exclude_regions' in model mapping for "
+                f"{self.model} in {self.file}. If they are not meant to be included "
+                "in the results add to the 'exclude_regions' section in the model "
+                "mapping to silence this error."
+            )
 
 
 class RegionProcessor(BaseModel):
     """Region aggregation mappings for scenario processing"""
 
+    region_codelist: RegionCodeList
+    variable_codelist: VariableCodeList
     mappings: Dict[str, RegionAggregationMapping]
 
     @classmethod
-    @validate_arguments
-    def from_directory(cls, path: DirectoryPath):
+    @validate_arguments(config={"arbitrary_types_allowed": True})
+    def from_directory(cls, path: DirectoryPath, dsd: DataStructureDefinition):
         """Initialize a RegionProcessor from a directory of model-aggregation mappings.
 
         Parameters
         ----------
         path : DirectoryPath
             Directory which holds all the mappings.
+        dsd : DataStructureDefinition
+            Instance of DataStructureDefinition used for validation of mappings and
+            region aggregation.
 
         Returns
         -------
         RegionProcessor
             The resulting region processor object.
 
         Raises
@@ -340,170 +363,181 @@
                             )
                         )
             except (pydantic.ValidationError, jsonschema.ValidationError) as e:
                 errors.append(ErrorWrapper(e, "__root__"))
 
         if errors:
             raise pydantic.ValidationError(errors, model=RegionProcessor)
-        return cls(mappings=mapping_dict)
 
-    def validate_with_definition(self, dsd: DataStructureDefinition) -> None:
+        if missing_dims := [
+            dim for dim in ("region", "variable") if not hasattr(dsd, dim)
+        ]:
+            raise AttributeError(
+                "Provided DataStructureDefinition is missing the following attributes "
+                f"{missing_dims}"
+            )
+        return cls(
+            mappings=mapping_dict,
+            region_codelist=dsd.region,
+            variable_codelist=dsd.variable,
+        )
+
+    @validator("mappings", each_item=True)
+    def validate_with_definition(cls, v, values):
         """Check if all mappings are valid and collect all errors."""
-        errors = []
-        for mapping in self.mappings.values():
-            try:
-                mapping.validate_regions(dsd)
-            except RegionNotDefinedError as rnde:
-                errors.append(ErrorWrapper(rnde, f"mappings -> {mapping.model}"))
-        if errors:
-            raise pydantic.ValidationError(errors, model=self.__class__)
+        v.validate_regions(values["region_codelist"])
+        return v
 
-    def apply(self, df: IamDataFrame, dsd: DataStructureDefinition) -> IamDataFrame:
+    def apply(self, df: IamDataFrame) -> IamDataFrame:
         """Apply region processing
 
         Parameters
         ----------
         df : IamDataFrame
             Input data that the region processing is applied to
-        dsd : DataStructureDefinition
-            Used for region validation and variable information for performing region
-            processing
 
         Returns
         -------
         IamDataFrame
             Processed data
 
         Raises
         ------
         ValueError
             * If *df* contains regions that are not listed in the model mapping, or
             * If the region-processing results in an empty **IamDataFrame**.
         """
         processed_dfs: List[IamDataFrame] = []
         for model in df.model:
+
             model_df = df.filter(model=model)
 
-            # If no mapping is defined the data frame is returned unchanged
+            # if no mapping is defined the data frame is returned unchanged
             if model not in self.mappings:
-                logger.info(f"No model mapping found for model {model}")
+                logger.info(f"No model mapping found for model '{model}'")
                 processed_dfs.append(model_df)
 
-            # Otherwise we first rename, then aggregate
+            # otherwise we first rename, then aggregate
             else:
-                # before aggregating, check that all regions are valid
-                self.mappings[model].validate_regions(dsd)
+                file = self.mappings[model].file
                 logger.info(
-                    f"Applying region-processing for model {model} from file "
-                    f"{self.mappings[model].file}"
+                    f"Applying region-processing for model '{model}' from '{file}'"
+                )
+                processed_dfs.append(self._apply_region_processing(model_df))
+
+        return pyam.concat(processed_dfs)
+
+    def _apply_region_processing(self, model_df: IamDataFrame) -> IamDataFrame:
+        """Apply the region processing for a single model"""
+        if len(model_df.model) != 1:
+            raise ValueError(
+                f"Must be called for a unique model, found: {model_df.model}"
+            )
+        model = model_df.model[0]
+
+        # before aggregating, check that all regions are valid
+        self.mappings[model].validate_regions(self.region_codelist)
+
+        # check for regions not mentioned in the model mapping
+        self.mappings[model].check_unexpected_regions(model_df)
+
+        _processed_data: List[pd.Series] = []
+
+        # silence pyam's empty filter warnings
+        with adjust_log_level(logger="pyam", level="ERROR"):
+            # rename native regions
+            if self.mappings[model].native_regions is not None:
+                _df = model_df.filter(
+                    region=self.mappings[model].model_native_region_names
                 )
-                # Check for regions not mentioned in the model mapping
-                _check_unexpected_regions(model_df, self.mappings[model])
-                _processed_dfs = []
-
-                # Silence pyam's empty filter warnings
-                with adjust_log_level(logger="pyam", level="ERROR"):
-                    # Rename
-                    if self.mappings[model].native_regions is not None:
-                        _df = model_df.filter(
-                            region=self.mappings[model].model_native_region_names
+                if not _df.empty:
+                    _processed_data.append(
+                        _df.rename(region=self.mappings[model].rename_mapping)._data
+                    )
+
+            # aggregate common regions
+            if self.mappings[model].common_regions is not None:
+
+                for cr in self.mappings[model].common_regions:
+                    # if a common region is consists of a single native region, rename
+                    if cr.is_single_constituent_region:
+                        _df = model_df.filter(region=cr.constituent_regions[0]).rename(
+                            region=cr.rename_dict
                         )
                         if not _df.empty:
-                            _processed_dfs.append(
-                                _df.rename(region=self.mappings[model].rename_mapping)
-                            )
+                            _processed_data.append(_df._data)
+                        continue
+
+                    # if there are multiple constituent regions, aggregate
+                    regions = [cr.name, cr.constituent_regions]
+
+                    # first, perform 'simple' aggregation (no arguments)
+                    simple_vars = [
+                        var.name
+                        for var in self.variable_codelist.vars_default_args(
+                            model_df.variable
+                        )
+                    ]
+                    _df = model_df.aggregate_region(
+                        simple_vars,
+                        *regions,
+                    )
+                    if _df is not None and not _df.empty:
+                        _processed_data.append(_df._data)
 
-                    # Aggregate
-                    if self.mappings[model].common_regions is not None:
-                        vars = self._filter_dict_args(model_df.variable, dsd)
-                        vars_default_args = [
-                            var for var, kwargs in vars.items() if not kwargs
-                        ]
-                        # TODO skip if required weight does not exist
-                        vars_kwargs = {
-                            var: kwargs
-                            for var, kwargs in vars.items()
-                            if var not in vars_default_args
-                        }
-                        for cr in self.mappings[model].common_regions:
-                            # If the common region is only comprised of a single model
-                            # native region, just rename
-                            if cr.is_single_constituent_region:
-                                _processed_dfs.append(
-                                    model_df.filter(
-                                        region=cr.constituent_regions[0]
-                                    ).rename(region=cr.rename_dict)
-                                )
-                                continue
-                            # if there are multiple constituent regions, aggregate
-                            regions = [cr.name, cr.constituent_regions]
-                            # First, perform 'simple' aggregation (no arguments)
-                            _processed_dfs.append(
-                                model_df.aggregate_region(vars_default_args, *regions)
+                    # second, special weighted aggregation
+                    for var in self.variable_codelist.vars_kwargs(model_df.variable):
+                        if var.region_aggregation is None:
+                            _df = _aggregate_region(
+                                model_df,
+                                var.name,
+                                *regions,
+                                **var.pyam_agg_kwargs,
                             )
-                            # Second, special weighted aggregation
-                            for var, kwargs in vars_kwargs.items():
-                                if "region_aggregation" not in kwargs:
+                            if _df is not None and not _df.empty:
+                                _processed_data.append(_df._data)
+                        else:
+                            for rename_var in var.region_aggregation:
+                                for _rename, _kwargs in rename_var.items():
                                     _df = _aggregate_region(
                                         model_df,
-                                        var,
+                                        var.name,
                                         *regions,
-                                        **kwargs,
+                                        **_kwargs,
                                     )
                                     if _df is not None and not _df.empty:
-                                        _processed_dfs.append(_df)
-                                else:
-                                    for rename_var in kwargs["region_aggregation"]:
-                                        for _rename, _kwargs in rename_var.items():
-                                            _df = _aggregate_region(
-                                                model_df,
-                                                var,
-                                                *regions,
-                                                **_kwargs,
-                                            )
-                                            if _df is not None and not _df.empty:
-                                                _processed_dfs.append(
-                                                    _df.rename(variable={var: _rename})
-                                                )
-
-                    common_region_df = model_df.filter(
-                        region=self.mappings[model].common_region_names,
-                        variable=dsd.variable,
-                    )
-
-                    # concatenate and merge with data provided at common-region level
-                    if _processed_dfs:
-                        processed_dfs.append(
-                            _merge_with_provided_data(_processed_dfs, common_region_df)
-                        )
-                    # if data exists only at the common-region level
-                    elif not common_region_df.empty:
-                        processed_dfs.append(common_region_df)
-
-        # raise an error if processed_dfs has no entries or all are empty
-        if not processed_dfs or all(df.empty for df in processed_dfs):
-            raise ValueError(
-                f"The region-processing for model(s) {df.model} returned an empty "
-                "dataset"
+                                        _processed_data.append(
+                                            _df.rename(
+                                                variable={var.name: _rename}
+                                            )._data
+                                        )
+
+            common_region_df = model_df.filter(
+                region=self.mappings[model].common_region_names,
+                variable=self.variable_codelist,
             )
 
-        return pyam.concat(processed_dfs)
+            # concatenate and merge with data provided at common-region level
+            if _processed_data:
+                _data = pd.concat(_processed_data)
+                if not common_region_df.empty:
+                    _data = _compare_and_merge(common_region_df._data, _data)
+
+            # if data exists only at the common-region level
+            elif not common_region_df.empty:
+                _data = common_region_df._data
 
-    def _filter_dict_args(
-        self, variables, dsd: DataStructureDefinition, keys: Set[str] = AGG_KWARGS
-    ) -> Dict[str, Dict]:
-        return {
-            name: {
-                key: value
-                for key, value in code.dict().items()
-                if key in keys and value is not None
-            }
-            for name, code in dsd.variable.items()
-            if name in variables and not code.skip_region_aggregation
-        }
+            # raise an error if region-processing yields an empty result
+            else:
+                raise ValueError(
+                    f"Region-processing for model '{model}' returned an empty dataset"
+                )
+
+        # cast processed timeseries data and meta indicators to IamDataFrame
+        return IamDataFrame(_data, meta=model_df.meta)
 
 
 def _aggregate_region(df, var, *regions, **kwargs):
     """Perform region aggregation with kwargs catching inconsistent-index errors"""
     try:
         return df.aggregate_region(var, *regions, **kwargs)
     except ValueError as e:
@@ -511,66 +545,41 @@
             logger.info(
                 f"Could not aggregate '{var}' for region '{regions[0]}' ({kwargs})"
             )
         else:
             raise e
 
 
-def _merge_with_provided_data(
-    _processed_df: IamDataFrame, common_region_df: IamDataFrame
-) -> IamDataFrame:
-    """Compare and merge provided and aggregated results"""
-
-    # validate that aggregated data matches to original data
-    aggregate_df = pyam.concat(_processed_df)
-    compare = pyam.compare(
-        common_region_df,
-        aggregate_df,
-        left_label="common-region",
-        right_label="aggregation",
+def _compare_and_merge(original: pd.Series, aggregated: pd.Series) -> IamDataFrame:
+    """Compare and merge original and aggregated results"""
+
+    # compare processed (aggregated) data and data provided at the common-region level
+    compare = pd.merge(
+        left=original.rename(index="original"),
+        right=aggregated.rename(index="aggregated"),
+        how="outer",
+        left_index=True,
+        right_index=True,
     )
-    # drop all data which is not in both data frames
-    diff = compare.dropna()
 
-    if diff is not None and len(diff):
-        logging.warning("Difference between original and aggregated data:\n" f"{diff}")
+    # drop rows that are not in conflict
+    compare = compare.dropna()
+    compare = compare[~np.isclose(compare["original"], compare["aggregated"])]
+
+    if compare is not None and len(compare):
+        logging.warning(f"Difference between original and aggregated data:\n{compare}")
 
     # merge aggregated data onto original common-region data
-    index = aggregate_df._data.index.difference(common_region_df._data.index)
-    return common_region_df.append(aggregate_df._data[index])
+    index = aggregated.index.difference(original.index)
+    return pd.concat([original, aggregated[index]])
 
 
 def _check_exclude_region_overlap(values: Dict, region_type: str) -> Dict:
     if values.get("exclude_regions") is None or values.get(region_type) is None:
         return values
     if overlap := set(values["exclude_regions"]) & {
         r.name for r in values[region_type]
     }:
         raise ExcludeRegionOverlapError(
             region=overlap, region_type=region_type, file=values["file"]
         )
     return values
-
-
-def _check_unexpected_regions(
-    df: IamDataFrame, mapping: RegionAggregationMapping
-) -> None:
-    # Raise value error if a region in the input data is not mentioned in the model
-    # mapping
-
-    if regions_not_found := set(df.region) - set(
-        mapping.model_native_region_names
-        + mapping.common_region_names
-        + [
-            const_reg
-            for comm_reg in mapping.common_regions or []
-            for const_reg in comm_reg.constituent_regions
-        ]
-        + (mapping.exclude_regions or [])
-    ):
-        raise ValueError(
-            f"Did not find region(s) {regions_not_found} in 'native_regions', "
-            "'common_regions' or 'exclude_regions' in model mapping for "
-            f"{mapping.model} in {mapping.file}. If they are not meant to be included "
-            "in the results add to the 'exclude_regions' section in the model mapping "
-            "to silence this error."
-        )
```

### Comparing `nomenclature-iamc-0.8/nomenclature/processor/required_data.py` & `nomenclature-iamc-0.9/nomenclature/processor/required_data.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature/testing.py` & `nomenclature-iamc-0.9/nomenclature/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,17 @@
     definitions: str = "definitions",
     dimensions: Optional[List[str]] = None,
     mappings: Optional[str] = None,
 ) -> None:
     dsd = DataStructureDefinition(path / definitions, dimensions)
     if mappings is None:
         if (path / "mappings").is_dir():
-            RegionProcessor.from_directory(path / "mappings").validate_with_definition(
-                dsd
-            )
+            RegionProcessor.from_directory(path / "mappings", dsd)
     elif (path / mappings).is_dir():
-        RegionProcessor.from_directory(path / mappings).validate_with_definition(dsd)
+        RegionProcessor.from_directory(path / mappings, dsd)
     else:
         raise FileNotFoundError(f"Mappings directory not found: {path / mappings}")
 
 
 def _collect_requiredData_errors(
     requiredDatadir: Path, dsd: DataStructureDefinition
 ) -> None:
```

### Comparing `nomenclature-iamc-0.8/nomenclature/validation.py` & `nomenclature-iamc-0.9/nomenclature/validation.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature/validation_schemas/generic_schema.yaml` & `nomenclature-iamc-0.9/nomenclature/validation_schemas/generic_schema.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature/validation_schemas/region_mapping_schema.yaml` & `nomenclature-iamc-0.9/nomenclature/validation_schemas/region_mapping_schema.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature/validation_schemas/region_schema.yaml` & `nomenclature-iamc-0.9/nomenclature/validation_schemas/region_schema.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature/validation_schemas/tag_schema.yaml` & `nomenclature-iamc-0.9/nomenclature/validation_schemas/tag_schema.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature/validation_schemas/variable_schema.yaml` & `nomenclature-iamc-0.9/nomenclature/validation_schemas/variable_schema.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/nomenclature_iamc.egg-info/PKG-INFO` & `nomenclature-iamc-0.9/nomenclature_iamc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenclature-iamc
-Version: 0.8
+Version: 0.9
 Summary: Package for managing codelists & attributes for IAMC-format datasets
 Home-page: https://github.com/IAMconsortium/nomenclature
 Author: Scenario Services team, ECE program, IIASA
 Author-email: ece-scse@iiasa.ac.at
 License: APACHE-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nomenclature-iamc-0.8/nomenclature_iamc.egg-info/SOURCES.txt` & `nomenclature-iamc-0.9/nomenclature_iamc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 nomenclature/validation_schemas/variable_schema.yaml
 nomenclature_iamc.egg-info/PKG-INFO
 nomenclature_iamc.egg-info/SOURCES.txt
 nomenclature_iamc.egg-info/dependency_links.txt
 nomenclature_iamc.egg-info/entry_points.txt
 nomenclature_iamc.egg-info/requires.txt
 nomenclature_iamc.egg-info/top_level.txt
-tests/alias_test.py
 tests/conftest.py
 tests/test_check_aggregate.py
 tests/test_cli.py
 tests/test_code.py
 tests/test_codelist.py
 tests/test_core.py
 tests/test_definition.py
@@ -76,14 +75,15 @@
 tests/test_region_aggregation.py
 tests/test_required_data.py
 tests/test_testing.py
 tests/test_validation.py
 tests/data/validation_nc.xlsx
 tests/data/validation_nc_duplicates.xlsx
 tests/data/validation_nc_flat.yaml
+tests/data/validation_nc_list_arg.xlsx
 tests/data/check_aggregate/components/region/regions.yaml
 tests/data/check_aggregate/components/variable/variables.yaml
 tests/data/check_aggregate/components_dict/region/regions.yaml
 tests/data/check_aggregate/components_dict/variable/variables.yaml
 tests/data/custom_dimension_nc/region/regions.yaml
 tests/data/custom_dimension_nc/scenario/scenarios.yaml
 tests/data/custom_dimension_nc/variable/tag_fuel.yaml
@@ -95,14 +95,15 @@
 tests/data/empty_definitions_dir/definitions/.gitkeep
 tests/data/end_whitespace/definitions/scenario/scenarios.yaml
 tests/data/extras_nc/region/regions.yaml
 tests/data/extras_nc/variable/variables.yaml
 tests/data/failing_variable_codelist/rename_arg_conflict/variable/variables.yaml
 tests/data/failing_variable_codelist/rename_undefined_target/variable/variables.yaml
 tests/data/failing_variable_codelist/unknown_weight/variable/variables.yaml
+tests/data/general_filtering/basic_codelist.yaml
 tests/data/hidden_character/definitions/scenario/scenarios.yaml
 tests/data/invalid_yaml/foo.yaml
 tests/data/multiple_unit_codelist/variable.yaml
 tests/data/non-default_dimensions/definitions/region/regions.yaml
 tests/data/non-default_dimensions/definitions/scenario/scenarios.yaml
 tests/data/non-default_dimensions/definitions/variable/variables.yaml
 tests/data/non-default_dimensions/mappings/mapping_1.yaml
@@ -146,14 +147,15 @@
 tests/data/region_processing/skip_aggregation/mappings/model_b.yaml
 tests/data/region_processing/weighted_aggregation/aggregate/aggregate_only.yaml
 tests/data/region_processing/weighted_aggregation/dsd/region/regions.yaml
 tests/data/region_processing/weighted_aggregation/dsd/variable/variables.yaml
 tests/data/region_processing/weighted_aggregation_rename/aggregate/aggregate_only.yaml
 tests/data/region_processing/weighted_aggregation_rename/dsd/region/regions.yaml
 tests/data/region_processing/weighted_aggregation_rename/dsd/variable/variables.yaml
+tests/data/region_to_filter_codelist/region_filtering.yaml
 tests/data/regionprocessor_duplicate/mapping_1.yaml
 tests/data/regionprocessor_duplicate/mapping_2.yaml
 tests/data/regionprocessor_exclude_region_overlap/exclude_common_overlap.yaml
 tests/data/regionprocessor_exclude_region_overlap/exclude_native_overlap.yaml
 tests/data/regionprocessor_not_defined/mapping_1.yaml
 tests/data/regionprocessor_not_defined/mapping_2.yaml
 tests/data/regionprocessor_unexpected_region/model_a.yaml
@@ -181,8 +183,9 @@
 tests/data/structure_validation_no_mappings/definitions/region/regions.yaml
 tests/data/structure_validation_no_mappings/definitions/variable/variables.yaml
 tests/data/tagged_codelist/foo.yaml
 tests/data/tagged_codelist/tag_sector.yaml
 tests/data/tagged_codelist/tag_source.yaml
 tests/data/validation_nc/region/regions.yaml
 tests/data/validation_nc/variable/tag_fuel.yaml
-tests/data/validation_nc/variable/variables.yaml
+tests/data/validation_nc/variable/variables.yaml
+tests/data/variable_codelist_complex_attr/variable_complex_attr.yaml
```

### Comparing `nomenclature-iamc-0.8/setup.cfg` & `nomenclature-iamc-0.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 	pyam-iamc >= 1.7.0
 	openpyxl
 	setuptools >= 41
 	pydantic
 	pyyaml
 	jsonschema
 	setuptools_scm
-	pandas
+	pandas >= 1.5.2
+	numpy
 setup_requires = 
 	setuptools >= 41
 	setuptools_scm
 
 [options.extras_require]
 tests = 
 	pytest
```

### Comparing `nomenclature-iamc-0.8/tests/data/check_aggregate/components/variable/variables.yaml` & `nomenclature-iamc-0.9/tests/data/check_aggregate/components/variable/variables.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/tests/data/check_aggregate/components_dict/variable/variables.yaml` & `nomenclature-iamc-0.9/tests/data/check_aggregate/components_dict/variable/variables.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/tests/data/region_processing/dsd/variable/variables.yaml` & `nomenclature-iamc-0.9/tests/data/region_processing/dsd/variable/variables.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/tests/data/validation_nc_duplicates.xlsx` & `nomenclature-iamc-0.9/tests/data/validation_nc_duplicates.xlsx`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/tests/test_check_aggregate.py` & `nomenclature-iamc-0.9/tests/test_check_aggregate.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 def expected_fail_return(name):
     index = pd.Index(
         [
             ("model_a", "scen_a", "World", f"Final Energy{name}", "EJ/yr", 2005),
             ("model_a", "scen_a", "World", "Final Energy|Industry", "EJ/yr", 2005),
         ],
-        names=["model", "scenario", "region", "variable", "unit", "year"],
+        name=("model", "scenario", "region", "variable", "unit", "year"),
     )
     columns = ["variable", "components"]
     return pd.DataFrame([[9.0, 10.0], [8.0, 7.0]], columns=columns, index=index)
 
 
 @pytest.mark.parametrize(
     "components, components_type",
```

### Comparing `nomenclature-iamc-0.8/tests/test_cli.py` & `nomenclature-iamc-0.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/tests/test_core.py` & `nomenclature-iamc-0.9/tests/test_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import pandas as pd
 from nomenclature.core import process
 from nomenclature.definition import DataStructureDefinition
 from nomenclature.processor.region import RegionProcessor
 from pyam import IAMC_IDX, IamDataFrame, assert_iamframe_equal
 
-from conftest import TEST_DATA_DIR
+from conftest import TEST_DATA_DIR, add_meta
 
 
 @pytest.mark.parametrize("model_name", ["model_a", "model_c"])
 def test_region_processing_rename(model_name):
     # Test **only** the renaming aspect, i.e. 3 things:
     # 1. All native regions **with** a renaming property should be renamed correctly
     # 2. All native regions **without** a renaming property should be passed through
@@ -28,26 +28,25 @@
                 [model_name, "scen_a", "region_a", "Primary Energy", "EJ/yr", 1, 2],
                 [model_name, "scen_a", "region_B", "Primary Energy", "EJ/yr", 3, 4],
                 [model_name, "scen_a", "region_C", "Primary Energy", "EJ/yr", 5, 6],
             ],
             columns=IAMC_IDX + [2005, 2010],
         )
     )
+    add_meta(test_df)
 
     exp = copy.deepcopy(test_df)
     exp.filter(region=["region_a", "region_B"], inplace=True)
     exp.rename(region={"region_a": "region_A"}, inplace=True)
 
-    obs = process(
-        test_df,
-        DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
-        processor=RegionProcessor.from_directory(
-            TEST_DATA_DIR / "region_processing/rename_only"
-        ),
+    dsd = DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd")
+    region_processor = RegionProcessor.from_directory(
+        TEST_DATA_DIR / "region_processing/rename_only", dsd
     )
+    obs = process(test_df, dsd, processor=region_processor)
 
     assert_iamframe_equal(obs, exp)
 
 
 @pytest.mark.parametrize(
     "rp_dir", ["region_processing/rename_only", "region_processing/empty_aggregation"]
 )
@@ -60,32 +59,32 @@
             [
                 ["model_a", "scen_a", "region_foo", "Primary Energy", "EJ/yr", 1, 2],
                 ["model_b", "scen_a", "region_foo", "Primary Energy", "EJ/yr", 1, 2],
             ],
             columns=IAMC_IDX + [2005, 2010],
         )
     )
-    with pytest.raises(ValueError, match=("'model_a', 'model_b'.*empty dataset")):
+    with pytest.raises(ValueError, match=("Region.*'model_a'.*empty dataset")):
         process(
             test_df,
-            DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
-            processor=RegionProcessor.from_directory(TEST_DATA_DIR / rp_dir),
+            dsd := DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
+            processor=RegionProcessor.from_directory(TEST_DATA_DIR / rp_dir, dsd),
         )
 
 
 def test_region_processing_no_mapping(simple_df):
     # Test that a model without a mapping is passed untouched
 
     exp = copy.deepcopy(simple_df)
 
     obs = process(
         simple_df,
-        DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
+        dsd := DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
         processor=RegionProcessor.from_directory(
-            TEST_DATA_DIR / "region_processing/no_mapping"
+            TEST_DATA_DIR / "region_processing/no_mapping", dsd
         ),
     )
     assert_iamframe_equal(obs, exp)
 
 
 def test_region_processing_aggregate():
     # Test only the aggregation feature
@@ -97,29 +96,32 @@
                 ["model_a", "scen_a", "region_C", "Primary Energy", "EJ/yr", 5, 6],
                 ["model_a", "scen_b", "region_A", "Primary Energy", "EJ/yr", 1, 2],
                 ["model_a", "scen_b", "region_B", "Primary Energy", "EJ/yr", 3, 4],
             ],
             columns=IAMC_IDX + [2005, 2010],
         )
     )
+    add_meta(test_df)
+
     exp = IamDataFrame(
         pd.DataFrame(
             [
                 ["model_a", "scen_a", "World", "Primary Energy", "EJ/yr", 4, 6],
                 ["model_a", "scen_b", "World", "Primary Energy", "EJ/yr", 4, 6],
             ],
             columns=IAMC_IDX + [2005, 2010],
         )
     )
+    add_meta(exp)
 
     obs = process(
         test_df,
-        DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
+        dsd := DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
         processor=RegionProcessor.from_directory(
-            TEST_DATA_DIR / "region_processing/aggregate_only"
+            TEST_DATA_DIR / "region_processing/aggregate_only", dsd
         ),
     )
 
     assert_iamframe_equal(obs, exp)
 
 
 @pytest.mark.parametrize(
@@ -140,34 +142,37 @@
                 ["m_a", "s_a", "region_a", "Primary Energy|Coal", "EJ/yr", 0.5, 1],
                 ["m_a", "s_a", "region_B", "Primary Energy|Coal", "EJ/yr", 1.5, 2],
                 ["m_b", "s_b", "region_A", "Primary Energy", "EJ/yr", 1, 2],
             ],
             columns=IAMC_IDX + [2005, 2010],
         )
     )
+    add_meta(test_df)
+
     exp = IamDataFrame(
         pd.DataFrame(
             [
                 ["m_a", "s_a", "region_A", "Primary Energy", "EJ/yr", 1, 2],
                 ["m_a", "s_a", "region_B", "Primary Energy", "EJ/yr", 3, 4],
                 ["m_a", "s_a", "World", "Primary Energy", "EJ/yr", 4, 6],
                 ["m_a", "s_a", "region_A", "Primary Energy|Coal", "EJ/yr", 0.5, 1],
                 ["m_a", "s_a", "region_B", "Primary Energy|Coal", "EJ/yr", 1.5, 2],
                 ["m_a", "s_a", "World", "Primary Energy|Coal", "EJ/yr", 2, 3],
                 ["m_b", "s_b", "region_A", "Primary Energy", "EJ/yr", 1, 2],
             ],
             columns=IAMC_IDX + [2005, 2010],
         )
     )
+    add_meta(exp)
 
     obs = process(
         test_df,
-        DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
+        dsd := DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
         processor=RegionProcessor.from_directory(
-            TEST_DATA_DIR / "region_processing" / directory
+            TEST_DATA_DIR / "region_processing" / directory, dsd
         ),
     )
     assert_iamframe_equal(obs, exp)
 
 
 @pytest.mark.parametrize(
     "folder, exp_df, args",
@@ -215,25 +220,29 @@
                 ["model_a", "scen_a", "region_B", "Emissions|CO2", "Mt CO2", 1, 2],
                 ["model_a", "scen_a", "region_A", "Price|Carbon", "USD/t CO2", 3, 8],
                 ["model_a", "scen_a", "region_B", "Price|Carbon", "USD/t CO2", 2, 4],
             ],
             columns=IAMC_IDX + [2005, 2010],
         )
     )
+    add_meta(test_df)
 
     if args is not None:
         test_df = test_df.filter(**args)
 
     exp = IamDataFrame(pd.DataFrame(exp_df, columns=IAMC_IDX + [2005, 2010]))
+    add_meta(exp)
 
     obs = process(
         test_df,
-        DataStructureDefinition(TEST_DATA_DIR / "region_processing" / folder / "dsd"),
+        dsd := DataStructureDefinition(
+            TEST_DATA_DIR / "region_processing" / folder / "dsd"
+        ),
         processor=RegionProcessor.from_directory(
-            TEST_DATA_DIR / "region_processing" / folder / "aggregate"
+            TEST_DATA_DIR / "region_processing" / folder / "aggregate", dsd
         ),
     )
     assert_iamframe_equal(obs, exp)
     # check the logs since the presence of args should cause a warning in the logs
     if args:
         logmsg = (
             "Could not aggregate 'Price|Carbon' for region 'World' "
@@ -247,40 +256,43 @@
     [("model_a", ("region_A", "region_B")), ("model_b", ("region_A", "region_b"))],
 )
 def test_region_processing_skip_aggregation(model_name, region_names):
     # Testing two cases:
     # * model "m_a" renames native regions and the world region is skipped
     # * model "m_b" renames single constituent common regions
 
-    input_df = IamDataFrame(
+    test_df = IamDataFrame(
         pd.DataFrame(
             [
                 [model_name, "s_a", region_names[0], "Primary Energy", "EJ/yr", 1, 2],
                 [model_name, "s_a", region_names[1], "Primary Energy", "EJ/yr", 3, 4],
             ],
             columns=IAMC_IDX + [2005, 2010],
         )
     )
+    add_meta(test_df)
+
     exp = IamDataFrame(
         pd.DataFrame(
             [
                 [model_name, "s_a", "region_A", "Primary Energy", "EJ/yr", 1, 2],
                 [model_name, "s_a", "region_B", "Primary Energy", "EJ/yr", 3, 4],
             ],
             columns=IAMC_IDX + [2005, 2010],
         )
     )
+    add_meta(exp)
 
     obs = process(
-        input_df,
-        DataStructureDefinition(
+        test_df,
+        dsd := DataStructureDefinition(
             TEST_DATA_DIR / "region_processing/skip_aggregation/dsd"
         ),
         processor=RegionProcessor.from_directory(
-            TEST_DATA_DIR / "region_processing/skip_aggregation/mappings"
+            TEST_DATA_DIR / "region_processing/skip_aggregation/mappings", dsd
         ),
     )
     assert_iamframe_equal(obs, exp)
 
 
 @pytest.mark.parametrize(
     "input_data, exp_data, warning",
@@ -347,29 +359,27 @@
                 ["m_a", "s_a", "region_A", "Primary Energy", "EJ/yr", 1, 2],
                 ["m_a", "s_a", "region_B", "Primary Energy", "EJ/yr", 3, 4],
                 ["m_a", "s_a", "World", "Primary Energy", "EJ/yr", 5, 6],
             ],
             [["m_a", "s_a", "World", "Primary Energy", "EJ/yr", 5, 6]],
             [
                 "Difference between original and aggregated data:",
-                "m_a   s_a      World  Primary Energy",
-                "2005              5            4",
+                "m_a   s_a      World  Primary Energy EJ/yr 2005         5           4",
             ],
         ),
         (  # Conflict between overlapping renamed variable and provided data
             [
                 ["m_a", "s_a", "region_A", "Variable B", "EJ/yr", 1, 2],
                 ["m_a", "s_a", "region_B", "Variable B", "EJ/yr", 3, 4],
                 ["m_a", "s_a", "World", "Variable B", "EJ/yr", 4, 6],
             ],
             [["m_a", "s_a", "World", "Variable B", "EJ/yr", 4, 6]],
             [
                 "Difference between original and aggregated data:",
-                "m_a   s_a      World  Variable B EJ/yr",
-                "2005              4            3",
+                "m_a   s_a      World  Variable B EJ/yr 2005         4           3",
             ],
         ),
     ],
 )
 def test_partial_aggregation(input_data, exp_data, warning, caplog):
     # Dedicated test for partial aggregation
     # Test cases are:
@@ -377,22 +387,27 @@
     # * Variable is only available in the provided data
     # * Variable is only available in the aggregated data
     # * Variable is not available in all scenarios in the provided data
     # * Using skip-aggregation: true should only take provided results
     # * Using the region-aggregation attribute to create an additional variable
     # * Variable is available in provided and aggregated data but different
 
+    test_df = IamDataFrame(pd.DataFrame(input_data, columns=IAMC_IDX + [2005, 2010]))
+    add_meta(test_df)
+
     obs = process(
-        IamDataFrame(pd.DataFrame(input_data, columns=IAMC_IDX + [2005, 2010])),
-        DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
+        test_df,
+        dsd := DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
         processor=RegionProcessor.from_directory(
-            TEST_DATA_DIR / "region_processing/partial_aggregation"
+            TEST_DATA_DIR / "region_processing/partial_aggregation", dsd
         ),
     )
+
     exp = IamDataFrame(pd.DataFrame(exp_data, columns=IAMC_IDX + [2005, 2010]))
+    add_meta(exp)
 
     # Assert that we get the expected values
     assert_iamframe_equal(obs, exp)
 
     # Assert that we get the correct warnings
     if warning is None:
         assert "WARNING" not in caplog.text
```

### Comparing `nomenclature-iamc-0.8/tests/test_definition.py` & `nomenclature-iamc-0.9/tests/test_definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,24 +49,31 @@
     simple_definition.to_excel(file)
 
     obs = pd.read_excel(file)
     exp = pd.read_excel(TEST_DATA_DIR / "validation_nc.xlsx")
     pd.testing.assert_frame_equal(obs, exp)
 
 
-def test_create_yaml_from_xlsx(tmpdir):
+@pytest.mark.parametrize(
+    "input_file, attrs",
+    [
+        ("validation_nc.xlsx", ["Description", "Unit"]),
+        ("validation_nc_list_arg.xlsx", ["Description", "Unit", "Region-aggregation"]),
+    ],
+)
+def test_create_yaml_from_xlsx(input_file, attrs, tmpdir):
     """Check that creating a yaml codelist from xlsx yields the expected output file"""
     file = tmpdir / "foo.yaml"
 
     create_yaml_from_xlsx(
-        source=TEST_DATA_DIR / "validation_nc.xlsx",
+        source=TEST_DATA_DIR / input_file,
         target=file,
         sheet_name="variable_definitions",
         col="Variable",
-        attrs=["Description", "Unit"],
+        attrs=attrs,
     )
 
     with open(file, "r") as f:
         obs = f.read()
     with open(TEST_DATA_DIR / "validation_nc_flat.yaml", "r") as f:
         exp = f.read()
 
@@ -77,9 +84,9 @@
     """Check that creating a yaml codelist from xlsx with duplicates raises"""
     with pytest.raises(ValueError, match="Duplicate values in the codelist:"):
         create_yaml_from_xlsx(
             source=TEST_DATA_DIR / "validation_nc_duplicates.xlsx",
             target="_",
             sheet_name="duplicate_index_raises",
             col="Variable",
-            attrs=["Unit", "Definition"],
+            attrs=["Unit", "Description"],
         )
```

### Comparing `nomenclature-iamc-0.8/tests/test_definition_variable.py` & `nomenclature-iamc-0.9/tests/test_definition_variable.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/tests/test_region_aggregation.py` & `nomenclature-iamc-0.9/tests/test_region_aggregation.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,17 +104,17 @@
 @pytest.mark.parametrize(
     "region_processor_path",
     [
         TEST_DATA_DIR / "regionprocessor_working",
         (TEST_DATA_DIR / "regionprocessor_working").relative_to(Path.cwd()),
     ],
 )
-def test_region_processor_working(region_processor_path):
+def test_region_processor_working(region_processor_path, simple_definition):
 
-    obs = RegionProcessor.from_directory(region_processor_path)
+    obs = RegionProcessor.from_directory(region_processor_path, simple_definition)
     exp_data = [
         {
             "model": ["model_a"],
             "file": (
                 TEST_DATA_DIR / "regionprocessor_working/mapping_1.yml"
             ).relative_to(Path.cwd()),
             "native_regions": [
@@ -151,22 +151,24 @@
     error_msg = (
         "model_(a|b).*\n.*region_a.*mapping_(1|2).yaml.*value_error.region_not_defined"
         ".*\n.*model_(a|b).*\n.*region_a.*mapping_(1|2).yaml.*value_error."
         "region_not_defined"
     )
     with pytest.raises(pydantic.ValidationError, match=error_msg):
         RegionProcessor.from_directory(
-            TEST_DATA_DIR / "regionprocessor_not_defined"
-        ).validate_with_definition(simple_definition)
+            TEST_DATA_DIR / "regionprocessor_not_defined", simple_definition
+        )
 
 
-def test_region_processor_duplicate_model_mapping():
+def test_region_processor_duplicate_model_mapping(simple_definition):
     error_msg = ".*model_a.*mapping_(1|2).yaml.*mapping_(1|2).yaml"
     with pytest.raises(pydantic.ValidationError, match=error_msg):
-        RegionProcessor.from_directory(TEST_DATA_DIR / "regionprocessor_duplicate")
+        RegionProcessor.from_directory(
+            TEST_DATA_DIR / "regionprocessor_duplicate", simple_definition
+        )
 
 
 def test_region_processor_wrong_args():
     # Test if pydantic correctly type checks the input of RegionProcessor.from_directory
 
     # Test with an integer
     with pytest.raises(pydantic.ValidationError, match=".*path\n.*not a valid path.*"):
@@ -178,34 +180,36 @@
         match=".*path\n.*does not point to a directory.*",
     ):
         RegionProcessor.from_directory(
             TEST_DATA_DIR / "regionprocessor_working/mapping_1.yml"
         )
 
 
-def test_region_processor_multiple_wrong_mappings():
+def test_region_processor_multiple_wrong_mappings(simple_definition):
     # Read in the entire region_aggregation directory and return **all** errors
     msg = "9 validation errors for RegionProcessor"
 
     with pytest.raises(pydantic.ValidationError, match=msg):
-        RegionProcessor.from_directory(TEST_DATA_DIR / "region_aggregation")
+        RegionProcessor.from_directory(
+            TEST_DATA_DIR / "region_aggregation", simple_definition
+        )
 
 
-def test_region_processor_exclude_model_native_overlap_raises():
+def test_region_processor_exclude_model_native_overlap_raises(simple_definition):
     # Test that exclude regions in either native or common regions raise errors
 
     with pytest.raises(
         pydantic.ValidationError,
         match=(
             "'region_a'.* ['native_regions'|'common_regions'].*\n.*\n.*'region_a'.*"
             "['native_regions'|'common_regions']"
         ),
     ):
         RegionProcessor.from_directory(
-            TEST_DATA_DIR / "regionprocessor_exclude_region_overlap"
+            TEST_DATA_DIR / "regionprocessor_exclude_region_overlap", simple_definition
         )
 
 
 def test_region_processor_unexpected_region_raises():
 
     test_df = IamDataFrame(
         pd.DataFrame(
@@ -215,12 +219,12 @@
             ],
             columns=IAMC_IDX + [2005],
         )
     )
     with pytest.raises(ValueError, match="Did not find.*'region_B'.*in.*model_a.yaml"):
         process(
             test_df,
-            DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
+            dsd := DataStructureDefinition(TEST_DATA_DIR / "region_processing/dsd"),
             processor=RegionProcessor.from_directory(
-                TEST_DATA_DIR / "regionprocessor_unexpected_region"
+                TEST_DATA_DIR / "regionprocessor_unexpected_region", dsd
             ),
         )
```

### Comparing `nomenclature-iamc-0.8/tests/test_required_data.py` & `nomenclature-iamc-0.9/tests/test_required_data.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/tests/test_testing.py` & `nomenclature-iamc-0.9/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.8/tests/test_validation.py` & `nomenclature-iamc-0.9/tests/test_validation.py`

 * *Files identical despite different names*

