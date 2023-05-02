# Comparing `tmp/plugincode-31.0.0b1.tar.gz` & `tmp/plugincode-32.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugincode-31.0.0b1.tar", last modified: Tue May 17 12:41:22 2022, max compression
+gzip compressed data, was "plugincode-32.0.0.tar", last modified: Tue May  2 19:12:58 2023, max compression
```

## Comparing `plugincode-31.0.0b1.tar` & `plugincode-32.0.0.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.877720 plugincode-31.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.869720 plugincode-31.0.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.873720 plugincode-31.0.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/.github/workflows/docs-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3422 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-05-17 12:41:22.877720 plugincode-31.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/azure-pipelines.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)     6010 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/configure
--rw-r--r--   0 runner    (1001) docker     (121)     6930 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/configure.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.873720 plugincode-31.0.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.873720 plugincode-31.0.0b1/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/docs/scripts/doc8_style_check.sh
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/docs/scripts/sphinx_build_link_check.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.873720 plugincode-31.0.0b1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.873720 plugincode-31.0.0b1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     8022 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/docs/source/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (121)     3123 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.873720 plugincode-31.0.0b1/docs/source/contribute/
--rw-r--r--   0 runner    (1001) docker     (121)    10245 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/docs/source/contribute/contrib_doc.rst
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5491 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/docs/source/skeleton-usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.869720 plugincode-31.0.0b1/etc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.873720 plugincode-31.0.0b1/etc/ci/
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/ci/azure-container-deb.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/ci/azure-container-rpm.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/ci/azure-posix.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/ci/azure-win.yml
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/ci/install_sudo.sh
--rw-r--r--   0 runner    (1001) docker     (121)     8365 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/ci/macports-ci
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/ci/macports-ci.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/ci/mit.LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.877720 plugincode-31.0.0b1/etc/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3745 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/check_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (121)     8209 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/fetch_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (121)     9595 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/gen_pypi_simple.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/gen_pypi_simple.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/gen_pypi_simple.py.NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/gen_requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/gen_requirements_dev.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4497 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/test_utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/test_utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     6419 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/utils_dejacode.py
--rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     6141 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/utils_requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)    75924 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/utils_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/etc/scripts/utils_thirdparty.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/plugincode.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-05-17 12:41:22.877720 plugincode-31.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.869720 plugincode-31.0.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.877720 plugincode-31.0.0b1/src/plugincode/
--rw-r--r--   0 runner    (1001) docker     (121)     9020 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/src/plugincode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5776 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/src/plugincode/location_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/src/plugincode/output.py
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/src/plugincode/output_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/src/plugincode/post_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/src/plugincode/pre_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     3343 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/src/plugincode/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.877720 plugincode-31.0.0b1/src/plugincode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-05-17 12:41:22.000000 plugincode-31.0.0b1/src/plugincode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-05-17 12:41:22.000000 plugincode-31.0.0b1/src/plugincode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-17 12:41:22.000000 plugincode-31.0.0b1/src/plugincode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-17 12:41:22.000000 plugincode-31.0.0b1/src/plugincode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-05-17 12:41:22.000000 plugincode-31.0.0b1/src/plugincode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-05-17 12:41:22.000000 plugincode-31.0.0b1/src/plugincode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.877720 plugincode-31.0.0b1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 12:41:22.877720 plugincode-31.0.0b1/tests/plugincode/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/tests/plugincode/test_plugincode.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-05-17 12:41:05.000000 plugincode-31.0.0b1/tests/test_skeleton_codestyle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.643075 plugincode-32.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-02 19:12:48.000000 plugincode-32.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.631075 plugincode-32.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.635075 plugincode-32.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-05-02 19:12:48.000000 plugincode-32.0.0/.github/workflows/docs-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-05-02 19:12:48.000000 plugincode-32.0.0/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-05-02 19:12:48.000000 plugincode-32.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-05-02 19:12:48.000000 plugincode-32.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-02 19:12:48.000000 plugincode-32.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-05-02 19:12:48.000000 plugincode-32.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3422 2023-05-02 19:12:48.000000 plugincode-32.0.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-05-02 19:12:48.000000 plugincode-32.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-05-02 19:12:48.000000 plugincode-32.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-05-02 19:12:48.000000 plugincode-32.0.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-05-02 19:12:58.643075 plugincode-32.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-02 19:12:48.000000 plugincode-32.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-02 19:12:48.000000 plugincode-32.0.0/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-02 19:12:48.000000 plugincode-32.0.0/appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-05-02 19:12:48.000000 plugincode-32.0.0/azure-pipelines.yml
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6328 2023-05-02 19:12:48.000000 plugincode-32.0.0/configure
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-05-02 19:12:48.000000 plugincode-32.0.0/configure.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.635075 plugincode-32.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-02 19:12:48.000000 plugincode-32.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-05-02 19:12:48.000000 plugincode-32.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.635075 plugincode-32.0.0/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-05-02 19:12:48.000000 plugincode-32.0.0/docs/scripts/doc8_style_check.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-02 19:12:48.000000 plugincode-32.0.0/docs/scripts/sphinx_build_link_check.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.635075 plugincode-32.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.635075 plugincode-32.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)     8022 2023-05-02 19:12:48.000000 plugincode-32.0.0/docs/source/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-05-02 19:12:48.000000 plugincode-32.0.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.635075 plugincode-32.0.0/docs/source/contribute/
+-rw-r--r--   0 runner    (1001) docker     (122)    10245 2023-05-02 19:12:48.000000 plugincode-32.0.0/docs/source/contribute/contrib_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-05-02 19:12:48.000000 plugincode-32.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-05-02 19:12:48.000000 plugincode-32.0.0/docs/source/skeleton-usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.631075 plugincode-32.0.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.639075 plugincode-32.0.0/etc/ci/
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/ci/azure-container-deb.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/ci/azure-container-rpm.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/ci/azure-posix.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/ci/azure-win.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/ci/install_sudo.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     8365 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/ci/macports-ci
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/ci/macports-ci.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/ci/mit.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.639075 plugincode-32.0.0/etc/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3744 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/check_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9486 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/fetch_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9699 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/gen_pypi_simple.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/gen_pypi_simple.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/gen_pypi_simple.py.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/gen_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/gen_requirements_dev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4497 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/test_utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/test_utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     6418 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/utils_dejacode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6704 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     6152 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/utils_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75931 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/utils_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-05-02 19:12:48.000000 plugincode-32.0.0/etc/scripts/utils_thirdparty.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-02 19:12:48.000000 plugincode-32.0.0/plugincode.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-05-02 19:12:48.000000 plugincode-32.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-05-02 19:12:48.000000 plugincode-32.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-05-02 19:12:48.000000 plugincode-32.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-02 19:12:58.643075 plugincode-32.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-02 19:12:48.000000 plugincode-32.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.631075 plugincode-32.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.639075 plugincode-32.0.0/src/plugincode/
+-rw-r--r--   0 runner    (1001) docker     (122)     9090 2023-05-02 19:12:48.000000 plugincode-32.0.0/src/plugincode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-05-02 19:12:48.000000 plugincode-32.0.0/src/plugincode/location_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2657 2023-05-02 19:12:48.000000 plugincode-32.0.0/src/plugincode/output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-05-02 19:12:48.000000 plugincode-32.0.0/src/plugincode/output_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-05-02 19:12:48.000000 plugincode-32.0.0/src/plugincode/post_scan.py
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-05-02 19:12:48.000000 plugincode-32.0.0/src/plugincode/pre_scan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3343 2023-05-02 19:12:48.000000 plugincode-32.0.0/src/plugincode/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.643075 plugincode-32.0.0/src/plugincode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-05-02 19:12:58.000000 plugincode-32.0.0/src/plugincode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-05-02 19:12:58.000000 plugincode-32.0.0/src/plugincode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 19:12:58.000000 plugincode-32.0.0/src/plugincode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 19:12:58.000000 plugincode-32.0.0/src/plugincode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-02 19:12:58.000000 plugincode-32.0.0/src/plugincode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-02 19:12:58.000000 plugincode-32.0.0/src/plugincode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.643075 plugincode-32.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 19:12:58.643075 plugincode-32.0.0/tests/plugincode/
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-05-02 19:12:48.000000 plugincode-32.0.0/tests/plugincode/test_plugincode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-05-02 19:12:48.000000 plugincode-32.0.0/tests/test_skeleton_codestyle.py
```

### Comparing `plugincode-31.0.0b1/.github/workflows/docs-ci.yml` & `plugincode-32.0.0/.github/workflows/docs-ci.yml`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/.github/workflows/pypi-release.yml` & `plugincode-32.0.0/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/.gitignore` & `plugincode-32.0.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Python compiled files
 *.py[cod]
 
 # virtualenv and other misc bits
+/src/*.egg-info
 *.egg-info
 /dist
 /build
 /bin
 /lib
 /scripts
 /Scripts
```

