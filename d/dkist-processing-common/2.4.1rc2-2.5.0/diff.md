# Comparing `tmp/dkist-processing-common-2.4.1rc2.tar.gz` & `tmp/dkist-processing-common-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-2.4.1rc2.tar", last modified: Fri Apr 14 21:05:03 2023, max compression
+gzip compressed data, was "dkist-processing-common-2.5.0.tar", last modified: Tue May  2 15:17:03 2023, max compression
```

## Comparing `dkist-processing-common-2.4.1rc2.tar` & `dkist-processing-common-2.5.0.tar`

### file list

```diff
@@ -1,116 +1,115 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.839607 dkist-processing-common-2.4.1rc2/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    11805 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-04-14 21:05:03.839607 dkist-processing-common-2.4.1rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.827607 dkist-processing-common-2.4.1rc2/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/changelog/128.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.827607 dkist-processing-common-2.4.1rc2/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.827607 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.827607 dkist-processing-common-2.4.1rc2/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6987 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.831606 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3304 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     7365 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.831606 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6264 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5598 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.831606 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     8152 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10675 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.835606 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13155 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.835606 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8226 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47886 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     7123 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18355 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.835606 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     9758 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_l1_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10499 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36040 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11128 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14982 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.827607 dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-04-14 21:05:03.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4211 2023-04-14 21:05:03.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-14 21:05:03.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-04-14 21:05:03.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-14 21:05:03.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.839607 dkist-processing-common-2.4.1rc2/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.839607 dkist-processing-common-2.4.1rc2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-04-14 21:05:03.839607 dkist-processing-common-2.4.1rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.928857 dkist-processing-common-2.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    12871 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-02 15:17:03.928857 dkist-processing-common-2.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.912857 dkist-processing-common-2.5.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.912857 dkist-processing-common-2.5.0/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.916857 dkist-processing-common-2.5.0/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.916857 dkist-processing-common-2.5.0/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6987 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.920857 dkist-processing-common-2.5.0/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/models/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     7365 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.920857 dkist-processing-common-2.5.0/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.920857 dkist-processing-common-2.5.0/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     8152 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10675 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.924857 dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6718 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13155 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.924857 dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8226 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     7123 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18550 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.928857 dkist-processing-common-2.5.0/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12961 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_l1_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10499 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36040 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11128 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.916857 dkist-processing-common-2.5.0/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-02 15:17:03.000000 dkist-processing-common-2.5.0/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4188 2023-05-02 15:17:03.000000 dkist-processing-common-2.5.0/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-02 15:17:03.000000 dkist-processing-common-2.5.0/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-05-02 15:17:03.000000 dkist-processing-common-2.5.0/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-02 15:17:03.000000 dkist-processing-common-2.5.0/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.928857 dkist-processing-common-2.5.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 15:17:03.928857 dkist-processing-common-2.5.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-02 15:17:03.928857 dkist-processing-common-2.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-02 15:16:58.000000 dkist-processing-common-2.5.0/setup.py
```

### Comparing `dkist-processing-common-2.4.1rc2/.gitignore` & `dkist-processing-common-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/.pre-commit-config.yaml` & `dkist-processing-common-2.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/CHANGELOG.rst` & `dkist-processing-common-2.5.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+v2.5.0 (2023-05-02)
+===================
+
+Bugfixes
+--------
+
+- Replace `astropy.time.Time` with `datetime.datetime` for reading header "DATE-OBS" values in `ParseL0InputData` task. This should produce a very large speedup in the task when parsing large datasets. (`#134 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/134>`__)
+
+
+Misc
+----
+
+- Set WAVEMIN and WAVEMAX header keys based on abstract method get_wavelength_range implemented by each instrument (`#133 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/133>`__)
+- Improved `__repr__` in `CSStep` and `FitsAccessBase` objects. The latter affects all `*FitsAccess` subclasses as well. (`#135 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/135>`__)
+
+
+v2.4.1 (2023-04-14)
+===================
+
+Misc
+----
+
+- remove spectral line support from dkist-processing-common because it now resides in `dkist-spectral-lines <https://pypi.org/project/dkist-spectral-lines/>`_ (`#128 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/128>`__)
+
+
 v2.4.0 (2023-04-12)
 ===================
 
 Features
 --------
 
 - Make histogram plots of all parameters that are free in local PolCal fits. (`#132 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/132>`__)
