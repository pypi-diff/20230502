# Comparing `tmp/dkist_processing_vbi-1.1.9.tar.gz` & `tmp/dkist_processing_vbi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_vbi-1.1.9.tar", last modified: Thu Apr 13 20:02:03 2023, max compression
+gzip compressed data, was "dkist_processing_vbi-1.2.0.tar", last modified: Tue May  2 21:53:15 2023, max compression
```

## Comparing `dkist_processing_vbi-1.1.9.tar` & `dkist_processing_vbi-1.2.0.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     8210 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4774 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4172 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3425 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      894 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8991 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/dsps_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/num_exp_per_dsp.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/vbi_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/vbi_l1_fits_access.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2266 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4428 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)     6456 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/gain.py
--rw-rw-rw-   0 root         (0) root         (0)    13777 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)     3139 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/process_summit_processed.py
--rw-rw-rw-   0 root         (0) root         (0)     2224 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     5610 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/vbi_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4907 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9156 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    12708 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/grogu_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2415 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4711 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_gain.py
--rw-rw-rw-   0 root         (0) root         (0)     3704 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_intermediate_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)     9856 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11423 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_parse_l0.py
--rw-rw-rw-   0 root         (0) root         (0)     3340 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_parse_summit.py
--rw-rw-rw-   0 root         (0) root         (0)     8332 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_process_summit.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_vbi_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_vbi_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     4613 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/dkist_processing_vbi/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2966 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     2787 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi/workflows/summit_data_processing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.555181 dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4774 2023-04-13 20:02:03.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2577 2023-04-13 20:02:03.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-13 20:02:03.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-13 20:02:03.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-13 20:02:03.000000 dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2026 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/l0_to_l1_vbi_no-speckle.rst
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/l0_to_l1_vbi_summit-calibrated.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/docs/requirements_table.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1541 2023-04-13 20:02:03.559181 dkist_processing_vbi-1.1.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-13 20:01:57.000000 dkist_processing_vbi-1.1.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 21:53:15.940239 dkist_processing_vbi-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     9490 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6298 2023-05-02 21:53:15.940239 dkist_processing_vbi-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5696 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3425 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 21:53:15.936239 dkist_processing_vbi-1.2.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 21:53:15.936239 dkist_processing_vbi-1.2.0/dkist_processing_vbi/
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 21:53:15.936239 dkist_processing_vbi-1.2.0/dkist_processing_vbi/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/models/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 21:53:15.936239 dkist_processing_vbi-1.2.0/dkist_processing_vbi/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6939 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/parsers/mosaic_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/parsers/vbi_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/parsers/vbi_l1_fits_access.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 21:53:15.936239 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3008 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4436 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     6462 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/gain.py
+-rw-rw-rw-   0 root         (0) root         (0)    13848 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 21:53:15.936239 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)     2659 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2185 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/process_summit_processed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     5607 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/vbi_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5013 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 21:53:15.940239 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9497 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    12936 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/grogu_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2437 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4711 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_gain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_intermediate_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10054 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    12628 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_parse_l0.py
+-rw-rw-rw-   0 root         (0) root         (0)     5518 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_parse_summit.py
+-rw-rw-rw-   0 root         (0) root         (0)     8313 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_process_summit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6722 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_vbi_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_vbi_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     4746 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 21:53:15.940239 dkist_processing_vbi-1.2.0/dkist_processing_vbi/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2966 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi/workflows/summit_data_processing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 21:53:15.936239 dkist_processing_vbi-1.2.0/dkist_processing_vbi.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6298 2023-05-02 21:53:15.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2574 2023-05-02 21:53:15.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-02 21:53:15.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-05-02 21:53:15.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-02 21:53:15.000000 dkist_processing_vbi-1.2.0/dkist_processing_vbi.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 21:53:15.940239 dkist_processing_vbi-1.2.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/docs/l0_to_l1_vbi_no-speckle.rst
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/docs/l0_to_l1_vbi_summit-calibrated.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 21:53:15.940239 dkist_processing_vbi-1.2.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-05-02 21:53:15.940239 dkist_processing_vbi-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-02 21:53:10.000000 dkist_processing_vbi-1.2.0/towncrier_science.toml
```

### Comparing `dkist_processing_vbi-1.1.9/.gitignore` & `dkist_processing_vbi-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/.pre-commit-config.yaml` & `dkist_processing_vbi-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/CHANGELOG.rst` & `dkist_processing_vbi-1.2.0/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,46 @@
+v1.2.0 (2023-05-02)
+===================
+
+Features
+--------
+
+- Add support for "subcycling" that can result in multiple repeats of a mosaic for a single DSPS repeat. (`#41 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/41>`__)
+
+
+Misc
+----
+
+- Offload calculation of "WAVEMIN/MAX" in L1 headers to new functionality in `*-common` that uses the already-defined `get_wavelength_range`. The result is that this logic now only lives in one place. (`#44 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/44>`__)
+
+
+Documentation
+-------------
+
+- Replace use of `logging.[thing]` with `logger.[thing]` from `logging42`. (`#42 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/42>`__)
+- Add machinery for a "Scientific" changelog that tracks only those changes that affect L1 output data. (`#43 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/43>`__)
+
+
+v1.1.11 (2023-04-24)
+====================
+
+Misc
+----
+
+- Update `dkist-fits-specifications` to include header keys for tracking VBI mosaics.
+
+v1.1.10 (2023-04-17)
+====================
+
+Bugfixes
+--------
+
+- Correct the determination of which spectral lines should be present in L1 frames. (`#40 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/40>`__)
+
+
 v1.1.9 (2023-04-13)
 ===================
 
 Misc
 ----
 - Bump version of `dkist-processing-common`
```

### Comparing `dkist_processing_vbi-1.1.9/PKG-INFO` & `dkist_processing_vbi-1.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_vbi
-Version: 1.1.9
+Version: 1.2.0
 Summary: Code that is used by the DKIST Science Data Processing Airflow pipelines to process VBI data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-vbi/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/vbi
 Classifier: Programming Language :: Python
@@ -108,7 +108,38 @@
     # Delete tags
     git tag -d vWHATEVER.THE.VERSION
     git push --delete origin vWHATEVER.THE.VERSION
 
     # Re-tag with the same version
     git tag vWHATEVER.THE.VERSION
     git push --tags origin main
+
+Science Changelog
+^^^^^^^^^^^^^^^^^
+
+Whenever a release involves changes to the scientific quality of L1 data, additional changelog fragment(s) should be
+created. These fragments are intended to be as verbose as is needed to accurately capture the scope of the change(s),
+so feel free to use all the fancy RST you want. Science fragments are placed in the same ``changelog/`` directory
+as other fragments, but are always called::
+
+  <PR NUMBER | +>.science[.<COUNTER>].rst
+
+In the case that a single pull request encapsulates the entirety of the scientific change then the first field should
+be that PR number (same as the normal CHANGELOG). If, however, there is not a simple mapping from a single PR to a scienctific
+change then use the character "+" instead; this will create a changelog entry with no associated PR. For example:
+
+.. code-block:: bash
+
+  $ ls changelog/
+  99.bugfix.rst    # This is a normal changelog fragment associated with a bugfix in PR 99
+  99.science.rst   # Apparently that bugfix also changed the scientific results, so that PR also gets a science fragment
+  +.science.rst    # This fragment is not associated with a PR
+
+
+When it comes time to build the SCIENCE_CHANGELOG, use the ``science_towncrier.sh`` script in this repo to do so.
+This script accepts all the same arguments as the default `towncrier`. For exmaple:
+
+.. code-block:: bash
+
+  ./science_towncrier.sh build --version vx.y.z
+
+This will update the SCIENCE_CHANGELOG and remove any science fragments from the changelog directory.
```

### Comparing `dkist_processing_vbi-1.1.9/README.rst` & `dkist_processing_vbi-1.2.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -91,7 +91,38 @@
     # Delete tags
     git tag -d vWHATEVER.THE.VERSION
     git push --delete origin vWHATEVER.THE.VERSION
 
     # Re-tag with the same version
     git tag vWHATEVER.THE.VERSION
     git push --tags origin main
+
+Science Changelog
+^^^^^^^^^^^^^^^^^
+
+Whenever a release involves changes to the scientific quality of L1 data, additional changelog fragment(s) should be
+created. These fragments are intended to be as verbose as is needed to accurately capture the scope of the change(s),
+so feel free to use all the fancy RST you want. Science fragments are placed in the same ``changelog/`` directory
+as other fragments, but are always called::
+
+  <PR NUMBER | +>.science[.<COUNTER>].rst
+
+In the case that a single pull request encapsulates the entirety of the scientific change then the first field should
+be that PR number (same as the normal CHANGELOG). If, however, there is not a simple mapping from a single PR to a scienctific
+change then use the character "+" instead; this will create a changelog entry with no associated PR. For example:
+
+.. code-block:: bash
+
+  $ ls changelog/
+  99.bugfix.rst    # This is a normal changelog fragment associated with a bugfix in PR 99
+  99.science.rst   # Apparently that bugfix also changed the scientific results, so that PR also gets a science fragment
+  +.science.rst    # This fragment is not associated with a PR
+
+
+When it comes time to build the SCIENCE_CHANGELOG, use the ``science_towncrier.sh`` script in this repo to do so.
+This script accepts all the same arguments as the default `towncrier`. For exmaple:
+
+.. code-block:: bash
+
+  ./science_towncrier.sh build --version vx.y.z
+
+This will update the SCIENCE_CHANGELOG and remove any science fragments from the changelog directory.
```

### Comparing `dkist_processing_vbi-1.1.9/bitbucket-pipelines.yml` & `dkist_processing_vbi-1.2.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/check_changelog_updated.sh` & `dkist_processing_vbi-1.2.0/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/constants.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/models/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 
 from dkist_processing_common.models.constants import ConstantsBase
 
 
 class VbiBudName(Enum):
     """Names to be used in VBI buds."""
 
-    dsps_repeat_pedestal = "DSPS_REPEAT_PEDESTAL"
+    num_mosaics_repeats = "NUM_MOSAIC_REPEATS"
     num_spatial_steps = "NUM_SPATIAL_STEPS"
-    num_exp_per_dsp = "NUM_EXP_PER_DSP"
     gain_exposure_times = "GAIN_EXPOSURE_TIMES"
     observe_exposure_times = "OBSERVE_EXPOSURE_TIMES"
 
 
 class VbiConstants(ConstantsBase):
     """VBI specific constants to add to the common constants."""
 
     @property
-    def dsps_repeat_pedestal(self) -> int:
-        """Minimum value of all DSPS repeat header values."""
-        return self._db_dict[VbiBudName.dsps_repeat_pedestal.value]
+    def num_mosaic_repeats(self) -> int:
+        """Return the number of times the full mosaic is repeated."""
+        return self._db_dict[VbiBudName.num_mosaics_repeats.value]
 
     @property
     def num_spatial_steps(self) -> int:
         """Spatial steps in a raster."""
         return self._db_dict[VbiBudName.num_spatial_steps.value]
 
     @property
@@ -32,13 +31,7 @@
         """Exposure times of gain frames."""
         return self._db_dict[VbiBudName.gain_exposure_times.value]
 
     @property
     def observe_exposure_times(self) -> [float]:
         """Exposure times of observe frames."""
         return self._db_dict[VbiBudName.observe_exposure_times.value]
-
-    @property
-    def num_exp_per_dsp(self) -> int:
-        """Exposures per DSP."""
-        # This might never be used?
-        return self._db_dict[VbiBudName.num_exp_per_dsp.value]
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/models/tags.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/models/tags.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dkist_processing_common.models.tags import Tag
 
 
 class VbiStemName(str, Enum):
     """VBI specific tag stems."""
 
     current_spatial_step = "STEP"
+    current_mosaic = "MOSAIC"
 
 
 class VbiTag(Tag):
     """VBI specific tag formatting."""
 
     @classmethod
     def spatial_step(cls, step_num: int) -> str:
@@ -20,7 +21,12 @@
 
         Parameters
         ----------
         step_num: int
             The step number in the FOV
         """
         return cls.format_tag(VbiStemName.current_spatial_step, step_num)
+
+    @classmethod
+    def mosaic(cls, mosaic_num: int) -> str:
+        """Tags by mosaic number."""
+        return cls.format_tag(VbiStemName.current_mosaic, mosaic_num)
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/vbi_l0_fits_access.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/parsers/vbi_l0_fits_access.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,9 +27,9 @@
         name: str | None = None,
         auto_squeeze: bool = True,
     ):
         super().__init__(hdu=hdu, name=name, auto_squeeze=auto_squeeze)
 
         self.number_of_spatial_steps: int = self.header.get("VBINSTP")
         self.current_spatial_step: int = self.header.get("VBISTP")
-        self.number_of_exp_per_dsp: int = self.header.get("VBINFRAM")
-        self.current_dsp_exp: int = self.header.get("VBICFRAM")
+        self.number_of_exp_per_mosaic_step: int = self.header.get("VBINFRAM")
+        self.current_mosaic_step_exp: int = self.header.get("VBICFRAM")
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/parsers/vbi_l1_fits_access.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/parsers/vbi_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/assemble_movie.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/assemble_movie.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """VBI-specific assemble movie task subclass."""
+from typing import Type
+
 import numpy as np
 from astropy.visualization import ZScaleInterval
+from dkist_processing_common.models.constants import ConstantsBase
 from dkist_processing_common.tasks import AssembleMovie
 from matplotlib import cm
 from PIL import ImageDraw
 
+from dkist_processing_vbi.models.constants import VbiConstants
+from dkist_processing_vbi.models.tags import VbiTag
 from dkist_processing_vbi.parsers.vbi_l1_fits_access import VbiL1FitsAccess
 
 
 class AssembleVbiMovie(AssembleMovie):
     """
     Class for assembling pre-made movie frames (as FITS/numpy) into an mp4 movie file.
 
@@ -20,19 +25,36 @@
         id of the recipe run used to identify the workflow run this task is part of
     workflow_name : str
         name of the workflow to which this instance of the task belongs
     workflow_version : str
         version of the workflow to which this instance of the task belongs
     """
 
+    # So tab completion shows all the ViSP constants
+    constants: VbiConstants
+
+    @property
+    def constants_model_class(self) -> Type[ConstantsBase]:
+        """Class used to access constant database."""
+        return VbiConstants
+
     @property
     def fits_parsing_class(self):
         """VBI specific subclass of L1FitsAccess to use for reading images."""
         return VbiL1FitsAccess
 
+    @property
+    def num_images(self) -> int:
+        """Total number of images in final movie."""
+        return self.constants.num_mosaic_repeats
+
+    def tags_for_image_n(self, n: int) -> list[str]:
+        """Return the tags needed to find image n."""
+        return [VbiTag.mosaic(n + 1)]
+
     def apply_colormap(self, array: np.ndarray) -> np.ndarray:
         """
         Convert floats to RGB colors using the ZScale normalization scheme.
 
         Parameters
         ----------
         array : np.ndarray
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/dark.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/dark.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """VBI dark calibration task."""
-import logging
-
 from astropy.io import fits
 from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.statistics import average_numpy_arrays