### Comparing `plugincode-31.0.0b1/CODE_OF_CONDUCT.rst` & `plugincode-32.0.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/NOTICE` & `plugincode-32.0.0/NOTICE`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/PKG-INFO` & `plugincode-32.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: plugincode
-Version: 31.0.0b1
+Version: 32.0.0
 Summary: plugincode is a library that provides plugin functionality for ScanCode toolkit.
 Home-page: https://github.com/nexB/plugincode
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: open source,utilities,plugincode,scancode,scancode-toolkit,plugins,open source,plugin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6.*
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: apache-2.0.LICENSE
 License-File: NOTICE
 License-File: AUTHORS.rst
 License-File: CHANGELOG.rst
```

### Comparing `plugincode-31.0.0b1/README.rst` & `plugincode-32.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/apache-2.0.LICENSE` & `plugincode-32.0.0/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/appveyor.yml` & `plugincode-32.0.0/appveyor.yml`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/configure` & `plugincode-32.0.0/configure`

 * *Files 17% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 DEV_REQUIREMENTS="--editable .[testing] --constraint requirements.txt --constraint requirements-dev.txt"
 DOCS_REQUIREMENTS="--editable .[docs] --constraint requirements.txt"
 
 # where we create a virtualenv
 VIRTUALENV_DIR=venv
 
 # Cleanable files and directories to delete with the --clean option