```

### Comparing `dkist-processing-common-2.4.1rc2/PKG-INFO` & `dkist-processing-common-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.4.1rc2
+Version: 2.5.0
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.4.1rc2/README.rst` & `dkist-processing-common-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/bitbucket-pipelines.yml` & `dkist-processing-common-2.5.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/check_changelog_updated.sh` & `dkist-processing-common-2.5.0/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/config.py` & `dkist-processing-common-2.5.0/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/constants.py` & `dkist-processing-common-2.5.0/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-2.5.0/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-2.5.0/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-2.5.0/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/tags.py` & `dkist-processing-common-2.5.0/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-2.5.0/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/manual.py` & `dkist-processing-common-2.5.0/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/constants.py` & `dkist-processing-common-2.5.0/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-2.5.0/dkist_processing_common/models/fits_access.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,21 +20,24 @@
     auto_squeeze
         A boolean indicating whether to 'squeeze' out dimensions of size 1
     """
 
     def __init__(
         self,
         hdu: fits.ImageHDU | fits.PrimaryHDU | fits.CompImageHDU,
-        name: str | None = None,
+        name: str | Path | None = None,
         auto_squeeze: bool = True,
     ):
         self._hdu = hdu
         self.name = name
         self.auto_squeeze = auto_squeeze
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}(hdu={self._hdu!r}, name={self.name!r}, auto_squeeze={self.auto_squeeze})"
+
     @property
     def data(self) -> np.ndarray:
         """
         Return the data array from the associated FITS object, with axes of length 1 removed if the array has three dimensions and the unit axis is the zeroth one.
 
         This is intended solely to remove the dummy dimension that is in raw data from the summit.