+from logging42 import logger
 
 from dkist_processing_vbi.models.tags import VbiTag
 from dkist_processing_vbi.parsers.vbi_l0_fits_access import VbiL0FitsAccess
 from dkist_processing_vbi.tasks.vbi_base import VbiTaskBase
 
 
 class DarkCalibration(VbiTaskBase, FitsDataMixin, QualityMixin):
@@ -40,22 +39,22 @@
         -------
         None
 
         """
         target_exp_times = list(
             set(self.constants.gain_exposure_times + self.constants.observe_exposure_times)
         )
-        logging.info(f"{target_exp_times = }")
+        logger.info(f"{target_exp_times = }")
         with self.apm_task_step(
             f"Calculating dark frames for {self.constants.num_spatial_steps} steps and {len(target_exp_times)} exp times",
         ):
             total_dark_frames_used = 0
             for exp_time in target_exp_times:
                 for step in range(1, self.constants.num_spatial_steps + 1):
-                    logging.info(f"collecting dark frames for step {step}")
+                    logger.info(f"collecting dark frames for step {step}")
                     dark_tags = [
                         VbiTag.input(),
                         VbiTag.frame(),
                         VbiTag.task("DARK"),
                         VbiTag.spatial_step(step),
                         VbiTag.exposure_time(exp_time),
                     ]
@@ -68,24 +67,24 @@
                         cls=VbiL0FitsAccess,
                     )
                     input_dark_arrays = (obj.data for obj in input_dark_fits_access)
 
                     with self.apm_processing_step(
                         f"Processing dark for {step = } and {exp_time = }"
                     ):
-                        logging.info(f"averaging arrays for step {step}")
+                        logger.info(f"averaging arrays for step {step}")
                         averaged_dark_array = average_numpy_arrays(input_dark_arrays)
-                        logging.info(
+                        logger.info(
                             f"average dark signal in step {step} = {averaged_dark_array.mean():.3e}"
                         )
 
                     with self.apm_writing_step(
                         f"Writing intermediate dark for {step = } and {exp_time = }",
                     ):
-                        logging.info(f"writing dark calibration for step {step}")
+                        logger.info(f"writing dark calibration for step {step}")
                         hdul = fits.HDUList([fits.PrimaryHDU(data=averaged_dark_array)])
                         self.fits_data_write(
                             hdu_list=hdul,
                             tags=[
                                 VbiTag.intermediate(),
                                 VbiTag.frame(),
                                 VbiTag.task("DARK"),
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/gain.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/gain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """VBI gain task."""
-import logging
-
 import numpy as np
 from astropy.io import fits
 from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
+from logging42 import logger
 
 from dkist_processing_vbi.models.tags import VbiTag
 from dkist_processing_vbi.parsers.vbi_l0_fits_access import VbiL0FitsAccess
 from dkist_processing_vbi.tasks.mixin.intermediate_loaders import IntermediateLoaderMixin
 from dkist_processing_vbi.tasks.vbi_base import VbiTaskBase
 
 
@@ -53,49 +52,49 @@
         step_gain_dict: dict = {}
 
         with self.apm_processing_step(
             f"Collecting and reducing gain arrays from {self.constants.num_spatial_steps} steps and {len(self.constants.gain_exposure_times)} exp times",
         ):
             for exp_time in self.constants.gain_exposure_times:
                 for step in range(1, self.constants.num_spatial_steps + 1):
-                    logging.info(f"retrieving dark frame step {step} and {exp_time = }")
+                    logger.info(f"retrieving dark frame step {step} and {exp_time = }")
                     try:
                         dark_calibration_array = self.intermediate_dark_array(
                             spatial_step=step, exposure_time=exp_time
                         )
                     except StopIteration:
                         raise ValueError(f"No matching dark found for {exp_time = }")
 
-                    logging.info(f"collecting gain frames for {step = }")
+                    logger.info(f"collecting gain frames for {step = }")
                     input_gain_access = self.fits_data_read_fits_access(
                         tags=[
                             VbiTag.input(),
                             VbiTag.frame(),
                             VbiTag.spatial_step(step),
                             VbiTag.task("GAIN"),
                             VbiTag.exposure_time(exp_time),
                         ],
                         cls=VbiL0FitsAccess,
                     )
                     input_gain_arrays = (obj.data for obj in input_gain_access)
 
-                    logging.info(f"averaging arrays from {step = }")
+                    logger.info(f"averaging arrays from {step = }")
                     averaged_gain_array = average_numpy_arrays(input_gain_arrays)
-                    logging.info(
+                    logger.info(
                         f"average raw gain signal in step {step} = {averaged_gain_array.mean():.3e}"
                     )
 
-                    logging.info(f"subtracting dark from average gain for {step = }")
+                    logger.info(f"subtracting dark from average gain for {step = }")
                     dark_subtracted_gain_array = next(
                         subtract_array_from_arrays(
                             arrays=averaged_gain_array, array_to_subtract=dark_calibration_array
                         )
                     )
 
-                    logging.info(f"Recording processed gain image for {step = }")
+                    logger.info(f"Recording processed gain image for {step = }")
                     self.total_non_nan_pix += np.sum(~np.isnan(dark_subtracted_gain_array))
                     self.total_counts += np.nansum(dark_subtracted_gain_array)
                     step_gain_dict[step] = dark_subtracted_gain_array
 
         with self.apm_processing_step("normalizing gain arrays"):
             normalized_array_dict = self.normalize_fov(step_gain_dict)
 
@@ -125,15 +124,15 @@
 
         Returns
         -------
         Dict
             Dict of FOV normalized gain arrays
         """
         fov_mean = self.total_counts / self.total_non_nan_pix
-        logging.info(f"full FOV mean = {fov_mean:.3e}")
+        logger.info(f"full FOV mean = {fov_mean:.3e}")
         for k in step_gain_dict:
             step_gain_dict[k] = step_gain_dict[k] / fov_mean
 
         return step_gain_dict
 
     def write_gain_calibration(self, gain_array_dict: dict[int, np.ndarray]) -> None:
         """
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/make_movie_frames.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/make_movie_frames.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """VBI movie frame creation."""
-import logging
-
 import numpy as np
 import scipy.ndimage as spnd
 from astropy.io import fits
 from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
 from dkist_processing_math.statistics import average_numpy_arrays
+from logging42 import logger
 
 from dkist_processing_vbi.models.tags import VbiTag
 from dkist_processing_vbi.parsers.vbi_l1_fits_access import VbiL1FitsAccess
 from dkist_processing_vbi.tasks.vbi_base import VbiTaskBase
 
 
 class MakeVbiMovieFrames(VbiTaskBase, FitsDataMixin):
@@ -24,126 +23,128 @@
         name of the workflow to which this instance of the task belongs
     workflow_version : str
         version of the workflow to which this instance of the task belongs
     """
 
     def run(self) -> None:
         """
-        For each dsps repeat.
+        For each mosaic repeat.
 
           - Average all exposures for each spatial step
           - Stitch spatial positions into a full-FOV array
           - Write full FOV as a move_frame
 
         Returns
         -------
         None
 
         """
         with self.apm_processing_step("averaging exposures"):
             self.average_all_exposures()
 
         with self.apm_processing_step("stitching full FOV frames"):
-            for drep in range(1, self.constants.num_dsps_repeats + 1):
-                logging.info(f"stitching full FOV for dsps repeat {drep}")
-                output_hdl = self.stitch_single_dsps_repeat(drep)
-
-                with self.apm_writing_step(f"writing stitched movie frame for dsps repeat {drep}"):
-                    logging.info(f"writing stitched movie frame for dsps repeat {drep}")
+            for mosaic in range(1, self.constants.num_mosaic_repeats + 1):
+                logger.info(f"stitching full FOV for mosaic repeat {mosaic}")
+                output_hdl = self.stitch_single_mosaic_repeat(mosaic)
+
+                with self.apm_writing_step(
+                    f"writing stitched movie frame for mosaic repeat {mosaic}"
+                ):
+                    logger.info(f"writing stitched movie frame for mosaic repeat {mosaic}")
                     self.fits_data_write(
-                        hdu_list=output_hdl, tags=[VbiTag.movie_frame(), VbiTag.dsps_repeat(drep)]
+                        hdu_list=output_hdl, tags=[VbiTag.movie_frame(), VbiTag.mosaic(mosaic)]
                     )
 
     def average_all_exposures(self):
-        """For each spatial step and each dsps repeat, average all exposures into a single frame."""
+        """For each spatial step and each mosaic repeat, average all exposures into a single frame."""
         for step in range(1, self.constants.num_spatial_steps + 1):
-            for drep in range(1, self.constants.num_dsps_repeats + 1):
-                apm_str = f"step {step} and repeat number {drep}"
+            for mosaic in range(1, self.constants.num_mosaic_repeats + 1):
+                apm_str = f"step {step} and repeat number {mosaic}"
 
-                logging.info(f"averaging exposures for {apm_str}")
+                logger.info(f"averaging exposures for {apm_str}")
                 output_hdu_generator = self.fits_data_read_hdu(
                     tags=[
                         VbiTag.output(),
                         VbiTag.frame(),
                         VbiTag.spatial_step(step),
-                        VbiTag.dsps_repeat(drep),
+                        VbiTag.mosaic(mosaic),
                     ]
                 )
 
                 # We're doing it with a list right now to save having to construct a second generator just to get
                 # the first header. This may need to change if LOTS of exposures are taken.
                 output_hdus = [tup[1] for tup in output_hdu_generator]
                 # We're still keeping the data access in a generator, though
                 output_arrays = (h.data for h in output_hdus)
                 averaged_frame = average_numpy_arrays(output_arrays)
                 first_header = output_hdus[0].header
 
-                logging.info(f"writing averaged data for {apm_str}")
+                logger.info(f"writing averaged data for {apm_str}")
                 self.fits_data_write(
                     hdu_list=fits.HDUList(
                         [fits.PrimaryHDU(data=averaged_frame, header=first_header)]
                     ),
                     tags=[
                         VbiTag.intermediate(),
                         VbiTag.task("AVG_MOVIE_FRAME"),
                         VbiTag.spatial_step(step),
-                        VbiTag.dsps_repeat(drep),
+                        VbiTag.mosaic(mosaic),
                     ],
                 )
 
-    def stitch_single_dsps_repeat(self, dsps_repeat: int) -> fits.HDUList:
+    def stitch_single_mosaic_repeat(self, mosaic_repeat: int) -> fits.HDUList:
         """
-        Take all spatial positions from a single dsps and stitch them together into a full FOV.
+        Take all spatial positions from a single mosaic and stitch them together into a full FOV.
 
         Each spatial position's location within the full FOV is determined via WCS header information. Overlap regions
         are simply averaged together.
 
         Parameters
         ----------
-        dsps_repeat : int
+        mosaic_repeat : int
              The current dataset parameters repeat
 
         Returns
         -------
         fits.HDUList
             Full FOV HDUList
         """
         # noinspection PyTypeChecker
         all_step_access: list[VbiL1FitsAccess] = list(
             self.fits_data_read_fits_access(
                 tags=[
                     VbiTag.intermediate(),
                     VbiTag.task("AVG_MOVIE_FRAME"),
-                    VbiTag.dsps_repeat(dsps_repeat),
+                    VbiTag.mosaic(mosaic_repeat),
                 ],
                 cls=VbiL1FitsAccess,
             )
         )
 
         if len(all_step_access) != self.constants.num_spatial_steps:
             raise ValueError(
-                f"Found {len(all_step_access)} spatial positions instead of {self.constants.num_spatial_steps} for {dsps_repeat=}"
+                f"Found {len(all_step_access)} spatial positions instead of {self.constants.num_spatial_steps} for {mosaic_repeat=}"
             )
 
         ref_pos = self.find_ref_pos(all_step_access)
-        logging.info(f"reference position automatically determined to be {ref_pos}")
+        logger.info(f"reference position automatically determined to be {ref_pos}")
         ref_header = [o.header for o in all_step_access if o.header["VBISTP"] == ref_pos][0]
 
         # We get weird with the order of axes here. This is because we want to create frames that "look right" in ds9
         # The names used here in the code will always correspond to numpy ordering, but their order will change.
         size_x, size_y = self.get_fov_size(all_step_access, ref_header)
-        logging.info(f"size of stitched output array: ({size_x}, {size_y})")
+        logger.info(f"size of stitched output array: ({size_x}, {size_y})")
         output = np.zeros((size_y, size_x))
         px_count = np.zeros((size_y, size_x))
 
         with self.apm_processing_step(
-            f"stitching all camera positions together for {dsps_repeat=}"
+            f"stitching all camera positions together for {mosaic_repeat=}"
         ):
             for o in all_step_access:
-                logging.info(f"Placing position {o.current_spatial_step} into full frame")
+                logger.info(f"Placing position {o.current_spatial_step} into full frame")
                 self.place_pos_in_full_fov(o, ref_header, output, px_count)
 
         # Normalize by the number of overlapping pixels and the Hanning weights
         non_zero_idx = np.where(px_count != 0)
         output[non_zero_idx] /= px_count[non_zero_idx]
 
         hdl = fits.HDUList([fits.PrimaryHDU(data=px_count)])
@@ -168,40 +169,40 @@
 
             For both frames we'll say CRVAL is 6. This implies that frame 1 has CRPIX = 4, while frame 2 has CRPIX = 1.
             Thus we can see that the largest CRPIX corresponds to the smallest extent of the WCS coords.
 
         Parameters
         ----------
         access_list
-            list of VBI intermediate movie frames for a single dsps repeat
+            list of VBI intermediate movie frames for a single mosaic repeat
 
 
         Returns
         -------
         int
             spatial position with the smallest wcs coordinates
 
         """
         rpix_list = [o.header["CRPIX1"] ** 2 + o.header["CRPIX2"] ** 2 for o in access_list]
-        logging.info(f"{rpix_list=}")
-        logging.info(f"positions={[o.header['VBISTP'] for o in access_list]}")
+        logger.info(f"{rpix_list=}")
+        logger.info(f"positions={[o.header['VBISTP'] for o in access_list]}")
         ref_idx = np.argmax(rpix_list)
 
         return access_list[ref_idx].header["VBISTP"]
 
     def get_fov_size(
         self, access_list: list[VbiL1FitsAccess], ref_header: fits.Header
     ) -> tuple[int, int]:
         """
         Look at the WCS information for all spatial positions and determine the array size needed to just contain all pixels in the FOV.
 
         Parameters
         ----------
         access_list