-CLEANABLE="build venv"
+CLEANABLE="build dist venv .cache .eggs"
 
 # extra  arguments passed to pip
 PIP_EXTRA_ARGS=" "
 
 # the URL to download virtualenv.pyz if needed
 VIRTUALENV_PYZ_URL=https://bootstrap.pypa.io/virtualenv.pyz
 ################################
@@ -49,20 +49,29 @@
 ################################
 # Current directory where this script lives
 CFG_ROOT_DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" && pwd )"
 CFG_BIN_DIR=$CFG_ROOT_DIR/$VIRTUALENV_DIR/bin
 
 
 ################################
+# Install with or without and index. With "--no-index" this is using only local wheels
+# This is an offline mode with no index and no network operations
+# NO_INDEX="--no-index "
+NO_INDEX=""
+
+
+################################
 # Thirdparty package locations and index handling
-# Find packages from the local thirdparty directory
-if [ -d "$CFG_ROOT_DIR/thirdparty" ]; then
-    PIP_EXTRA_ARGS="--find-links $CFG_ROOT_DIR/thirdparty"
+# Find packages from the local thirdparty directory if present
+THIRDPARDIR=$CFG_ROOT_DIR/thirdparty
+if [[ "$(echo $THIRDPARDIR/*.whl)x" != "$THIRDPARDIR/*.whlx" ]]; then
+    PIP_EXTRA_ARGS="$NO_INDEX --find-links $THIRDPARDIR"
 fi
 
+
 ################################
 # Set the quiet flag to empty if not defined
 if [[ "$CFG_QUIET" == "" ]]; then
     CFG_QUIET=" "
 fi
 
 
@@ -177,14 +186,15 @@
                 clean ) find_python && clean;;
                 dev   ) CFG_REQUIREMENTS="$DEV_REQUIREMENTS";;
                 docs   ) CFG_REQUIREMENTS="$DOCS_REQUIREMENTS";;
             esac;;
     esac
 done
 
+
 PIP_EXTRA_ARGS="$PIP_EXTRA_ARGS"
 
 find_python
 create_virtualenv "$VIRTUALENV_DIR"
 install_packages "$CFG_REQUIREMENTS"
 . "$CFG_BIN_DIR/activate"
```

### Comparing `plugincode-31.0.0b1/configure.bat` & `plugincode-32.0.0/configure.bat`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 set "DEV_REQUIREMENTS=--editable .[testing] --constraint requirements.txt --constraint requirements-dev.txt"
 set "DOCS_REQUIREMENTS=--editable .[docs] --constraint requirements.txt"
 
 @rem # where we create a virtualenv
 set "VIRTUALENV_DIR=venv"
 
 @rem # Cleanable files and directories to delete with the --clean option
-set "CLEANABLE=build venv"
+set "CLEANABLE=build dist venv .cache .eggs"
 
 @rem # extra  arguments passed to pip
 set "PIP_EXTRA_ARGS= "
 
 @rem # the URL to download virtualenv.pyz if needed
 set VIRTUALENV_PYZ_URL=https://bootstrap.pypa.io/virtualenv.pyz
 @rem ################################
```