```

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-2.5.0/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/graphql.py` & `dkist-processing-common-2.5.0/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/json_encoder.py` & `dkist-processing-common-2.5.0/dkist_processing_common/models/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/message.py` & `dkist-processing-common-2.5.0/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/parameters.py` & `dkist-processing-common-2.5.0/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/quality.py` & `dkist-processing-common-2.5.0/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/tags.py` & `dkist-processing-common-2.5.0/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-2.5.0/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-2.5.0/dkist_processing_common/parsers/cs_step.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Classes supporting Calibration Sequence steps."""
 from __future__ import annotations
 
+from datetime import datetime
+from datetime import timezone
 from typing import Type
 
-from astropy.time import Time
-
 from dkist_processing_common.models.constants import BudName
 from dkist_processing_common.models.flower_pot import SpilledDirt
 from dkist_processing_common.models.flower_pot import Stem
 from dkist_processing_common.models.tags import StemName
 from dkist_processing_common.parsers.l0_fits_access import L0FitsAccess
 
 
@@ -41,43 +41,43 @@
     def __init__(self, fits_obj: L0FitsAccess, max_cs_time_sec: float):
         """Initialize and read the GOS configuration and time from a SPEC-0122 FITS header."""
         self.pol_in = fits_obj.gos_polarizer_status not in ["undefined", "clear"]
         self.pol_theta = round(fits_obj.gos_polarizer_angle, 3) % 360
         self.ret_in = fits_obj.gos_retarder_status not in ["undefined", "clear"]
         self.ret_theta = round(fits_obj.gos_retarder_angle, 3) % 360
         self.dark_in = fits_obj.gos_level0_status == "DarkShutter"
-        self.obs_time = Time(fits_obj.time_obs, precision=6)
+        self.obs_time = datetime.fromisoformat(fits_obj.time_obs).replace(tzinfo=timezone.utc)
         self.max_cs_time_sec = max_cs_time_sec
 
-        self.max_cs_time_sec = max_cs_time_sec
+        self.fits_obj = fits_obj
 
     def __repr__(self):
-        return f"CS step taken on {self.obs_time.fits}"
+        return f"{self.__class__.__name__}({self.fits_obj!r}, max_cs_time_sec={self.max_cs_time_sec!r})"
 
     def __str__(self):
         return "CS step with Pol = {}:{}, Ret = {}:{}, Dark = {}. Taken at {}".format(
             self.pol_in,
             self.pol_theta,
             self.ret_in,
             self.ret_theta,
             self.dark_in,
-            self.obs_time.fits,
+            self.obs_time.isoformat(),
         )
 
     def __eq__(self, other: object) -> bool:
         """Two steps are equal if they have the same GOS configuration and are taken within some package-defined time of each other."""
         if not isinstance(other, CSStep):
             raise TypeError(f"Cannot compare CSStep with type {type(other)}")
 
         for item in ["pol_in", "pol_theta", "ret_in", "ret_theta", "dark_in"]:
             if getattr(self, item) != getattr(other, item):
                 return False
 
         tdelt = abs(self.obs_time - other.obs_time)
-        if tdelt.sec > self.max_cs_time_sec:
+        if tdelt.total_seconds() > self.max_cs_time_sec:
             return False
 
         return True
 
     def __lt__(self, other: CSStep) -> bool:
         """Only based on time."""
         return self.obs_time < other.obs_time
```

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-2.5.0/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-2.5.0/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-2.5.0/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-2.5.0/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-2.5.0/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-2.5.0/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-2.5.0/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-2.5.0/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/time.py` & `dkist-processing-common-2.5.0/dkist_processing_common/parsers/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Time parser."""
+from datetime import datetime
+from datetime import timezone
 from typing import Hashable
 from typing import Type
 
 import numpy as np
-from astropy.time import Time
 
 from dkist_processing_common.models.constants import BudName
 from dkist_processing_common.models.flower_pot import SpilledDirt
 from dkist_processing_common.models.flower_pot import Stem
 from dkist_processing_common.models.tags import EXP_TIME_ROUND_DIGITS
 from dkist_processing_common.models.tags import StemName
 from dkist_processing_common.parsers.l0_fits_access import L0FitsAccess
@@ -32,15 +33,19 @@
         fits_obj
             The input fits object
         Returns
         -------
         The observe time in seconds
         """
         if fits_obj.ip_task_type == "observe":
-            return Time(getattr(fits_obj, self.metadata_key), precision=6).unix
+            return (
+                datetime.fromisoformat(getattr(fits_obj, self.metadata_key))
+                .replace(tzinfo=timezone.utc)
+                .timestamp()
+            )
         return SpilledDirt
 
 
 class AverageCadenceBud(TimeBud):
     """Class for the average cadence Bud."""
 
     def __init__(self):
@@ -55,15 +60,14 @@
         key
             The input key
 
         Returns
         -------
         The mean value of the cadences of the input frames
         """
-        """"""
         return np.mean(np.diff(sorted(list(self.key_to_petal_dict.values()))))
 
 
 class MaximumCadenceBud(TimeBud):
     """Class for the maximum cadence bud."""
 
     def __init__(self):
```

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-2.5.0/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/base.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tasks/write_l1.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,14 @@
             header["IDSOBSID"] = ids_obs_id
         if ids_cal_id := self.metadata_store_input_dataset_calibration_frames_part_id:
             header["IDSCALID"] = ids_cal_id
         header["WKFLNAME"] = self.workflow_name
         header["WKFLVERS"] = self.workflow_version
         header = self._add_contributing_id_headers(header=header)
         # Spectral line keywords
-        header["WAVEBAND"] = get_closest_spectral_line(wavelength=header["LINEWAV"] * u.nm).name
         wavelength_range = self.get_wavelength_range(header=header)
         spectral_lines = get_spectral_lines(
             wavelength_min=wavelength_range.min,
             wavelength_max=wavelength_range.max,
         )
         if spectral_lines:
             header["NSPECLNS"] = len(spectral_lines)
@@ -221,15 +220,18 @@
         header["OBS_VR"] = (
             itrs.get_gcrs(obstime=Time(header["DATE-AVG"]))
             .transform_to(HeliocentricInertial(obstime=Time(header["DATE-AVG"])))
             .d_distance.to_value(unit=u.m / u.s)
         )  # relative velocity of observer with respect to the sun in m/s
         header["SPECSYS"] = "TOPOCENT"  # no wavelength correction made due to doppler velocity
         header["VELOSYS"] = 0.0  # no wavelength correction made due to doppler velocity
-
+        header["WAVEBAND"] = get_closest_spectral_line(wavelength=header["LINEWAV"] * u.nm).name
+        wavelength_range = self.get_wavelength_range(header=header)
+        header["WAVEMIN"] = wavelength_range.min.to_value(u.nm)
+        header["WAVEMAX"] = wavelength_range.max.to_value(u.nm)
         return header
 
     def l1_filename(self, header: fits.Header, stokes: Literal["I", "Q", "U", "V"]):
         """
         Use a FITS header to derive its filename in the following format.
 
         instrument_datetime_wavelength__stokes_datasetid_L1.fits.