-            list of VBI intermediate movie frames for a single dsps repeat
+            list of VBI intermediate movie frames for a single mosaic repeat
 
         ref_header
             reference header used for normalization factors
 
         Returns
         -------
         2D FOV size (x, y)
@@ -274,15 +275,15 @@
         px_count : np.ndarray
             pixel count
 
         Returns
         -------
         None
         """
-        # See the note in stitch_single_dsps_repeat() about the transposition of x and y coordinates.
+        # See the note in stitch_single_mosaic_repeat() about the transposition of x and y coordinates.
         # tl;dr: it's because ds9 and numpy aren't the same when it comes to [row|column] major.
         size_x, size_y = output.shape
         data = access_obj.data
         small_size_y, small_size_x = [int(s) for s in data.shape]
         counts = np.ones((small_size_y, small_size_x))
         counts[np.where(data == 0)] = 0
 
@@ -300,17 +301,17 @@
             y_shift = 0
         if 1 - x_shift < 1e-4:
             x_shift = 0
             x_pos += 1
         if 1 - y_shift < 1e-4:
             y_shift = 0
             y_pos += 1
-        logging.info(f"[x,y] location of first px in output coordinate space: [{x_pos}, {y_pos}]")
-        logging.info(f"[x,y] shift values: [{x_shift}, {y_shift}]")
-        logging.info(f"shape of input data: {data.shape}")
+        logger.info(f"[x,y] location of first px in output coordinate space: [{x_pos}, {y_pos}]")
+        logger.info(f"[x,y] shift values: [{x_shift}, {y_shift}]")
+        logger.info(f"shape of input data: {data.shape}")
 
         data[~np.isfinite(data)] = np.max(data[np.isfinite(data)])
         shifted = spnd.shift(data, (x_shift, y_shift))
         counts = spnd.shift(counts, (x_shift, y_shift))
 
         x_min = int(x_pos)
         y_min = int(y_pos)
@@ -331,19 +332,19 @@
             counts = counts[: size_y - y_max, :]
             y_max = size_y
         if x_max > size_x:
             shifted = shifted[:, : size_x - x_max]
             counts = counts[:, : size_x - x_max]
             x_max = size_x
 
-        logging.info(f"output slice: [{y_min}:{y_max}, {x_min}:{x_max}]")
-        logging.info(f"shape of shifted data: {shifted.shape}")
-        logging.info(f"shape of output slice: {output[y_min:y_max, x_min:x_max].shape}")
+        logger.info(f"output slice: [{y_min}:{y_max}, {x_min}:{x_max}]")
+        logger.info(f"shape of shifted data: {shifted.shape}")
+        logger.info(f"shape of output slice: {output[y_min:y_max, x_min:x_max].shape}")
 
-        logging.info("Applying Hann window to output")
+        logger.info("Applying Hann window to output")
         # This is purely aesthetic; it removes hard edges along the mosaic stitch lines
         #   why those edges are there at all? I have no idea.
 
         # Method for 2D Hann from
         # https://stackoverflow.com/questions/65940166/create-2d-hanning-hamming-blackman-gaussian-window-in-numpy
         hann_x = np.abs(np.hanning(shifted.shape[0]))
         hann_y = np.abs(np.hanning(shifted.shape[1]))
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/parse.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/parse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 """VBI parse task."""
 from dkist_processing_common.models.tags import StemName
-from dkist_processing_common.parsers.dsps_repeat import DspsRepeatNumberFlower
-from dkist_processing_common.parsers.dsps_repeat import TotalDspsRepeatsBud
 from dkist_processing_common.parsers.single_value_single_key_flower import (
     SingleValueSingleKeyFlower,
 )
 from dkist_processing_common.parsers.time import ExposureTimeFlower
 from dkist_processing_common.parsers.time import TaskExposureTimesBud
 from dkist_processing_common.parsers.unique_bud import UniqueBud
 from dkist_processing_common.tasks import ParseL0InputData
 from dkist_processing_common.tasks.parse_l0_input_data import S
 
 from dkist_processing_vbi.models.constants import VbiBudName
 from dkist_processing_vbi.models.tags import VbiStemName
-from dkist_processing_vbi.parsers.dsps_repeats import VbiDspsRepeatNumberFlower
-from dkist_processing_vbi.parsers.dsps_repeats import VbiDspsRepeatPedestalBud
-from dkist_processing_vbi.parsers.dsps_repeats import VbiTotalDspsRepeatsBud
-from dkist_processing_vbi.parsers.num_exp_per_dsp import NumExpPerDspBud
-from dkist_processing_vbi.parsers.spectral_line import SpectralLineBud
+from dkist_processing_vbi.parsers.mosaic_repeats import MosaicRepeatNumberFlower
+from dkist_processing_vbi.parsers.mosaic_repeats import TotalMosaicRepeatsBud
 from dkist_processing_vbi.parsers.vbi_l0_fits_access import VbiL0FitsAccess
 
 
 class ParseL0VbiInputData(ParseL0InputData):
     """
     Parse input VBI data.
 
@@ -47,18 +42,15 @@
     def constant_flowers(self) -> list[S]:
         """VBI specific constants to append to the common constants."""
         return super().constant_flowers + [
             UniqueBud(
                 constant_name=VbiBudName.num_spatial_steps.value,
                 metadata_key="number_of_spatial_steps",
             ),
-            VbiTotalDspsRepeatsBud(),
-            VbiDspsRepeatPedestalBud(),
-            SpectralLineBud(),
-            NumExpPerDspBud(),
+            TotalMosaicRepeatsBud(),
             TaskExposureTimesBud(VbiBudName.gain_exposure_times.value, ip_task_type="GAIN"),
             TaskExposureTimesBud(VbiBudName.observe_exposure_times.value, ip_task_type="OBSERVE"),
         ]
 
     @property
     def tag_flowers(self) -> list[S]:
         """VBI specific tags to append to the common tags."""
@@ -66,10 +58,10 @@
             SingleValueSingleKeyFlower(
                 tag_stem_name=VbiStemName.current_spatial_step.value,
                 metadata_key="current_spatial_step",
             ),
             SingleValueSingleKeyFlower(
                 tag_stem_name=StemName.task.value, metadata_key="ip_task_type"
             ),
-            VbiDspsRepeatNumberFlower(),
+            MosaicRepeatNumberFlower(),
             ExposureTimeFlower(),
         ]
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/process_summit_processed.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/quality_metrics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,64 @@
-"""Repackage VBI data already calibrated before receipt at the Data Center."""
-import logging
-
-from dkist_processing_common.tasks import WorkflowTaskBase
+"""VBI specific quality metrics."""
+from dkist_processing_common.parsers.quality import L1QualityFitsAccess
 from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
+from dkist_processing_common.tasks.mixin.quality import QualityMixin
+from dkist_processing_common.tasks.quality_metrics import QualityL0Metrics
 
 from dkist_processing_vbi.models.tags import VbiTag
+from dkist_processing_vbi.tasks.vbi_base import VbiTaskBase
 
 
-class GenerateL1SummitData(WorkflowTaskBase, FitsDataMixin):
+class VbiQualityL0Metrics(QualityL0Metrics):
     """
-    Task class for updating the headers of on-summit processed VBI data.
+    Task class for collecting VBI L0 quality metrics.
 
     Parameters
     ----------
     recipe_run_id : int
         id of the recipe run used to identify the workflow run this task is part of
     workflow_name : str
         name of the workflow to which this instance of the task belongs
     workflow_version : str
         version of the workflow to which this instance of the task belongs
 
     """
 
-    record_provenance = True
-
     def run(self) -> None:
-        """
-        For all input frames.
+        """Calculate L0 metrics for VBI data."""
+        paths = self.read(tags=[VbiTag.input()])
+        self.calculate_l0_metrics(paths=paths)
+
+
+class VbiQualityL1Metrics(VbiTaskBase, QualityMixin, FitsDataMixin):
+    """
+    Task class for collecting VBI L1 quality metrics.
+
+    Parameters
+    ----------
+    recipe_run_id : int
+        id of the recipe run used to identify the workflow run this task is part of
+    workflow_name : str
+        name of the workflow to which this instance of the task belongs
+    workflow_version : str
+        version of the workflow to which this instance of the task belongs
+
+    """
+
+    def run(self):
+        """Calculate L1 metrics for VBI data."""
+        frames = self.fits_data_read_fits_access(
+            tags=[
+                VbiTag.output(),
+                VbiTag.frame(),
+            ],
+            cls=L1QualityFitsAccess,
+        )
+        datetimes = []
+        noise_values = []
+        with self.apm_processing_step("Calculating VBI L1 quality metrics"):
+            for frame in frames:
+                datetimes.append(frame.time_obs)
+                noise_values.append(self.avg_noise(frame.data))
 
-            - Add data-dependent SPEC-0214 headers
-            - Write out
-        """
-        # This loop is how we ensure that only completed mosaics get processed.
-        with self.apm_task_step("Re-tagging INPUT observe frames as CALIBRATED"):
-            for dsps_num in range(1, self.constants.num_dsps_repeats + 1):
-                for file_name in self.read(
-                    tags=[
-                        VbiTag.input(),
-                        VbiTag.frame(),
-                        VbiTag.task("Observe"),
-                        VbiTag.dsps_repeat(dsps_num),
-                    ]
-                ):
-                    self.remove_tags(file_name, VbiTag.input())
-                    new_tags = [VbiTag.calibrated(), VbiTag.stokes("I")]
-                    self.tag(file_name, tags=new_tags)  # Tags are additive
-                    logging.debug(f"Tags after tagging are {self.tags(file_name)}")
+        with self.apm_processing_step("Sending lists for storage"):
+            self.quality_store_noise(datetimes=datetimes, values=noise_values)
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/science.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/science.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """VBI science task."""
-import logging
-
 from astropy.io import fits
 from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import divide_fits_access_by_array
 from dkist_processing_math.arithmetic import subtract_array_from_fits_access
+from logging42 import logger
 
 from dkist_processing_vbi.models.tags import VbiTag
 from dkist_processing_vbi.parsers.vbi_l0_fits_access import VbiL0FitsAccess
 from dkist_processing_vbi.tasks.mixin.intermediate_loaders import IntermediateLoaderMixin
 from dkist_processing_vbi.tasks.vbi_base import VbiTaskBase
 
 
@@ -38,85 +37,89 @@
         - Record quality metrics
 
         Returns
         -------
         None
 
         """
-        logging.info(
-            f"Starting science with {self.constants.num_spatial_steps} steps and {self.constants.num_dsps_repeats} repeats"
+        logger.info(
+            f"Starting science with {self.constants.num_spatial_steps} steps and {self.constants.num_mosaic_repeats} mosaic repeats"
         )
         with self.apm_task_step(
-            f"Reducing science frames from {self.constants.num_spatial_steps} steps and {self.constants.num_dsps_repeats} repeats",
+            f"Reducing science frames from {self.constants.num_spatial_steps} steps and {self.constants.num_mosaic_repeats} mosaic repeats",
         ):
             for exp_time in self.constants.observe_exposure_times:
                 for step in range(1, self.constants.num_spatial_steps + 1):
-                    logging.info(f"retrieving dark calibration for step {step} and {exp_time = }")
+                    logger.info(f"retrieving dark calibration for step {step} and {exp_time = }")
                     dark_calibration_array = self.intermediate_dark_array(
                         spatial_step=step, exposure_time=exp_time
                     )
 
-                    logging.info(f"retrieving gain calibration for step {step}")
+                    logger.info(f"retrieving gain calibration for step {step}")
                     gain_calibration_array = self.intermediate_gain_array(spatial_step=step)
 
-                    for drep in range(1, self.constants.num_dsps_repeats + 1):
-                        apm_str = f"step {step} and repeat number {drep}"
-                        logging.info(f"collecting observe frames for {apm_str}")
+                    for mosaic in range(1, self.constants.num_mosaic_repeats + 1):
+                        apm_str = f"step {step} and repeat number {mosaic}"
+                        logger.info(f"collecting observe frames for {apm_str}")
                         sci_access = self.fits_data_read_fits_access(
                             tags=[
                                 VbiTag.input(),
                                 VbiTag.frame(),
                                 VbiTag.task("OBSERVE"),
-                                VbiTag.dsps_repeat(drep),
+                                VbiTag.mosaic(mosaic),
                                 VbiTag.spatial_step(step),
                                 VbiTag.exposure_time(exp_time),
                             ],
                             cls=VbiL0FitsAccess,
                         )
 
                         with self.apm_processing_step("dark and gain corrections"):
-                            logging.info(f"subtracting dark from {apm_str}")
+                            logger.info(f"subtracting dark from {apm_str}")
                             sci_access = subtract_array_from_fits_access(
                                 access_objs=sci_access, array_to_subtract=dark_calibration_array
                             )
 
-                            logging.info(f"dividing gain from {apm_str}")
+                            logger.info(f"dividing gain from {apm_str}")
                             sci_access = divide_fits_access_by_array(
                                 access_objs=sci_access, array_to_divide_by=gain_calibration_array
                             )
 
                         with self.apm_writing_step("writing calibrated science frames"):
                             for i, access_obj in enumerate(sci_access):
-                                exp_num = access_obj.current_dsp_exp
-                                processed_hdu_list = fits.HDUList(
-                                    [
-                                        fits.PrimaryHDU(),
-                                        fits.CompImageHDU(
-                                            data=access_obj.data, header=access_obj.header
-                                        ),
-                                    ]
-                                )
-
-                                logging.info(f"Writing output for {apm_str} and {exp_num = }")
-                                # It was an intentional decision to not tag with exposure time here
-                                self.fits_data_write(
-                                    processed_hdu_list,
-                                    tags=[
-                                        VbiTag.calibrated(),
-                                        VbiTag.frame(),
-                                        VbiTag.spatial_step(step),
-                                        VbiTag.dsps_repeat(drep),
-                                        VbiTag.stokes("I"),
-                                    ],
-                                )
+                                exp_num = access_obj.current_mosaic_step_exp
+                                logger.info(f"Writing output for {apm_str} and {exp_num = }")
+                                self.write_calibrated_fits_obj(access_obj, mosaic, step)
 
         with self.apm_processing_step("Computing and logging quality metrics"):
             no_of_raw_obs_frames: int = self.count(
                 tags=[
                     VbiTag.input(),
                     VbiTag.frame(),
                     VbiTag.task("OBSERVE"),
                 ],
             )
             self.quality_store_task_type_counts(
                 task_type="observe", total_frames=no_of_raw_obs_frames
             )
+
+    def write_calibrated_fits_obj(self, fits_obj: VbiL0FitsAccess, mosaic: int, step: int) -> None:
+        """Write a VbiL0FitsAccess object containing a calibrated array to disk and tag correctly.
+
+        Also update the header with necessary mosaic information.
+        """
+        processed_hdu_list = fits.HDUList(
+            [fits.PrimaryHDU(), fits.CompImageHDU(data=fits_obj.data, header=fits_obj.header)]
+        )
+        processed_hdu_list[1].header["VBINMOSC"] = self.constants.num_mosaic_repeats
+        processed_hdu_list[1].header["VBICMOSC"] = mosaic
+
+        # It is an intentional decision to not tag with exposure time here
+        self.fits_data_write(
+            processed_hdu_list,
+            tags=[
+                VbiTag.calibrated(),
+                VbiTag.frame(),
+                VbiTag.spatial_step(step),
+                VbiTag.mosaic(mosaic),
+                VbiTag.stokes("I"),
+            ],
+        )
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/vbi_base.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/vbi_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,11 +17,14 @@
     workflow_name : str
         name of the workflow to which this instance of the task belongs
     workflow_version : str
         version of the workflow to which this instance of the task belongs
 
     """
 