### Comparing `plugincode-31.0.0b1/docs/Makefile` & `plugincode-32.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/docs/make.bat` & `plugincode-32.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/docs/source/_static/theme_overrides.css` & `plugincode-32.0.0/docs/source/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/docs/source/conf.py` & `plugincode-32.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/docs/source/contribute/contrib_doc.rst` & `plugincode-32.0.0/docs/source/contribute/contrib_doc.rst`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/docs/source/skeleton-usage.rst` & `plugincode-32.0.0/docs/source/skeleton-usage.rst`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/ci/azure-container-deb.yml` & `plugincode-32.0.0/etc/ci/azure-container-deb.yml`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/ci/azure-container-rpm.yml` & `plugincode-32.0.0/etc/ci/azure-container-rpm.yml`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/ci/azure-posix.yml` & `plugincode-32.0.0/etc/ci/azure-posix.yml`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/ci/azure-win.yml` & `plugincode-32.0.0/etc/ci/azure-win.yml`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/ci/macports-ci` & `plugincode-32.0.0/etc/ci/macports-ci`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/ci/macports-ci.ABOUT` & `plugincode-32.0.0/etc/ci/macports-ci.ABOUT`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/ci/mit.LICENSE` & `plugincode-32.0.0/etc/ci/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/scripts/README.rst` & `plugincode-32.0.0/etc/scripts/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -17,28 +17,28 @@
     virtualenv as instructed below (This is to avoid injecting requirements
     specific to the tools used here in the main requirements).
 
   * For other usages, the tools here can run either in their own isolated
     virtualenv or in the the main configured development virtualenv.
     These requireements need to be installed::
 
-        pip install --requirement etc/release/requirements.txt
+        pip install --requirement etc/scripts/requirements.txt
 
 TODO: we need to pin the versions of these tools
 
 
 
 Generate or update pip requirement files
 ----------------------------------------
 
 Scripts
 ~~~~~~~
 
 **gen_requirements.py**: create/update requirements files from currently
-  installed requirements. 
+  installed requirements.
 
 **gen_requirements_dev.py** does the same but can subtract the main requirements
   to get extra requirements used in only development.
 
 
 Usage
 ~~~~~
@@ -46,24 +46,24 @@
 The sequence of commands to run are:
 
 
 * Start with these to generate the main pip requirements file::
 
     ./configure --clean
     ./configure
-    python etc/release/gen_requirements.py --site-packages-dir <path to site-packages dir>
+    python etc/scripts/gen_requirements.py --site-packages-dir <path to site-packages dir>
 
 * You can optionally install or update extra main requirements after the
   ./configure step such that these are included in the generated main requirements.
 
 * Optionally, generate a development pip requirements file by running these::
 
     ./configure --clean
     ./configure --dev
-    python etc/release/gen_requirements_dev.py --site-packages-dir <path to site-packages dir>
+    python etc/scripts/gen_requirements_dev.py --site-packages-dir <path to site-packages dir>
 
 * You can optionally install or update extra dev requirements after the
   ./configure step such that these are included in the generated dev
   requirements.
 
 Notes: we generate development requirements after the main as this step requires
 the main requirements.txt to be up-to-date first. See **gen_requirements.py and
```

### Comparing `plugincode-31.0.0b1/etc/scripts/check_thirdparty.py` & `plugincode-32.0.0/etc/scripts/check_thirdparty.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/scripts/fetch_thirdparty.py` & `plugincode-32.0.0/etc/scripts/fetch_thirdparty.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # See https://github.com/nexB/skeleton for support or download.
 # See https://aboutcode.org for more information about nexB OSS projects.
 #
 
 import itertools
 import os
 import sys
+from collections import defaultdict
 
 import click
 
 import utils_thirdparty
 import utils_requirements
 
 TRACE = False
@@ -106,26 +107,62 @@
     help="PyPI index URL(s) to use for wheels and sources, in order of preferences.",
 )
 @click.option(
     "--use-cached-index",
     is_flag=True,
     help="Use on disk cached PyPI indexes list of packages and versions and do not refetch if present.",
 )