```

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,88 +8,113 @@
 from dkist_processing_common.parsers.cs_step import NumCSStepBud
 from dkist_processing_common.parsers.dsps_repeat import DspsRepeatNumberFlower
 from dkist_processing_common.parsers.dsps_repeat import TotalDspsRepeatsBud
 from dkist_processing_common.parsers.proposal_id_bud import ProposalIdBud
 from dkist_processing_common.parsers.single_value_single_key_flower import (
     SingleValueSingleKeyFlower,
 )
+from dkist_processing_common.parsers.time import AverageCadenceBud
 from dkist_processing_common.parsers.time import ExposureTimeFlower
+from dkist_processing_common.parsers.time import MaximumCadenceBud
+from dkist_processing_common.parsers.time import MinimumCadenceBud
 from dkist_processing_common.parsers.time import TaskExposureTimesBud
+from dkist_processing_common.parsers.time import VarianceCadenceBud
 from dkist_processing_common.parsers.unique_bud import UniqueBud
 
 
 class FitsReader(FitsAccessBase):
     def __init__(self, hdu, name):
         super().__init__(hdu, name)
         self.thing_id: int = self.header["id_key"]
         self.constant_thing: float = self.header["constant"]
         self.name = name
         self.proposal_id: str = self.header.get("ID___013")
         self.ip_task_type: str = self.header.get("DKIST004")
         self.fpa_exposure_time_ms: float = self.header.get("TEXPOSUR")
         self.num_dsps_repeats: int = self.header["DSPSREPS"]
         self.current_dsps_repeat: int = self.header["DSPSNUM"]
+        self.time_obs: str = self.header["DATE-OBS"]
 
 
 @pytest.fixture()
 def basic_header_objs():
     header_dict = {
         "thing0": fits.header.Header(
             {
                 "id_key": 0,
                 "constant": 6.28,
                 "DKIST004": "observe",
                 "ID___013": "proposal_id_1",
                 "TEXPOSUR": 0.0013000123,
                 "DSPSNUM": 1,
                 "DSPSREPS": 2,
+                "DATE-OBS": "2022-06-17T22:00:00.000",
             }
         ),
         "thing1": fits.header.Header(
             {
                 "id_key": 1,
                 "constant": 6.28,
                 "DKIST004": "observe",
                 "ID___013": "proposal_id_1",
                 "TEXPOSUR": 0.0013000987,
                 "DSPSNUM": 1,
                 "DSPSREPS": 2,
+                "DATE-OBS": "2022-06-17T22:00:01.000",
             }
         ),
         "thing2": fits.header.Header(
             {
                 "id_key": 2,
                 "constant": 6.28,
                 "DKIST004": "dark",
                 "ID___013": "proposal_id_2",
                 "TEXPOSUR": 12.345,
                 "DSPSNUM": 2,
                 "DSPSREPS": 2,
+                "DATE-OBS": "2022-06-17T22:00:02.000",
             }
         ),
         "thing3": fits.header.Header(
             {
                 "id_key": 0,
                 "constant": 6.28,
                 "DKIST004": "observe",
                 "ID___013": "proposal_id_1",
                 "TEXPOSUR": 100.0,
                 "DSPSNUM": 2,
                 "DSPSREPS": 2,
+                "DATE-OBS": "2022-06-17T22:00:03.000",
             }
         ),
     }
     return (FitsReader.from_header(header, name=path) for path, header in header_dict.items())
 
 
 @pytest.fixture()
 def bad_header_objs():
     bad_headers = {
-        "thing0": fits.header.Header({"id_key": 0, "constant": 6.28, "DSPSREPS": 2, "DSPSNUM": 2}),
-        "thing1": fits.header.Header({"id_key": 1, "constant": 3.14, "DSPSREPS": 2, "DSPSNUM": 2}),
+        "thing0": fits.header.Header(
+            {
+                "id_key": 0,
+                "constant": 6.28,
+                "DSPSREPS": 2,
+                "DSPSNUM": 2,
+                "DATE-OBS": "2022-06-17T22:00:00.000",
+            }
+        ),
+        "thing1": fits.header.Header(
+            {
+                "id_key": 1,
+                "constant": 3.14,
+                "DSPSREPS": 2,
+                "DSPSNUM": 2,
+                "DATE-OBS": "2022-06-17T22:00:03.000",
+            }
+        ),
     }
     return (FitsReader.from_header(header, name=path) for path, header in bad_headers.items())
 
 
 def test_unique_bud(basic_header_objs):
     """
     Given: A set of headers with a constant value header key
@@ -267,8 +292,84 @@
     assert len(petals) == 2
     assert petals[0].value == 1
     assert petals[0].keys == ["thing0", "thing1"]
     assert petals[1].value == 2
     assert petals[1].keys == ["thing3"]
 
 
+def test_average_cadence_bud(basic_header_objs):
+    """
+    Given: A set of filepaths and associated headers with DATE-OBS keywords
+    When: Ingesting with the AverageCadenceBud
+    Then: The correct values are returned
+    """
+    bud = AverageCadenceBud()
+    assert bud.stem_name == BudName.average_cadence.value
+    for fo in basic_header_objs:
+        key = fo.name
+        bud.update(key, fo)
+
+    petal = list(bud.petals)
+    assert len(petal) == 1
+
+    # Because there are 3 observe frames in `basic_header_objs` spaced 1, and 2 seconds apart.
+    assert petal[0].value == 1.5
+
+
+def test_max_cadence_bud(basic_header_objs):
+    """
+    Given: A set of filepaths and associated headers with DATE-OBS keywords
+    When: Ingesting with the MaxCadenceBud
+    Then: The correct values are returned
+    """
+    bud = MaximumCadenceBud()
+    assert bud.stem_name == BudName.maximum_cadence.value
+    for fo in basic_header_objs:
+        key = fo.name
+        bud.update(key, fo)
+
+    petal = list(bud.petals)
+    assert len(petal) == 1
+
+    # Because there are 3 observe frames in `basic_header_objs` spaced 1, and 2 seconds apart.
+    assert petal[0].value == 2
+
+
+def test_minimum_cadence_bud(basic_header_objs):
+    """
+    Given: A set of filepaths and associated headers with DATE-OBS keywords
+    When: Ingesting with the MinimumCadenceBud
+    Then: The correct values are returned
+    """
+    bud = MinimumCadenceBud()
+    assert bud.stem_name == BudName.minimum_cadence.value
+    for fo in basic_header_objs:
+        key = fo.name
+        bud.update(key, fo)
+
+    petal = list(bud.petals)
+    assert len(petal) == 1
+
+    # Because there are 3 observe frames in `basic_header_objs` spaced 1, and 2 seconds apart.
+    assert petal[0].value == 1
+
+
+def test_variance_cadence_bud(basic_header_objs):
+    """
+    Given: A set of filepaths and associated headers with DATE-OBS keywords
+    When: Ingesting with the VarianceCadenceBud
+    Then: The correct values are returned
+    """
+    bud = VarianceCadenceBud()
+    assert bud.stem_name == BudName.variance_cadence.value
+    for fo in basic_header_objs:
+        key = fo.name
+        bud.update(key, fo)
+
+    petal = list(bud.petals)
+    assert len(petal) == 1
+
+    # Because there are 3 observe frames in `basic_header_objs` spaced 1, and 2 seconds apart.
+    assert petal[0].value == 0.25
+
+
 # TODO: test new flowers that have been added to parse_l0_input_data
```

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_l1_output_data_base.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_l1_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-2.5.0/dkist_processing_common/tests/test_write_l1.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from astropy.time import Time
 from astropy.time import TimeDelta
 from dkist_fits_specifications import __version__ as spec_version
 from dkist_header_validator import spec214_validator
 
 from dkist_processing_common import __version__ as common_version
 from dkist_processing_common.models.tags import Tag