+    # So tab completion shows all the ViSP constants
+    constants: VbiConstants
+
     @property
     def constants_model_class(self):
         """Provide VBI constants access."""
         return VbiConstants
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tasks/write_l1.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tasks/write_l1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """VBI Write L1 task."""
 from typing import Literal
 from typing import Type
 
+import astropy.units as u
 import numpy as np
 from astropy.io import fits
 from astropy.time import Time
 from astropy.time import TimeDelta
 from dkist_processing_common.models.constants import ConstantsBase
+from dkist_processing_common.tasks.write_l1 import WavelengthRange
 from dkist_processing_common.tasks.write_l1 import WriteL1Frame
 
 from dkist_processing_vbi.models.constants import VbiConstants
-from dkist_processing_vbi.models.spectral_line import VBI_SPECTRAL_LINES
+from dkist_processing_vbi.models.filter import find_associated_filter
 
 
 class VbiWriteL1Frame(WriteL1Frame):
     """
     Task class for writing out calibrated L1 VBI frames.
 
     Parameters
@@ -67,32 +69,25 @@
         header["DTYPE2"] = "SPATIAL"
         header["DPNAME2"] = "helioprojective longitude"
         header["DWNAME2"] = "helioprojective longitude"
         header["DUNIT2"] = header["CUNIT2"]
 
         # ---Temporal---
         num_exp_per_dsp = header["VBINFRAM"]
-        header["DNAXIS3"] = self.constants.num_dsps_repeats * num_exp_per_dsp
+        header["DNAXIS3"] = self.constants.num_mosaic_repeats * num_exp_per_dsp
         header["DTYPE3"] = "TEMPORAL"
         header["DPNAME3"] = "time"
         header["DWNAME3"] = "time"
         header["DUNIT3"] = "s"
         # Temporal position in dataset
-        current_dsps_repeat = header["DSPSNUM"]
+        current_mosaic_number = header["VBICMOSC"]
         current_exposure = header["VBICFRAM"]
-        header["DINDEX3"] = (
-            current_dsps_repeat - 1 - self.constants.dsps_repeat_pedestal
-        ) * num_exp_per_dsp + current_exposure
+        header["DINDEX3"] = (current_mosaic_number - 1) * num_exp_per_dsp + current_exposure
 
         # ---Wavelength Info---
-        # Do we need to check that this has length == 1?
-        spectral_line = [l for l in VBI_SPECTRAL_LINES if l.name == self.constants.spectral_line][0]
-        header["WAVEMIN"] = spectral_line.wavemin
-        header["WAVEMAX"] = spectral_line.wavemax
-        header["WAVEBAND"] = spectral_line.name
         header["WAVEUNIT"] = -9  # nanometers
         header["WAVEREF"] = "Air"
 
         # --- Mosaic ---
         number_of_spatial_steps = int(header["VBINSTP"])
         current_step = int(header["VBISTP"])
         axis_length = int(np.sqrt(number_of_spatial_steps))
@@ -132,7 +127,16 @@
         -------
         The isot formatted string of the DATE-END keyword value
         """
         return (
             Time(header["DATE-BEG"], format="isot", precision=6)
             + TimeDelta(float(header["TEXPOSUR"]) / 1000, format="sec")
         ).to_value("isot")
+
+    def get_wavelength_range(self, header: fits.Header) -> WavelengthRange:
+        """
+        Return the wavelength range of this frame.
+
+        Range is the wavelengths at the edges of the filter bandpass.
+        """
+        vbi_filter = find_associated_filter(wavelength=header["LINEWAV"] * u.nm)
+        return WavelengthRange(min=vbi_filter.min, max=vbi_filter.max)
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/conftest.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,43 +16,42 @@
 
 
 @pytest.fixture()
 def recipe_run_id():
     return randint(0, 99999)
 
 
-@pytest.fixture(scope="session")
-def DKIST009_offset() -> int:
-    return 1000
-
-
 class VbiS122Headers(Spec122Dataset):
     def __init__(
         self,
         array_shape: tuple[int, ...],
         num_steps: int = 4,
         num_exp_per_step: int = 1,
         num_dsps_repeats: int = 5,
+        num_mosaics_per_dsps_repeat: int = 1,
         time_delta: float = 10.0,
         instrument: str = "vbi",
         DKIST008_value: int | None = None,
         DKIST009_offset_value: int = 0,
     ):
         if DKIST008_value is None:
             DKIST008_value = num_dsps_repeats
-        dataset_shape = (num_exp_per_step * num_steps * num_dsps_repeats,) + array_shape[-2:]
+        dataset_shape = (
+            num_exp_per_step * num_steps * num_dsps_repeats * num_mosaics_per_dsps_repeat,
+        ) + array_shape[-2:]
         super().__init__(
             dataset_shape=dataset_shape,
             array_shape=array_shape,
             time_delta=time_delta,
             instrument=instrument,
         )
         self.num_steps = num_steps
         self.num_exp_per_step = num_exp_per_step
         self.num_dsps_repeats = num_dsps_repeats
+        self.num_mosaic_per_dsps_repeat = num_mosaics_per_dsps_repeat
         self.DKIST009_offset = DKIST009_offset_value
         self.add_constant_key("WAVELNTH", 656.282)
         self.add_constant_key("TELSCAN", "None")
         self.add_constant_key("ID___004")
         self.add_constant_key("ID___013")
         self.add_constant_key("CAM__001", "test")
         self.add_constant_key("CAM__002", "test")
@@ -96,15 +95,22 @@
 
     @key_function("VBI__008")
     def current_dsp_output(self, key: str) -> int:
         return (self.index % self.num_exp_per_step) + 1
 
     @key_function("DKIST009")
     def dsps_num(self, key: str) -> int:
-        return (self.index // (self.num_steps * self.num_exp_per_step)) + 1 + self.DKIST009_offset
+        return (
+            (
+                self.index
+                // (self.num_steps * self.num_exp_per_step * self.num_mosaic_per_dsps_repeat)
+            )
+            + 1
+            + self.DKIST009_offset
+        )
 
 
 class Vbi122DarkFrames(VbiS122Headers):
     def __init__(self, array_shape: tuple[int, ...], num_steps: int = 4, num_exp_per_step: int = 1):
         super().__init__(
             array_shape, num_steps=num_steps, num_exp_per_step=num_exp_per_step, num_dsps_repeats=1
         )
@@ -123,45 +129,49 @@
 
 class Vbi122ObserveFrames(VbiS122Headers):
     def __init__(
         self,
         array_shape: tuple[int, ...],
         num_steps: int = 4,
         num_exp_per_step: int = 1,
-        num_dsps_repeats: int = 5,
+        num_dsps_repeats: int = 1,
+        num_mosaics_per_dsps_repeat: int = 5,
         DKIST008_value: int | None = None,
         DKIST009_offset_value: int = 0,
     ):
         super().__init__(
             array_shape,
             num_steps=num_steps,
             num_exp_per_step=num_exp_per_step,
             num_dsps_repeats=num_dsps_repeats,
+            num_mosaics_per_dsps_repeat=num_mosaics_per_dsps_repeat,
             DKIST008_value=DKIST008_value,
             DKIST009_offset_value=DKIST009_offset_value,
         )
         self.add_constant_key("DKIST004", "observe")
         self.add_constant_key("ID___012", "EXPERIMENT ID")
 
 
 class Vbi122SummitObserveFrames(VbiS122Headers):
     def __init__(
         self,
         array_shape: tuple[int, ...],
         num_steps: int = 4,
         num_exp_per_step: int = 1,
         num_dsps_repeats: int = 1,
+        num_mosaics_per_dsps_repeat: int = 1,
         DKIST008_value: int | None = None,
         DKIST009_offset_value: int = 0,
     ):
         super().__init__(
             array_shape,
             num_steps=num_steps,
             num_exp_per_step=num_exp_per_step,
             num_dsps_repeats=num_dsps_repeats,
+            num_mosaics_per_dsps_repeat=num_mosaics_per_dsps_repeat,
             DKIST008_value=DKIST008_value,
             DKIST009_offset_value=DKIST009_offset_value,
         )
         self.add_constant_key("DKIST004", "observe")
         self.add_constant_key("VBI__005", "SpeckleImaging")
         self.add_constant_key("ID___012", "EXPERIMENT ID")
 
@@ -229,19 +239,16 @@
 
     return constants_maker
 
 
 @dataclass
 class VbiConstantsDb:
     INSTRUMENT: str = "VBI"
-    NUM_DSPS_REPEATS: int = 3
-    DSPS_REPEAT_PEDESTAL: int = 0
+    NUM_MOSAIC_REPEATS: int = 3
     NUM_SPATIAL_STEPS: int = 4
-    NUM_EXP_PER_DSP: int = 1
-    SPECTRAL_LINE: str = "VBI-Red H-alpha"
     DARK_EXPOSURE_TIMES: tuple[float, ...] = (0.01, 1.0, 100.0)
     GAIN_EXPOSURE_TIMES: tuple[float, ...] = (1.0,)
     OBSERVE_EXPOSURE_TIMES: tuple[float, ...] = (0.01,)
     AVERAGE_CADENCE: float = 10.0
     MINIMUM_CADENCE: float = 10.0
     MAXIMUM_CADENCE: float = 10.0
     VARIANCE_CADENCE: float = 0.0
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/grogu_test.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/grogu_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import argparse
 import json
-import logging
 import os
 import sys
 from pathlib import Path
 
 import numpy as np
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_header_validator import spec214_validator
 from dkist_processing_common.manual import ManualProcessing
 from dkist_processing_common.tasks import QualityL1Metrics
 from dkist_processing_common.tasks import WorkflowTaskBase
 from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
 from dkist_processing_common.tasks.mixin.metadata_store import MetadataStoreMixin
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
+from logging42 import logger
 
 from dkist_processing_vbi.models.tags import VbiTag
 from dkist_processing_vbi.parsers.vbi_l0_fits_access import VbiL0FitsAccess
 from dkist_processing_vbi.tasks.assemble_movie import AssembleVbiMovie
 from dkist_processing_vbi.tasks.dark import DarkCalibration
 from dkist_processing_vbi.tasks.gain import GainCalibration
 from dkist_processing_vbi.tasks.make_movie_frames import MakeVbiMovieFrames
@@ -33,51 +33,54 @@
 INV = False
 try:
     from dkist_inventory.asdf_generator import dataset_from_fits
 
     INV = True
 except ModuleNotFoundError:
     # Bitbucket pipelines won't have dkist-inventory installed
-    logging.warning("Could not load dkist-inventory. This is OK on Bitbucket.")
+    logger.warning("Could not load dkist-inventory. This is OK on Bitbucket.")
     pass
 
 QRM = False
 try:
     from quality_report_maker.libraries import report
     from quality_report_maker.libraries.json_encoder import datetime_json_object_hook
     from quality_report_maker.libraries.json_encoder import DatetimeEncoder
 
     QRM = True
 except ModuleNotFoundError:
-    logging.warning("Could not find quality_report_maker (must be installed manually)")
+    logger.warning("Could not find quality_report_maker (must be installed manually)")
 if QRM:
     import matplotlib.pyplot as plt
 
     plt.ioff()
 
 
-class TagInputs(WorkflowTaskBase):
-    def run(self) -> None:
-        logging.info(f"Looking in {os.path.abspath(self.scratch.workflow_base_path)}")
-        for file in self.scratch.workflow_base_path.glob("*.FITS"):
-            logging.info(f"Found {file}")
-            self.tag(path=file, tags=[VbiTag.input(), VbiTag.frame()])
+def tag_inputs_task(suffix: str):
+    class TagInputs(WorkflowTaskBase):
+        def run(self) -> None:
+            logger.info(f"Looking in {os.path.abspath(self.scratch.workflow_base_path)}")
+            for file in self.scratch.workflow_base_path.glob(f"*.{suffix}"):
+                logger.info(f"Found {file}")
+                self.tag(path=file, tags=[VbiTag.input(), VbiTag.frame()])
+
+    return TagInputs
 
 
 def translate_task(summit_processed: bool = False):
     class Translate122To214L0(WorkflowTaskBase):
         def run(self) -> None:
             raw_dir = Path(self.scratch.scratch_base_path) / f"VBI{self.recipe_run_id:03n}"
             if not os.path.exists(self.scratch.workflow_base_path):
                 os.makedirs(self.scratch.workflow_base_path)
             for file in raw_dir.glob("*.FITS"):
                 translated_file_name = Path(self.scratch.workflow_base_path) / os.path.basename(
                     file
                 )
-                logging.info(f"Translating and compressing {file} -> {translated_file_name}")
+                logger.info(f"Translating and compressing {file} -> {translated_file_name}")
                 hdl = fits.open(file)
                 data = hdl[0].data
                 if summit_processed:
                     data = data.astype(np.float32)
                 header = spec122_validator.validate_and_translate_to_214_l0(
                     hdl[0].header, return_type=fits.HDUList
                 )[0].header
@@ -91,63 +94,63 @@
                 del hdl, trans_hdl
 
     return Translate122To214L0
 
 
 class ShowExposureTimes(VbiTaskBase):
     def run(self) -> None:
-        logging.info(f"{self.constants.dark_exposure_times = }")
-        logging.info(f"{self.constants.gain_exposure_times = }")
-        logging.info(f"{self.constants.observe_exposure_times = }")
+        logger.info(f"{self.constants.dark_exposure_times = }")
+        logger.info(f"{self.constants.gain_exposure_times = }")
+        logger.info(f"{self.constants.observe_exposure_times = }")
 
 
 class ExposeOutputData(VbiTaskBase, FitsDataMixin):
     def run(self) -> None:
         for step in range(self.constants.num_spatial_steps):
             output_access_list = list(
                 self.fits_data_read_fits_access(
                     tags=[VbiTag.output(), VbiTag.frame(), VbiTag.spatial_step(step)],
                     cls=VbiL0FitsAccess,
                 )
             )
-            logging.info(f"found {len(output_access_list)} outputs for step {step}")
+            logger.info(f"found {len(output_access_list)} outputs for step {step}")
             fits.PrimaryHDU(output_access_list[0].data).writeto(f"comp_{step}.FITS", overwrite=True)
 
 
 class SubmitAndExposeQuality(WorkflowTaskBase, QualityMixin, MetadataStoreMixin):
     """A direct copy paste of SumbitQuality with an additional step of writing the report to disk"""
 
     def run(self):
         with self.apm_processing_step("Building quality report"):
-            logging.info("Building quality report")
+            logger.info("Building quality report")
             report_str = self.quality_build_report()
 
         with self.apm_task_step("Submitting quality report"):
-            logging.info("Submitting quality report")
+            logger.info("Submitting quality report")
             self.metadata_store_add_quality_report(
                 dataset_id=self.constants.dataset_id, quality_report=report_str
             )
 
         if QRM:
             doc_path = self.scratch.workflow_base_path / "quality_report.json"
             report_container = {
                 "datasetId": self.constants.dataset_id,
                 "qualityReport": json.dumps(report_str, cls=DatetimeEncoder),
             }
             json_str = json.dumps(report_container)
             with open(doc_path, "w") as f:
                 f.write(json_str)
-            logging.info(f"Wrote report to {doc_path}")
+            logger.info(f"Wrote report to {doc_path}")
 
 
 class ValidateL1Output(VbiTaskBase):
     def run(self) -> None:
         files = self.read(tags=[VbiTag.output(), VbiTag.frame()])
         for f in files:
-            logging.info(f"Validating {f}")
+            logger.info(f"Validating {f}")
             spec214_validator.validate(f, extra=False)
 
 
 def setup_APM_config() -> None:
     mesh_config = {
         "system-monitoring-log-apm": {
             "mesh_address": "system-monitoring-log-apm.service.sim.consul",
@@ -183,17 +186,15 @@
 
 def summit_data_processing_workflow(manual_processing_run: ManualProcessing) -> None:
     manual_processing_run.run_task(task=GenerateL1SummitData)
 
 
 def make_pdf_report(scratch_path: str, recipe_run_id: int) -> None:
     if not QRM:
-        logging.info(
-            "Did NOT make quality report pdf because quality_report_maker is not installed"
-        )
+        logger.info("Did NOT make quality report pdf because quality_report_maker is not installed")
         return
 
     json_file = os.path.join(scratch_path, str(recipe_run_id), "quality_report.json")
     pdf_file = os.path.join(scratch_path, str(recipe_run_id), "quality_report.pdf")
     with open(json_file, "r") as f:
         report_container = json.load(f)
         dataset_id = report_container["datasetId"]
@@ -201,31 +202,32 @@
             report_container["qualityReport"], object_hook=datetime_json_object_hook
         )
 
     pdf_bytes = report.format_report(report_str, f"GROGU_TEST_{dataset_id}")
     with open(pdf_file, "wb") as f:
         f.write(pdf_bytes)
 
-    logging.info(f"Wrote quality report PDF to {pdf_file}")
+    logger.info(f"Wrote quality report PDF to {pdf_file}")
 
 
 def make_dataset_asdf(scratch_path, recipe_run_id):
     if not INV:
-        logging.warning("Did NOT make dataset asdf file because dkist_inventory is not installed")
+        logger.warning("Did NOT make dataset asdf file because dkist_inventory is not installed")
         return
 
     output_dir = os.path.join(scratch_path, str(recipe_run_id))
     asdf_name = f"dataset_{recipe_run_id:03n}.asdf"
-    logging.info(f"Creating ASDF file from {output_dir} and saving to {asdf_name}")
+    logger.info(f"Creating ASDF file from {output_dir} and saving to {asdf_name}")
     dataset_from_fits(output_dir, asdf_name, hdu=1)
 
 
 def main(
     scratch_path="/media/FastPipelin/vbi/scratch",
     recipe_run_id=4,
+    suffix: str = "FITS",
     sv_file_to_test: str | None = None,
     skip_translation: bool = False,
     skip_movie: bool = False,
     only_translate: bool = False,
     science_workflow_name: str = "l0_processing",
     use_apm: bool = False,
 ):
@@ -247,15 +249,15 @@
             manual_processing_run.run_task(
                 task=translate_task(
                     summit_processed=science_workflow_name == "summit_data_processed"
                 )
             )
         if only_translate:
             return
-        manual_processing_run.run_task(task=TagInputs)
+        manual_processing_run.run_task(task=tag_inputs_task(suffix))
         manual_processing_run.run_task(task=ParseL0VbiInputData)
         science_workflow(manual_processing_run)
         manual_processing_run.run_task(task=VbiWriteL1Frame)
         manual_processing_run.run_task(task=QualityL1Metrics)
         manual_processing_run.run_task(task=VbiQualityL1Metrics)
         manual_processing_run.run_task(task=SubmitAndExposeQuality)
         manual_processing_run.run_task(task=ValidateL1Output)
@@ -269,22 +271,23 @@
             manual_processing_run.run_task(task=AssembleVbiMovie)
 
         manual_processing_run.count_provenance()
 
         if sv_file_to_test:
             manual_processing_run.run_task(task=ExposeOutputData)
             assert compare_to_sv_data(sv_file_to_test)
-            logging.info("DC output matches SV output!")
+            logger.info("DC output matches SV output!")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description="Run an end-to-end test of the VBI DC Science pipeline"
     )
     parser.add_argument("scratch_path", help="Location to use as the DC 'scratch' disk")
+    parser.add_argument("--suffix", help="File suffix to treat as INPUT frames", default="FITS")
     parser.add_argument(
         "-W",
         "--workflow_name",
         help="Name of VBI workflow to test",
         choices=["l0_pipeline", "summit_data_processed"],
         default="l0_pipeline",
     )
@@ -314,14 +317,15 @@
     parser.add_argument("-A", "--use-apm", help="Send APM spans to SIM", action="store_true")
     args = parser.parse_args()
 
     sys.exit(
         main(
             scratch_path=args.scratch_path,
             recipe_run_id=args.run_id,
+            suffix=args.suffix,
             sv_file_to_test=args.sv_file_to_test,
             skip_translation=args.skip_translation,
             only_translate=args.only_translate,
             skip_movie=args.skip_movie,
             science_workflow_name=args.workflow_name,
             use_apm=args.use_apm,
         )
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_assemble_movie.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_assemble_movie.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,41 +8,41 @@
 from dkist_processing_vbi.tests.conftest import generate_214_l1_fits_frame
 from dkist_processing_vbi.tests.conftest import Vbi122ObserveFrames
 from dkist_processing_vbi.tests.conftest import VbiConstantsDb
 
 
 @pytest.fixture(scope="function")
 def assemble_task_with_tagged_movie_frames(tmp_path, recipe_run_id, init_vbi_constants_db):
-    num_dsps_repeats = 10
-    constants_db = VbiConstantsDb(NUM_DSPS_REPEATS=num_dsps_repeats)
+    num_mosaic_repeats = 10
+    constants_db = VbiConstantsDb(NUM_MOSAIC_REPEATS=num_mosaic_repeats)
     init_vbi_constants_db(recipe_run_id, constants_db)
     with AssembleVbiMovie(
         recipe_run_id=recipe_run_id, workflow_name="vbi_make_movie_frames", workflow_version="VX.Y"
     ) as task:
         task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path, recipe_run_id=recipe_run_id)
-        task.testing_num_dsps_repeats = num_dsps_repeats
+        task.testing_num_mosaic_repeats = num_mosaic_repeats
         task.num_steps = 1
         task.num_exp_per_step = 1
         ds = Vbi122ObserveFrames(
             array_shape=(1, 100, 100),
             num_steps=task.num_steps,
             num_exp_per_step=task.num_exp_per_step,
-            num_dsps_repeats=task.testing_num_dsps_repeats,
+            num_mosaics_per_dsps_repeat=task.testing_num_mosaic_repeats,
+            num_dsps_repeats=1,  # No subcycling
         )
         header_generator = (d.header() for d in ds)
-        for d, header in enumerate(header_generator):
+        for m, header in enumerate(header_generator):
             data = np.ones((100, 100))
-            data[: d * 10, :] = 0.0
+            data[: m * 10, :] = 0.0
             hdl = generate_214_l1_fits_frame(data=data, s122_header=header)
-            hdl[1].header["DSPSNUM"] = d + 1
             task.fits_data_write(
                 hdu_list=hdl,
                 tags=[
                     VbiTag.movie_frame(),
-                    VbiTag.dsps_repeat(d + 1),
+                    VbiTag.mosaic(m + 1),
                 ],
             )
         yield task
         task.scratch.purge()
         task.constants._purge()
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_dark.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_gain.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_intermediate_loaders.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_intermediate_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_make_movie_frames.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_make_movie_frames.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,109 +17,116 @@
 from dkist_processing_vbi.tests.conftest import Vbi122ObserveFrames
 from dkist_processing_vbi.tests.conftest import VbiConstantsDb
 
 
 @pytest.fixture(scope="function")
 def raw_make_movie_frames_task(tmp_path, recipe_run_id, init_vbi_constants_db):
     num_steps = 4
-    num_dsps_repeats = 2
-    constants_db = VbiConstantsDb(NUM_SPATIAL_STEPS=num_steps, NUM_DSPS_REPEATS=num_dsps_repeats)
+    num_mosaic_repeats = 2
+    constants_db = VbiConstantsDb(
+        NUM_SPATIAL_STEPS=num_steps,
+        NUM_MOSAIC_REPEATS=num_mosaic_repeats,
+    )
     init_vbi_constants_db(recipe_run_id, constants_db)
     with MakeVbiMovieFrames(
         recipe_run_id=recipe_run_id, workflow_name="vbi_make_movie_frames", workflow_version="VX.Y"
     ) as task:
         task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path, recipe_run_id=recipe_run_id)
         task.num_steps = 4
         task.num_exp_per_step = 2
-        task.testing_num_dsps_repeats = 2
+        task.testing_num_mosaic_repeats = num_mosaic_repeats
         ds = Vbi122ObserveFrames(
             array_shape=(1, 10, 10),
             num_steps=task.num_steps,
             num_exp_per_step=task.num_exp_per_step,
-            num_dsps_repeats=task.testing_num_dsps_repeats,
+            num_dsps_repeats=task.testing_num_mosaic_repeats,
+            num_mosaics_per_dsps_repeat=1,  # No subcycling
         )
         header_generator = (d.header() for d in ds)
         for s in range(1, task.num_steps + 1):
             for e in range(1, task.num_exp_per_step + 1):