+@click.option(
+    "--sdist-only",
+    "sdist_only",
+    type=str,
+    metavar="SDIST",
+    default=tuple(),
+    show_default=False,
+    multiple=True,
+    help="Package name(s) that come only in sdist format (no wheels). "
+         "The command will not fail and exit if no wheel exists for these names",
+)
+@click.option(
+    "--wheel-only",
+    "wheel_only",
+    type=str,
+    metavar="WHEEL",
+    default=tuple(),
+    show_default=False,
+    multiple=True,
+    help="Package name(s) that come only in wheel format (no sdist). "
+         "The command will not fail and exit if no sdist exists for these names",
+)
+@click.option(
+    "--no-dist",
+    "no_dist",
+    type=str,
+    metavar="DIST",
+    default=tuple(),
+    show_default=False,
+    multiple=True,
+    help="Package name(s) that do not come either in wheel or sdist format. "
+         "The command will not fail and exit if no distribution exists for these names",
+)
 @click.help_option("-h", "--help")
 def fetch_thirdparty(
     requirements_files,
     specifiers,
     latest_version,
     dest_dir,
     python_versions,
     operating_systems,
     wheels,
     sdists,
     index_urls,
     use_cached_index,
+    sdist_only,
+    wheel_only,
+    no_dist,
 ):
     """
     Download to --dest THIRDPARTY_DIR the PyPI wheels, source distributions,
     and their ABOUT metadata, license and notices files.
 
     Download the PyPI packages listed in the combination of:
     - the pip requirements --requirements REQUIREMENT-FILE(s),
@@ -200,66 +237,70 @@
         else:
             repo = utils_thirdparty.PypiSimpleRepository(
                 index_url=index_url,
                 use_cached_index=use_cached_index,
             )
             repos.append(repo)
 
-    wheels_fetched = []
-    wheels_not_found = []
-
-    sdists_fetched = []
-    sdists_not_found = []
+    wheels_or_sdist_not_found = defaultdict(list)
 
     for name, version in sorted(required_name_versions):
         nv = name, version
         print(f"Processing: {name} @ {version}")
         if wheels:
             for environment in environments:
+
                 if TRACE:
                     print(f"  ==> Fetching wheel for envt: {environment}")
-                fwfns = utils_thirdparty.download_wheel(
+
+                fetched = utils_thirdparty.download_wheel(
                     name=name,
                     version=version,
                     environment=environment,
                     dest_dir=dest_dir,
                     repos=repos,
                 )
-                if fwfns:
-                    wheels_fetched.extend(fwfns)
-                else:
-                    wheels_not_found.append(f"{name}=={version} for: {environment}")
+                if not fetched:
+                    wheels_or_sdist_not_found[f"{name}=={version}"].append(environment)
                     if TRACE:
                         print(f"      NOT FOUND")
 
-        if sdists:
+        if (sdists or
+            (f"{name}=={version}" in wheels_or_sdist_not_found and name in sdist_only)
+         ):
             if TRACE:
                 print(f"  ==> Fetching sdist: {name}=={version}")
+
             fetched = utils_thirdparty.download_sdist(
                 name=name,
                 version=version,
                 dest_dir=dest_dir,
                 repos=repos,
             )
-            if fetched:
-                sdists_fetched.append(fetched)
-            else:
-                sdists_not_found.append(f"{name}=={version}")
+            if not fetched:
+                wheels_or_sdist_not_found[f"{name}=={version}"].append("sdist")
                 if TRACE:
                     print(f"      NOT FOUND")
 
-    if wheels and wheels_not_found:
-        print(f"==> MISSING WHEELS")
-        for wh in wheels_not_found:
-            print(f"  {wh}")
-
-    if sdists and sdists_not_found:
-        print(f"==> MISSING SDISTS")
-        for sd in sdists_not_found:
-            print(f"  {sd}")
+    mia = []
+    for nv, dists in wheels_or_sdist_not_found.items():
+        name, _, version = nv.partition("==")
+        if name in no_dist:
+            continue
+        sdist_missing = sdists and "sdist" in dists and not name in wheel_only
+        if sdist_missing:
+            mia.append(f"SDist missing: {nv} {dists}")
+        wheels_missing = wheels and any(d for d in dists if d != "sdist") and not name in sdist_only
+        if wheels_missing:
+            mia.append(f"Wheels missing: {nv} {dists}")
+
+    if mia:
+        for m in mia:
+            print(m)
+        raise Exception(mia)
 
     print(f"==> FETCHING OR CREATING ABOUT AND LICENSE FILES")
     utils_thirdparty.fetch_abouts_and_licenses(dest_dir=dest_dir, use_cached_index=use_cached_index)
     utils_thirdparty.clean_about_files(dest_dir=dest_dir)
 
     # check for problems
     print(f"==> CHECK FOR PROBLEMS")
```

### Comparing `plugincode-31.0.0b1/etc/scripts/gen_pypi_simple.py` & `plugincode-32.0.0/etc/scripts/gen_pypi_simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,15 +114,15 @@
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Links for {pkg_name}</title>
   </head>
   <body>"""
     document.append(header)
 