-from dkist_processing_common.tasks.write_l1 import WavelengthRange
+from dkist_processing_common.models.wavelength import WavelengthRange
 from dkist_processing_common.tasks.write_l1 import WriteL1Frame
 from dkist_processing_common.tests.conftest import FakeGQLClient
 from dkist_processing_common.tests.conftest import FakeGQLClientNoRecipeConfiguration
 from dkist_processing_common.tests.conftest import TILE_SIZE
 
 
 class CompleteWriteL1Frame(WriteL1Frame):
@@ -26,16 +26,14 @@
         self, header: fits.Header, stokes: Literal["I", "Q", "U", "V"]
     ) -> fits.Header:
         header["DAAXES"] = 2
         header["DEAXES"] = 3
         header["DNAXIS"] = 5
         header["FRAMEWAV"] = 123.45
         header["LEVEL"] = 1
-        header["WAVEMAX"] = 124
-        header["WAVEMIN"] = 123
         header["WAVEREF"] = "Air"
         header["WAVEUNIT"] = -9
         header["DINDEX3"] = 3
         header["DINDEX4"] = 2
         header["DINDEX5"] = 1
         header["DNAXIS1"] = header["NAXIS1"]
         header["DNAXIS2"] = header["NAXIS2"]
@@ -245,14 +243,16 @@
         assert header["DATEREF"] == header["DATE-BEG"]
         assert round(header["OBSGEO-X"]) == -5466045
         assert round(header["OBSGEO-Y"]) == -2404389
         assert round(header["OBSGEO-Z"]) == 2242134
         assert header["SPECSYS"] == "TOPOCENT"
         assert header["VELOSYS"] == 0.0
         assert header["WAVEBAND"] == "Fe XIII (1079.8 nm)"