-                for d in range(1, task.testing_num_dsps_repeats + 1):
-                    value = (s - 1) + (e - 1) * 2 + (d - 1)
+                for m in range(1, task.testing_num_mosaic_repeats + 1):
+                    value = (s - 1) + (e - 1) * 2 + (m - 1)
                     data = np.ones((10, 10)) * value
                     header = next(header_generator)
                     hdl = generate_214_l1_fits_frame(data=data, s122_header=header)
                     hdl[1].header["CRVAL1"] = 0.0
                     hdl[1].header["CRVAL2"] = 0.0
                     hdl[1].header["CDELT1"] = 1.0
                     hdl[1].header["CDELT2"] = 1.0
                     hdl[1].header["CRPIX1"] = (s % 2) * 7
                     hdl[1].header["CRPIX2"] = -1 * ((s - 1) // 2 - 1) * 7
-                    hdl[1].header["DSPSNUM"] = d
+                    hdl[1].header["DSPSNUM"] = m
                     hdl[1].header["VBISTP"] = s
                     task.fits_data_write(
                         hdu_list=hdl,
                         tags=[
                             VbiTag.output(),
                             VbiTag.frame(),
                             VbiTag.spatial_step(s),
-                            VbiTag.dsps_repeat(d),
+                            VbiTag.mosaic(m),
                         ],
                     )
         ensure_all_inputs_used(header_generator)
         yield task
         task.scratch.purge()
         task.constants._purge()
 
 
 @pytest.fixture(scope="module")
 def make_movie_frames_task_with_averages(tmp_path_factory):
     num_steps = 4
-    num_dsps_repeats = 2
+    num_mosaic_repeats = 2
     recipe_run_id = randint(0, 99999)
-    constants_db = VbiConstantsDb(NUM_SPATIAL_STEPS=num_steps, NUM_DSPS_REPEATS=num_dsps_repeats)
+    constants_db = VbiConstantsDb(
+        NUM_SPATIAL_STEPS=num_steps, NUM_MOSAIC_REPEATS=num_mosaic_repeats
+    )
     # Repeat ini_vbi_constants fixture here because of a scope conflict
     constants = VbiConstants(recipe_run_id=recipe_run_id, task_name="test")
     constants._update(asdict(constants_db))
     with MakeVbiMovieFrames(
         recipe_run_id=recipe_run_id,
         workflow_name="vbi_make_movie_frames",
         workflow_version="VX.Y",
     ) as task:
         task.scratch = WorkflowFileSystem(
             scratch_base_path=tmp_path_factory.mktemp("scratch"), recipe_run_id=recipe_run_id
         )
         task.num_steps = 4
         task.num_exp_per_step = 1
-        task.testing_num_dsps_repeats = 2
+        task.testing_num_mosaic_repeats = num_mosaic_repeats
         ds = Vbi122ObserveFrames(
             array_shape=(1, 10, 10),
             num_steps=task.num_steps,
             num_exp_per_step=task.num_exp_per_step,
-            num_dsps_repeats=task.testing_num_dsps_repeats,
+            num_dsps_repeats=task.testing_num_mosaic_repeats,
+            num_mosaics_per_dsps_repeat=1,  # No subcycling
         )
         header_generator = (d.header() for d in ds)
         for s in range(1, task.num_steps + 1):
-            for d in range(1, task.testing_num_dsps_repeats + 1):
+            for m in range(1, task.testing_num_mosaic_repeats + 1):
                 header = next(header_generator)
-                value = s - 1 + d - 1
+                value = s - 1 + m - 1
                 data = np.ones((10, 10)) * value
                 hdl = generate_214_l1_fits_frame(s122_header=header, data=data)
                 hdl[1].header["CRVAL1"] = 0.0
                 hdl[1].header["CRVAL2"] = 0.0
                 hdl[1].header["CDELT1"] = 1.0
                 hdl[1].header["CDELT2"] = 1.0
                 hdl[1].header["CRPIX1"] = (s % 2) * 7
                 hdl[1].header["CRPIX2"] = -1 * ((s - 1) // 2 - 1) * 7
-                hdl[1].header["DSPSNUM"] = d
+                hdl[1].header["DSPSNUM"] = m
                 hdl[1].header["VBISTP"] = s
                 task.fits_data_write(
                     hdu_list=hdl,
                     tags=[
                         VbiTag.intermediate(),
                         VbiTag.task("AVG_MOVIE_FRAME"),
                         VbiTag.spatial_step(s),
-                        VbiTag.dsps_repeat(d),
+                        VbiTag.mosaic(m),
                     ],
                 )
         ensure_all_inputs_used(header_generator)
         yield task
         task.scratch.purge()
         task.constants._purge()
 
@@ -176,58 +183,58 @@
     raw_make_movie_frames_task()
 
     frame_access_list = list(
         raw_make_movie_frames_task.fits_data_read_fits_access(
             tags=[VbiTag.movie_frame()], cls=VbiL1FitsAccess
         )
     )
-    assert len(frame_access_list) == raw_make_movie_frames_task.testing_num_dsps_repeats
+    assert len(frame_access_list) == raw_make_movie_frames_task.testing_num_mosaic_repeats
 
     frame_access_list = sorted(frame_access_list, key=lambda x: x.current_dsps_repeat)
     assert [o.current_dsps_repeat for o in frame_access_list] == list(
-        range(1, raw_make_movie_frames_task.testing_num_dsps_repeats + 1)
+        range(1, raw_make_movie_frames_task.testing_num_mosaic_repeats + 1)
     )
-    for i in range(raw_make_movie_frames_task.testing_num_dsps_repeats):
+    for i in range(raw_make_movie_frames_task.testing_num_mosaic_repeats):
         np.testing.assert_almost_equal(frame_access_list[i].data, compute_expected_mosiac(i))
 
 
 def test_average_all_exposures(raw_make_movie_frames_task):
     raw_make_movie_frames_task.average_all_exposures()
     for s in range(1, raw_make_movie_frames_task.num_steps + 1):
-        for d in range(1, raw_make_movie_frames_task.testing_num_dsps_repeats + 1):
+        for m in range(1, raw_make_movie_frames_task.testing_num_mosaic_repeats + 1):
             hdus = list(
                 raw_make_movie_frames_task.fits_data_read_hdu(
                     tags=[
                         VbiTag.intermediate(),
                         VbiTag.task("AVG_MOVIE_FRAME"),
                         VbiTag.spatial_step(s),
-                        VbiTag.dsps_repeat(d),
+                        VbiTag.mosaic(m),
                     ]
                 )
             )
             assert len(hdus) == 1
             data = hdus[0][1].data
-            expected = np.ones((10, 10)) * (s + d - 1)
+            expected = np.ones((10, 10)) * (s + m - 1)
             np.testing.assert_equal(data, expected)
 
 
 def test_find_ref_pos(make_movie_frames_task_with_averages):
     access_list = list(
         make_movie_frames_task_with_averages.fits_data_read_fits_access(
-            tags=[VbiTag.intermediate(), VbiTag.task("AVG_MOVIE_FRAME"), VbiTag.dsps_repeat(2)],
+            tags=[VbiTag.intermediate(), VbiTag.task("AVG_MOVIE_FRAME"), VbiTag.mosaic(2)],
             cls=VbiL1FitsAccess,
         )
     )
     assert make_movie_frames_task_with_averages.find_ref_pos(access_list) == 1
 
 
 def test_get_fov_size(make_movie_frames_task_with_averages):
     access_list = list(
         make_movie_frames_task_with_averages.fits_data_read_fits_access(
-            tags=[VbiTag.intermediate(), VbiTag.task("AVG_MOVIE_FRAME"), VbiTag.dsps_repeat(1)],
+            tags=[VbiTag.intermediate(), VbiTag.task("AVG_MOVIE_FRAME"), VbiTag.mosaic(1)],
             cls=VbiL1FitsAccess,
         )
     )
     assert make_movie_frames_task_with_averages.get_fov_size(
         access_list, access_list[0].header
     ) == (17, 17)
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_parse_l0.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_parse_l0.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,150 +1,174 @@
 from itertools import chain
 
 import pytest
 from dkist_processing_common._util.scratch import WorkflowFileSystem
-from dkist_processing_common.models.constants import BudName
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_vbi.models.constants import VbiBudName
 from dkist_processing_vbi.models.tags import VbiTag
 from dkist_processing_vbi.tasks.parse import ParseL0VbiInputData
 from dkist_processing_vbi.tests.conftest import generate_214_l0_fits_frame
 from dkist_processing_vbi.tests.conftest import Vbi122DarkFrames
 from dkist_processing_vbi.tests.conftest import Vbi122GainFrames
 from dkist_processing_vbi.tests.conftest import Vbi122ObserveFrames
 
 
 @pytest.fixture(scope="function")
-def parse_inputs_task(tmp_path, recipe_run_id, DKIST009_offset):
+def parse_inputs_task(tmp_path, recipe_run_id):
     with ParseL0VbiInputData(
         recipe_run_id=recipe_run_id,
         workflow_name="vbi_parse_l0_inputs",
         workflow_version="VX.Y",
     ) as task:
         task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path, recipe_run_id=recipe_run_id)
         task.num_program_types = 3
         task.num_steps = 4
         task.num_exp_per_step = 3
-        task.test_num_dsps_repeats = 2
+        task.test_num_mosaic_repeats = 2
         ds1 = Vbi122DarkFrames(
             array_shape=(1, 10, 10),
             num_steps=task.num_steps,
             num_exp_per_step=1,
         )
         ds2 = Vbi122GainFrames(
             array_shape=(1, 10, 10),
             num_steps=task.num_steps,
             num_exp_per_step=1,
         )
         ds3 = Vbi122ObserveFrames(
             array_shape=(1, 10, 10),
             num_steps=task.num_steps,
             num_exp_per_step=task.num_exp_per_step,
-            num_dsps_repeats=task.test_num_dsps_repeats,
-            DKIST008_value=5280,  # Just a number clearly larger than test_num_dsps_repeats
-            DKIST009_offset_value=DKIST009_offset,
+            num_dsps_repeats=task.test_num_mosaic_repeats,
+            num_mosaics_per_dsps_repeat=1,  # No subrepeats
         )
         ds = chain(ds1, ds2, ds3)
         header_generator = (d.header() for d in ds)
         for header in header_generator:
             hdul = generate_214_l0_fits_frame(s122_header=header)
             task.fits_data_write(hdu_list=hdul, tags=[VbiTag.input(), VbiTag.frame()])
         yield task
         task.scratch.purge()
         task.constants._purge()
 
 
 @pytest.fixture(scope="function")
-def parse_inputs_task_with_only_observe(tmp_path, recipe_run_id, DKIST009_offset):
+def parse_inputs_task_with_only_observe(tmp_path, recipe_run_id):
+    with ParseL0VbiInputData(
+        recipe_run_id=recipe_run_id,
+        workflow_name="vbi_parse_l0_inputs",
+        workflow_version="VX.Y",
+    ) as task:
+        task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path, recipe_run_id=recipe_run_id)
+        task.num_program_types = 3
+        task.num_steps = 4
+        task.num_exp_per_step = 1
+        task.test_num_mosaic_repeats = 2
+        ds = Vbi122ObserveFrames(
+            array_shape=(1, 10, 10),
+            num_steps=task.num_steps,
+            num_exp_per_step=task.num_exp_per_step,
+            num_dsps_repeats=task.test_num_mosaic_repeats,
+            num_mosaics_per_dsps_repeat=1,  # No subrepeats
+        )
+        header_generator = (d.header() for d in ds)
+        for header in header_generator:
+            hdul = generate_214_l0_fits_frame(s122_header=header)
+            task.fits_data_write(hdu_list=hdul, tags=[VbiTag.input(), VbiTag.frame()])
+        yield task
+        task.scratch.purge()
+        task.constants._purge()
+
+
+@pytest.fixture(scope="function")
+def parse_inputs_task_with_subrepeats(tmp_path, recipe_run_id):
     with ParseL0VbiInputData(
         recipe_run_id=recipe_run_id,
         workflow_name="vbi_parse_l0_inputs",
         workflow_version="VX.Y",
     ) as task:
         task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path, recipe_run_id=recipe_run_id)
         task.num_program_types = 3
         task.num_steps = 4
         task.num_exp_per_step = 1
+        task.test_num_mosaic_repeats = 4
         task.test_num_dsps_repeats = 2
         ds = Vbi122ObserveFrames(
             array_shape=(1, 10, 10),
             num_steps=task.num_steps,
             num_exp_per_step=task.num_exp_per_step,
             num_dsps_repeats=task.test_num_dsps_repeats,
-            DKIST008_value=5280,  # Just a number clearly larger than test_num_dsps_repeats
-            DKIST009_offset_value=DKIST009_offset,
+            num_mosaics_per_dsps_repeat=task.test_num_mosaic_repeats // task.test_num_dsps_repeats,
         )
         header_generator = (d.header() for d in ds)
         for header in header_generator:
             hdul = generate_214_l0_fits_frame(s122_header=header)
             task.fits_data_write(hdu_list=hdul, tags=[VbiTag.input(), VbiTag.frame()])
         yield task
         task.scratch.purge()
         task.constants._purge()
 
 
 @pytest.fixture(scope="function")
-def parse_inputs_task_with_out_of_sequence_DSPSNUMS(tmp_path, recipe_run_id, DKIST009_offset):
+def parse_inputs_task_with_out_of_sequence_DSPSNUMS(tmp_path, recipe_run_id):
     with ParseL0VbiInputData(
         recipe_run_id=recipe_run_id,
         workflow_name="vbi_parse_l0_inputs",
         workflow_version="VX.Y",
     ) as task:
         task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path, recipe_run_id=recipe_run_id)
         task.num_steps = 4
         task.num_exp_per_step = 1
-        task.test_num_dsps_repeats = 4
+        task.test_num_mosaic_repeats = 4
         ds = Vbi122ObserveFrames(
             array_shape=(1, 10, 10),
             num_steps=task.num_steps,
             num_exp_per_step=task.num_exp_per_step,
-            num_dsps_repeats=task.test_num_dsps_repeats,
-            DKIST008_value=5280,  # Just a number clearly larger than test_num_dsps_repeats
-            DKIST009_offset_value=DKIST009_offset,
+            num_dsps_repeats=task.test_num_mosaic_repeats,
+            num_mosaics_per_dsps_repeat=1,  # No subrepeats
         )
         header_generator = (d.header() for d in ds)
         for i, header in enumerate(header_generator):
             if header["DKIST009"] == 1003:
                 # Skip the 3rd frame (this needs to not be the last one; that would be an aborted last mosaic)
                 continue
             hdul = generate_214_l0_fits_frame(s122_header=header)
             task.fits_data_write(hdu_list=hdul, tags=[VbiTag.input(), VbiTag.frame()])
         yield task
         task.scratch.purge()
         task.constants._purge()
 
 
 @pytest.fixture(scope="function")
-def parse_inputs_task_with_aborted_last_mosaic(tmp_path, recipe_run_id, DKIST009_offset):
+def parse_inputs_task_with_aborted_last_mosaic(tmp_path, recipe_run_id):
     num_steps = 4
     num_exp_per_step = 3
-    num_dsps_repeats = 4
+    num_mosaic_repeats = 4
     with ParseL0VbiInputData(
         recipe_run_id=recipe_run_id,
         workflow_name="vbi_parse_l0_inputs",
         workflow_version="VX.Y",
     ) as task:
         task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path)
         ds = Vbi122ObserveFrames(
             array_shape=(1, 10, 10),
             num_steps=num_steps,
             num_exp_per_step=num_exp_per_step,
-            num_dsps_repeats=num_dsps_repeats,
-            DKIST008_value=5280,  # Just a number clearly larger than test_num_dsps_repeats
-            DKIST009_offset_value=DKIST009_offset,
+            num_dsps_repeats=num_mosaic_repeats,
+            num_mosaics_per_dsps_repeat=1,  # No subrepeats
         )
         header_generator = (d.header() for d in ds)
         for i, header in enumerate(header_generator):
-            if header["DKIST009"] == 1004 and header["VBI__004"] > num_steps - 2:
+            if header["DKIST009"] == num_mosaic_repeats and header["VBI__004"] > num_steps - 2:
                 # Skip the last 2 mosaic steps of the last repeat
                 continue
             hdul = generate_214_l0_fits_frame(s122_header=header)
             task.fits_data_write(hdu_list=hdul, tags=[VbiTag.input(), VbiTag.frame()])