-    for package in packages:
+    for package in sorted(packages, key=lambda p: p.archive_file):
         document.append(package.simple_index_entry(base_url))
 
     footer = """  </body>
 </html>
 """
     document.append(footer)
     return "\n".join(document)
@@ -137,16 +137,16 @@
 <html>
   <head>
     <title>Links for all packages</title>
   </head>
   <body>"""
     document.append(header)
 
-    for _name, packages in packages_by_package_name.items():
-        for package in packages:
+    for _name, packages in sorted(packages_by_package_name.items(), key=lambda i: i[0]):
+        for package in sorted(packages, key=lambda p: p.archive_file):
             document.append(package.simple_index_entry(base_url))
 
     footer = """  </body>
 </html>
 """
     document.append(footer)
     return "\n".join(document)
```

### Comparing `plugincode-31.0.0b1/etc/scripts/gen_pypi_simple.py.NOTICE` & `plugincode-32.0.0/etc/scripts/gen_pypi_simple.py.NOTICE`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/scripts/gen_requirements.py` & `plugincode-32.0.0/etc/scripts/gen_requirements.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/scripts/gen_requirements_dev.py` & `plugincode-32.0.0/etc/scripts/gen_requirements_dev.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/scripts/test_utils_pip_compatibility_tags.py` & `plugincode-32.0.0/etc/scripts/test_utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/scripts/test_utils_pypi_supported_tags.py` & `plugincode-32.0.0/etc/scripts/test_utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT` & `plugincode-32.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/scripts/utils_dejacode.py` & `plugincode-32.0.0/etc/scripts/utils_dejacode.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import io
 import os
 import zipfile
 
 import requests
 import saneyaml
 
-from packaging import version as packaging_version
+from packvers import version as packaging_version
 
 """
 Utility to create and retrieve package and ABOUT file data from DejaCode.
 """
 
 DEJACODE_API_KEY = os.environ.get("DEJACODE_API_KEY", "")
 DEJACODE_API_URL = os.environ.get("DEJACODE_API_URL", "")
```

### Comparing `plugincode-31.0.0b1/etc/scripts/utils_pip_compatibility_tags.py` & `plugincode-32.0.0/etc/scripts/utils_pip_compatibility_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 import re
 
-from packaging.tags import (
+from packvers.tags import (
     compatible_tags,
     cpython_tags,
     generic_tags,
     interpreter_name,
     interpreter_version,
     mac_platforms,
 )
```

### Comparing `plugincode-31.0.0b1/etc/scripts/utils_pypi_supported_tags.py` & `plugincode-32.0.0/etc/scripts/utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/scripts/utils_pypi_supported_tags.py.ABOUT` & `plugincode-32.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/etc/scripts/utils_requirements.py` & `plugincode-32.0.0/etc/scripts/utils_requirements.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # Copyright (c) nexB Inc. and others. All rights reserved.
 # ScanCode is a trademark of nexB Inc.
 # SPDX-License-Identifier: Apache-2.0
 # See http://www.apache.org/licenses/LICENSE-2.0 for the license text.
 # See https://github.com/nexB/skeleton for support or download.
 # See https://aboutcode.org for more information about nexB OSS projects.
 #
+
+import os
 import re
 import subprocess
 
 """
 Utilities to manage requirements files and call pip.
 NOTE: this should use ONLY the standard library and not import anything else
 because this is used for boostrapping with no requirements installed.
```

### Comparing `plugincode-31.0.0b1/etc/scripts/utils_thirdparty.py` & `plugincode-32.0.0/etc/scripts/utils_thirdparty.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 import license_expression
 import packageurl
 import requests
 import saneyaml
 from commoncode import fileutils
 from commoncode.hash import multi_checksums
 from commoncode.text import python_safe_name