+        assert header["WAVEMIN"] == 1075.0
+        assert header["WAVEMAX"] == 1085.0
 
 
 def test_documentation_keys(write_l1_task, mocker):
     """
     :Given: files with headers converted to SPEC 214 L1
     :When: checking the documentation header URLs
     :Then: the correct values are found
@@ -406,13 +406,12 @@
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient",
         new=FakeGQLClient,
     )
     task, _ = write_l1_task
     header = task._add_datacenter_headers(
         header=complete_common_header, hdu_size=1024, stokes=["I", "Q", "U", "V"]
     )
-    assert header["WAVEBAND"] == "Fe XIII (1079.8 nm)"
     assert header["SPECLN01"] == "Fe XIII (1079.8 nm)"
     assert header["SPECLN02"] == "He I (1083.0 nm)"
     assert header["NSPECLNS"] == 2
     with pytest.raises(KeyError):
         assert header["SPECLN03"]
```

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-2.5.0/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.4.1rc2
+Version: 2.5.0
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-2.5.0/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
-changelog/128.misc.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
 dkist_processing_common.egg-info/requires.txt
 dkist_processing_common.egg-info/top_level.txt
```

### Comparing `dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-2.5.0/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/docs/Makefile` & `dkist-processing-common-2.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/docs/conf.py` & `dkist-processing-common-2.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/docs/make.bat` & `dkist-processing-common-2.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/licenses/LICENSE.rst` & `dkist-processing-common-2.5.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/pyproject.toml` & `dkist-processing-common-2.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc2/setup.cfg` & `dkist-processing-common-2.5.0/setup.cfg`

 * *Files identical despite different names*