-        yield task, num_dsps_repeats - 1
+        yield task, num_mosaic_repeats - 1
         task.scratch.purge()
         task.constants._purge()
 
 
 def test_parse_l0_input_data_spatial_pos(parse_inputs_task, mocker):
     """
     Given: a set of raw inputs of multiple task types and a ParseL0VbiInputData task
@@ -160,21 +184,23 @@
         translated_files = list(
             parse_inputs_task.read(tags=[VbiTag.input(), VbiTag.frame(), VbiTag.spatial_step(step)])
         )
         assert (
             len(translated_files)
             == (parse_inputs_task.num_program_types - 1)  # for non observe frames
             + parse_inputs_task.num_exp_per_step
-            * parse_inputs_task.constants.num_dsps_repeats  # for observe frames
+            * parse_inputs_task.constants._db_dict[
+                VbiBudName.num_mosaics_repeats.value
+            ]  # for observe frames
         )
         for filepath in translated_files:
             assert filepath.exists()
 
 
-def test_parse_l0_input_constants(parse_inputs_task, mocker, DKIST009_offset):
+def test_parse_l0_input_constants(parse_inputs_task, mocker):
     """
     Given: a set of raw inputs of multiple task types and a ParseL0VbiInputData task
     When: the task is run
     Then: pipeline constants are correctly updated from the input headers
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
@@ -182,25 +208,16 @@
     parse_inputs_task()
 
     assert (
         parse_inputs_task.constants._db_dict[VbiBudName.num_spatial_steps.value]
         == parse_inputs_task.num_steps
     )
     assert (
-        parse_inputs_task.constants._db_dict[BudName.num_dsps_repeats.value]
-        == parse_inputs_task.test_num_dsps_repeats
-    )
-    assert (
-        parse_inputs_task.constants._db_dict[VbiBudName.dsps_repeat_pedestal.value]
-        == DKIST009_offset
-    )
-    assert parse_inputs_task.constants._db_dict[BudName.spectral_line.value] == "VBI-Red H-alpha"
-    assert (
-        parse_inputs_task.constants._db_dict[VbiBudName.num_exp_per_dsp.value]
-        == parse_inputs_task.num_exp_per_step
+        parse_inputs_task.constants._db_dict[VbiBudName.num_mosaics_repeats.value]
+        == parse_inputs_task.test_num_mosaic_repeats
     )
 
 
 def test_parse_l0_input_frames_found(parse_inputs_task, mocker):
     """
     Given: a set of raw inputs of multiple task types and a ParseL0VbiInputData task
     When: the task is run
@@ -219,67 +236,86 @@
         == parse_inputs_task.num_steps
     )
 
     assert (
         len(list(parse_inputs_task.read(tags=[VbiTag.input(), VbiTag.task("OBSERVE")])))
         == parse_inputs_task.num_steps
         * parse_inputs_task.num_exp_per_step
-        * parse_inputs_task.test_num_dsps_repeats
+        * parse_inputs_task.test_num_mosaic_repeats
     )
 
 
 def test_parse_l0_input_with_only_observe(parse_inputs_task_with_only_observe, mocker):
     """
     Given: a set of raw inputs of a single task type and a ParseL0VbiInputData task
     When: the task is run
     Then: the observe frames are correctly identified and tagged
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
     parse_inputs_task_with_only_observe()
-    for dsps_repeat in range(1, parse_inputs_task_with_only_observe.test_num_dsps_repeats + 1):
+    for mosaic_repeat in range(1, parse_inputs_task_with_only_observe.test_num_mosaic_repeats + 1):
         for step in range(1, parse_inputs_task_with_only_observe.num_steps + 1):
             translated_files = list(
                 parse_inputs_task_with_only_observe.read(
                     tags=[
                         VbiTag.input(),
                         VbiTag.frame(),
                         VbiTag.task("OBSERVE"),
                         VbiTag.spatial_step(step),
-                        VbiTag.dsps_repeat(dsps_repeat),
+                        VbiTag.mosaic(mosaic_repeat),
                     ]
                 )
             )
             assert len(translated_files) == parse_inputs_task_with_only_observe.num_exp_per_step
             for filepath in translated_files:
                 assert filepath.exists()
 
 
-def test_parse_l0_raises_error_on_bad_DSPSNUM_sequence(
-    parse_inputs_task_with_out_of_sequence_DSPSNUMS, mocker
-):
-    """
-    Given: a set of observe frames that are missing a DSPSNUM
-    When: parsing the frames
-    Then: an error is raised
+def test_parse_l0_aborted_last_mosaic(parse_inputs_task_with_aborted_last_mosaic, mocker):
+    """
+    Given: a set of raw inputs representing a dataset with an aborted last mosaic
+    When: the task is run
+    Then: pipeline constants are correctly updated from the input headers
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
-    with pytest.raises(ValueError, match="Set of DSPS nums is not equal"):
-        parse_inputs_task_with_out_of_sequence_DSPSNUMS()
+    task, expected_num_mosaic_repeats = parse_inputs_task_with_aborted_last_mosaic
+    task()
 
+    assert (
+        task.constants._db_dict[VbiBudName.num_mosaics_repeats.value] == expected_num_mosaic_repeats
+    )
 
-def test_parse_l0_aborted_last_mosaic(parse_inputs_task_with_aborted_last_mosaic, mocker):
+
+def test_parse_l0_correctly_tagged_mosaic_subrepeats(parse_inputs_task_with_subrepeats, mocker):
     """
-    Given: a set of raw inputs representing a dataset with an aborted last mosaic
-    When: the task is run
-    Then: pipeline constants are correctly updated from the input headers
+    Given: A set of observe frames taken with subrepeats (i.e., multiple mosaics per DSPS repeat)
+    When: the parse task is run
+    Then: pipeline constants are correctly updated and the correct
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
-    task, expected_num_dsps_repeats = parse_inputs_task_with_aborted_last_mosaic
+    task = parse_inputs_task_with_subrepeats
     task()
 
-    assert task.constants._db_dict[BudName.num_dsps_repeats.value] == expected_num_dsps_repeats
+    found_num_mosaic_repeats = task.constants._db_dict[VbiBudName.num_mosaics_repeats.value]
+    assert found_num_mosaic_repeats == task.test_num_mosaic_repeats
+    for mosaic in range(1, found_num_mosaic_repeats + 1):
+        for step in range(1, task.num_steps + 1):
+            file_list = list(
+                task.read(
+                    tags=[
+                        VbiTag.input(),
+                        VbiTag.frame(),
+                        VbiTag.task("OBSERVE"),
+                        VbiTag.spatial_step(step),
+                        VbiTag.mosaic(mosaic),
+                    ],
+                )
+            )
+            assert len(file_list) == task.num_exp_per_step
+            for f in file_list:
+                assert f.exists()
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_process_summit.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_process_summit.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,61 +17,62 @@
 from dkist_processing_vbi.tests.conftest import VbiConstantsDb
 
 RNG = np.random.default_rng()
 
 
 @pytest.fixture(scope="function")
 def process_summit_processed(tmp_path, recipe_run_id, init_vbi_constants_db):
-    constants_db = VbiConstantsDb(SPECTRAL_LINE="VBI TEST LINE", NUM_DSPS_REPEATS=1)
+    constants_db = VbiConstantsDb(NUM_MOSAIC_REPEATS=1)
     init_vbi_constants_db(recipe_run_id, constants_db)
     with GenerateL1SummitData(
         recipe_run_id=recipe_run_id,
         workflow_name="vbi_process_summit_processed",
         workflow_version="VX.Y",
     ) as task:
         task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path, recipe_run_id=recipe_run_id)
         task.num_steps = 4
         num_exp_per_step = 1
         ds = Vbi122SummitObserveFrames(
             array_shape=(1, 10, 10),
             num_steps=task.num_steps,
             num_exp_per_step=num_exp_per_step,
             num_dsps_repeats=1,
+            num_mosaics_per_dsps_repeat=1,
         )
         dsd = Vbi122DarkFrames(
             array_shape=(1, 10, 10),
             num_steps=task.num_steps,
             num_exp_per_step=num_exp_per_step,
         )
         header_generator = (d.header() for d in ds)
         dark_header_generator = (d.header() for d in dsd)
-        data_dict = defaultdict(lambda: defaultdict(list))
+        data_dict = defaultdict(dict)
         for p in range(1, task.num_steps + 1):
             for e in range(num_exp_per_step):
                 header = next(header_generator)
                 # We need to set these so the compression doesn't make wrong data
                 header["BZERO"] = 0.0
                 header["BSCALE"] = 1.0
                 data = np.random.normal(loc=p, size=(10, 10)).astype(np.float32)
                 hdul = generate_compressed_214_l0_fits_frame(s122_header=header, data=data)
                 hdul[1].header["TEST_EXP"] = e  # This is just for testing data equivalence
                 hdul.writeto(tmp_path / "tmp.fits", overwrite=True)
 
                 # We need to write it out once because the compression will slightly change the values
                 thdul = fits.open(tmp_path / "tmp.fits")
-                data_dict[p][e].append(thdul[1].data)
+                data_dict[p][e] = thdul[1].data
                 del thdul
 
                 task.fits_data_write(
                     hdu_list=hdul,
                     tags=[
                         VbiTag.input(),
                         VbiTag.task("Observe"),
                         VbiTag.spatial_step(p),
-                        VbiTag.dsps_repeat(header["DKIST009"]),
+                        VbiTag.mosaic(header["DKIST009"]),
                         VbiTag.frame(),
                     ],
                 )
                 dark_header = next(dark_header_generator)
                 hdul = generate_214_l0_fits_frame(s122_header=dark_header, data=np.ones((10, 10)))
                 task.fits_data_write(
                     hdu_list=hdul,
@@ -89,49 +90,47 @@
 
 @pytest.fixture(scope="function")
 def process_summit_processed_with_aborted_last_mosaic(
     tmp_path, recipe_run_id, init_vbi_constants_db
 ):
     num_steps = 4
     num_exp_per_step = 3
-    num_dsps_repeats = 3
-    constants_db = VbiConstantsDb(
-        SPECTRAL_LINE="VBI TEST LINE", NUM_DSPS_REPEATS=num_dsps_repeats - 1
-    )
+    num_mosaic_repeats = 3
+    constants_db = VbiConstantsDb(NUM_MOSAIC_REPEATS=num_mosaic_repeats - 1)
     init_vbi_constants_db(recipe_run_id, constants_db)
     with GenerateL1SummitData(
         recipe_run_id=recipe_run_id,
         workflow_name="vbi_process_summit_processed",
         workflow_version="VX.Y",
     ) as task:
         task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path, recipe_run_id=recipe_run_id)
         ds = Vbi122SummitObserveFrames(
             array_shape=(1, 10, 10),
             num_steps=num_steps,
             num_exp_per_step=num_exp_per_step,
-            num_dsps_repeats=num_dsps_repeats,
-            DKIST008_value=5280,
+            num_mosaics_per_dsps_repeat=1,  # No subcycle
+            num_dsps_repeats=num_mosaic_repeats,
         )
         header_generator = (d.header() for d in ds)
         for i, header in enumerate(header_generator):
-            if header["DKIST009"] == num_dsps_repeats and header["VBI__004"] > num_steps - 2:
+            if header["DKIST009"] == num_mosaic_repeats and header["VBI__004"] > num_steps - 2:
                 # Skip the last 2 mosaic steps of the last repeat
                 continue
-            hdul = generate_214_l0_fits_frame(s122_header=header)
+            hdul = generate_compressed_214_l0_fits_frame(s122_header=header)
             task.fits_data_write(
                 hdu_list=hdul,
                 tags=[
                     VbiTag.input(),
                     VbiTag.frame(),
                     VbiTag.task("observe"),
-                    VbiTag.dsps_repeat(header["DKIST009"]),
+                    VbiTag.mosaic(header["DKIST009"]),
                     VbiTag.spatial_step(header["VBI__004"]),
                 ],
             )
-        yield task, num_dsps_repeats - 1, num_exp_per_step, num_steps
+        yield task, num_mosaic_repeats - 1, num_exp_per_step, num_steps
         task.scratch.purge()
         task.constants._purge()
 
 
 def test_process_summit_data(process_summit_processed, mocker):
     """
     Given: a set of parsed input frames of summit-processed data and a GenerateL1SummitData task
@@ -158,19 +157,19 @@
                 ],
                 cls=VbiL0FitsAccess,
             )
         )
         assert len(sci_access_list) == num_exp_per_step
         sorted_access = sorted(sci_access_list, key=lambda x: x.header["TEST_EXP"])
         for e in range(num_exp_per_step):
-            assert VbiTag.input() not in task.read(sorted_access[0].name)
-            hdu = sorted_access[0]._hdu
+            assert VbiTag.input() not in task.tags(sorted_access[e].name)
+            hdu = sorted_access[e]._hdu
             assert isinstance(hdu, fits.CompImageHDU)
             assert hdu.data.dtype == "float32"