-from packaging import tags as packaging_tags
-from packaging import version as packaging_version
+from packvers import tags as packaging_tags
+from packvers import version as packaging_version
 
 import utils_pip_compatibility_tags
 
 """
 Utilities to manage Python thirparty libraries source, binaries and metadata in
 local directories and remote repositories.
 
@@ -111,18 +111,17 @@
 """
 
 TRACE = False
 TRACE_DEEP = False
 TRACE_ULTRA_DEEP = False
 
 # Supported environments
-PYTHON_VERSIONS = "36", "37", "38", "39", "310"
+PYTHON_VERSIONS = "37", "38", "39", "310"
 
 PYTHON_DOT_VERSIONS_BY_VER = {
-    "36": "3.6",
     "37": "3.7",
     "38": "3.8",
     "39": "3.9",
     "310": "3.10",
 }
 
 
@@ -130,15 +129,14 @@
     """
     Return a dot version from a plain, non-dot version.
     """
     return PYTHON_DOT_VERSIONS_BY_VER[version]
 
 
 ABIS_BY_PYTHON_VERSION = {
-    "36": ["cp36", "cp36m", "abi3"],
     "37": ["cp37", "cp37m", "abi3"],
     "38": ["cp38", "cp38m", "abi3"],
     "39": ["cp39", "cp39m", "abi3"],
     "310": ["cp310", "cp310m", "abi3"],
 }
 
 PLATFORMS_BY_OS = {
@@ -908,15 +906,15 @@
         raw_data = email.message_from_string(pkginfo_text)
 
         classifiers = raw_data.get_all("Classifier") or []
 
         declared_license = [raw_data["License"]] + [
             c for c in classifiers if c.startswith("License")
         ]
-        license_expression = compute_normalized_license_expression(declared_license)
+        license_expression = get_license_expression(declared_license)
         other_classifiers = [c for c in classifiers if not c.startswith("License")]
 
         holder = raw_data["Author"]
         holder_contact = raw_data["Author-email"]
         copyright_statement = f"Copyright (c) {holder} <{holder_contact}>"
 
         pkginfo_data = dict(
@@ -1333,18 +1331,18 @@
     def package_from_dists(cls, dists):
         """
         Return a new PypiPackage built from an iterable of Wheels and Sdist
         objects all for the same package name and version.
 
         For example:
         >>> w1 = Wheel(name='bitarray', version='0.8.1', build='',
-        ...    python_versions=['cp36'], abis=['cp36m'],
+        ...    python_versions=['cp38'], abis=['cp38m'],
         ...    platforms=['linux_x86_64'])
         >>> w2 = Wheel(name='bitarray', version='0.8.1', build='',
-        ...    python_versions=['cp36'], abis=['cp36m'],
+        ...    python_versions=['cp38'], abis=['cp38m'],
         ...    platforms=['macosx_10_9_x86_64', 'macosx_10_10_x86_64'])
         >>> sd = Sdist(name='bitarray', version='0.8.1')
         >>> package = PypiPackage.package_from_dists(dists=[w1, w2, sd])
         >>> assert package.name == 'bitarray'
         >>> assert package.version == '0.8.1'
         >>> assert package.sdist == sd
         >>> assert package.wheels == [w1, w2]
@@ -1674,14 +1672,15 @@
     def get_package_version(self, name, version=None):
         """
         Return the PypiPackage with name and version or None.
         Return the latest PypiPackage version if version is None.
         """
         if not version:
             versions = list(self._get_package_versions_map(name).values())
+            # return the latest version
             return versions and versions[-1]
         else:
             return self._get_package_versions_map(name).get(version)
 
     def fetch_links(self, normalized_name):
         """
         Return a list of download link URLs found in a PyPI simple index for package
@@ -2269,21 +2268,21 @@
                 print(f"   Invalid checksums in file://{abpth}")
             if not dist.sha1 and dist.md5:
                 print(f"   Missing checksums in file://{abpth}")
 
     check_about(dest_dir=dest_dir)
 
 
-def compute_normalized_license_expression(declared_licenses):
+def get_license_expression(declared_licenses):
     """
     Return a normalized license expression or None.
     """
     if not declared_licenses:
         return
     try:
-        from packagedcode import pypi
+        from packagedcode.licensing import get_only_expression_from_extracted_license
 
-        return pypi.compute_normalized_license(declared_licenses)
+        return get_only_expression_from_extracted_license(declared_licenses)
     except ImportError:
         # Scancode is not installed, clean and join all the licenses
         lics = [python_safe_name(l).lower() for l in declared_licenses]
         return " AND ".join(lics).lower()
```

### Comparing `plugincode-31.0.0b1/etc/scripts/utils_thirdparty.py.ABOUT` & `plugincode-32.0.0/etc/scripts/utils_thirdparty.py.ABOUT`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/pyproject.toml` & `plugincode-32.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/setup.cfg` & `plugincode-32.0.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -8,19 +8,14 @@
 author = nexB. Inc. and others
 author_email = info@aboutcode.org
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 	Topic :: Software Development
 	Topic :: Utilities
 keywords = 
 	open source
 	utilities
 	plugincode
 	scancode
@@ -38,29 +33,32 @@
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = true
 zip_safe = false
 setup_requires = setuptools_scm[toml] >= 4
-python_requires = >=3.6.*
+python_requires = >=3.7
 install_requires = 
 	click >= 6.7, !=7.0
-	commoncode >= 30.2.0
+	commoncode >= 31.0.0
 	pluggy >= 0.12.0
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 testing = 
 	pytest >= 6, != 7.0.0
 	pytest-xdist >= 2
-	aboutcode-toolkit >= 6.0.0
+	aboutcode-toolkit >= 7.0.2
+	pycodestyle >= 2.8.0
+	twine
 	black
+	isort
 docs = 
 	Sphinx >= 3.3.1
 	sphinx-rtd-theme >= 0.5.0
 	doc8 >= 0.8.1
 
 [egg_info]
 tag_build =
```

### Comparing `plugincode-31.0.0b1/src/plugincode/__init__.py` & `plugincode-32.0.0/src/plugincode/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,20 +90,23 @@
     # A ScanCode run will fail with an error if these attributes are not
     # provided either as part of the scan data if resuing an existing scan or by
     # another plugin.
     # Subclasses should set this as needed.
     required_resource_attributes = []
 
     # A relative sort order number (integer or float).
-    # This is used to compute the order in which a plugin runs before
-    # another plugin in a given stage
-    # This is also used in scan results, results from scanners are sorted by
+    # This is used in scan results, results from scanners are sorted by
     # this sort_order then by plugin "name".
     sort_order = 100
 
+    # A relative run order number (integer or float).
+    # This is used to compute the order in which a plugin runs before
+    # another plugin in a given stage
+    run_order = 100
+
     # flag set to True once this plugin class has been initialized by calling it
     # setup() class method.
     # This is set automatically when a plugin class is loaded in its manager.
     # Subclasses must not set this.
     initialized = False
 
     def __init__(self, *args, **kwargs):
```

### Comparing `plugincode-31.0.0b1/src/plugincode/location_provider.py` & `plugincode-32.0.0/src/plugincode/location_provider.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/src/plugincode/output.py` & `plugincode-32.0.0/src/plugincode/output.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/src/plugincode/output_filter.py` & `plugincode-32.0.0/src/plugincode/output_filter.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/src/plugincode/post_scan.py` & `plugincode-32.0.0/src/plugincode/post_scan.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/src/plugincode/pre_scan.py` & `plugincode-32.0.0/src/plugincode/pre_scan.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/src/plugincode/scan.py` & `plugincode-32.0.0/src/plugincode/scan.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/src/plugincode.egg-info/PKG-INFO` & `plugincode-32.0.0/src/plugincode.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: plugincode
-Version: 31.0.0b1
+Version: 32.0.0
 Summary: plugincode is a library that provides plugin functionality for ScanCode toolkit.
 Home-page: https://github.com/nexB/plugincode
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: open source,utilities,plugincode,scancode,scancode-toolkit,plugins,open source,plugin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6.*
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: apache-2.0.LICENSE
 License-File: NOTICE
 License-File: AUTHORS.rst
 License-File: CHANGELOG.rst
```

### Comparing `plugincode-31.0.0b1/src/plugincode.egg-info/SOURCES.txt` & `plugincode-32.0.0/src/plugincode.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitattributes
 .gitignore
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CODE_OF_CONDUCT.rst
 MANIFEST.in
+Makefile
 NOTICE
 README.rst
 apache-2.0.LICENSE
 appveyor.yml
 azure-pipelines.yml
 configure
 configure.bat
```

### Comparing `plugincode-31.0.0b1/tests/plugincode/test_plugincode.py` & `plugincode-32.0.0/tests/plugincode/test_plugincode.py`

 * *Files identical despite different names*

### Comparing `plugincode-31.0.0b1/tests/test_skeleton_codestyle.py` & `plugincode-32.0.0/tests/test_skeleton_codestyle.py`

 * *Files identical despite different names*