-            np.testing.assert_array_equal(hdu.data, expected_data[step][e][0])
+            np.testing.assert_array_equal(hdu.data, expected_data[step][e])
 
 
 def test_process_summit_data_with_aborted_last_mosaic(
     process_summit_processed_with_aborted_last_mosaic, mocker
 ):
     """
     Given: a set of parsed input frames of summit-processed data that contain an aborted mosaic
@@ -178,15 +177,15 @@
     Then: only frames from complete mosaics are pass through as "calibrated"
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
     (
         task,
-        expected_num_dsps_repeats,
+        expected_num_mosaic_repeats,
         num_exp_per_step,
         num_steps,
     ) = process_summit_processed_with_aborted_last_mosaic
     task()
 
     # Make sure the input tag was removed
     assert len(list(task.read(tags=[VbiTag.input(), VbiTag.output()]))) == 0
@@ -198,10 +197,10 @@
                     VbiTag.calibrated(),
                     VbiTag.frame(),
                     VbiTag.spatial_step(step),
                     VbiTag.stokes("I"),
                 ]
             )
         )
-        assert len(files) == num_exp_per_step * expected_num_dsps_repeats
+        assert len(files) == num_exp_per_step * expected_num_mosaic_repeats
         for filepath in files:
             assert filepath.exists()
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_quality_metrics.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_science.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_science.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 from dkist_processing_vbi.tests.conftest import Vbi122ObserveFrames
 from dkist_processing_vbi.tests.conftest import VbiConstantsDb
 
 
 @pytest.fixture(scope="function")
 def science_calibration_task(tmp_path, recipe_run_id, init_vbi_constants_db, abort_mosaic):
     num_steps = 4
-    num_dsps_repeats = 3
+    num_mosaic_repeats = 3
     num_exp_per_step = 2
     exp_time = 0.01
     constants_db = VbiConstantsDb(
         NUM_SPATIAL_STEPS=num_steps,
-        NUM_DSPS_REPEATS=num_dsps_repeats - (1 * abort_mosaic),  # Freaky
-        SPECTRAL_LINE="VBI TEST LINE",
+        NUM_MOSAIC_REPEATS=num_mosaic_repeats - (1 * abort_mosaic),
         OBSERVE_EXPOSURE_TIMES=(exp_time,),
     )
     init_vbi_constants_db(recipe_run_id, constants_db)
     with ScienceCalibration(
         recipe_run_id=recipe_run_id,
         workflow_name="vbi_science_calibration",
         workflow_version="VX.Y",
     ) as task:
         task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path, recipe_run_id=recipe_run_id)
         ds = Vbi122ObserveFrames(
             array_shape=(1, 10, 10),
             num_steps=num_steps,
             num_exp_per_step=num_exp_per_step,
-            num_dsps_repeats=num_dsps_repeats,
+            num_mosaics_per_dsps_repeat=1,
+            num_dsps_repeats=num_mosaic_repeats,
         )
         header_generator = (d.header() for d in ds)
         for s in range(1, num_steps + 1):
             dark_cal = np.zeros((10, 10)) + (s * 10)
             dark_hdul = fits.HDUList([fits.PrimaryHDU(data=dark_cal)])
             task.fits_data_write(
                 hdu_list=dark_hdul,
@@ -79,39 +79,39 @@
                     VbiTag.frame(),
                     VbiTag.task("GAIN"),
                     VbiTag.spatial_step(s),
                 ],
             )
 
             for e in range(num_exp_per_step):
-                for d in range(1, num_dsps_repeats + 1):
-                    if abort_mosaic and d == num_dsps_repeats and s > num_steps - 2:
+                for m in range(1, num_mosaic_repeats + 1):
+                    if abort_mosaic and m == num_mosaic_repeats and s > num_steps - 2:
                         # Abort the last two mosaic steps of the last DSPS repeat
                         continue
                     header = next(header_generator)
-                    data = (np.ones((1, 10, 10)) * (e + 1)) + s + (d * 10)
+                    data = (np.ones((1, 10, 10)) * (e + 1)) + s + (m * 10)
                     # Multiple by gain
                     data *= gain_cal
                     # Add dark
                     data += dark_cal
                     hdul = generate_214_l0_fits_frame(s122_header=header, data=data)
                     task.fits_data_write(
                         hdu_list=hdul,
                         tags=[
                             VbiTag.input(),
                             VbiTag.task("OBSERVE"),
                             VbiTag.spatial_step(s),
-                            VbiTag.dsps_repeat(d),
+                            VbiTag.mosaic(m),
                             VbiTag.frame(),
                             VbiTag.exposure_time(exp_time),
                         ],
                     )
         if not abort_mosaic:
             ensure_all_inputs_used(header_generator)
-        yield task, num_steps, num_exp_per_step, num_dsps_repeats - (1 * abort_mosaic)
+        yield task, num_steps, num_exp_per_step, num_mosaic_repeats - (1 * abort_mosaic)
         task.scratch.purge()
         task.constants._purge()
 
 
 @pytest.mark.parametrize(
     "abort_mosaic",
     [pytest.param(False, id="Full set"), pytest.param(True, id="Aborted last mosaic")],
@@ -121,40 +121,40 @@
     Given: a set of parsed input observe frames, dark and gain calibrations, and a ScienceCalibration task
     When: the task is run
     Then: the science frames are processed, no exposures are averaged, and the array values are correct
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
-    task, num_steps, num_exp_per_step, expected_num_dsps_repeats = science_calibration_task
+    task, num_steps, num_exp_per_step, expected_num_mosaic_repeats = science_calibration_task
     task()
 
     for s in range(1, num_steps + 1):
         tags = [
             VbiTag.calibrated(),
             VbiTag.frame(),
             VbiTag.spatial_step(s),
             VbiTag.stokes("I"),
         ]
         file_list = list(task.read(tags=tags))
         # Make sure any aborted mosaics didn't get processed
-        assert len(file_list) == num_exp_per_step * expected_num_dsps_repeats
+        assert len(file_list) == num_exp_per_step * expected_num_mosaic_repeats
 
-        for d in range(1, expected_num_dsps_repeats + 1):
+        for m in range(1, expected_num_mosaic_repeats + 1):
             sci_access_list = list(
                 task.fits_data_read_fits_access(
-                    tags=tags + [VbiTag.dsps_repeat(d)],
+                    tags=tags + [VbiTag.mosaic(m)],
                     cls=VbiL0FitsAccess,
                 )
             )
             assert len(sci_access_list) == num_exp_per_step
             sorted_access = sorted(sci_access_list, key=lambda x: np.mean(x.data))
             for e, obj in enumerate(sorted_access):
                 assert isinstance(obj._hdu, fits.CompImageHDU)
-                expected_array = (np.ones((10, 10)) * (e + 1)) + s + (d * 10)
+                expected_array = (np.ones((10, 10)) * (e + 1)) + s + (m * 10)
                 np.testing.assert_equal(expected_array, obj.data)
 
     input_obs_frames = list(
         task.read(tags=[VbiTag.input(), VbiTag.frame(), VbiTag.task("OBSERVE")])
     )
 
     quality_files = list(task.read(tags=[Tag.quality("TASK_TYPES")]))
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_vbi_base.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_vbi_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_vbi_constants.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_vbi_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/tests/test_write_l1.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/tests/test_write_l1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import logging
 from dataclasses import asdict
 from random import randint
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_fits_specifications import __version__ as spec_version
 from dkist_header_validator import spec122_validator
 from dkist_header_validator import spec214_validator
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tests.conftest import FakeGQLClient
+from logging42 import logger
 
 from dkist_processing_vbi.models.constants import VbiConstants
 from dkist_processing_vbi.tasks.write_l1 import VbiWriteL1Frame
 from dkist_processing_vbi.tests.conftest import VbiConstantsDb
 from dkist_processing_vbi.tests.conftest import VbiS122Headers
 
 
@@ -31,31 +31,31 @@
     header["CUNIT1"] = "m"
     header["CUNIT2"] = "arcsec"
     header["CUNIT3"] = "s"
     header["VBINSTP"] = 9
     header["VBISTP"] = 5
     header["VBINFRAM"] = 3
     header["VBICFRAM"] = 2
+    header["VBINMOSC"] = 3
+    header["VBICMOSC"] = 2
     header["DSPSNUM"] = 1002  # To mimic a large offset
     header["DATE-BEG"] = "2033-07-11T00:00:00"
     header["TEXPOSUR"] = 100
     return header
 
 
 @pytest.fixture(scope="session")
 def write_l1_task(calibrated_header):
     recipe_run_id = randint(0, 99999)
     constants_db = VbiConstantsDb(
         AVERAGE_CADENCE=10,
         MINIMUM_CADENCE=10,
         MAXIMUM_CADENCE=10,
         VARIANCE_CADENCE=0,
-        NUM_DSPS_REPEATS=2,
-        DSPS_REPEAT_PEDESTAL=1000,
-        SPECTRAL_LINE="VBI-Red H-alpha",
+        NUM_MOSAIC_REPEATS=3,
     )
     # Repeat ini_vbi_constants fixture here because of a scope conflict
     constants = VbiConstants(recipe_run_id=recipe_run_id, task_name="test")
     constants._update(asdict(constants_db))
     with VbiWriteL1Frame(
         recipe_run_id=recipe_run_id,
         workflow_name="workflow_name",
@@ -83,30 +83,29 @@
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
     task = write_l1_task
     task()
     files = list(task.read(tags=[Tag.frame(), Tag.output(), Tag.stokes("I")]))
     assert len(files) == 1
     for file in files:
-        logging.info(f"Checking file {file}")
+        logger.info(f"Checking file {file}")
         assert file.exists
         hdl = fits.open(file)
         assert len(hdl) == 2
         header = hdl[1].header
         assert spec214_validator.validate(input_headers=header, extra=False)
         assert header["DNAXIS1"] == 11
         assert header["DNAXIS2"] == 10
-        assert header["DNAXIS3"] == 6  # num_dsps * num_exp_per_dsp
+        assert header["DNAXIS3"] == header["VBINFRAM"] * header["VBINMOSC"]
         assert header["DINDEX3"] == 5
         assert header["DUNIT1"] == "m"
         assert header["DUNIT2"] == "arcsec"
         assert header["DUNIT3"] == "s"
         assert header["WAVEMIN"] == 656.258
         assert header["WAVEMAX"] == 656.306
-        assert header["WAVEBAND"] == "VBI-Red H-alpha"
         assert header["MAXIS1"] == 3
         assert header["MAXIS2"] == 3
         assert header["MINDEX1"] == 2
         assert header["MINDEX2"] == 2
         assert header["INFO_URL"] == task.docs_base_url
         assert header["HEADVERS"] == spec_version
         assert (
@@ -121,7 +120,11 @@
         assert header["DATE-END"] == "2033-07-11T00:00:00.100000"
         assert isinstance(header["HLSVERS"], str)
         assert header["PROPID01"] == "PROPID1"
         assert header["PROPID02"] == "PROPID2"
         assert header["EXPRID01"] == "EXPERID1"
         assert header["EXPRID02"] == "EXPERID2"
         assert header["EXPRID03"] == "EXPERID3"
+        assert header["WAVEBAND"] == "H alpha (656.28 nm)"
+        assert header["SPECLN01"] == "H alpha (656.28 nm)"
+        with pytest.raises(KeyError):
+            header["SPECLN02"]
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/workflows/l0_processing.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi/workflows/summit_data_processing.py` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi/workflows/summit_data_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/PKG-INFO` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-vbi
-Version: 1.1.9
+Version: 1.2.0
 Summary: Code that is used by the DKIST Science Data Processing Airflow pipelines to process VBI data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-vbi/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/vbi
 Classifier: Programming Language :: Python
@@ -108,7 +108,38 @@
     # Delete tags
     git tag -d vWHATEVER.THE.VERSION
     git push --delete origin vWHATEVER.THE.VERSION
 
     # Re-tag with the same version
     git tag vWHATEVER.THE.VERSION
     git push --tags origin main
+
+Science Changelog
+^^^^^^^^^^^^^^^^^
+
+Whenever a release involves changes to the scientific quality of L1 data, additional changelog fragment(s) should be
+created. These fragments are intended to be as verbose as is needed to accurately capture the scope of the change(s),
+so feel free to use all the fancy RST you want. Science fragments are placed in the same ``changelog/`` directory
+as other fragments, but are always called::
+
+  <PR NUMBER | +>.science[.<COUNTER>].rst
+
+In the case that a single pull request encapsulates the entirety of the scientific change then the first field should
+be that PR number (same as the normal CHANGELOG). If, however, there is not a simple mapping from a single PR to a scienctific
+change then use the character "+" instead; this will create a changelog entry with no associated PR. For example:
+
+.. code-block:: bash
+
+  $ ls changelog/
+  99.bugfix.rst    # This is a normal changelog fragment associated with a bugfix in PR 99
+  99.science.rst   # Apparently that bugfix also changed the scientific results, so that PR also gets a science fragment
+  +.science.rst    # This fragment is not associated with a PR
+
+
+When it comes time to build the SCIENCE_CHANGELOG, use the ``science_towncrier.sh`` script in this repo to do so.
+This script accepts all the same arguments as the default `towncrier`. For exmaple:
+
+.. code-block:: bash
+
+  ./science_towncrier.sh build --version vx.y.z
+
+This will update the SCIENCE_CHANGELOG and remove any science fragments from the changelog directory.
```

### Comparing `dkist_processing_vbi-1.1.9/dkist_processing_vbi.egg-info/SOURCES.txt` & `dkist_processing_vbi-1.2.0/dkist_processing_vbi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 CHANGELOG.rst
 README.rst
+SCIENCE_CHANGELOG.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
+science_towncrier.sh
 setup.cfg
 setup.py
+towncrier_science.toml
 changelog/.gitempty
 dkist_processing_vbi/__init__.py
 dkist_processing_vbi.egg-info/PKG-INFO
 dkist_processing_vbi.egg-info/SOURCES.txt
 dkist_processing_vbi.egg-info/dependency_links.txt
 dkist_processing_vbi.egg-info/requires.txt
 dkist_processing_vbi.egg-info/top_level.txt
 dkist_processing_vbi/models/__init__.py
 dkist_processing_vbi/models/constants.py
-dkist_processing_vbi/models/spectral_line.py
+dkist_processing_vbi/models/filter.py
 dkist_processing_vbi/models/tags.py
 dkist_processing_vbi/parsers/__init__.py
-dkist_processing_vbi/parsers/dsps_repeats.py
-dkist_processing_vbi/parsers/num_exp_per_dsp.py
-dkist_processing_vbi/parsers/spectral_line.py
+dkist_processing_vbi/parsers/mosaic_repeats.py
 dkist_processing_vbi/parsers/vbi_l0_fits_access.py
 dkist_processing_vbi/parsers/vbi_l1_fits_access.py
 dkist_processing_vbi/tasks/__init__.py
 dkist_processing_vbi/tasks/assemble_movie.py
 dkist_processing_vbi/tasks/dark.py
 dkist_processing_vbi/tasks/gain.py
 dkist_processing_vbi/tasks/make_movie_frames.py
@@ -63,8 +64,9 @@
 docs/conf.py
 docs/index.rst
 docs/l0_to_l1_vbi_no-speckle.rst
 docs/l0_to_l1_vbi_summit-calibrated.rst
 docs/make.bat
 docs/requirements.txt
 docs/requirements_table.rst
+docs/scientific_changelog.rst
 licenses/LICENSE.rst
```

### Comparing `dkist_processing_vbi-1.1.9/docs/Makefile` & `dkist_processing_vbi-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/docs/conf.py` & `dkist_processing_vbi-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/docs/l0_to_l1_vbi_no-speckle.rst` & `dkist_processing_vbi-1.2.0/docs/l0_to_l1_vbi_no-speckle.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/docs/l0_to_l1_vbi_summit-calibrated.rst` & `dkist_processing_vbi-1.2.0/docs/l0_to_l1_vbi_summit-calibrated.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/docs/make.bat` & `dkist_processing_vbi-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/licenses/LICENSE.rst` & `dkist_processing_vbi-1.2.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/pyproject.toml` & `dkist_processing_vbi-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.1.9/setup.cfg` & `dkist_processing_vbi-1.2.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -15,46 +15,48 @@
 
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 2.4.0
+	dkist-processing-common == 2.5.0
 	dkist-processing-math == 1.0.1
 	dkist-header-validator == 3.0.5
-	dkist-fits-specifications == 3.5.0
+	dkist-fits-specifications == 3.6.0
 	astropy == 5.1.1
 	numpy == 1.23.1
-	sunpy == 4.0.3
+	sunpy == 4.1.4
 	scipy == 1.9.0
 	pillow == 9.2.0
 	moviepy == 1.0.3
+	dkist-spectral-lines == 1.0.0
+	logging42 == 0.0.8
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 	pytest-mock
 	pytest-xdist
 	towncrier
 	dkist-data-simulator >= 2.1.0
 grogu = 
-	dkist == 1.0.0b9
+	dkist == 1.0.0b11
 	asdf == 2.10.1
 	pyparsing
-	dkist-inventory == 0.12.0
+	dkist-inventory == 0.16.0
 	parfive < 2.0.0
 docs = 
 	sphinx
 	sphinx-astropy
-	sphinx-changelog
+	sphinx-changelog == 1.3.0
 	sphinx-autoapi
 	pytest
-	towncrier < 22.12.0
+	towncrier == 22.12.0
 	dkist-sphinx-theme
 
 [build_docs]
 source-dir = docs
 build-dir = docs/_build
 all_files = 1
```

