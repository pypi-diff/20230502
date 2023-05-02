# Comparing `tmp/magic-folder-23.3.1.tar.gz` & `tmp/magic-folder-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic-folder-23.3.1.tar", last modified: Mon Mar 20 18:13:24 2023, max compression
+gzip compressed data, was "magic-folder-23.5.0.tar", last modified: Tue May  2 18:45:15 2023, max compression
```

## Comparing `magic-folder-23.3.1.tar` & `magic-folder-23.5.0.tar`

### file list

```diff
@@ -1,671 +1,672 @@
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.173080 magic-folder-23.3.1/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      207 2022-02-03 01:05:52.000000 magic-folder-23.3.1/.coveragerc
--rw-r--r--   0 meejah    (1000) meejah    (1000)      324 2022-09-20 06:29:38.000000 magic-folder-23.3.1/.flake8
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.053080 magic-folder-23.3.1/.github/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:36:41.000000 magic-folder-23.3.1/.github/pull_request_template.md
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.053080 magic-folder-23.3.1/.github/workflows/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      935 2023-01-20 00:19:51.000000 magic-folder-23.3.1/.github/workflows/codechecks.yml
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4319 2023-01-20 00:19:51.000000 magic-folder-23.3.1/.github/workflows/linux.yml
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3192 2023-01-20 00:19:51.000000 magic-folder-23.3.1/.github/workflows/macos.yaml
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3231 2023-01-20 00:19:51.000000 magic-folder-23.3.1/.github/workflows/windows.yml
--rw-r--r--   0 meejah    (1000) meejah    (1000)      269 2022-08-04 09:11:55.000000 magic-folder-23.3.1/.gitignore
--rw-r--r--   0 meejah    (1000) meejah    (1000)    24277 2020-02-04 18:00:11.000000 magic-folder-23.3.1/COPYING.GPL
--rw-r--r--   0 meejah    (1000) meejah    (1000)    17300 2020-02-04 18:00:11.000000 magic-folder-23.3.1/COPYING.TGPPL.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4840 2020-02-04 18:00:11.000000 magic-folder-23.3.1/CREDITS
--rw-r--r--   0 meejah    (1000) meejah    (1000)    10046 2023-03-16 04:36:41.000000 magic-folder-23.3.1/DEVELOPERS
--rw-r--r--   0 meejah    (1000) meejah    (1000)      226 2022-09-20 06:29:38.000000 magic-folder-23.3.1/MANIFEST.in
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2072 2022-09-20 06:29:38.000000 magic-folder-23.3.1/Makefile
--rw-r--r--   0 meejah    (1000) meejah    (1000)    24536 2023-03-20 18:13:21.000000 magic-folder-23.3.1/NEWS.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7592 2021-07-26 20:37:49.000000 magic-folder-23.3.1/NOTES.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7049 2023-03-20 18:13:24.173080 magic-folder-23.3.1/PKG-INFO
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5496 2023-02-07 22:05:58.000000 magic-folder-23.3.1/README.rst
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.057080 magic-folder-23.3.1/docs/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.017080 magic-folder-23.3.1/docs/.hypothesis/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.017080 magic-folder-23.3.1/docs/.hypothesis/examples/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.057080 magic-folder-23.3.1/docs/.hypothesis/examples/25667fd10de02221/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:32.000000 magic-folder-23.3.1/docs/.hypothesis/examples/25667fd10de02221/394341b7182cd227
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.057080 magic-folder-23.3.1/docs/.hypothesis/examples/26099471863eabde/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:34.000000 magic-folder-23.3.1/docs/.hypothesis/examples/26099471863eabde/394341b7182cd227
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.057080 magic-folder-23.3.1/docs/.hypothesis/examples/26b950c63ef40743/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      159 2023-03-16 04:52:27.000000 magic-folder-23.3.1/docs/.hypothesis/examples/26b950c63ef40743/2cd852709fc7beda
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.061080 magic-folder-23.3.1/docs/.hypothesis/examples/27a267c0b163fc05/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      159 2023-03-16 04:52:31.000000 magic-folder-23.3.1/docs/.hypothesis/examples/27a267c0b163fc05/2cd852709fc7beda
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.061080 magic-folder-23.3.1/docs/.hypothesis/examples/2bdd697e3cea2a04/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      226 2023-03-16 04:52:44.000000 magic-folder-23.3.1/docs/.hypothesis/examples/2bdd697e3cea2a04/f4644a30270a4ea6
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.061080 magic-folder-23.3.1/docs/.hypothesis/examples/3674e9cecacd98c9/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      159 2023-03-16 04:52:28.000000 magic-folder-23.3.1/docs/.hypothesis/examples/3674e9cecacd98c9/2cd852709fc7beda
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.061080 magic-folder-23.3.1/docs/.hypothesis/examples/532c4ead6274d000/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      212 2023-03-16 04:52:28.000000 magic-folder-23.3.1/docs/.hypothesis/examples/532c4ead6274d000/42e9ca500f868ebd
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.061080 magic-folder-23.3.1/docs/.hypothesis/examples/5ac28ffd404dc215/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        5 2023-03-16 04:52:38.000000 magic-folder-23.3.1/docs/.hypothesis/examples/5ac28ffd404dc215/68e09c5bfbe3cdbe
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.061080 magic-folder-23.3.1/docs/.hypothesis/examples/704d1edf754e9033/
--rw-r--r--   0 meejah    (1000) meejah    (1000)       20 2023-03-16 04:52:39.000000 magic-folder-23.3.1/docs/.hypothesis/examples/704d1edf754e9033/d0ff8af3e4baa190
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.061080 magic-folder-23.3.1/docs/.hypothesis/examples/9e68e03a9abe82a7/
--rw-r--r--   0 meejah    (1000) meejah    (1000)       11 2023-03-16 04:52:30.000000 magic-folder-23.3.1/docs/.hypothesis/examples/9e68e03a9abe82a7/d271b3d8c89fbe5f
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.061080 magic-folder-23.3.1/docs/.hypothesis/examples/b069c007d3e9f6fb/
--rw-r--r--   0 meejah    (1000) meejah    (1000)       24 2023-03-16 04:52:38.000000 magic-folder-23.3.1/docs/.hypothesis/examples/b069c007d3e9f6fb/eaef33fe07ad3597
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.061080 magic-folder-23.3.1/docs/.hypothesis/examples/c06175530ec95812/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      238 2023-03-16 04:52:45.000000 magic-folder-23.3.1/docs/.hypothesis/examples/c06175530ec95812/fd83ff26e80c6fad
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.061080 magic-folder-23.3.1/docs/.hypothesis/examples/e1ab432a194b3b87/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:32.000000 magic-folder-23.3.1/docs/.hypothesis/examples/e1ab432a194b3b87/394341b7182cd227
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.021080 magic-folder-23.3.1/docs/.hypothesis/unicode_data/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.061080 magic-folder-23.3.1/docs/.hypothesis/unicode_data/13.0.0/
--rw-------   0 meejah    (1000) meejah    (1000)    20988 2023-03-16 04:52:30.000000 magic-folder-23.3.1/docs/.hypothesis/unicode_data/13.0.0/charmap.json.gz
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3458 2023-03-16 04:36:41.000000 magic-folder-23.3.1/docs/CODE_OF_CONDUCT.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      634 2020-07-06 21:59:25.000000 magic-folder-23.3.1/docs/Makefile
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.021080 magic-folder-23.3.1/docs/_build/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.069080 magic-folder-23.3.1/docs/_build/doctrees/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    14226 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/CODE_OF_CONDUCT.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9338 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/backdoors.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    38021 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/config.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    43869 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/datamodel.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    31814 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/development.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    33138 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/downloader.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)  1261313 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 meejah    (1000) meejah    (1000)    13136 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/index.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    66571 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/interface.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    54817 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/invites.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    59020 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/leif-design.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11222 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/limitations.doctree
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.069080 magic-folder-23.3.1/docs/_build/doctrees/proposed/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18815 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/proposed/conflict-api.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4250 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/proposed/index.doctree
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.069080 magic-folder-23.3.1/docs/_build/doctrees/proposed/magic-folder/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18656 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/proposed/magic-folder/filesystem-integration.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)   178832 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/proposed/magic-folder/remote-to-local-sync.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    32883 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/proposed/magic-folder/user-interface-design.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    19020 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/proposed/recovery.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    37513 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/proposed/scanning-for-changes.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11826 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/release-process.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)   182197 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/releases.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    23355 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/snapshots.doctree
--rw-r--r--   0 meejah    (1000) meejah    (1000)    42464 2023-03-17 00:18:57.000000 magic-folder-23.3.1/docs/_build/doctrees/usage.doctree
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.073080 magic-folder-23.3.1/docs/_build/html/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      230 2023-03-17 00:18:59.000000 magic-folder-23.3.1/docs/_build/html/.buildinfo
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11411 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/CODE_OF_CONDUCT.html
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.073080 magic-folder-23.3.1/docs/_build/html/_images/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    27173 2023-03-16 20:16:58.000000 magic-folder-23.3.1/docs/_build/html/_images/magic-folder-data-model--high-level.svg
--rw-r--r--   0 meejah    (1000) meejah    (1000)    30197 2023-03-17 00:18:54.000000 magic-folder-23.3.1/docs/_build/html/_images/magic-folder-data-model-abstract--conflict.plain.svg
--rw-r--r--   0 meejah    (1000) meejah    (1000)    24088 2023-03-16 21:22:18.000000 magic-folder-23.3.1/docs/_build/html/_images/magic-folder-data-model-abstract.svg
--rw-r--r--   0 meejah    (1000) meejah    (1000)   436150 2023-03-17 00:06:11.000000 magic-folder-23.3.1/docs/_build/html/_images/magic-folder-data-model.svg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.077080 magic-folder-23.3.1/docs/_build/html/_sources/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3458 2023-03-16 04:36:41.000000 magic-folder-23.3.1/docs/_build/html/_sources/CODE_OF_CONDUCT.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1981 2020-04-02 18:49:18.000000 magic-folder-23.3.1/docs/_build/html/_sources/backdoors.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7226 2023-03-16 08:24:55.000000 magic-folder-23.3.1/docs/_build/html/_sources/config.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11620 2023-03-17 00:18:36.000000 magic-folder-23.3.1/docs/_build/html/_sources/datamodel.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6441 2021-07-26 20:37:49.000000 magic-folder-23.3.1/docs/_build/html/_sources/development.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7928 2023-03-07 23:57:50.000000 magic-folder-23.3.1/docs/_build/html/_sources/downloader.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3001 2023-03-16 20:41:52.000000 magic-folder-23.3.1/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)    15051 2023-03-16 08:24:55.000000 magic-folder-23.3.1/docs/_build/html/_sources/interface.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)    13780 2023-02-16 06:39:44.000000 magic-folder-23.3.1/docs/_build/html/_sources/invites.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)    17077 2023-03-16 20:45:29.000000 magic-folder-23.3.1/docs/_build/html/_sources/leif-design.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1512 2023-02-07 22:05:58.000000 magic-folder-23.3.1/docs/_build/html/_sources/limitations.rst.txt
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.077080 magic-folder-23.3.1/docs/_build/html/_sources/proposed/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4076 2023-03-16 04:36:41.000000 magic-folder-23.3.1/docs/_build/html/_sources/proposed/conflict-api.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      612 2023-03-16 20:41:30.000000 magic-folder-23.3.1/docs/_build/html/_sources/proposed/index.rst.txt
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.081080 magic-folder-23.3.1/docs/_build/html/_sources/proposed/magic-folder/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5850 2020-02-04 18:00:11.000000 magic-folder-23.3.1/docs/_build/html/_sources/proposed/magic-folder/filesystem-integration.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)    46411 2023-03-16 20:36:16.000000 magic-folder-23.3.1/docs/_build/html/_sources/proposed/magic-folder/remote-to-local-sync.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     8620 2020-07-06 21:59:25.000000 magic-folder-23.3.1/docs/_build/html/_sources/proposed/magic-folder/user-interface-design.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4909 2023-03-16 04:36:41.000000 magic-folder-23.3.1/docs/_build/html/_sources/proposed/recovery.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7356 2021-07-26 20:37:49.000000 magic-folder-23.3.1/docs/_build/html/_sources/proposed/scanning-for-changes.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2075 2023-03-16 04:36:41.000000 magic-folder-23.3.1/docs/_build/html/_sources/release-process.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      253 2023-03-16 04:36:41.000000 magic-folder-23.3.1/docs/_build/html/_sources/releases.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6226 2023-03-16 04:36:41.000000 magic-folder-23.3.1/docs/_build/html/_sources/snapshots.rst.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11683 2023-03-16 20:45:54.000000 magic-folder-23.3.1/docs/_build/html/_sources/usage.rst.txt
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.085080 magic-folder-23.3.1/docs/_build/html/_static/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    14813 2023-03-17 00:18:59.000000 magic-folder-23.3.1/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.085080 magic-folder-23.3.1/docs/_build/html/_static/css/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3229 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.093080 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    87624 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)    67312 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)    86288 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)    66444 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)   165742 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 meejah    (1000) meejah    (1000)   444379 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 meejah    (1000) meejah    (1000)   165548 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 meejah    (1000) meejah    (1000)    98024 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)    77160 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)   323344 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)   193308 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)   309728 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)   184912 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)   328412 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)   195704 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)   309192 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 meejah    (1000) meejah    (1000)   182708 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 meejah    (1000) meejah    (1000)   135235 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 meejah    (1000) meejah    (1000)       61 2020-07-06 21:59:25.000000 magic-folder-23.3.1/docs/_build/html/_static/custom.css
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4472 2023-03-08 00:43:20.000000 magic-folder-23.3.1/docs/_build/html/_static/doctools.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)      418 2023-03-17 00:18:59.000000 magic-folder-23.3.1/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)      286 2023-03-08 00:43:20.000000 magic-folder-23.3.1/docs/_build/html/_static/file.png
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.093080 magic-folder-23.3.1/docs/_build/html/_static/js/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      934 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4370 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2734 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5023 2023-03-08 00:44:09.000000 magic-folder-23.3.1/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4758 2023-03-17 00:18:59.000000 magic-folder-23.3.1/docs/_build/html/_static/language_data.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)       90 2023-03-08 00:43:20.000000 magic-folder-23.3.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 meejah    (1000) meejah    (1000)       90 2023-03-08 00:43:20.000000 magic-folder-23.3.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4846 2023-03-17 00:18:59.000000 magic-folder-23.3.1/docs/_build/html/_static/pygments.css
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18215 2023-03-08 00:43:20.000000 magic-folder-23.3.1/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4712 2023-03-08 00:43:20.000000 magic-folder-23.3.1/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)     8183 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/backdoors.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    19001 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/config.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    23764 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/datamodel.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20860 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/development.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18079 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/downloader.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5143 2023-03-17 00:18:59.000000 magic-folder-23.3.1/docs/_build/html/genindex.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11167 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/index.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    44501 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/interface.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    35282 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/invites.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    30106 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/leif-design.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7597 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/limitations.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1120 2023-03-17 00:18:59.000000 magic-folder-23.3.1/docs/_build/html/objects.inv
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.093080 magic-folder-23.3.1/docs/_build/html/proposed/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16640 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/proposed/conflict-api.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     8297 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/proposed/index.html
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.093080 magic-folder-23.3.1/docs/_build/html/proposed/magic-folder/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    14301 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/proposed/magic-folder/filesystem-integration.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    73834 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/proposed/magic-folder/remote-to-local-sync.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20764 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/proposed/magic-folder/user-interface-design.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16041 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/proposed/recovery.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    19921 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/proposed/scanning-for-changes.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9495 2023-03-17 00:18:58.000000 magic-folder-23.3.1/docs/_build/html/release-process.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    51586 2023-03-17 00:18:59.000000 magic-folder-23.3.1/docs/_build/html/releases.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5542 2023-03-17 00:18:59.000000 magic-folder-23.3.1/docs/_build/html/search.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    63003 2023-03-17 00:18:59.000000 magic-folder-23.3.1/docs/_build/html/searchindex.js
--rw-r--r--   0 meejah    (1000) meejah    (1000)    15500 2023-03-17 00:18:59.000000 magic-folder-23.3.1/docs/_build/html/snapshots.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)    29531 2023-03-17 00:18:59.000000 magic-folder-23.3.1/docs/_build/html/usage.html
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.093080 magic-folder-23.3.1/docs/_static/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-02-04 18:00:11.000000 magic-folder-23.3.1/docs/_static/.empty
--rw-r--r--   0 meejah    (1000) meejah    (1000)       61 2020-07-06 21:59:25.000000 magic-folder-23.3.1/docs/_static/custom.css
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.093080 magic-folder-23.3.1/docs/_templates/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-02-04 18:00:11.000000 magic-folder-23.3.1/docs/_templates/.empty
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.097080 magic-folder-23.3.1/docs/_trial_temp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:53.000000 magic-folder-23.3.1/docs/_trial_temp/_trial_marker
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.021080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.025080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.021080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.025080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.021080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.021080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.097080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:53.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.025080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.021080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.097080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:53.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.097080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/NOQa688y-gasC8_mtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        7 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/NOQa688y-gasC8_mtmp/file
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.025080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.025080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.097080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.097080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/nHFbIFQTTLJlnSdPtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        7 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/nHFbIFQTTLJlnSdPtmp/file
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.025080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.025080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.097080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.097080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/kZwY9CKpgneIJrdHtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        7 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/kZwY9CKpgneIJrdHtmp/file
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.029080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.025080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.101080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.101080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.025080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.101080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      284 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.101080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.101080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.025080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.101080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.101080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.101080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      289 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.025080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.105080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      285 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.105080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.105080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.029080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.105080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.105080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.105080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      292 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       19 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/api_client_endpoint
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.029080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.105080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      300 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.105080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.109080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.029080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.029080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.109080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.109080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.109080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      292 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.109080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory_is_file/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        6 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory_is_file/h87a74R8VavQbimAtmp
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.029080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.109080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.109080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.109080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      300 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.029080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.109080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.109080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.109080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.113080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.113080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.113080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/folder-y8qFhiM2lyCn8nJGeaH4ciGaHxbMbSziNeOGf-Bnma0=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/folder-y8qFhiM2lyCn8nJGeaH4ciGaHxbMbSziNeOGf-Bnma0=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.113080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/folder-hoqYtkBoInB3B9NowQg2NYo1DccfQVbrYOYb5dPgURo=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/folder-hoqYtkBoInB3B9NowQg2NYo1DccfQVbrYOYb5dPgURo=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.033080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.113080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.113080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      271 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.113080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      273 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.117080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      271 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.117080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      275 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_client_endpoint/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.117080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_client_endpoint/o5Gxw0rWx_fb1-hAtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)       12 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_client_endpoint/o5Gxw0rWx_fb1-hAtmp/api_client_endpoint
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_invalid_api_token/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.117080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_invalid_api_token/aENw4EmGAVYEk3U_tmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)       10 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_invalid_api_token/aENw4EmGAVYEk3U_tmp/api_token
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_short_api_token/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.117080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_short_api_token/dRWMXaz4R2sxDwgStmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_short_api_token/dRWMXaz4R2sxDwgStmp/api_token
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.121080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      269 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.121080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.121080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.037080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.121080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.121080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/private/api_auth_token
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      448 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/private/magic_folders.yaml
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.121080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.121080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/private/api_auth_token
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      447 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/private/magic_folders.yaml
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.121080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      271 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/api_token
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.121080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/folder-SQu5fiZdVu3yYi_fXHOGasM9lBPJrIhE_LYn2BPLbv0=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/folder-SQu5fiZdVu3yYi_fXHOGasM9lBPJrIhE_LYn2BPLbv0=/state.sqlite
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.125080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.125080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/private/api_auth_token
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      434 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/private/magic_folders.yaml
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.125080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.125080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/private/api_auth_token
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      451 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/private/magic_folders.yaml
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.125080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      269 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:57.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/api_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:57.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.125080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.125080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/private/api_auth_token
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      437 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/private/magic_folders.yaml
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.041080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.045080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.129080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      298 2023-03-16 04:53:01.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:53:01.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/api_token
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.129080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/folder-ijMf3ecDLzOnHhsuJX2AFm40jgD8sXkU9IvbV6HGMAc=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:53:01.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/folder-ijMf3ecDLzOnHhsuJX2AFm40jgD8sXkU9IvbV6HGMAc=/state.sqlite
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:53:01.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.129080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      298 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:53:01.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/api_token
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.129080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/folder-56wHhmaOD_DwK2K9BPRf9jb9gttjsRBGAcl13ABfOmc=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:53:01.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/folder-56wHhmaOD_DwK2K9BPRf9jb9gttjsRBGAcl13ABfOmc=/state.sqlite
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:53:01.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.129080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.129080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.129080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      298 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/api_token
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.129080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/folder-zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag=/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/folder-zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag=/state.sqlite
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/global.sqlite
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.133080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.133080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.133080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.133080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:00.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/tahoe.cfg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.137080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:01.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/magic-folder.url
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:01.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/node.url
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.137080 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/private/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:01.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/private/api_auth_token
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:01.000000 magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/tahoe.cfg
--rw-r--r--   0 meejah    (1000) meejah    (1000)       41 2023-03-16 04:52:53.000000 magic-folder-23.3.1/docs/_trial_temp/test.log
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1981 2020-04-02 18:49:18.000000 magic-folder-23.3.1/docs/backdoors.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9480 2021-07-26 20:37:49.000000 magic-folder-23.3.1/docs/conf.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7226 2023-03-16 08:24:55.000000 magic-folder-23.3.1/docs/config.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6441 2021-07-26 20:37:49.000000 magic-folder-23.3.1/docs/development.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7928 2023-03-07 23:57:50.000000 magic-folder-23.3.1/docs/downloader.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)   664833 2023-03-16 04:53:01.000000 magic-folder-23.3.1/docs/eliot.log
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2973 2023-03-20 18:05:45.000000 magic-folder-23.3.1/docs/index.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)    15051 2023-03-16 08:24:55.000000 magic-folder-23.3.1/docs/interface.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)    14482 2022-11-11 00:40:27.000000 magic-folder-23.3.1/docs/invite-diagram-readonly.png
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1230 2023-02-07 22:05:58.000000 magic-folder-23.3.1/docs/invite-diagram-readonly.seqdiag
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16247 2023-01-07 21:02:05.000000 magic-folder-23.3.1/docs/invite-diagram.png
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1229 2023-02-07 22:05:58.000000 magic-folder-23.3.1/docs/invite-diagram.seqdiag
--rw-r--r--   0 meejah    (1000) meejah    (1000)    13780 2023-02-16 06:39:44.000000 magic-folder-23.3.1/docs/invites.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1512 2023-02-07 22:05:58.000000 magic-folder-23.3.1/docs/limitations.rst
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.137080 magic-folder-23.3.1/docs/proposed/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    24834 2021-06-11 15:26:48.000000 magic-folder-23.3.1/docs/proposed/LightweightDesignscanfornewfiles.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4076 2023-03-16 04:36:41.000000 magic-folder-23.3.1/docs/proposed/conflict-api.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      659 2023-03-20 18:05:45.000000 magic-folder-23.3.1/docs/proposed/index.rst
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.137080 magic-folder-23.3.1/docs/proposed/magic-folder/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5850 2020-02-04 18:00:11.000000 magic-folder-23.3.1/docs/proposed/magic-folder/filesystem-integration.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18174 2023-03-20 18:05:45.000000 magic-folder-23.3.1/docs/proposed/magic-folder/multi-party-conflict-detection.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)    46411 2023-03-16 20:36:16.000000 magic-folder-23.3.1/docs/proposed/magic-folder/remote-to-local-sync.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     8620 2020-07-06 21:59:25.000000 magic-folder-23.3.1/docs/proposed/magic-folder/user-interface-design.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)   257416 2021-06-11 16:23:59.000000 magic-folder-23.3.1/docs/proposed/markdown
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4909 2023-03-16 04:36:41.000000 magic-folder-23.3.1/docs/proposed/recovery.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7356 2021-07-26 20:37:49.000000 magic-folder-23.3.1/docs/proposed/scanning-for-changes.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2075 2023-03-16 04:36:41.000000 magic-folder-23.3.1/docs/release-process.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      253 2023-03-16 04:36:41.000000 magic-folder-23.3.1/docs/releases.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6226 2023-03-16 04:36:41.000000 magic-folder-23.3.1/docs/snapshots.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11683 2023-03-20 18:05:45.000000 magic-folder-23.3.1/docs/usage.rst
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.141080 magic-folder-23.3.1/integration/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1397 2022-09-20 06:29:38.000000 magic-folder-23.3.1/integration/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2021-07-26 20:37:49.000000 magic-folder-23.3.1/integration/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3001 2021-06-22 06:43:35.000000 magic-folder-23.3.1/integration/bar
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11596 2023-02-07 22:05:58.000000 magic-folder-23.3.1/integration/conftest.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9445 2020-06-25 22:39:41.000000 magic-folder-23.3.1/integration/conftest.py.orig
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2110 2021-06-22 06:43:20.000000 magic-folder-23.3.1/integration/foo
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1780 2021-12-21 23:52:48.000000 magic-folder-23.3.1/integration/log.integ
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2021-06-22 06:45:13.000000 magic-folder-23.3.1/integration/pytest.log
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4271 2022-09-20 06:29:38.000000 magic-folder-23.3.1/integration/test_add.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2758 2022-09-20 06:29:38.000000 magic-folder-23.3.1/integration/test_general_cli.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2802 2023-02-16 06:39:44.000000 magic-folder-23.3.1/integration/test_invite.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3060 2023-03-16 08:24:55.000000 magic-folder-23.3.1/integration/test_kitties.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2312 2023-02-07 22:05:58.000000 magic-folder-23.3.1/integration/test_list.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      592 2022-09-20 06:29:38.000000 magic-folder-23.3.1/integration/test_magic_folder.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16384 2020-06-25 22:17:40.000000 magic-folder-23.3.1/integration/test_magic_folder.py.orig
--rw-r--r--   0 meejah    (1000) meejah    (1000)    10302 2020-06-25 22:39:42.000000 magic-folder-23.3.1/integration/test_magic_folder.py.rej
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2561 2023-03-16 08:24:55.000000 magic-folder-23.3.1/integration/test_same_files.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2045 2023-03-16 08:24:55.000000 magic-folder-23.3.1/integration/test_status.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    23667 2022-09-20 06:29:38.000000 magic-folder-23.3.1/integration/test_synchronize.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4367 2023-02-07 22:05:58.000000 magic-folder-23.3.1/integration/test_tahoe_objects.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    45741 2023-02-20 06:53:12.000000 magic-folder-23.3.1/integration/util.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    23625 2020-06-25 22:17:40.000000 magic-folder-23.3.1/integration/util.py.orig
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5425 2020-06-25 22:39:43.000000 magic-folder-23.3.1/integration/util.py.rej
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.045080 magic-folder-23.3.1/misc/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.145080 magic-folder-23.3.1/misc/build_helpers/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2889 2022-08-04 09:11:55.000000 magic-folder-23.3.1/misc/build_helpers/platform-pins.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3919 2021-11-25 22:22:35.000000 magic-folder-23.3.1/misc/build_helpers/run-deprecations.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      228 2021-11-25 22:22:35.000000 magic-folder-23.3.1/misc/build_helpers/sqlite_version.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2475 2023-01-20 00:19:51.000000 magic-folder-23.3.1/misc/build_helpers/update-version.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.145080 magic-folder-23.3.1/misc/coding_tools/
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      807 2021-07-26 20:37:49.000000 magic-folder-23.3.1/misc/coding_tools/check-debugging.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.145080 magic-folder-23.3.1/newsfragments/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2022-09-20 06:29:38.000000 magic-folder-23.3.1/newsfragments/.keep-directory
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1455 2022-09-20 06:29:38.000000 magic-folder-23.3.1/pyproject.toml
--rw-r--r--   0 meejah    (1000) meejah    (1000)      287 2021-08-27 20:55:28.000000 magic-folder-23.3.1/pytest.ini
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.145080 magic-folder-23.3.1/requirements/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      443 2021-11-25 22:22:35.000000 magic-folder-23.3.1/requirements/README
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1397 2023-01-30 21:42:35.000000 magic-folder-23.3.1/requirements/base.in
--rw-r--r--   0 meejah    (1000) meejah    (1000)    44868 2023-02-07 22:05:58.000000 magic-folder-23.3.1/requirements/base.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      254 2022-09-20 06:29:38.000000 magic-folder-23.3.1/requirements/build.in
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11012 2023-02-07 22:05:58.000000 magic-folder-23.3.1/requirements/build.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3489 2023-02-07 22:05:58.000000 magic-folder-23.3.1/requirements/platform.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       19 2022-09-20 06:29:38.000000 magic-folder-23.3.1/requirements/tahoe-integration-1.17.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       19 2023-02-07 22:05:58.000000 magic-folder-23.3.1/requirements/tahoe-integration-1.18.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       67 2021-07-26 20:37:49.000000 magic-folder-23.3.1/requirements/tahoe-integration-master.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      827 2023-02-07 22:05:58.000000 magic-folder-23.3.1/requirements/test.in
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16621 2023-02-07 22:05:58.000000 magic-folder-23.3.1/requirements/test.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       48 2022-08-04 09:11:55.000000 magic-folder-23.3.1/requirements/tox.in
--rw-r--r--   0 meejah    (1000) meejah    (1000)      949 2023-02-07 22:05:58.000000 magic-folder-23.3.1/requirements/tox.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       38 2023-03-20 18:13:24.173080 magic-folder-23.3.1/setup.cfg
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2661 2022-09-20 06:29:38.000000 magic-folder-23.3.1/setup.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.049080 magic-folder-23.3.1/src/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.157080 magic-folder-23.3.1/src/magic_folder/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      123 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      152 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/__main__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1171 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/_coverage.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1670 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/_endpoint_parser.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5780 2023-02-07 22:05:58.000000 magic-folder-23.3.1/src/magic_folder/_schema.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      162 2023-03-20 18:13:23.000000 magic-folder-23.3.1/src/magic_folder/_version.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20176 2023-03-20 18:05:48.000000 magic-folder-23.3.1/src/magic_folder/api_cli.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    32268 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/cli.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    13339 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/client.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5264 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/common.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    76226 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/config.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    22008 2023-03-16 04:36:41.000000 magic-folder-23.3.1/src/magic_folder/downloader.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2741 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/endpoints.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1611 2023-02-07 22:05:58.000000 magic-folder-23.3.1/src/magic_folder/initialize.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    20672 2023-03-20 18:05:48.000000 magic-folder-23.3.1/src/magic_folder/invite.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-02-07 22:05:58.000000 magic-folder-23.3.1/src/magic_folder/join.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2173 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/list.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    46889 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/magic_file.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    17879 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/magic_folder.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      539 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/magicpath.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2786 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/migrate.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11567 2023-02-07 22:05:58.000000 magic-folder-23.3.1/src/magic_folder/participants.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4142 2023-01-20 00:19:51.000000 magic-folder-23.3.1/src/magic_folder/pid.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9328 2023-02-08 01:51:42.000000 magic-folder-23.3.1/src/magic_folder/scanner.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    17540 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/service.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1286 2023-02-16 06:39:44.000000 magic-folder-23.3.1/src/magic_folder/show_config.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    23391 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/snapshot.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18221 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/status.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    14506 2023-02-17 18:23:28.000000 magic-folder-23.3.1/src/magic_folder/tahoe_client.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.169080 magic-folder-23.3.1/src/magic_folder/test/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3189 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      849 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/agentutil.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.169080 magic-folder-23.3.1/src/magic_folder/test/cli/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-05-05 16:38:01.000000 magic-folder-23.3.1/src/magic_folder/test/cli/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6104 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/cli/common.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4451 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/cli/test_api_cli.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    24265 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/cli/test_magic_folder.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6801 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/common.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4962 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/eliotutil.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16666 2023-03-20 18:05:48.000000 magic-folder-23.3.1/src/magic_folder/test/fixtures.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5130 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/matchers.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.169080 magic-folder-23.3.1/src/magic_folder/test/plugins/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      334 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/plugins/magic_folder_tests_dropin.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    12527 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/strategies.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    26802 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/test_api_cli.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    16654 2023-02-07 22:05:58.000000 magic-folder-23.3.1/src/magic_folder/test/test_cli.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4367 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/test_client.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4663 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/test_common.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    47820 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/test_config.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    70265 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/test_download.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5476 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/test_eliotutil.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1281 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/test_endpoints.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1188 2022-03-15 06:53:54.000000 magic-folder-23.3.1/src/magic_folder/test/test_foo.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    28355 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/test_invite.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11736 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/test_local_snapshot.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5339 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/test_magic_file.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     8522 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/test_magic_folder_service.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1199 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/test_magicpath.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    17352 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/test_participants.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4646 2023-01-20 00:19:51.000000 magic-folder-23.3.1/src/magic_folder/test/test_pid.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    15519 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/test_scanner.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7004 2023-02-07 22:05:58.000000 magic-folder-23.3.1/src/magic_folder/test/test_schema.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7549 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/test_service.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18979 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/test_snapshot.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7268 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/test_status.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2040 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/test_strategies.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    12958 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/test_tahoe_client.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5832 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/test_testing.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    27392 2023-03-16 08:24:55.000000 magic-folder-23.3.1/src/magic_folder/test/test_upload.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2532 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/test_util_database.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4535 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/test_util_file.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6446 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/test/test_util_twisted.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    79279 2023-03-20 18:05:48.000000 magic-folder-23.3.1/src/magic_folder/test/test_web.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.169080 magic-folder-23.3.1/src/magic_folder/testing/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-07-07 16:51:27.000000 magic-folder-23.3.1/src/magic_folder/testing/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    18739 2023-01-30 21:42:35.000000 magic-folder-23.3.1/src/magic_folder/testing/web.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11738 2023-03-14 22:51:27.000000 magic-folder-23.3.1/src/magic_folder/uploader.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.173080 magic-folder-23.3.1/src/magic_folder/util/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-05-05 16:38:01.000000 magic-folder-23.3.1/src/magic_folder/util/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6852 2023-02-09 07:57:43.000000 magic-folder-23.3.1/src/magic_folder/util/capabilities.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5603 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/util/database.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9471 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/util/eliotutil.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      617 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/util/encoding.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2473 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/util/file.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1403 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/util/observer.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6547 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/util/twisted.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2176 2022-09-20 06:29:38.000000 magic-folder-23.3.1/src/magic_folder/util/wrap.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    29705 2023-03-20 18:05:48.000000 magic-folder-23.3.1/src/magic_folder/web.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.157080 magic-folder-23.3.1/src/magic_folder.egg-info/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7049 2023-03-20 18:13:23.000000 magic-folder-23.3.1/src/magic_folder.egg-info/PKG-INFO
--rw-r--r--   0 meejah    (1000) meejah    (1000)    31277 2023-03-20 18:13:23.000000 magic-folder-23.3.1/src/magic_folder.egg-info/SOURCES.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)        1 2023-03-20 18:13:23.000000 magic-folder-23.3.1/src/magic_folder.egg-info/dependency_links.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      104 2023-03-20 18:13:23.000000 magic-folder-23.3.1/src/magic_folder.egg-info/entry_points.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      532 2023-03-20 18:13:23.000000 magic-folder-23.3.1/src/magic_folder.egg-info/requires.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       21 2023-03-20 18:13:23.000000 magic-folder-23.3.1/src/magic_folder.egg-info/top_level.txt
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.049080 magic-folder-23.3.1/src/twisted/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-20 18:13:24.173080 magic-folder-23.3.1/src/twisted/plugins/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      301 2021-07-26 20:37:49.000000 magic-folder-23.3.1/src/twisted/plugins/magic_folder_dropin.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5616 2023-02-07 22:05:58.000000 magic-folder-23.3.1/tox.ini
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      207 2022-02-03 01:05:52.000000 magic-folder-23.5.0/.coveragerc
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      324 2022-09-20 06:29:38.000000 magic-folder-23.5.0/.flake8
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.193878 magic-folder-23.5.0/.github/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:36:41.000000 magic-folder-23.5.0/.github/pull_request_template.md
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.193878 magic-folder-23.5.0/.github/workflows/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      935 2023-01-20 00:19:51.000000 magic-folder-23.5.0/.github/workflows/codechecks.yml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4319 2023-01-20 00:19:51.000000 magic-folder-23.5.0/.github/workflows/linux.yml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3192 2023-01-20 00:19:51.000000 magic-folder-23.5.0/.github/workflows/macos.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3231 2023-01-20 00:19:51.000000 magic-folder-23.5.0/.github/workflows/windows.yml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      269 2022-08-04 09:11:55.000000 magic-folder-23.5.0/.gitignore
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    24277 2020-02-04 18:00:11.000000 magic-folder-23.5.0/COPYING.GPL
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    17300 2020-02-04 18:00:11.000000 magic-folder-23.5.0/COPYING.TGPPL.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4840 2020-02-04 18:00:11.000000 magic-folder-23.5.0/CREDITS
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    10046 2023-03-16 04:36:41.000000 magic-folder-23.5.0/DEVELOPERS
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      226 2022-09-20 06:29:38.000000 magic-folder-23.5.0/MANIFEST.in
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2242 2023-05-02 18:43:42.000000 magic-folder-23.5.0/Makefile
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    25457 2023-05-02 18:45:12.000000 magic-folder-23.5.0/NEWS.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7592 2021-07-26 20:37:49.000000 magic-folder-23.5.0/NOTES.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7049 2023-05-02 18:45:15.309878 magic-folder-23.5.0/PKG-INFO
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5496 2023-02-07 22:05:58.000000 magic-folder-23.5.0/README.rst
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.157878 magic-folder-23.5.0/docs/.hypothesis/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.157878 magic-folder-23.5.0/docs/.hypothesis/examples/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/25667fd10de02221/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:32.000000 magic-folder-23.5.0/docs/.hypothesis/examples/25667fd10de02221/394341b7182cd227
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/26099471863eabde/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:34.000000 magic-folder-23.5.0/docs/.hypothesis/examples/26099471863eabde/394341b7182cd227
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/26b950c63ef40743/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      159 2023-03-16 04:52:27.000000 magic-folder-23.5.0/docs/.hypothesis/examples/26b950c63ef40743/2cd852709fc7beda
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/27a267c0b163fc05/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      159 2023-03-16 04:52:31.000000 magic-folder-23.5.0/docs/.hypothesis/examples/27a267c0b163fc05/2cd852709fc7beda
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/2bdd697e3cea2a04/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      226 2023-03-16 04:52:44.000000 magic-folder-23.5.0/docs/.hypothesis/examples/2bdd697e3cea2a04/f4644a30270a4ea6
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/3674e9cecacd98c9/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      159 2023-03-16 04:52:28.000000 magic-folder-23.5.0/docs/.hypothesis/examples/3674e9cecacd98c9/2cd852709fc7beda
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/532c4ead6274d000/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      212 2023-03-16 04:52:28.000000 magic-folder-23.5.0/docs/.hypothesis/examples/532c4ead6274d000/42e9ca500f868ebd
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/5ac28ffd404dc215/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        5 2023-03-16 04:52:38.000000 magic-folder-23.5.0/docs/.hypothesis/examples/5ac28ffd404dc215/68e09c5bfbe3cdbe
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/704d1edf754e9033/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       20 2023-03-16 04:52:39.000000 magic-folder-23.5.0/docs/.hypothesis/examples/704d1edf754e9033/d0ff8af3e4baa190
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/9e68e03a9abe82a7/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       11 2023-03-16 04:52:30.000000 magic-folder-23.5.0/docs/.hypothesis/examples/9e68e03a9abe82a7/d271b3d8c89fbe5f
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/b069c007d3e9f6fb/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       24 2023-03-16 04:52:38.000000 magic-folder-23.5.0/docs/.hypothesis/examples/b069c007d3e9f6fb/eaef33fe07ad3597
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/c06175530ec95812/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      238 2023-03-16 04:52:45.000000 magic-folder-23.5.0/docs/.hypothesis/examples/c06175530ec95812/fd83ff26e80c6fad
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/examples/e1ab432a194b3b87/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:32.000000 magic-folder-23.5.0/docs/.hypothesis/examples/e1ab432a194b3b87/394341b7182cd227
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.157878 magic-folder-23.5.0/docs/.hypothesis/unicode_data/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.201878 magic-folder-23.5.0/docs/.hypothesis/unicode_data/13.0.0/
+-rw-------   0 meejah    (1000) meejah    (1000)    20988 2023-03-16 04:52:30.000000 magic-folder-23.5.0/docs/.hypothesis/unicode_data/13.0.0/charmap.json.gz
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3458 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      634 2020-07-06 21:59:25.000000 magic-folder-23.5.0/docs/Makefile
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.157878 magic-folder-23.5.0/docs/_build/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.209878 magic-folder-23.5.0/docs/_build/doctrees/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    14226 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/CODE_OF_CONDUCT.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9338 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/backdoors.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    38021 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/config.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    43869 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/datamodel.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    31814 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/development.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    33138 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/downloader.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)  1261313 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    13136 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    66571 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/interface.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    54817 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/invites.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    59020 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/leif-design.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11222 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/limitations.doctree
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.209878 magic-folder-23.5.0/docs/_build/doctrees/proposed/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18815 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/conflict-api.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4250 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/index.doctree
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.209878 magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18656 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/filesystem-integration.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   178832 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/remote-to-local-sync.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    32883 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/user-interface-design.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    19020 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/recovery.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    37513 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/proposed/scanning-for-changes.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11826 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/release-process.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   182197 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/releases.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    23355 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/snapshots.doctree
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    42464 2023-03-17 00:18:57.000000 magic-folder-23.5.0/docs/_build/doctrees/usage.doctree
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.213878 magic-folder-23.5.0/docs/_build/html/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      230 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/.buildinfo
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11411 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/CODE_OF_CONDUCT.html
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.213878 magic-folder-23.5.0/docs/_build/html/_images/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    27173 2023-03-16 20:16:58.000000 magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model--high-level.svg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    30197 2023-03-17 00:18:54.000000 magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model-abstract--conflict.plain.svg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    24088 2023-03-16 21:22:18.000000 magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model-abstract.svg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   436150 2023-03-17 00:06:11.000000 magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model.svg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.221878 magic-folder-23.5.0/docs/_build/html/_sources/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3458 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/_build/html/_sources/CODE_OF_CONDUCT.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1981 2020-04-02 18:49:18.000000 magic-folder-23.5.0/docs/_build/html/_sources/backdoors.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7226 2023-03-16 08:24:55.000000 magic-folder-23.5.0/docs/_build/html/_sources/config.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11620 2023-03-17 00:18:36.000000 magic-folder-23.5.0/docs/_build/html/_sources/datamodel.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6441 2021-07-26 20:37:49.000000 magic-folder-23.5.0/docs/_build/html/_sources/development.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7928 2023-03-07 23:57:50.000000 magic-folder-23.5.0/docs/_build/html/_sources/downloader.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3001 2023-03-16 20:41:52.000000 magic-folder-23.5.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    15051 2023-03-16 08:24:55.000000 magic-folder-23.5.0/docs/_build/html/_sources/interface.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    13780 2023-02-16 06:39:44.000000 magic-folder-23.5.0/docs/_build/html/_sources/invites.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    17077 2023-03-16 20:45:29.000000 magic-folder-23.5.0/docs/_build/html/_sources/leif-design.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1512 2023-02-07 22:05:58.000000 magic-folder-23.5.0/docs/_build/html/_sources/limitations.rst.txt
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.221878 magic-folder-23.5.0/docs/_build/html/_sources/proposed/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4076 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/conflict-api.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      612 2023-03-16 20:41:30.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/index.rst.txt
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.221878 magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5850 2020-02-04 18:00:11.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/filesystem-integration.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    46411 2023-03-16 20:36:16.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/remote-to-local-sync.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8620 2020-07-06 21:59:25.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/user-interface-design.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4909 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/recovery.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7356 2021-07-26 20:37:49.000000 magic-folder-23.5.0/docs/_build/html/_sources/proposed/scanning-for-changes.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2075 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/_build/html/_sources/release-process.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      253 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/_build/html/_sources/releases.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6226 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/_build/html/_sources/snapshots.rst.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11683 2023-03-16 20:45:54.000000 magic-folder-23.5.0/docs/_build/html/_sources/usage.rst.txt
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.221878 magic-folder-23.5.0/docs/_build/html/_static/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    14813 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.225878 magic-folder-23.5.0/docs/_build/html/_static/css/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3229 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.229878 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    87624 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    67312 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    86288 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    66444 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   165742 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   444379 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   165548 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    98024 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    77160 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   323344 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   193308 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   309728 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   184912 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   328412 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   195704 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   309192 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   182708 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   135235 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       61 2020-07-06 21:59:25.000000 magic-folder-23.5.0/docs/_build/html/_static/custom.css
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4472 2023-03-08 00:43:20.000000 magic-folder-23.5.0/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      418 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      286 2023-03-08 00:43:20.000000 magic-folder-23.5.0/docs/_build/html/_static/file.png
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.229878 magic-folder-23.5.0/docs/_build/html/_static/js/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      934 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4370 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2734 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5023 2023-03-08 00:44:09.000000 magic-folder-23.5.0/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4758 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       90 2023-03-08 00:43:20.000000 magic-folder-23.5.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       90 2023-03-08 00:43:20.000000 magic-folder-23.5.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4846 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18215 2023-03-08 00:43:20.000000 magic-folder-23.5.0/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4712 2023-03-08 00:43:20.000000 magic-folder-23.5.0/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8183 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/backdoors.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    19001 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/config.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    23764 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/datamodel.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20860 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/development.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18079 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/downloader.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5143 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/genindex.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11167 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/index.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    44501 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/interface.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    35282 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/invites.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    30106 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/leif-design.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7597 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/limitations.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1120 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/objects.inv
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.229878 magic-folder-23.5.0/docs/_build/html/proposed/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    16640 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/conflict-api.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8297 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/index.html
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.233878 magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    14301 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/filesystem-integration.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    73834 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/remote-to-local-sync.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20764 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/user-interface-design.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    16041 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/recovery.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    19921 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/proposed/scanning-for-changes.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9495 2023-03-17 00:18:58.000000 magic-folder-23.5.0/docs/_build/html/release-process.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    51586 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/releases.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5542 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/search.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    63003 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/searchindex.js
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    15500 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/snapshots.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    29531 2023-03-17 00:18:59.000000 magic-folder-23.5.0/docs/_build/html/usage.html
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.233878 magic-folder-23.5.0/docs/_static/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-02-04 18:00:11.000000 magic-folder-23.5.0/docs/_static/.empty
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       61 2020-07-06 21:59:25.000000 magic-folder-23.5.0/docs/_static/custom.css
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.233878 magic-folder-23.5.0/docs/_templates/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-02-04 18:00:11.000000 magic-folder-23.5.0/docs/_templates/.empty
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.233878 magic-folder-23.5.0/docs/_trial_temp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:53.000000 magic-folder-23.5.0/docs/_trial_temp/_trial_marker
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.233878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:53.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.233878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:53.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/NOQa688y-gasC8_mtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        7 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/NOQa688y-gasC8_mtmp/file
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/nHFbIFQTTLJlnSdPtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        7 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/nHFbIFQTTLJlnSdPtmp/file
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/kZwY9CKpgneIJrdHtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        7 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/kZwY9CKpgneIJrdHtmp/file
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.165878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_fail/CN3vFrZNrnniQDqitmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.161878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      284 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.237878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/k4z3v0On0pXC3-zTtmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.165878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/5VwCskTBOF_iI3Dntmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      289 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.165878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      285 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/jHISzxBPQ2jpzf5ntmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.165878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.241878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/SogsXydSSwy3WtIHtmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      292 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       19 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/api_client_endpoint
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:54.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.165878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      300 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/hL00vGeKA5Zi1TK-tmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.165878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/UkvCu78pHGi9U_vbtmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      292 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.245878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory_is_file/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        6 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory_is_file/h87a74R8VavQbimAtmp
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.249878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.249878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/RIUY3b0xqnEpWnertmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.249878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      300 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.249878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.169878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/folder-y8qFhiM2lyCn8nJGeaH4ciGaHxbMbSziNeOGf-Bnma0=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:55.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/folder-y8qFhiM2lyCn8nJGeaH4ciGaHxbMbSziNeOGf-Bnma0=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/folder-hoqYtkBoInB3B9NowQg2NYo1DccfQVbrYOYb5dPgURo=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/folder-hoqYtkBoInB3B9NowQg2NYo1DccfQVbrYOYb5dPgURo=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      271 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.253878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      273 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      271 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.173878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      275 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_client_endpoint/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_client_endpoint/o5Gxw0rWx_fb1-hAtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       12 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_client_endpoint/o5Gxw0rWx_fb1-hAtmp/api_client_endpoint
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_invalid_api_token/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_invalid_api_token/aENw4EmGAVYEk3U_tmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       10 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_invalid_api_token/aENw4EmGAVYEk3U_tmp/api_token
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_short_api_token/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_short_api_token/dRWMXaz4R2sxDwgStmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        4 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestBaseOptions/test_short_api_token/dRWMXaz4R2sxDwgStmp/api_token
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      269 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/node/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.257878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/private/api_auth_token
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      448 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/private/magic_folders.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_connect_string/lcRi6zLf3fCO_2Sjtmp/node/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/private/api_auth_token
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      447 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/private/magic_folders.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_bad_listen_string/tFSWItcSXwVx2SCdtmp/node/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.177878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      271 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/api_token
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/folder-SQu5fiZdVu3yYi_fXHOGasM9lBPJrIhE_LYn2BPLbv0=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/folder-SQu5fiZdVu3yYi_fXHOGasM9lBPJrIhE_LYn2BPLbv0=/state.sqlite
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/private/api_auth_token
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      434 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/private/magic_folders.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/node/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.261878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.265878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/private/api_auth_token
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      451 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/private/magic_folders.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_invalid_listen_string/cPF6UO8E_qi5NSbvtmp/node/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.265878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      269 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:52:57.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/api_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:52:57.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/private/api_auth_token
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      437 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/private/magic_folders.yaml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:52:56.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/node/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.181878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.185878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      298 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/api_token
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/folder-ijMf3ecDLzOnHhsuJX2AFm40jgD8sXkU9IvbV6HGMAc=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/folder-ijMf3ecDLzOnHhsuJX2AFm40jgD8sXkU9IvbV6HGMAc=/state.sqlite
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      298 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/api_token
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/folder-56wHhmaOD_DwK2K9BPRf9jb9gttjsRBGAcl13ABfOmc=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/folder-56wHhmaOD_DwK2K9BPRf9jb9gttjsRBGAcl13ABfOmc=/state.sqlite
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.269878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/VfAR58j3XZd49jIbtmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      298 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       44 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/api_token
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/folder-zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag=/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53248 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/folder-zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag=/state.sqlite
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20480 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/global.sqlite
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/gDTTNmpPCKMzAQswtmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:00.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/nAddw1Ta7vcqpksOtmp/tahoe.cfg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/magic-folder.url
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)       22 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/node.url
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.273878 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/private/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)        3 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/private/api_auth_token
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/skBBUk-JEnup1V-1tmp/tahoe.cfg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       41 2023-03-16 04:52:53.000000 magic-folder-23.5.0/docs/_trial_temp/test.log
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1981 2020-04-02 18:49:18.000000 magic-folder-23.5.0/docs/backdoors.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9480 2021-07-26 20:37:49.000000 magic-folder-23.5.0/docs/conf.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7228 2023-05-02 17:54:21.000000 magic-folder-23.5.0/docs/config.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6441 2021-07-26 20:37:49.000000 magic-folder-23.5.0/docs/development.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7928 2023-03-07 23:57:50.000000 magic-folder-23.5.0/docs/downloader.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   664833 2023-03-16 04:53:01.000000 magic-folder-23.5.0/docs/eliot.log
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2973 2023-04-11 21:30:57.000000 magic-folder-23.5.0/docs/index.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    14816 2023-05-02 17:54:21.000000 magic-folder-23.5.0/docs/interface.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    14482 2022-11-11 00:40:27.000000 magic-folder-23.5.0/docs/invite-diagram-readonly.png
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1230 2023-02-07 22:05:58.000000 magic-folder-23.5.0/docs/invite-diagram-readonly.seqdiag
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    16247 2023-01-07 21:02:05.000000 magic-folder-23.5.0/docs/invite-diagram.png
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1229 2023-02-07 22:05:58.000000 magic-folder-23.5.0/docs/invite-diagram.seqdiag
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    13780 2023-02-16 06:39:44.000000 magic-folder-23.5.0/docs/invites.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1512 2023-02-07 22:05:58.000000 magic-folder-23.5.0/docs/limitations.rst
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.277878 magic-folder-23.5.0/docs/proposed/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    24834 2021-06-11 15:26:48.000000 magic-folder-23.5.0/docs/proposed/LightweightDesignscanfornewfiles.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4076 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/proposed/conflict-api.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      659 2023-04-11 21:30:57.000000 magic-folder-23.5.0/docs/proposed/index.rst
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.277878 magic-folder-23.5.0/docs/proposed/magic-folder/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5850 2020-02-04 18:00:11.000000 magic-folder-23.5.0/docs/proposed/magic-folder/filesystem-integration.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18174 2023-04-11 21:30:57.000000 magic-folder-23.5.0/docs/proposed/magic-folder/multi-party-conflict-detection.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    46411 2023-03-16 20:36:16.000000 magic-folder-23.5.0/docs/proposed/magic-folder/remote-to-local-sync.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8620 2020-07-06 21:59:25.000000 magic-folder-23.5.0/docs/proposed/magic-folder/user-interface-design.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)   257416 2021-06-11 16:23:59.000000 magic-folder-23.5.0/docs/proposed/markdown
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4909 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/proposed/recovery.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7356 2021-07-26 20:37:49.000000 magic-folder-23.5.0/docs/proposed/scanning-for-changes.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2075 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/release-process.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      253 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/releases.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6226 2023-03-16 04:36:41.000000 magic-folder-23.5.0/docs/snapshots.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11683 2023-04-11 21:30:57.000000 magic-folder-23.5.0/docs/usage.rst
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.285878 magic-folder-23.5.0/integration/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1397 2022-09-20 06:29:38.000000 magic-folder-23.5.0/integration/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2021-07-26 20:37:49.000000 magic-folder-23.5.0/integration/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3001 2021-06-22 06:43:35.000000 magic-folder-23.5.0/integration/bar
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    12174 2023-04-29 14:16:49.000000 magic-folder-23.5.0/integration/conftest.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9445 2020-06-25 22:39:41.000000 magic-folder-23.5.0/integration/conftest.py.orig
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2110 2021-06-22 06:43:20.000000 magic-folder-23.5.0/integration/foo
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1780 2021-12-21 23:52:48.000000 magic-folder-23.5.0/integration/log.integ
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2021-06-22 06:45:13.000000 magic-folder-23.5.0/integration/pytest.log
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4271 2022-09-20 06:29:38.000000 magic-folder-23.5.0/integration/test_add.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2758 2022-09-20 06:29:38.000000 magic-folder-23.5.0/integration/test_general_cli.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2802 2023-02-16 06:39:44.000000 magic-folder-23.5.0/integration/test_invite.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3363 2023-05-02 17:54:21.000000 magic-folder-23.5.0/integration/test_kitties.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2312 2023-02-07 22:05:58.000000 magic-folder-23.5.0/integration/test_list.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      592 2022-09-20 06:29:38.000000 magic-folder-23.5.0/integration/test_magic_folder.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    16384 2020-06-25 22:17:40.000000 magic-folder-23.5.0/integration/test_magic_folder.py.orig
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    10302 2020-06-25 22:39:42.000000 magic-folder-23.5.0/integration/test_magic_folder.py.rej
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5711 2023-05-02 18:43:42.000000 magic-folder-23.5.0/integration/test_multiuser.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2846 2023-05-02 17:54:21.000000 magic-folder-23.5.0/integration/test_same_files.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1977 2023-05-02 17:54:21.000000 magic-folder-23.5.0/integration/test_status.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    23667 2023-04-18 02:49:28.000000 magic-folder-23.5.0/integration/test_synchronize.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4367 2023-02-07 22:05:58.000000 magic-folder-23.5.0/integration/test_tahoe_objects.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    47467 2023-05-02 18:43:42.000000 magic-folder-23.5.0/integration/util.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    23625 2020-06-25 22:17:40.000000 magic-folder-23.5.0/integration/util.py.orig
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5425 2020-06-25 22:39:43.000000 magic-folder-23.5.0/integration/util.py.rej
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.185878 magic-folder-23.5.0/misc/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.285878 magic-folder-23.5.0/misc/build_helpers/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2889 2022-08-04 09:11:55.000000 magic-folder-23.5.0/misc/build_helpers/platform-pins.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3919 2021-11-25 22:22:35.000000 magic-folder-23.5.0/misc/build_helpers/run-deprecations.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      228 2021-11-25 22:22:35.000000 magic-folder-23.5.0/misc/build_helpers/sqlite_version.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2475 2023-01-20 00:19:51.000000 magic-folder-23.5.0/misc/build_helpers/update-version.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.285878 magic-folder-23.5.0/misc/coding_tools/
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      807 2021-07-26 20:37:49.000000 magic-folder-23.5.0/misc/coding_tools/check-debugging.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.285878 magic-folder-23.5.0/newsfragments/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2022-09-20 06:29:38.000000 magic-folder-23.5.0/newsfragments/.keep-directory
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1455 2022-09-20 06:29:38.000000 magic-folder-23.5.0/pyproject.toml
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      287 2021-08-27 20:55:28.000000 magic-folder-23.5.0/pytest.ini
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.289878 magic-folder-23.5.0/requirements/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      443 2021-11-25 22:22:35.000000 magic-folder-23.5.0/requirements/README
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1397 2023-01-30 21:42:35.000000 magic-folder-23.5.0/requirements/base.in
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    44868 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/base.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      254 2022-09-20 06:29:38.000000 magic-folder-23.5.0/requirements/build.in
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11012 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/build.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3489 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/platform.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       19 2022-09-20 06:29:38.000000 magic-folder-23.5.0/requirements/tahoe-integration-1.17.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       19 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/tahoe-integration-1.18.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       67 2021-07-26 20:37:49.000000 magic-folder-23.5.0/requirements/tahoe-integration-master.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      827 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/test.in
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    16621 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/test.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       48 2022-08-04 09:11:55.000000 magic-folder-23.5.0/requirements/tox.in
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      949 2023-02-07 22:05:58.000000 magic-folder-23.5.0/requirements/tox.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       38 2023-05-02 18:45:15.309878 magic-folder-23.5.0/setup.cfg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2661 2022-09-20 06:29:38.000000 magic-folder-23.5.0/setup.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.189878 magic-folder-23.5.0/src/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.297878 magic-folder-23.5.0/src/magic_folder/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      123 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      152 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/__main__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1171 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/_coverage.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1670 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/_endpoint_parser.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5780 2023-02-07 22:05:58.000000 magic-folder-23.5.0/src/magic_folder/_schema.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      162 2023-05-02 18:45:14.000000 magic-folder-23.5.0/src/magic_folder/_version.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20176 2023-04-29 14:16:49.000000 magic-folder-23.5.0/src/magic_folder/api_cli.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    38333 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/cli.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    13666 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/client.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5264 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/common.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    78056 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/config.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    22660 2023-05-02 18:43:42.000000 magic-folder-23.5.0/src/magic_folder/downloader.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2741 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/endpoints.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1611 2023-02-07 22:05:58.000000 magic-folder-23.5.0/src/magic_folder/initialize.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    20672 2023-04-29 14:16:49.000000 magic-folder-23.5.0/src/magic_folder/invite.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2023-02-07 22:05:58.000000 magic-folder-23.5.0/src/magic_folder/join.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2173 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/list.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    47419 2023-05-02 18:43:42.000000 magic-folder-23.5.0/src/magic_folder/magic_file.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18012 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/magic_folder.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      539 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/magicpath.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2786 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/migrate.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    13438 2023-04-29 14:16:49.000000 magic-folder-23.5.0/src/magic_folder/participants.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4142 2023-01-20 00:19:51.000000 magic-folder-23.5.0/src/magic_folder/pid.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9328 2023-02-08 01:51:42.000000 magic-folder-23.5.0/src/magic_folder/scanner.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18416 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/service.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1286 2023-02-16 06:39:44.000000 magic-folder-23.5.0/src/magic_folder/show_config.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    23391 2023-04-21 21:55:43.000000 magic-folder-23.5.0/src/magic_folder/snapshot.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    21598 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/status.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    14506 2023-02-17 18:23:28.000000 magic-folder-23.5.0/src/magic_folder/tahoe_client.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/src/magic_folder/test/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3189 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      849 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/agentutil.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/src/magic_folder/test/cli/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-05-05 16:38:01.000000 magic-folder-23.5.0/src/magic_folder/test/cli/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6104 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/cli/common.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4451 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/cli/test_api_cli.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    24283 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/cli/test_magic_folder.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6801 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/common.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4962 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/eliotutil.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    16684 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/fixtures.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5130 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/matchers.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/src/magic_folder/test/plugins/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      334 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/plugins/magic_folder_tests_dropin.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    12527 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/strategies.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    26838 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_api_cli.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    22808 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_cli.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4839 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_client.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4663 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_common.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    49601 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_config.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    73041 2023-05-02 18:43:42.000000 magic-folder-23.5.0/src/magic_folder/test/test_download.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5476 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_eliotutil.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1281 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_endpoints.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1188 2022-03-15 06:53:54.000000 magic-folder-23.5.0/src/magic_folder/test/test_foo.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    28373 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_invite.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11803 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_local_snapshot.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    10182 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_magic_file.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8112 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_magic_folder_service.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1199 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_magicpath.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    17352 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_participants.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4646 2023-01-20 00:19:51.000000 magic-folder-23.5.0/src/magic_folder/test/test_pid.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    15544 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_scanner.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7004 2023-02-07 22:05:58.000000 magic-folder-23.5.0/src/magic_folder/test/test_schema.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8026 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_service.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18979 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_snapshot.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    10854 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_status.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2040 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_strategies.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    12958 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_tahoe_client.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5832 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_testing.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    25929 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_upload.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2532 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_util_database.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4535 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_util_file.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6446 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/test/test_util_twisted.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    80071 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/test/test_web.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/src/magic_folder/testing/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-07-07 16:51:27.000000 magic-folder-23.5.0/src/magic_folder/testing/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    18739 2023-01-30 21:42:35.000000 magic-folder-23.5.0/src/magic_folder/testing/web.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    12645 2023-04-29 14:16:49.000000 magic-folder-23.5.0/src/magic_folder/uploader.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/src/magic_folder/util/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2020-05-05 16:38:01.000000 magic-folder-23.5.0/src/magic_folder/util/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6852 2023-04-22 08:12:52.000000 magic-folder-23.5.0/src/magic_folder/util/capabilities.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5603 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/database.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9471 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/eliotutil.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      617 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/encoding.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2473 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/file.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1403 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/observer.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6547 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/twisted.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2176 2022-09-20 06:29:38.000000 magic-folder-23.5.0/src/magic_folder/util/wrap.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    30795 2023-05-02 17:54:21.000000 magic-folder-23.5.0/src/magic_folder/web.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.297878 magic-folder-23.5.0/src/magic_folder.egg-info/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7049 2023-05-02 18:45:14.000000 magic-folder-23.5.0/src/magic_folder.egg-info/PKG-INFO
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    31307 2023-05-02 18:45:15.000000 magic-folder-23.5.0/src/magic_folder.egg-info/SOURCES.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        1 2023-05-02 18:45:14.000000 magic-folder-23.5.0/src/magic_folder.egg-info/dependency_links.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      104 2023-05-02 18:45:14.000000 magic-folder-23.5.0/src/magic_folder.egg-info/entry_points.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      532 2023-05-02 18:45:14.000000 magic-folder-23.5.0/src/magic_folder.egg-info/requires.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       21 2023-05-02 18:45:14.000000 magic-folder-23.5.0/src/magic_folder.egg-info/top_level.txt
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.189878 magic-folder-23.5.0/src/twisted/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-02 18:45:15.309878 magic-folder-23.5.0/src/twisted/plugins/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      301 2021-07-26 20:37:49.000000 magic-folder-23.5.0/src/twisted/plugins/magic_folder_dropin.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5616 2023-02-07 22:05:58.000000 magic-folder-23.5.0/tox.ini
```

### Comparing `magic-folder-23.3.1/.github/workflows/codechecks.yml` & `magic-folder-23.5.0/.github/workflows/codechecks.yml`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/.github/workflows/linux.yml` & `magic-folder-23.5.0/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/.github/workflows/macos.yaml` & `magic-folder-23.5.0/.github/workflows/macos.yaml`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/.github/workflows/windows.yml` & `magic-folder-23.5.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/COPYING.GPL` & `magic-folder-23.5.0/COPYING.GPL`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/COPYING.TGPPL.rst` & `magic-folder-23.5.0/COPYING.TGPPL.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/CREDITS` & `magic-folder-23.5.0/CREDITS`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/DEVELOPERS` & `magic-folder-23.5.0/DEVELOPERS`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/Makefile` & `magic-folder-23.5.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -48,7 +48,13 @@
 	testmf_venv/bin/pip install dist/magic-folder-`git describe --abbrev=0`.tar.gz
 	testmf_venv/bin/magic-folder --version
 	testmf_venv/bin/magic-folder-api --version
 	rm -rf testmf_venv
 
 release-upload:
 	twine upload dist/magic_folder-`git describe --abbrev=0`-py3-none-any.whl dist/magic_folder-`git describe --abbrev=0`-py3-none-any.whl.asc dist/magic-folder-`git describe --abbrev=0`.tar.gz dist/magic-folder-`git describe --abbrev=0`.tar.gz.asc
+
+coverage:
+	-coverage erase
+	MAGIC_FOLDER_HYPOTHESIS_PROFILE=magic-folder-fast coverage run -m twisted.trial magic_folder
+	coverage combine
+	git diff main.. | cuv diff -
```

### Comparing `magic-folder-23.3.1/NEWS.rst` & `magic-folder-23.5.0/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,33 @@
 ﻿.. -*- coding: utf-8-with-signature -*-
 
 .. towncrier start line
+Magic_Folder 23.5.0 (2023-05-02)
+''''''''''''''''''''''''''''''''
+
+Backwards Incompatible Changes
+------------------------------
+
+- The /status endpoint now produces event-based output
+
+  This means the messages emitted via the WebSocket are entirely different.
+  Please see the documentation under "Status API" for the new method.
+  Ordinarily, this would mean a new version of the API (e.g. /v2/) but we
+  do not yet declare a stable /v1 API so it has simply changed.
+
+  Please get in touch if this causes you problems. (`#686 <https://github.com/LeastAuthority/magic-folder/issues/686>`_)
+
+
+Bug Fixes
+---------
+
+- Old or redundant updates from other participants are correctly ignored (`#703 <https://github.com/LeastAuthority/magic-folder/issues/703>`_)
+- If a client saw multiple other Participants with the same update a Conflict was produced (`#713 <https://github.com/LeastAuthority/magic-folder/issues/713>`_)
+
+
 Magic_Folder 23.3.1 (2023-03-20)
 ''''''''''''''''''''''''''''''''
 
 Features
 --------
 
 - Various consistency, formatting and content updates to documentation (`#699 <https://github.com/LeastAuthority/magic-folder/issues/699>`_)
```

### Comparing `magic-folder-23.3.1/NOTES.rst` & `magic-folder-23.5.0/NOTES.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/PKG-INFO` & `magic-folder-23.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-folder
-Version: 23.3.1
+Version: 23.5.0
 Summary: Tahoe-LAFS-based file synchronization
 Home-page: https://github.com/LeastAuthority/magic-folder/
 Author: the Tahoe-LAFS developers, the Magic-Folder developers
 Author-email: tahoe-dev@tahoe-lafs.org
 License: GNU GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `magic-folder-23.3.1/README.rst` & `magic-folder-23.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/.hypothesis/unicode_data/13.0.0/charmap.json.gz` & `magic-folder-23.5.0/docs/.hypothesis/unicode_data/13.0.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/CODE_OF_CONDUCT.rst` & `magic-folder-23.5.0/docs/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/Makefile` & `magic-folder-23.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/CODE_OF_CONDUCT.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/CODE_OF_CONDUCT.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/backdoors.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/backdoors.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/config.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/config.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/datamodel.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/datamodel.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/development.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/development.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/downloader.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/downloader.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/environment.pickle` & `magic-folder-23.5.0/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/index.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/interface.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/interface.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/invites.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/invites.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/leif-design.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/leif-design.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/limitations.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/limitations.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/proposed/conflict-api.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/proposed/conflict-api.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/proposed/index.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/proposed/index.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/proposed/magic-folder/filesystem-integration.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/filesystem-integration.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/proposed/magic-folder/remote-to-local-sync.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/remote-to-local-sync.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/proposed/magic-folder/user-interface-design.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/proposed/magic-folder/user-interface-design.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/proposed/recovery.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/proposed/recovery.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/proposed/scanning-for-changes.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/proposed/scanning-for-changes.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/release-process.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/release-process.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/releases.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/releases.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/snapshots.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/snapshots.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/doctrees/usage.doctree` & `magic-folder-23.5.0/docs/_build/doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/CODE_OF_CONDUCT.html` & `magic-folder-23.5.0/docs/_build/html/CODE_OF_CONDUCT.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_images/magic-folder-data-model--high-level.svg` & `magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model--high-level.svg`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_images/magic-folder-data-model-abstract--conflict.plain.svg` & `magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model-abstract--conflict.plain.svg`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_images/magic-folder-data-model-abstract.svg` & `magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model-abstract.svg`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_images/magic-folder-data-model.svg` & `magic-folder-23.5.0/docs/_build/html/_images/magic-folder-data-model.svg`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/CODE_OF_CONDUCT.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/CODE_OF_CONDUCT.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/backdoors.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/backdoors.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/config.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/config.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/datamodel.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/datamodel.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/development.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/development.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/downloader.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/downloader.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/index.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/interface.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/interface.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/invites.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/invites.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/leif-design.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/leif-design.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/limitations.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/limitations.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/proposed/conflict-api.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/proposed/conflict-api.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/proposed/index.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/proposed/index.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/proposed/magic-folder/filesystem-integration.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/filesystem-integration.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/proposed/magic-folder/remote-to-local-sync.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/remote-to-local-sync.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/proposed/magic-folder/user-interface-design.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/proposed/magic-folder/user-interface-design.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/proposed/recovery.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/proposed/recovery.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/proposed/scanning-for-changes.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/proposed/scanning-for-changes.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/release-process.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/release-process.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/snapshots.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/snapshots.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_sources/usage.rst.txt` & `magic-folder-23.5.0/docs/_build/html/_sources/usage.rst.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/basic.css` & `magic-folder-23.5.0/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/badge_only.css` & `magic-folder-23.5.0/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-bold.woff` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-normal.woff` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `magic-folder-23.5.0/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/css/theme.css` & `magic-folder-23.5.0/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/doctools.js` & `magic-folder-23.5.0/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/js/badge_only.js` & `magic-folder-23.5.0/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `magic-folder-23.5.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/js/html5shiv.min.js` & `magic-folder-23.5.0/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/js/theme.js` & `magic-folder-23.5.0/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/language_data.js` & `magic-folder-23.5.0/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/pygments.css` & `magic-folder-23.5.0/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/searchtools.js` & `magic-folder-23.5.0/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/_static/sphinx_highlight.js` & `magic-folder-23.5.0/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/backdoors.html` & `magic-folder-23.5.0/docs/_build/html/backdoors.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/config.html` & `magic-folder-23.5.0/docs/_build/html/config.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/datamodel.html` & `magic-folder-23.5.0/docs/_build/html/datamodel.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/development.html` & `magic-folder-23.5.0/docs/_build/html/development.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/downloader.html` & `magic-folder-23.5.0/docs/_build/html/downloader.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/genindex.html` & `magic-folder-23.5.0/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/index.html` & `magic-folder-23.5.0/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/interface.html` & `magic-folder-23.5.0/docs/_build/html/interface.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/invites.html` & `magic-folder-23.5.0/docs/_build/html/invites.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/leif-design.html` & `magic-folder-23.5.0/docs/_build/html/leif-design.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/limitations.html` & `magic-folder-23.5.0/docs/_build/html/limitations.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/objects.inv` & `magic-folder-23.5.0/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/proposed/conflict-api.html` & `magic-folder-23.5.0/docs/_build/html/proposed/conflict-api.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/proposed/index.html` & `magic-folder-23.5.0/docs/_build/html/proposed/index.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/proposed/magic-folder/filesystem-integration.html` & `magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/filesystem-integration.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/proposed/magic-folder/remote-to-local-sync.html` & `magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/remote-to-local-sync.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/proposed/magic-folder/user-interface-design.html` & `magic-folder-23.5.0/docs/_build/html/proposed/magic-folder/user-interface-design.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/proposed/recovery.html` & `magic-folder-23.5.0/docs/_build/html/proposed/recovery.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/proposed/scanning-for-changes.html` & `magic-folder-23.5.0/docs/_build/html/proposed/scanning-for-changes.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/release-process.html` & `magic-folder-23.5.0/docs/_build/html/release-process.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/releases.html` & `magic-folder-23.5.0/docs/_build/html/releases.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/search.html` & `magic-folder-23.5.0/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/searchindex.js` & `magic-folder-23.5.0/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/snapshots.html` & `magic-folder-23.5.0/docs/_build/html/snapshots.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_build/html/usage.html` & `magic-folder-23.5.0/docs/_build/html/usage.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder/P3vUVeyBdQnm5S2ztmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_poll_magic_folder_missing_name/EQuaV2Wj2iFHMr89tmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder/c8cAydQ3L9v5oIFrtmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_api_cli/ScanMagicFolder/test_scan_magic_folder_missing_name/E7RU2Fm2bKW6FA5Itmp/folder-N6juwc4ZaH0TL-KQUdymKdFk4sSVi6FB1fQTOjPwaI8=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp/IIzFX8YQ1w6AP1Vttmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_tcp_host/GyI4uBnJtcR17_7ktmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_convert_unix/HTlRFJZ1igEjagGFtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_client_endpoint/YVFST1O-m259ALkQtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ClientEndpoint/test_set_invalid_client_endpoint/ALMSWcCS66iiSNFptmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_config_directory/tXvVinVg5i7-h4FFtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ConfigOptionTests/test_default_config_directory/jAKmUn8aLqzdaCeptmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder/qcJXmoMJXdoNQa_htmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_disable_scanning/KGQGf_rIamqAcEb3tmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_add_magic_folder_intervals/GpixFAwadiwqY_EVtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_create_duplicate_name/nRwusIx_8qp2GfIdtmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/CreateMagicFolder/test_leave_wrong_folder/kTorha6pC6toQEmltmp/folder-LCa0a2j_xo_5m0U8HTBBNBNCLXBkg7-g-YpeiGJm564=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/folder-y8qFhiM2lyCn8nJGeaH4ciGaHxbMbSziNeOGf-Bnma0=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some/g0kA6GBvvzHktIV1tmp/folder-y8qFhiM2lyCn8nJGeaH4ciGaHxbMbSziNeOGf-Bnma0=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/folder-hoqYtkBoInB3B9NowQg2NYo1DccfQVbrYOYb5dPgURo=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/cli/test_magic_folder/ListMagicFolder/test_list_some_json/bp5dhja1WTDZ27T5tmp/folder-hoqYtkBoInB3B9NowQg2NYo1DccfQVbrYOYb5dPgURo=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestDumpState/test_happy/nAao0ZJlC3oPMXWjtmp/folder-n4bQgYhMfWWaL-qgxVrQFaO_TxsrC4Is0V1sFbDwCgg=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_api_error/Vx5KlL9T1q1q8oWltmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_load_config/kXhM7SD1RblH3h24tmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_no_access/AB5b1s1NbU1JB4mXtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_api_cli/TestMagicApi/test_unknown_error/i-QO8cNfgLZXFBHwtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestInitialize/test_good/etzHYCVC-dNkO8yWtmp/good/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/folder-SQu5fiZdVu3yYi_fXHOGasM9lBPJrIhE_LYn2BPLbv0=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/folder-SQu5fiZdVu3yYi_fXHOGasM9lBPJrIhE_LYn2BPLbv0=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestMigrate/test_good/fbxa6aQRXES-0aMItmp/new_magic/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_cli/TestShowConfig/test_good/39zSVD7tYk-qJO-8tmp/good/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/folder-ijMf3ecDLzOnHhsuJX2AFm40jgD8sXkU9IvbV6HGMAc=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/folder-ijMf3ecDLzOnHhsuJX2AFm40jgD8sXkU9IvbV6HGMAc=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/TSsu8aPir7VH4GJxtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/folder-56wHhmaOD_DwK2K9BPRf9jb9gttjsRBGAcl13ABfOmc=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/folder-56wHhmaOD_DwK2K9BPRf9jb9gttjsRBGAcl13ABfOmc=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/UpK-8PZFEptcHxGAtmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/folder-zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag=/state.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/folder-zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag=/state.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/global.sqlite` & `magic-folder-23.5.0/docs/_trial_temp/magic_folder/test/test_config/GlobalConfigDatabaseMagicFolderTests/test_create_folder/eNdQcEFHqJNqB6Bitmp/global.sqlite`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/backdoors.rst` & `magic-folder-23.5.0/docs/backdoors.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/conf.py` & `magic-folder-23.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/config.rst` & `magic-folder-23.5.0/docs/config.rst`

 * *Files 0% similar despite different names*

```diff
@@ -64,16 +64,18 @@
 As we are currently re-designing the storage mechanism, some of this
 might change. However, based on current understanding the state we
 WANT to store is:
 
 - for each magic-folder (indexed by "name"):
   - local directory path (the "magic folder")
   - an author:
+
     - name
     - private_key (32 bytes, a NaCl signing key)
+
   - a write-cap of our mutable directory
   - some state (see below)
 - the node-directory of our Tahoe-LAFS client
   - we may need the ``private/api_auth_token``
   - we will need the ``node.url`` (at least)
   - (it MAY be sufficient to only store the API endpoint (the contents
     of ``node.url``), not node-directory. If it's feasible to only store
```

### Comparing `magic-folder-23.3.1/docs/development.rst` & `magic-folder-23.5.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/downloader.rst` & `magic-folder-23.5.0/docs/downloader.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/eliot.log` & `magic-folder-23.5.0/docs/eliot.log`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/index.rst` & `magic-folder-23.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/interface.rst` & `magic-folder-23.5.0/docs/interface.rst`

 * *Files 12% similar despite different names*

```diff
@@ -223,14 +223,33 @@
 There will be one entry in the list for every file.
 The list is ordered from most-recent to least-recent timestamp.
 ``relpath`` is the relative path in the magic-folder.
 ``mtime`` is in seconds.
 ``size`` is in bytes.
 
 
+GET ``/v1/magic-folder/<folder-name>/recent-changes``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Takes an optional ``?number=`` argument (default is 30).
+Returns a list of the most-recent changes, like::
+
+    [
+        {
+            "relpath": "rel/path/foo",
+            "modified": 12345,
+            "last-updated": 12345,
+            "conflicted": false
+        },
+        # ...
+    ]
+
+The results will be reverse-chronological on ``"last-updated"``.
+
+
 GET ``/v1/magic-folder/<folder-name>/tahoe-objects``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Returns a list of integers representing the sizes of all individual capabilities that this folder is using.
 That means a size for each Snapshot capability and its corresponding metadata capability and content capability.
 The list is flat; if there are 2 Snapshots on the grid this will return 6 integers.
 
@@ -321,78 +340,54 @@
 Status API
 ----------
 
 There is a WebSocket-based status API located at ``/v1/status``.
 This is authenticated the same way as the HTTP API with an ``Authorization:`` header (see above).
 
 All messages are JSON.
-Upon connecting, a new client will immediately receive a "state" message::
+Every message looks like this::
 
     {
-        "state": {
-            "folders": {
-                "default": {
-                    "downloads": [],
-                    "errors": [],
-                    "uploads": [],
-                    "recent": [
-                        {
-                            "relpath": "foo"
-                            "conflicted": false,
-                            "modified": 1634431697,
-                            "last-updated": 1634431700
-                        }
-                    ]
-                }
-            },
-            "synchronizing": false,
-            "tahoe": {
-                "connected": 3,
-                "happy": true,
-                "desired": 2
-            },
-            "scanner": {
-                "last-scan": 1634431700.1234
-            },
-            "poller": {
-                "last-poll": null
-            }
-        }
+        "events": []
     }
 
-After that the client may receive further state updates with a ``"state"`` message like the above.
-Currently the only valid kind of message is ``"state"``.
-The above example has no uploads or downloads happening and a single recent file, ``foo``.
-
-The state for each folder consists of the following information:
-
-- ``"synchronizing"``: ``true`` or ``false``. When ``true`` the
-  magic-folder daemon is uploading data to or downloading data from
-  Tahoe-LAFS.
-- ``"tahoe"``: a dict containing status information about the Tahoe-LAFS connection
-  - ``"connected"``: the number of storage-servers the client is connected to
-  - ``"desired"``: the number of storage-servers we want to connect to
-  - ``"happy"``: ``true`` if ``"connected"`` is greater than the client's configured "happy"
-- ``"folders"`` contains keys mapping the folder name to:
-  - ``"uploads"`` and ``"downloads"`` contain currently queued or active uploads (or downloads). Each ``dict`` in these lists contain:
-
-    - ``"relpath"``: the relative-path
-    - ``"queued-at"``: the Unix timestamp when this item was queued
-    - ``"started-at"``: the Unix timestamp when we started uploading (or downloading) this item. This key will not exist until we do start.
-
-  - ``"recent"`` contains a list up to 30 of the most-recently updated files. Each ``dict`` in this list contains:
-
-    - ``"relpath"``: the relative path of this item
-    - ``"modified"``: the Unix timestamp when the on-disk file was most-recently modified
-    - ``"last-updated"``: the Unix timestamp when this item's state was updated in the magic-folder
-    - ``"conflicted"``: a boolean indicating if there is a conflict for this relative path
-  - ``"scanner"`` contains information about the local changes scanner
-    - ``"last-scan"``: ``null`` if no scan is completed yet, or the timestamp of the last completion
-  - ``"poller"`` contains information about the remote changes poller
-    - ``"last-poll"``: ``null`` if no scan is completed yet, or the timestamp of the last completion
-
-Clients should be tolerant of keys in the state they don't understand.
-Unknown state keys should be ignored.
-Note that ``"modified"`` is when the local state for thie item changed while ``"last-updated"`` is to do with the filesystem modification time.
-For example, a file may have an on-disk modification time that is older than the last time we updated our state about it, especially one that came from another device.
+...where the ``events`` list contains some non-zero number of event messages.
+The first message, upon connect, will likely contain many events: enough to give a consistent view of the current state.
+Thereafter, most messages will include only a single event (although clients should handle any number).
+
+Every event has a ``"kind"`` key describing what sort of message it is.
+Events will contain other keys; clients should be tolerant of keys in the state they don't understand.
 
 The client doesn't send any messages to the server; it is an error to do so.
+
+The follow event kinds are understood (see ``status.py`` for more details on the sending side, and ``cli.py`` for an example of receiving them):
+
+- ``"scan-completed"``: has key ``timestamp`` which is a unix-timestamp saying when we last looked for local changes.
+
+- ``"poll-completed"``: has a key ``timestamp`` describing when we last asked for remote changes.
+
+- ``"tahoe-connection-changed"``: describes the status of our connected Tahoe-LAFS client: ``connected`` and ``desired`` are the number of servers we are conencted to (and how many we want). Whether we are currently connected to enough is in a boolean ``happy``.
+
+- ``"error-occurred"``: An error, with ``folder`` (the name for the affected folder) ``timestamp`` and ``summary`` (human-readable string).
+
+- ``"folder-added"``: Key ``folder`` says which folder was added.
+
+- ``"folder-left"``: Key ``folder`` says which folder has gone away.
+
+- ``"upload-queued"``: some file (``relpath``) in a folder (``folder``) is queued for upload since ``timestamp``.
+
+- ``"upload-started"``: some file (``relpath``) in a folder (``folder``) has begun upload since ``timestamp``. An ``upload-queued`` event will always preceed this.
+
+- ``"upload-finished"``: a file (``relpath``) in a folder (``folder``) has completed at ``timestamp``. An ``upload-started`` will always preceed this.
+
+- ``"download-queued"``: same as upload version.
+
+- ``"download-started"``: same as upload version.
+
+- ``"download-finished"``: same as upload version.
+
+All timestamps are "seconds since the Unix epoch", as numbers (JSON only has "numbers" and doesn't distinguish floats from ints).
+
+Note that the first "update events" message received will _not_ contain all the updates to that point; it will synthesize the correct events to communicate the current state.
+For example, if there are 50 files in the folder and 48 have already been uploaded, there will be just 2 ``upload-queued`` events (because the other 48 have all finished already).
+If one of these files is currently being uploaded, there will also be a ``upload-started`` event.
+To know the state of all files, use the other endpoints.
```

### Comparing `magic-folder-23.3.1/docs/invite-diagram-readonly.png` & `magic-folder-23.5.0/docs/invite-diagram-readonly.png`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/invite-diagram-readonly.seqdiag` & `magic-folder-23.5.0/docs/invite-diagram-readonly.seqdiag`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/invite-diagram.png` & `magic-folder-23.5.0/docs/invite-diagram.png`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/invite-diagram.seqdiag` & `magic-folder-23.5.0/docs/invite-diagram.seqdiag`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/invites.rst` & `magic-folder-23.5.0/docs/invites.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/limitations.rst` & `magic-folder-23.5.0/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/proposed/LightweightDesignscanfornewfiles.html` & `magic-folder-23.5.0/docs/proposed/LightweightDesignscanfornewfiles.html`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/proposed/conflict-api.rst` & `magic-folder-23.5.0/docs/proposed/conflict-api.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/proposed/index.rst` & `magic-folder-23.5.0/docs/proposed/index.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/proposed/magic-folder/filesystem-integration.rst` & `magic-folder-23.5.0/docs/proposed/magic-folder/filesystem-integration.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/proposed/magic-folder/multi-party-conflict-detection.rst` & `magic-folder-23.5.0/docs/proposed/magic-folder/multi-party-conflict-detection.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/proposed/magic-folder/remote-to-local-sync.rst` & `magic-folder-23.5.0/docs/proposed/magic-folder/remote-to-local-sync.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/proposed/magic-folder/user-interface-design.rst` & `magic-folder-23.5.0/docs/proposed/magic-folder/user-interface-design.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/proposed/markdown` & `magic-folder-23.5.0/docs/proposed/markdown`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/proposed/recovery.rst` & `magic-folder-23.5.0/docs/proposed/recovery.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/proposed/scanning-for-changes.rst` & `magic-folder-23.5.0/docs/proposed/scanning-for-changes.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/release-process.rst` & `magic-folder-23.5.0/docs/release-process.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/snapshots.rst` & `magic-folder-23.5.0/docs/snapshots.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/docs/usage.rst` & `magic-folder-23.5.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/README` & `magic-folder-23.5.0/integration/README`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/bar` & `magic-folder-23.5.0/integration/bar`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/conftest.py` & `magic-folder-23.5.0/integration/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,14 +372,33 @@
             wormhole_url="ws://localhost:4000/v1",
             storage=True,
         )
     )
 
 
 @pytest.fixture(scope='session')
+def fran(reactor, tahoe_venv, base_dir, introducer_furl, flog_gatherer, request):
+    return pytest_twisted.blockon(
+        MagicFolderEnabledNode.create(
+            reactor,
+            tahoe_venv,
+            request,
+            base_dir,
+            introducer_furl,
+            flog_gatherer,
+            u"fran",
+            tahoe_web_port=u"tcp:9986:interface=localhost",
+            magic_folder_web_port=u"tcp:19986:interface=localhost",
+            wormhole_url="ws://localhost:4000/v1",
+            storage=False,
+        )
+    )
+
+
+@pytest.fixture(scope='session')
 def wormhole(reactor, request):
     """
     A local Magic Wormhole mailbox server
     """
     return pytest_twisted.blockon(
         WormholeMailboxServer.create(
             reactor,
```

### Comparing `magic-folder-23.3.1/integration/conftest.py.orig` & `magic-folder-23.5.0/integration/conftest.py.orig`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/foo` & `magic-folder-23.5.0/integration/foo`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/log.integ` & `magic-folder-23.5.0/integration/log.integ`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/test_add.py` & `magic-folder-23.5.0/integration/test_add.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/test_general_cli.py` & `magic-folder-23.5.0/integration/test_general_cli.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/test_invite.py` & `magic-folder-23.5.0/integration/test_invite.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/test_kitties.py` & `magic-folder-23.5.0/integration/test_kitties.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,26 +70,40 @@
     # perform a scan, which will create LocalSnapshots for all the
     # files we already created in the magic-folder (but _not_ upload
     # them, necessarily, yet)
     print("start scan")
     await alice.scan("kitties")
     print("scan done")
 
+    def find_uploads(data):
+        pending = []
+        for event in data["events"]:
+            if event["kind"].startswith("upload-"):
+                pending.append(event)
+        return pending
+
     # wait for a limited time to be complete
+    uploads = 0
     for _ in range(10):
         st = await alice.status()
         data = json.loads(st.strip())
-        if data["state"]["synchronizing"] is False:
+        uploads = len(find_uploads(data))
+        if uploads == 0:
             break
         await twisted_sleep(reactor, 1)
-    assert data["state"]["synchronizing"] is False, "Should be finished uploading"
+    assert uploads == 0, "Should be finished uploading"
+
+    errors = [
+        evt for evt in data["events"]
+        if evt["kind"] == "error"
+    ]
+    assert errors == [], "Expected zero errors: {}".format(errors)
 
-    kitties = data["state"]["folders"]["kitties"]
-    assert kitties["errors"] == [], "Expected zero errors"
-    actual_cats = {cat["relpath"] for cat in kitties["recent"]}
+    recent = await alice.client.recent_changes("kitties")
+    actual_cats = {cat["relpath"] for cat in recent}
     expected = set(cat_names + ["subdir/{}".format(n) for n in cat_names])
     assert expected == actual_cats, "Data mismatch"
 
     # confirm that we can navigate Collective -> alice and find the
     # correct Snapshots (i.e. one for every cat-pic)
     folders = await alice.list_(True)
```

### Comparing `magic-folder-23.3.1/integration/test_list.py` & `magic-folder-23.5.0/integration/test_list.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/test_magic_folder.py` & `magic-folder-23.5.0/integration/test_magic_folder.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/test_magic_folder.py.orig` & `magic-folder-23.5.0/integration/test_magic_folder.py.orig`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/test_magic_folder.py.rej` & `magic-folder-23.5.0/integration/test_magic_folder.py.rej`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/test_same_files.py` & `magic-folder-23.5.0/integration/test_same_files.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,26 +60,39 @@
     # perform a scan, which will create LocalSnapshots for all the
     # files we already created in the magic-folder (but _not_ upload
     # them, necessarily, yet)
     print("start scan")
     await alice.scan("sames")
     print("scan done")
 
+    def find_uploads(data):
+        pending = []
+        for event in data["events"]:
+            if event["kind"].startswith("upload-"):
+                pending.append(event)
+        return pending
+
     # wait for a limited time to be complete
+    uploads = 0
     for _ in range(10):
-        st = await alice.status()
-        data = json.loads(st.strip())
-        if data["state"]["synchronizing"] is False:
+        data = json.loads(await alice.status())
+        uploads = len(find_uploads(data))
+        if uploads == 0:
             break
         await twisted_sleep(reactor, 1)
-    assert data["state"]["synchronizing"] is False, "Should be finished uploading"
+    assert uploads == 0, "Should be finished uploading"
+
+    errors = [
+        evt for evt in data["events"]
+        if evt["kind"] == "error"
+    ]
+    assert errors == [], "Expected zero errors: {}".format(errors)
 
-    sames = data["state"]["folders"]["sames"]
-    assert sames["errors"] == [], "Expected zero errors"
-    actual_cats = {cat["relpath"] for cat in sames["recent"]}
+    recent = await alice.client.recent_changes("sames")
+    actual_cats = {cat["relpath"] for cat in recent}
     expected = set(cat_names)
     assert expected == actual_cats, "Data mismatch"
 
     # confirm that we can navigate Collective -> alice and find the
     # correct Snapshots (i.e. one for every cat-pic)
     folders = await alice.list_(True)
```

### Comparing `magic-folder-23.3.1/integration/test_status.py` & `magic-folder-23.5.0/integration/test_status.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,19 +46,19 @@
         pytest_twisted.blockon(alice.leave("outstanding1"))
     request.addfinalizer(cleanup)
 
     # add the "other" folder as a participant .. simulate recovery
     await alice.add_participant("outstanding1", "old", zero_cap)
 
     downloads = None
-    while downloads is None:
+    while not downloads:
         status_data = await alice.status()
         status = json.loads(status_data)
-        one = status["state"]["folders"].get("outstanding1", None)
-        if one:
-            print(json.dumps(one, indent=4))
-            if one["downloads"]:
-                downloads = one["downloads"]
+        downloads = [
+            down
+            for down in status["events"]
+            if down["kind"].startswith("download-")
+        ]
         await twisted_sleep(reactor, .2)
 
     print("found downloads: {}".format(downloads))
     assert {d["relpath"] for d in downloads} == set(filenames)
```

### Comparing `magic-folder-23.3.1/integration/test_synchronize.py` & `magic-folder-23.5.0/integration/test_synchronize.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/test_tahoe_objects.py` & `magic-folder-23.5.0/integration/test_tahoe_objects.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/util.py` & `magic-folder-23.5.0/integration/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import time
 import json
 import sqlite3
 import os
+import re
 from os import mkdir
 from io import (
     BytesIO,
     StringIO,
 )
 from os.path import exists, join
 from functools import partial
@@ -34,14 +35,18 @@
     ProcessDone,
 )
 from twisted.python.filepath import (
     FilePath,
 )
 from twisted.web.client import Agent
 
+from autobahn.twisted.websocket import (
+    create_client_agent,
+)
+
 import treq
 
 from eliot import (
     log_message,
     current_action,
     start_action,
     start_task,
@@ -563,14 +568,51 @@
             [
                 "--config", self.magic_config_directory,
                 "monitor",
                 "--once",
             ],
         )
 
+    @inline_callbacks
+    def status_monitor(self, how_long):
+        """
+        collect the output of `magic-folder-api monitor` for `how_long`
+        seconds and return all the output (as a list of JSON-decoded
+        events)
+        """
+        # FIXME: should use FilePath throughout this class
+        config = FilePath(self.magic_config_directory)
+        # XXX some of this duplicated from api_cli / cli -- would be
+        # nice to not do that...
+        with config.child("api_client_endpoint").open("rb") as f:
+            endpoint_str = f.read().decode("utf8").strip()
+        websocket_uri = "{}/v1/status".format(endpoint_str.replace("tcp:", "ws://"))
+
+        agent = create_client_agent(self.reactor)
+        with config.child("api_token").open("rb") as f:
+            token = f.read()
+        proto = yield agent.open(
+            websocket_uri,
+            {
+                "headers": {
+                    "Authorization": "Bearer {}".format(token.decode("utf8")),
+                }
+            }
+        )
+        messages = []
+
+        def foo(data, is_binary=False):
+            msg = json.loads(data.decode("utf8"))
+            messages.extend(msg["events"])
+        proto.on("message", foo)
+
+        # collect some messages
+        yield deferLater(self.reactor, how_long)
+        returnValue(messages)
+
     def dump_state(self, folder_name):
         """
         magic-folder-api dump-state
         """
         return _magic_folder_api_runner(
             self.reactor, self.request, self.name,
             [
@@ -1138,14 +1180,27 @@
     """
     def __init__(self, path, timeout):
         super(FileShouldVanishException, self).__init__(
             u"'{}' still exists after {}s".format(path, timeout),
         )
 
 
+def find_conflicts(path):
+    """
+    Check a directory and any sub-directories for any files that look
+    like magic-folder conflict markers
+    """
+    conflict_re = re.compile(r".*\.conflict-.*")
+    return [
+        child
+        for child in path.walk()
+        if conflict_re.match(child.basename())
+    ]
+
+
 @log_inline_callbacks(action_type=u"integration:await-file-contents", include_args=True)
 def await_file_contents(path, contents, timeout=15):
     """
     Return a deferred that fires when the file at `path` (any path-like
     object) has the exact content `contents`.
 
     :raises ExpectedFileMismatchException: if the path doesn't have the
```

### Comparing `magic-folder-23.3.1/integration/util.py.orig` & `magic-folder-23.5.0/integration/util.py.orig`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/integration/util.py.rej` & `magic-folder-23.5.0/integration/util.py.rej`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/misc/build_helpers/platform-pins.py` & `magic-folder-23.5.0/misc/build_helpers/platform-pins.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/misc/build_helpers/run-deprecations.py` & `magic-folder-23.5.0/misc/build_helpers/run-deprecations.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/misc/build_helpers/update-version.py` & `magic-folder-23.5.0/misc/build_helpers/update-version.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/misc/coding_tools/check-debugging.py` & `magic-folder-23.5.0/misc/coding_tools/check-debugging.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/pyproject.toml` & `magic-folder-23.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/requirements/base.in` & `magic-folder-23.5.0/requirements/base.in`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/requirements/base.txt` & `magic-folder-23.5.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/requirements/build.txt` & `magic-folder-23.5.0/requirements/build.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/requirements/platform.txt` & `magic-folder-23.5.0/requirements/platform.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/requirements/test.in` & `magic-folder-23.5.0/requirements/test.in`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/requirements/test.txt` & `magic-folder-23.5.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/requirements/tox.txt` & `magic-folder-23.5.0/requirements/tox.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/setup.py` & `magic-folder-23.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/_coverage.py` & `magic-folder-23.5.0/src/magic_folder/_coverage.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/_endpoint_parser.py` & `magic-folder-23.5.0/src/magic_folder/_endpoint_parser.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/_schema.py` & `magic-folder-23.5.0/src/magic_folder/_schema.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/api_cli.py` & `magic-folder-23.5.0/src/magic_folder/api_cli.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/cli.py` & `magic-folder-23.5.0/src/magic_folder/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import sys
 import getpass
+import json
+import humanize
 from io import StringIO
+from collections import defaultdict
+from datetime import datetime
 
 from appdirs import (
     user_config_dir,
 )
 from base64 import (
     urlsafe_b64decode,
 )
@@ -29,14 +33,17 @@
     FilePath,
 )
 from twisted.python import usage
 from twisted.web import http
 from twisted.logger import (
     Logger,
 )
+from autobahn.twisted.websocket import (
+    create_client_agent,
+)
 from wormhole.cli.public_relay import (
     RENDEZVOUS_RELAY,
 )
 
 from eliot.twisted import (
     inline_callbacks,
 )
@@ -348,76 +355,217 @@
     description = (
         "Show status of magic-folders"
     )
     optFlags = [
     ]
 
 
-from autobahn.twisted.websocket import (
-    create_client_agent,
-)
-
 @inline_callbacks
 def status(options):
     """
     Status of magic-folders
     """
     endpoint_str = options.parent.api_client_endpoint
     websocket_uri = "{}/v1/status".format(endpoint_str.replace("tcp:", "ws://"))
+    agent = options.parent.websocket_agent
+    out = options.parent.stdout
+    reactor = options.parent.reactor
 
-    from twisted.internet import reactor
-    agent = create_client_agent(reactor)
-    proto = yield agent.open(
-        websocket_uri,
-        {
-            "headers": {
-                "Authorization": "Bearer {}".format(options.parent.config.api_token.decode("utf8")),
-            }
+    def fresh_folder():
+        """
+        Initial state for an as-yet-unseen folder
+        """
+        return {
+            "last-scan": None,
+            "last-poll": None,
+            "uploads": defaultdict(dict),
+            "downloads": defaultdict(dict),
+            "errors": [],
+        }
+
+    # the daemon sends us _updates_, so we must track our state
+    state = {
+        "folders": defaultdict(fresh_folder),
+        "tahoe": {
+            "happy": False,
+            "connected": None,
+            "desired": None,
         },
-    )
+    }
 
-    import json
-    import humanize
-    def message(payload, is_binary=False):
+    # lambdas can't assign things
+    def copy_state(dest, src, keys):
+        for k in keys:
+            dest[k] = src[k]
+
+    def error(e):
+        """
+        Handle a kind=error message
+        """
+        state["folders"][e["folder"]]["errors"].append({
+            "timestamp": e["timestamp"],
+            "summary": e["summary"],
+        })
+
+    def upload(e):
+        """
+        Handle all events related to uploads
+        """
+        ours = state["folders"][e["folder"]]["uploads"]
+        if e["kind"] == "upload-queued":
+            ours[e["relpath"]]["queued-at"] = e["timestamp"]
+        elif e["kind"] == "upload-started":
+            ours[e["relpath"]]["started-at"] = e["timestamp"]
+
+        # XXX might want a final "upload-stats" sort of thing as well?
+        elif e["kind"] == "upload-finished":
+            del ours[e["relpath"]]
+
+    def download(e):
+        """
+        Handle all events related to downloads
+        """
+        ours = state["folders"][e["folder"]]["downloads"]
+        if e["kind"] == "dowload-queued":
+            ours[e["relpath"]]["queued-at"] = e["timestamp"]
+        elif e["kind"] == "download-started":
+            ours[e["relpath"]]["started-at"] = e["timestamp"]
+
+        # XXX might want a final "download-stats" sort of thing as well?
+        if e["kind"] == "download-finished":
+            del ours[e["relpath"]]
+
+    # it might be interesting to have a status command that simply
+    # dumps event as they arrive. the original (state-message-based)
+    # UI did dump the "whole state at once" so at the very least this
+    # serves as proof a UI _can_ do that properly with this events API
+    folders = yield options.parent.client.list_folders()
+    for folder_name in folders.keys():
+        print("  recent:", file=out)
+        recent = yield options.parent.client.recent_changes(folder_name, 3)
         now = reactor.seconds()
-        data = json.loads(payload)["state"]
-        for folder_name, folder in data["folders"].items():
-            print('Folder "{}":'.format(folder_name))
-            print("  downloads: {}".format(len(folder["downloads"])))
-            if folder["downloads"]:
-                print("    {}".format(
-                    ", ".join(d["relpath"] for d in folder["downloads"])
-                ))
-            print("  uploads: {}".format(len(folder["uploads"])))
-            for u in folder["uploads"]:
-                queue = humanize.naturaldelta(now - u["queued-at"])
-                start = " (started {} ago)".format(humanize.naturaldelta(now - u["started-at"])) if "started-at" in u else ""
-                print("    {}: queued {} ago{}".format(u["relpath"], queue, start))
-            print("  recent:")
-            for f in folder["recent"]:
-                if f["relpath"] in folder["uploads"] or f["relpath"] in folder["downloads"]:
-                    continue
-                if f["modified"] is not None:
-                    modified_text = "modified {} ago".format(
-                        humanize.naturaldelta(now - f["modified"])
-                    )
-                else:
-                    modified_text = "[deleted]"
-                print("    {}: {}{} (updated {} ago)".format(
+        for f in recent:
+            if f["modified"] is not None:
+                modified_text = "modified {} ago".format(
+                    humanize.naturaldelta(now - f["modified"])
+                )
+            else:
+                modified_text = "[deleted]"
+            print(
+                "    {}: {}{} (updated {} ago)".format(
                     f["relpath"],
                     "[CONFLICT] " if f["conflicted"] else "",
                     modified_text,
                     humanize.naturaldelta(now - f["last-updated"]),
-                ))
+                ),
+                file=out,
+            )
+
+    # based on the "kind" of event, we update our state
+    updates = {
+        "scan-completed": lambda e: copy_state(state["folders"][e["folder"]], e, {"last-scan"}),
+        "poll-completed": lambda e: copy_state(state["folders"][e["folder"]], e, {"last-poll"}),
+        "tahoe-connection-changed": lambda e: copy_state(state["tahoe"], e, {"happy", "connected", "desired"}),
+        "error-occurred": error,
+        "folder-added": lambda _: None,
+        "folder-deleted": lambda _: None,
+        "upload-queued": upload,
+        "upload-started": upload,
+        "upload-finished": upload,
+        "download-queued": download,
+        "download-started": download,
+        "download-finished": download,
+    }
+
+    def message(payload, is_binary=False):
+        """
+        onMessage handler for WebSocket payloads.
+
+        The first message should contain all events necessary for our
+        state to match the actual state.
+        """
+        now = reactor.seconds()
+        data = json.loads(payload)
+
+        for event in data["events"]:
+            assert "kind" in event and event["kind"] in updates, "weird: {}".format(event["kind"])
+            updates[event["kind"]](event)
+
+        for folder_name, folder in state["folders"].items():
+            print('Folder "{}":'.format(folder_name), file=out)
+            print("  downloads: {}".format(len(folder["downloads"])), file=out)
+            if folder["downloads"]:
+                print(
+                    "    {}".format(
+                        ", ".join(folder["downloads"].keys())
+                    ),
+                    file=out,
+                )
+            print("  uploads: {}".format(len(folder["uploads"])), file=out)
+            for relpath, u in folder["uploads"].items():
+                queue = humanize.naturaldelta(now - u["queued-at"])
+                start = " (started {} ago)".format(humanize.naturaldelta(now - u["started-at"])) if "started-at" in u else ""
+                print("    {}: queued {} ago{}".format(relpath, queue, start), file=out)
+
             if folder["errors"]:
-                print("Errors:")
+                print("Errors:", file=out)
+                # filter out duplicates
+                different_errors = {}
                 for e in folder["errors"]:
-                    print("  {}: {}".format(e["timestamp"], e["summary"]))
-    proto.on('message', message)
+                    summary = e["summary"]
+                    if summary in different_errors:
+                        different_errors[summary]["timestamps"].append(e["timestamp"])
+                    else:
+                        different_errors[summary] = {
+                            "summary": summary,
+                            "timestamps": [e["timestamp"]],
+                        }
+                for summary, e in different_errors.items():
+                    if len(e["timestamps"]) == 1:
+                        ts = humanize.naturaldelta(now - e["timestamps"][0])
+                    else:
+                        ts = "{} times between {} and {}".format(
+                            len(e["timestamps"]),
+                            humanize.naturaldelta(now - e["timestamps"][-1]),
+                            humanize.naturaldelta(now - e["timestamps"][0]),
+                        )
+                    print("  {} ({} ago)".format(summary, ts), file=out)
+            if folder["last-scan"] is not None:
+                print(
+                    "Last scan for uploads at {}".format(
+                        datetime.fromtimestamp(folder["last-scan"]),
+                    ),
+                    file=out,
+                )
+            if folder["last-poll"] is not None:
+                print(
+                    "Last poll for downloads at {}".format(
+                        datetime.fromtimestamp(folder["last-poll"]),
+                    ),
+                    file=out,
+                )
+        print(
+            "Tahoe is {is_happy}: connected to {connected} servers (want {desired})".format(
+                is_happy="happy" if state["tahoe"]["happy"] else "UNHAPPY",
+                **state["tahoe"]
+            ),
+            file=out,
+        )
 
+    # note: can't do async work between creating the proto and adding
+    # the on-message handler, or you might miss an update
+    proto = yield agent.open(
+        websocket_uri,
+        {
+            "headers": {
+                "Authorization": "Bearer {}".format(options.parent.config.api_token.decode("utf8")),
+            }
+        },
+    )
+    proto.on('message', message)
     yield proto.is_closed
 
 
 class ListOptions(usage.Options):
     description = (
         "List all magic-folders this client has joined"
     )
@@ -740,14 +888,15 @@
         ("config", "c", _default_config_path,
          "The directory containing configuration"),
     ]
 
     _config = None  # lazy-instantiated by .config @property
     _http_client = None  # lazy-initalized by .client @property
     _client = None  # lazy-instantiated by .client @property
+    _ws_agent = None  # lazy-instantiated by .websocket_agent
 
     @property
     def _config_path(self):
         """
         The FilePath where our config is located
         """
         return FilePath(self['config'])
@@ -797,14 +946,23 @@
             data = self.config.api_token
         # confirm the data is syntactially correct: it is 32 bytes
         # of url-safe base64-encoded random data
         if len(urlsafe_b64decode(data)) != 32:
             raise Exception("Incorrect token data")
         return data
 
+    @property
+    def websocket_agent(self):
+        """
+        An implementor of IWebSocketClientAgent from autobahn
+        """
+        if self._ws_agent is None:
+            from twisted.internet import reactor
+            self._ws_agent = create_client_agent(reactor)
+        return self._ws_agent
 
     @property
     def client(self):
         if self._client is None:
             from twisted.internet import reactor
             endpoint_str = self.api_client_endpoint
 
@@ -889,28 +1047,33 @@
     "leave": leave,
     "list": list_,
     "status": status,
     "run": run,
 }
 
 
-def dispatch_magic_folder_command(args, stdout=None, stderr=None, client=None):
+def dispatch_magic_folder_command(reactor, args, stdout=None, stderr=None, client=None, agent=None):
     """
     Run a magic-folder command with the given args
 
+    :param IWebSocketClientAgent agent: override the WebSocket connection agent
+
     :returns: a Deferred which fires with the result of doing this
         magic-folder (sub)command.
     """
     options = MagicFolderCommand()
+    options.reactor = reactor
     if stdout is not None:
         options.stdout = stdout
     if stderr is not None:
         options.stderr = stderr
     if client is not None:
         options._client = client
+    if agent is not None:
+        options._ws_agent = agent
 
     try:
         options.parseOptions(args)
         maybe_fail_experimental_command(options)
     except usage.UsageError as e:
         print("Error: {}".format(e))
         # if a user just typed "magic-folder" don't make them re-run
@@ -1004,9 +1167,9 @@
 def _entry():
     """
     Implement the *magic-folder* console script declared in ``setup.py``.
 
     :return: ``None``
     """
     def main(reactor):
-        return dispatch_magic_folder_command(sys.argv[1:])
+        return dispatch_magic_folder_command(reactor, sys.argv[1:])
     return react(main)
```

### Comparing `magic-folder-23.3.1/src/magic_folder/client.py` & `magic-folder-23.5.0/src/magic_folder/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,20 @@
 
     def list_folders(self, include_secret_information=None):
         api_url = self.base_url.child(u'v1').child(u'magic-folder')
         if include_secret_information:
             api_url = api_url.replace(query=[(u"include_secret_information", u"1")])
         return self._authorized_request("GET", api_url)
 
+    def recent_changes(self, folder_name, number=None):
+        api_url = self.base_url.child(u'v1').child(u'magic-folder').child(folder_name).child("recent-changes")
+        if number is not None:
+            api_url = api_url.replace(query=[(u"number", str(number))])
+        return self._authorized_request("GET", api_url)
+
     def add_snapshot(self, magic_folder, relpath):
         api_url = self.base_url.child(u'v1', u'magic-folder', magic_folder, u'snapshot')
         api_url = api_url.set(u'path', relpath)
         return self._authorized_request("POST", api_url)
 
     def file_status(self, magic_folder):
         api_url = self.base_url.child(u'v1', u'magic-folder', magic_folder, u'file-status')
```

### Comparing `magic-folder-23.3.1/src/magic_folder/common.py` & `magic-folder-23.5.0/src/magic_folder/common.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/config.py` & `magic-folder-23.5.0/src/magic_folder/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,31 @@
     An attempt was made to store a local snapshot whose parents aren't in
     the local database.
     """
     parent_identifier = attr.ib(validator=attr.validators.instance_of(UUID))
 
 
 @attr.s(auto_exc=True)
+class LocalSnapshotRequiresParent(Exception):
+    """
+    An attempt was made to store a local snapshot but it doesn't
+    include any of the existing snapshots as a parent.
+    """
+    snapshot_identifier = attr.ib(validator=attr.validators.instance_of(UUID))
+    relpath = attr.ib()
+    missing_parents = attr.ib(validator=attr.validators.instance_of(list))  # of UUIDs
+
+    def __str__(self):
+        return "LocalSnapshot for {} should have at least one parent: {}".format(
+            repr(self.relpath),
+            ' '.join([str(sid) for sid in self.missing_parents]),
+        )
+
+
+@attr.s(auto_exc=True)
 class RemoteSnapshotWithoutPathState(Exception):
     """
     An attempt was made to insert a remote snapshot into the database without
     corresponding path state (either provided, or already in the database).
     """
 
     folder_name = attr.ib(validator=attr.validators.instance_of(str))
@@ -944,14 +961,44 @@
         Store or update the given local snapshot.
 
         :param LocalSnapshot snapshot: The snapshot to store.
 
         :param PathState path_state: Status of the on-disk data (can be
             None if there is nothing on disk, i.e. a delete).
         """
+        # XXX should confirm too that if this snapshot refers to a
+        # relpath that IS in the database already (i.e. > 0 local
+        # snapshots) then its local_parents MUST contain at least one
+        # of the existing local snapshots
+        rows = cursor.execute(
+            """
+            SELECT
+                identifier from [local_snapshots]
+            WHERE
+                relpath= ?
+            """,
+            (snapshot.relpath,),
+        ).fetchall()
+        if rows:
+            # each row is a 1-tuple
+            localsnap_identifiers = [UUID(row[0]) for row in rows]
+            # we have 1 or more local-snapshots already for this
+            # relpath -- so it better include at least one of them as
+            # parent. "Normally" these should relate like A -> A' ->
+            # A'' etc (i.e. each the parent of the last)
+            if not any(
+                    sn.identifier in localsnap_identifiers
+                    for sn in snapshot.parents_local
+            ):
+                raise LocalSnapshotRequiresParent(
+                    snapshot.identifier,
+                    snapshot.relpath,
+                    localsnap_identifiers,
+                )
+
         # Ensure that the local parent snapshots are already in the database.
         for parent in snapshot.parents_local:
             cursor.execute(
                 """
                 SELECT
                     count(*) from [local_snapshots]
                 WHERE
@@ -1359,16 +1406,17 @@
             SELECT
                 relpath, mtime_ns, last_updated_ns
             FROM
                 [current_snapshots]
             ORDER BY
                 last_updated_ns DESC
             LIMIT
-                30
-            """
+                ?
+            """,
+            (n, )
         )
         rows = cursor.fetchall()
         return [(r[0], ns_to_seconds(r[1]), ns_to_seconds(r[2])) for r in rows]
 
     @with_cursor
     def get_remotesnapshot(self, cursor, relpath):
         """
```

### Comparing `magic-folder-23.3.1/src/magic_folder/downloader.py` & `magic-folder-23.5.0/src/magic_folder/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,16 @@
 
         .. note::
 
             ``child_cap`` must have already have been dowloaded
 
         :returns bool:
         """
+        if target_cap == child_cap:
+            return True
         # TODO: We can make this more efficent in the future by tracking some extra data.
         # - for each snapshot in our remotesnapshotdb, we are going to check if something is
         #   an ancestor very often, so could cache that information (we'd probably want to
         #   integrate this with whatever updates that, as moving our remotesnapshot forward
         #   only incrementally adds to the ancestors of the remote
         # - for checking in the other direction, we can skip checking parents of any ancestors that are
         #   also ancestors of our remotesnapshot
@@ -568,14 +570,15 @@
                     files = yield participant.files()
                     for relpath, file_data in files.items():
                         if self._is_remote_update(relpath, file_data.snapshot_cap):
                             self._status.download_queued(self._config.name, relpath)
                             updates.append((relpath, file_data.snapshot_cap))
 
             # allow for parallel downloads
+            # (we could de-duplicate snapshots here, but the state-machine has to anyway)
             yield gatherResults([
                 self._process_snapshot(relpath, snapshot_cap)
                 for relpath, snapshot_cap in updates
             ])
 
     @inline_callbacks
     def _process_snapshot(self, relpath, snapshot_cap):
@@ -601,8 +604,19 @@
             assert snapshot.capability != our_snapshot_cap, "invalid input"
 
             # make sure "our_snapshot_cap" is cached
             if our_snapshot_cap is not None:
                 yield self._remote_snapshot_cache.get_snapshot_from_capability(our_snapshot_cap)
             abspath = self._config.magic_path.preauthChild(snapshot.relpath)
             mf = self._file_factory.magic_file_for(abspath)
-            yield maybeDeferred(mf.found_new_remote, snapshot)
+
+            # check if "snapshot" is already one of our ancestors; if
+            # it is, we've re-noticed an old update (so do not engage
+            # the state-machine)
+            if our_snapshot_cap is not None \
+               and self._remote_snapshot_cache.is_ancestor_of(snapshot.capability, our_snapshot_cap):
+                Message.log(
+                    message_type=u"downloader:redundant-update",
+                    relpath=snapshot.relpath,
+                )
+            else:
+                yield maybeDeferred(mf.found_new_remote, snapshot)
```

### Comparing `magic-folder-23.3.1/src/magic_folder/endpoints.py` & `magic-folder-23.5.0/src/magic_folder/endpoints.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/initialize.py` & `magic-folder-23.5.0/src/magic_folder/initialize.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/invite.py` & `magic-folder-23.5.0/src/magic_folder/invite.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/list.py` & `magic-folder-23.5.0/src/magic_folder/list.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/magic_file.py` & `magic-folder-23.5.0/src/magic_folder/magic_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from twisted.internet.defer import (
     Deferred,
     DeferredList,
     DeferredSemaphore,
     maybeDeferred,
     succeed,
     CancelledError,
+    returnValue,
 )
 from twisted.web.client import (
     ResponseNeverReceived,
 )
 from twisted.application.internet import (
     backoffPolicy,
 )
@@ -388,17 +389,14 @@
         state
         """
 
     @_machine.input()
     def _remote_update(self, snapshot):
         """
         The file has a remote update.
-
-        XXX should this be 'snapshots' for multiple participant updates 'at once'?
-        XXX does this include deletes?
         """
 
     @_machine.input()
     def _existing_local_snapshot(self, snapshot):
         """
         One or more LocalSnapshot instances already exist for this path.
 
@@ -486,15 +484,14 @@
         """
 
     @_machine.output()
     def _begin_download(self, snapshot):
         """
         Download a given Snapshot (including its content)
         """
-
         def downloaded(staged_path):
             self._call_later(self._download_completed, snapshot, staged_path)
 
         retry_delay_sequence = _delay_sequence()
 
         def error(f):
             if f.check(CancelledError):
@@ -772,15 +769,14 @@
 
     @_machine.output()
     def _create_local_snapshot(self):
         """
         Create a LocalSnapshot for this update
         """
         d = self._factory._local_snapshot_service.add_file(self._path)
-
         # when the local snapshot gets created, it _should_ have the
         # next thing in our queue (if any) as its parent (see assert below)
 
         def completed(snap):
             # _queue_local contains Deferreds .. but ideally we'd
             # check if "the thing those deferreds resolves to" is the
             # right one .. namely, the _next_ thing in the queue
@@ -952,14 +948,20 @@
         return ret_d
 
     @_machine.output()
     def _queue_remote_update(self, snapshot):
         """
         Save this remote snapshot for later processing (in _check_for_remote_work)
         """
+        # skip queueing this download if we already have this snapshot
+        # ahead in the queue
+        for _, queued_snap in self._queue_remote:
+            if snapshot == queued_snap:
+                # same return-value as _begin_download: None
+                return succeed(None)
         d = Deferred()
         self._queue_remote.append((d, snapshot))
         return d
 
     @_machine.output()
     def _check_for_local_work(self):
         """
@@ -1306,15 +1308,15 @@
     and retry upon error if `should_retry(exc)` returns a positive
     integer (which is the delay).
     """
     while True:
         try:
             d = maybeDeferred(function, *args, **kw)
             result = yield d
-            return result
+            returnValue(result)
 
         except Exception as e:
             delay = should_retry(e)
             if delay in (None, False):
                 return
             yield deferLater(reactor, delay, lambda: None)
 
@@ -1340,45 +1342,59 @@
         else:
             action.log(message_type=relpath, status="good")
     if not local_files:
         action.log(message_type="no-files")
 
 
 @inline_callbacks
-def maybe_update_personal_dmd_to_local(reactor, config, read_participant, write_participant):
+def maybe_update_personal_dmd_to_local(reactor, config, get_participants):
     """
     It is possible for us to crash or otherwise exit when updates have
     been made to local databases but not yet to our Personal DMD.
 
     For example, when downloading a new update, we may have downloaded
     the file and updated the [current_snapshots] database but then
     exit before successfully updating our Personal DMD.
 
     This function examines all entries in [current_snapshots] and
-    ensure that our Personal DMD matches. If it doesn't, the Personal
+    ensures that our Personal DMD matches. If it doesn't, the Personal
     DMD is updated (that is, local state is taken as the most
     up-to-date).
 
-    We run this function once at startup. To avoid fully starting with
-    inconsistent state, we keep re-trying this and will only be
-    "ready" once we've confirmed our state.
+    It is arranged for this function to run once at startup.
+
+    To avoid fully starting with inconsistent state, we internally
+    keep re-trying this and will only callback our Deferred when our
+    state is consistent.
 
     :param MagicFolderConfig config: our configuration state
-    :param IParticipant read_participant: read-API for our participant
-    :param IWriteableParticipant write_participant: write-API for our participant
+
+    :param get_participants: a possibly-async callable that returns
+        our IParticipant and IWriteParticipants (this is a callable so
+        we can retry it -- if we can't talk to Tahoe yet, we probably
+        can't list participants yet either)
     """
 
+    # XXX should probably do _some_ kind of falloff and jitter
+    # here..with max delay of some sort
+
     with start_action(action_type="confirm-personal-dmd-state", folder=config.name) as action:
 
         def maybe_retry(exc):
             """
             Always retry in 5 seconds.
             """
             action.log(message_type="error", e=str(exc))
             return 5
 
+        reader, writer = yield deferred_retry(
+            reactor,
+            get_participants,
+            maybe_retry,
+        )
+
         yield deferred_retry(
             reactor,
             _attempt_personal_dmd_sync,
             maybe_retry,
-            reactor, action, config, read_participant, write_participant
+            reactor, action, config, reader, writer
         )
```

### Comparing `magic-folder-23.3.1/src/magic_folder/magic_folder.py` & `magic-folder-23.5.0/src/magic_folder/magic_folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,26 +205,30 @@
     @inline_callbacks
     def check_local_state(self):
         """
         :returns: Deferred that fires with None when this magic-folder has
             successfully confirmed that its local state matches the
             Personal DMD.
         """
-        participants = yield self.participants()
-        self_reader = [
-            participant
-            for participant in participants
-            if participant.is_self
-        ]
-        assert len(self_reader) == 1, f"should be exactly one 'self' participant: {participants}"
+
+        @inline_callbacks
+        def get_participants():
+            participants = yield self.participants()
+            self_reader = [
+                participant
+                for participant in participants
+                if participant.is_self
+            ]
+            assert len(self_reader) == 1, f"should be exactly one 'self' participant: {participants}"
+            defer.returnValue(tuple((self_reader[0], self._participants.writer)))
+
         yield maybe_update_personal_dmd_to_local(
             self._clock,
             self.config,
-            self_reader[0],
-            self._participants.writer,
+            get_participants,
         )
 
     def scan_local(self):
         """
         Scan the magic folder for changes.
 
         :returns Deferred[None]: that fires when all the changed files have
```

### Comparing `magic-folder-23.3.1/src/magic_folder/magicpath.py` & `magic-folder-23.5.0/src/magic_folder/magicpath.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/migrate.py` & `magic-folder-23.5.0/src/magic_folder/migrate.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/participants.py` & `magic-folder-23.5.0/src/magic_folder/participants.py`

 * *Files 15% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 
 
 class IParticipants(Interface):
     """
     An ``IParticipants`` provider grants access to the group of other
     participants in a particular magic folder.
     """
+    writer = Attribute("an IWritableParticipant")
+
     def list():
         """
         Get all of the participants.
 
         :return Deferred[[IParticipant]]: A ``Deferred`` that fires with a
             ``list`` of ``IParticipant`` providers representing all of the
             participants in the particular magic folder this object is
@@ -116,14 +118,85 @@
 
     :return IParticipant: A participant object for accessing this
         participant's state.
     """
     return _CollectiveDirnodeParticipant(name, dirnode, is_self, tahoe_client)
 
 
+@implementer(IParticipant)
+@attr.s
+class _StaticParticipant(object):
+    """
+    An in-memory IParticipant provider
+    """
+    my_files = attr.ib()  # dict: str -> SnapshotEntry
+    _is_self = attr.ib(default=False)
+
+    def files(self):
+        return self.my_files
+
+    def is_self(self):
+        return self._is_self
+
+
+@implementer(IWriteableParticipant)
+@attr.s
+class _StaticWriteableParticipant(object):
+    """
+    An in-memory IWritableParticipant that just remembers what updates
+    it did.
+    """
+    updates = attr.ib(factory=list)
+
+    def update_snapshot(self, relpath, capability):
+        self.updates.append((relpath, capability))
+
+
+@implementer(IParticipants)
+@attr.s
+class _StaticParticipants(object):
+    """
+    An in-memory IParticipants provider
+    """
+    writer = attr.ib()
+    participants = attr.ib(default=None)
+
+    def __attrs_post_init__(self):
+        if self.participants is None:
+            self.participants = [
+                _StaticParticipant([], True),
+            ]
+        assert len([p.is_self() for p in self.participants]) == 1, "Must have exactly one 'self' participant"
+
+    def list(self):
+        return self.participants
+
+    def add(self, author, personal_dmd_cap):
+        self.participants.append(
+            _StaticParticipant(
+                author,
+                personal_dmd_cap,
+            )
+        )
+
+
+def static_participants(my_files=None, other_files=None):
+    """
+    An ``IParticipants`` provider. Usually for testing.
+    """
+    # XXX name, dircap, is_self for participants is public?
+    writer = _StaticWriteableParticipant()
+    reader = _StaticParticipant(my_files or [], True)
+    others = [
+        _StaticParticipant(files, False)
+        for files in (other_files or [])
+    ]
+    return _StaticParticipants(writer, [reader] + others)
+
+
 def participants_from_collective(collective_dirnode, upload_dirnode, tahoe_client):
     """
     Get an ``IParticipants`` provider that reads participants from the given
     Tahoe-LAFS dirnodes.
 
     :param IDirectoryNode collective_dirnode: The magic folder "collective"
         directory into which participant DMDs are linked.
```

### Comparing `magic-folder-23.3.1/src/magic_folder/pid.py` & `magic-folder-23.5.0/src/magic_folder/pid.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/scanner.py` & `magic-folder-23.5.0/src/magic_folder/scanner.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/service.py` & `magic-folder-23.5.0/src/magic_folder/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,22 +17,25 @@
 from twisted.internet.defer import Deferred, gatherResults, returnValue
 from twisted.internet.endpoints import serverFromString
 from twisted.web import http
 from twisted.web.client import Agent
 from twisted.python.compat import (
     nativeString,
 )
+from twisted.logger import (
+    Logger,
+)
 
 from .common import APIError, NoSuchMagicFolder
 from .endpoints import client_endpoint_from_address
 from .magic_folder import MagicFolder
 from .snapshot import create_local_author
 from .status import (
     IStatus,
-    WebSocketStatusService,
+    EventsWebSocketStatusService,
     TahoeStatus,
 )
 from .tahoe_client import (
     InsufficientStorageServers,
     create_tahoe_client,
 )
 from .util.observer import (
@@ -88,14 +91,16 @@
     tahoe_client = attr.ib()
 
     # internal state
     happy = attr.ib(default=None)
     _poller = attr.ib(default=None)
     _last_update = attr.ib(default=0)
     _storage_servers = attr.ib(factory=dict)
+    _currently_happy = attr.ib(default=False)
+    _awaiting_happy = attr.ib(factory=list)
 
     def __attrs_post_init__(self):
         MultiService.__init__(self)
 
     def startService(self):
         MultiService.startService(self)
         self.happy = self.find_happy_shares()
@@ -105,54 +110,67 @@
             self._update_status,
         )
         self._poller.setServiceParent(self)
 
     @inline_callbacks
     def is_happy_connections(self):
         yield self._poller.call_soon()
-        returnValue(self.connected_servers() >= self.happy)
+        self._currently_happy = (self.connected_servers() >= self.happy)
+        returnValue(self._currently_happy)
 
     def connected_servers(self):
         """
         :returns int: the number of storage-servers our Tahoe-LAFS client
         is currently connected to.
         """
         return sum(
             1 if server["connection_status"].startswith("Connected to") else 0
             for server in self._storage_servers
         )
 
+    def when_happy(self):
+        """
+        :returns Deferred[None]: triggers when this service determines we
+            are happy (which could be immediately)
+        """
+        d = Deferred()
+        if self._currently_happy:
+            d.callback(None)
+        else:
+            self._awaiting_happy.append(d)
+        return d
+
     @inline_callbacks
     def _update_status(self):
         try:
             welcome_body = yield self.tahoe_client.get_welcome()
             self._storage_servers = welcome_body["servers"]
             status = TahoeStatus(self.connected_servers(), self.happy, True)
         except Exception:
             self._storage_servers = {}
             status = TahoeStatus(0, self.happy, False)
 
         # update status
         self.status_service.tahoe_status(status)
+        self._currently_happy = status.is_happy
 
         # tell TahoeClient whether mutable operation is fine or not
-        if status.is_happy:
+        if self._currently_happy:
             self.tahoe_client.mutables_okay()
+            for d in self._awaiting_happy:
+                d.callback(None)
+            self._awaiting_happy = []
         else:
             self.tahoe_client.mutables_bad(
                 InsufficientStorageServers(
                     status.connected,
                     status.desired,
                 )
             )
 
-from twisted.logger import (
-    Logger,
-)
-
 
 @attr.s
 class MagicFolderService(MultiService):
     """
     :ivar reactor: the Twisted reactor to use
 
     :ivar GlobalConfigDatabase config: our system configuration
@@ -257,15 +275,15 @@
         Create a new service given a reactor and global configuration.
 
         :param GlobalConfigDatabase config: config to use
         """
         return cls(
             reactor,
             config,
-            WebSocketStatusService(reactor, config),
+            EventsWebSocketStatusService(reactor, config),
         )
 
     @inline_callbacks
     def run(self):
         yield self.startService()
         happy = yield self._tahoe_status_service.is_happy_connections()
         self.log.info(
@@ -273,14 +291,20 @@
                 self._tahoe_status_service.connected_servers()
             ),
         )
         if not happy:
             self.log.info(
                 "NOTE: not currently connected to enough storage-servers",
             )
+            self._tahoe_status_service.when_happy().addCallback(
+                lambda _: self.log.info(
+                    "service restored; now connected to enough storage-servers",
+                )
+            )
+
 
         def do_shutdown():
             self._run_deferred.callback(None)
             return self.stopService()
         self.reactor.addSystemEventTrigger("before", "shutdown", do_shutdown)
 
         yield self._run_deferred
@@ -401,15 +425,15 @@
             collective_write_cap,
             personal_write_cap,
             poll_interval,
             scan_interval,
         )
 
         self._add_service_for_folder(name)
-        self.status_service._maybe_update_clients()
+        self.status_service.folder_added(name)
 
     @inline_callbacks
     def invite_to_folder(self, folder_name, author_name, mode):
         """
         Create a new invite for a folder. This fires once the invite is
         created at the Magic Wormhole mailbox server; use
         invite.await_done() to wait for the invitee to accept (or
```

### Comparing `magic-folder-23.3.1/src/magic_folder/show_config.py` & `magic-folder-23.5.0/src/magic_folder/show_config.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/snapshot.py` & `magic-folder-23.5.0/src/magic_folder/snapshot.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/tahoe_client.py` & `magic-folder-23.5.0/src/magic_folder/tahoe_client.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/__init__.py` & `magic-folder-23.5.0/src/magic_folder/test/__init__.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/agentutil.py` & `magic-folder-23.5.0/src/magic_folder/test/agentutil.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/cli/common.py` & `magic-folder-23.5.0/src/magic_folder/test/cli/common.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/cli/test_api_cli.py` & `magic-folder-23.5.0/src/magic_folder/test/cli/test_api_cli.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/cli/test_magic_folder.py` & `magic-folder-23.5.0/src/magic_folder/test/cli/test_magic_folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     create_testing_configuration,
     load_global_configuration,
 )
 from ...client import (
     create_testing_http_client,
 )
 from ...status import (
-    WebSocketStatusService,
+    EventsWebSocketStatusService,
 )
 from ...endpoints import (
     CannotConvertEndpointError,
 )
 from ...service import MagicFolderService
 from ...snapshot import (
     create_local_author,
@@ -108,15 +108,15 @@
         # for these tests we never contact Tahoe so we can get
         # away with an "empty" Tahoe WebUI
         tahoe_client = create_tahoe_client(DecodedURL.from_text(u""), StubTreq(Resource())),
         self.config = create_testing_configuration(
             FilePath(self.mktemp()),
             FilePath(u"/no/tahoe/node-directory"),
         )
-        status_service = WebSocketStatusService(reactor, self.config)
+        status_service = EventsWebSocketStatusService(reactor, self.config)
         global_service = MagicFolderService(
             reactor, self.config, status_service, tahoe_client,
         )
         self.http_client = create_testing_http_client(
             reactor,
             self.config,
             global_service,
@@ -228,15 +228,15 @@
         )
 
         self.config_dir = FilePath(self.mktemp())
         self.config = create_testing_configuration(
             self.config_dir,
             FilePath(u"/non-tahoe-directory"),
         )
-        status_service = WebSocketStatusService(reactor, self.config)
+        status_service = EventsWebSocketStatusService(reactor, self.config)
         folder_service = MagicFolderService(
             reactor, self.config, status_service, tahoe_client,
         )
         self.http_client = create_testing_http_client(
             reactor,
             self.config,
             folder_service,
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/common.py` & `magic-folder-23.5.0/src/magic_folder/test/common.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/eliotutil.py` & `magic-folder-23.5.0/src/magic_folder/test/eliotutil.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/fixtures.py` & `magic-folder-23.5.0/src/magic_folder/test/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 )
 from ..tahoe_client import (
     create_tahoe_client,
 )
 from ..participants import participants_from_collective
 from ..snapshot import create_local_author
 from ..status import (
-    WebSocketStatusService,
+    EventsWebSocketStatusService,
 )
 from ..service import MagicFolderService
 
 from ..config import (
     GlobalConfigDatabase,
     SQLite3DatabaseLocation,
     MagicFolderConfig,
@@ -221,15 +221,15 @@
 
         self.filesystem = InMemoryMagicFolderFilesystem()
 
         self._global_config = create_testing_configuration(
             self.temp.child("config"),
             self.temp.child("tahoe-node"),
         )
-        self.status = WebSocketStatusService(Clock(), self._global_config)
+        self.status = EventsWebSocketStatusService(Clock(), self._global_config)
         folder_status = FolderStatus(self.config.name, self.status)
 
         uncooperator = Cooperator(
             terminationPredicateFactory=lambda: lambda: False,
             scheduler=lambda f: f(),
         )
         self.addCleanup(uncooperator.stop)
@@ -391,15 +391,15 @@
 
                         # personal DMD
                         Capability.from_string(u"URI:DIR2:{}:{}".format(b2a(("\2" * 16).encode("ascii")).decode("ascii"), b2a(("\3" * 32).encode("ascii")).decode("ascii"))),
                         config[u"poll-interval"],
                         config[u"scan-interval"],
                     )
 
-        status_service = WebSocketStatusService(
+        status_service = EventsWebSocketStatusService(
             reactor,
             global_config,
         )
         global_service = MagicFolderService(
             reactor,
             global_config,
             status_service,
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/matchers.py` & `magic-folder-23.5.0/src/magic_folder/test/matchers.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/strategies.py` & `magic-folder-23.5.0/src/magic_folder/test/strategies.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_api_cli.py` & `magic-folder-23.5.0/src/magic_folder/test/test_api_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 from ..config import (
     create_testing_configuration,
     create_global_configuration,
     GlobalConfigDatabase,
 )
 from ..status import (
     StatusFactory,
-    WebSocketStatusService,
+    EventsWebSocketStatusService,
 )
 from ..snapshot import (
     create_local_author,
     LocalSnapshot,
     RemoteSnapshot,
 )
 from ..util.file import (
@@ -830,15 +830,15 @@
         self.magic_config = FilePath(self.mktemp())
         self.global_config = create_testing_configuration(
             self.magic_config,
             FilePath(u"/no/tahoe/node-directory"),
         )
         self.reactor = MemoryReactorClockResolver()
         self.pumper = create_pumper()
-        self.service = WebSocketStatusService(
+        self.service = EventsWebSocketStatusService(
             self.reactor,
             self.global_config,
         )
         self.factory = StatusFactory(self.service)
         self.agent = create_memory_agent(
             self.reactor,
             self.pumper,
@@ -868,13 +868,12 @@
             config=self.global_config,
         )
         self.pumper._flush()
 
         self.assertThat(
             json.loads(stdout.getvalue()),
             Equals({
-                'state': {
-                    'folders': {},
-                    'synchronizing': False,
-                }
-            }),
+                "events": [
+                    {"connected": 0, "desired": 0, "happy": False, "kind": "tahoe-connection-changed"}
+                ]
+            })
         )
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_cli.py` & `magic-folder-23.5.0/src/magic_folder/test/test_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 import json
 from io import (
     StringIO,
 )
 
+from twisted.internet.address import (
+    IPv4Address,
+)
+from twisted.internet._resolver import HostResolution
 from twisted.internet.interfaces import (
     IStreamServerEndpoint,
+    IReactorPluggableNameResolver,
+)
+from autobahn.twisted.testing import (
+    create_memory_agent,
+    create_pumper,
 )
 from twisted.internet.testing import (
     MemoryReactorClock,
 )
 from twisted.internet.task import (
     Clock,
 )
@@ -26,14 +35,15 @@
     FilePath,
 )
 from twisted.python.runtime import (
     platform,
 )
 from zope.interface import (
     implementer,
+    directlyProvides,
 )
 from hyperlink import (
     DecodedURL,
 )
 
 import attr
 
@@ -70,14 +80,19 @@
     on_stdin_close,
     dispatch_magic_folder_command,
     maybe_fail_experimental_command,
 )
 from ..client import (
     create_magic_folder_client,
 )
+from ..status import (
+    StatusProtocol,
+    EventsWebSocketStatusService,
+    TahoeStatus,
+)
 from magic_folder.util.observer import (
     ListenObserver,
 )
 from magic_folder.initialize import (
     magic_folder_initialize,
 )
 from magic_folder.migrate import (
@@ -371,21 +386,23 @@
             ),
         ])
         http_client = StubTreq(
             StringStubbingResource(
                 request_sequence,
             )
         )
+        reactor = Clock()
         client = create_magic_folder_client(
-            Clock(),
+            reactor,
             self.global_config,
             http_client,
         )
         with request_sequence.consume(self.fail):
             yield dispatch_magic_folder_command(
+                reactor,
                 ["--config", self.magic_config.path, "set-config",
                  "--enable", "invites",
                 ],
                 stdout=stdout,
                 stderr=stderr,
                 client=client,
             )
@@ -417,21 +434,23 @@
             ),
         ])
         http_client = StubTreq(
             StringStubbingResource(
                 request_sequence,
             )
         )
+        reactor = Clock()
         client = create_magic_folder_client(
-            Clock(),
+            reactor,
             self.global_config,
             http_client,
         )
         with request_sequence.consume(self.fail):
             yield dispatch_magic_folder_command(
+                reactor,
                 ["--config", self.magic_config.path, "set-config",
                  "--disable", "invites",
                 ],
                 stdout=stdout,
                 stderr=stderr,
                 client=client,
             )
@@ -467,21 +486,23 @@
             ),
         ])
         http_client = StubTreq(
             StringStubbingResource(
                 request_sequence,
             )
         )
+        reactor = Clock()
         client = create_magic_folder_client(
-            Clock(),
+            reactor,
             self.global_config,
             http_client,
         )
         with request_sequence.consume(self.fail):
             yield dispatch_magic_folder_command(
+                reactor,
                 ["--config", self.magic_config.path, "set-config",
                  "--disable", "invites",
                 ],
                 stdout=stdout,
                 stderr=stderr,
                 client=client,
             )
@@ -489,28 +510,184 @@
     @inlineCallbacks
     def test_list_features(self):
         """
         list optional features
         """
         stdout = StringIO()
         stderr = StringIO()
+        reactor = Clock()
 
         yield dispatch_magic_folder_command(
+            reactor,
             ["--config", self.magic_config.path, "set-config",
              "--features",
             ],
             stdout=stdout,
             stderr=stderr,
         )
         self.assertThat(
             stdout.getvalue(),
             Contains(describe_experimental_features())
         )
 
 
+class TestStatus(AsyncTestCase):
+    """
+    Confirm operation of 'magic-folder status' command
+    """
+    url = DecodedURL.from_text(u"http://127.0.0.1:1234/v1/")
+
+    def setUp(self):
+        super(TestStatus, self).setUp()
+        self.reactor = MemoryReactorClock()
+
+        # XXX maybe there's a better way, but MemoryReactorClock
+        # doesn't provide resolving services, and it seems we need
+        # them...
+        # (see also https://github.com/twisted/twisted/issues/9032)
+        directlyProvides(self.reactor, IReactorPluggableNameResolver)
+
+        class Resolver:
+            def resolveHostName(self, rr, hostname, portNumber=0, **kw):
+                resolution = HostResolution(hostname)
+                rr.resolutionBegan(resolution)
+                rr.addressResolved(IPv4Address("TCP", '127.0.0.1', portNumber))
+                rr.resolutionComplete()
+                return
+        self.reactor.nameResolver = Resolver()
+
+        self.magic_config = FilePath(self.mktemp())
+        self.global_config = create_testing_configuration(
+            self.magic_config,
+            FilePath(u"/no/tahoe/node-directory"),
+        )
+        self.temp = FilePath(self.mktemp())
+        self.magic_folder = self.temp.child("daemon")
+        self.node_dir = self.useFixture(NodeDirectory(self.temp.child("node")))
+
+    @inlineCallbacks
+    def test_simple_status(self):
+        """
+        we connect and see a coherent status
+        """
+        stdout = StringIO()
+        stderr = StringIO()
+        magic_folder_initialize(
+            self.magic_folder,
+            u"tcp:1234",
+            self.node_dir.path,
+            u"tcp:127.0.0.1:1234",
+            u"ws://localhost.invalid/",  # dummy magic-wormhole URL
+        )
+        config = load_global_configuration(self.magic_folder)
+
+        pump = create_pumper()
+        status_service = EventsWebSocketStatusService(
+            self.reactor,
+            config,
+        )
+        # prepare some fake state for the service
+        status_service.tahoe_status(
+            TahoeStatus(2, 2, True)
+        )
+        status_service.folder_added("a")
+        status_service.upload_queued("a", "a-file")
+        status_service.download_queued("a", "b-file")
+        status_service.download_started("a", "b-file")
+        status_service.error_occurred("a", "Some sort of error")
+
+        # now we build up enough infrastructure to serve this status
+        # out
+        status_service.startService()
+        server_proto = StatusProtocol(status_service)
+        agent = create_memory_agent(self.reactor, pump, lambda: server_proto)
+
+        request_sequence = RequestSequence([
+            # ((method, url, params, headers, data), (code, headers, body)),
+            (
+                (b"get",
+                 DecodedURL.from_text(u"http://invalid./v1/magic-folder").to_text(),
+                 {},
+                 {
+                     b'Host': [b'invalid.'],
+                     b'Connection': [b'close'],
+                     b'Authorization': [b'Bearer ' + self.global_config.api_token],
+                     b'Accept-Encoding': [b'gzip']
+                 },
+                 b"",
+                ),
+                (200, {}, b'{"a": {}}')
+            ),
+            # asks for recent-changes too
+            (
+                (b"get",
+                 DecodedURL.from_text(u"http://invalid./v1/magic-folder/a/recent-changes").to_text(),
+                 {b"number": [b"3"]},
+                 {
+                     b'Host': [b'invalid.'],
+                     b'Connection': [b'close'],
+                     b'Authorization': [b'Bearer ' + self.global_config.api_token],
+                     b'Accept-Encoding': [b'gzip']
+                 },
+                 b"",
+                ),
+                (200, {}, b'[{"modified": 0, "relpath": "a-file", "conflicted": false, "last-updated": 2}]')
+            ),
+        ])
+        http_client = StubTreq(
+            StringStubbingResource(
+                request_sequence,
+            )
+        )
+        client = create_magic_folder_client(
+            self.reactor,
+            self.global_config,
+            http_client,
+        )
+
+        dispatch_magic_folder_command(
+            self.reactor,
+            ["--config", self.magic_folder.path, "status",
+            ],
+            stdout=stdout,
+            stderr=stderr,
+            client=client,
+            agent=agent,
+        )
+
+        pump.start()
+        # okay, here's what happens: the agent connects inside the
+        # above dispatch() and the server sends the state -- but all that
+        # happens _before_ it yields and lets the CLI run more code (because
+        # we're doing "immediate-mode" networking stuff. Normally, you
+        # cannot connect to a WebSocket _and_ get data out before
+        # yielding..
+        # ...so we "fake" client connect to get the initial message properly.
+        for client in status_service._clients:
+            status_service.client_connected(client)
+
+        # XXX not exactly sure why we need the advance() _and_ flush?
+        self.reactor.advance(1)
+        pump._flush()
+        yield status_service.stopService()
+        yield pump.stop()
+
+        # analyze output .. don't want to compare everything exact
+        output = stdout.getvalue()
+        self.assertThat(output, Contains('Folder "a"'))
+        self.assertThat(output, Contains('a-file'))
+        self.assertThat(output, Contains('b-file'))
+        self.assertThat(output, Contains("Tahoe is happy"))
+        self.assertThat(
+            stderr.getvalue(),
+            Equals("")
+        )
+
+
+
 class TestStdinClose(SyncTestCase):
     """
     Confirm operation of on_stdin_close
     """
 
     def test_close_called(self):
         """
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_client.py` & `magic-folder-23.5.0/src/magic_folder/test/test_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,21 +52,21 @@
         )
 
     def setUp(self):
         super(MagicFolderClientTests, self).setUp()
         self.setup_client()
 
     def _client_method_request(self, method, args, req_kind, req_url,
-                               body=b"", extra_headers={}):
+                               body=b"", extra_headers={}, expected_query_args={}):
         """
         Test that calling a given `method` results in the client making a
         request to the given `req_url` (with HTTP verb `req_kind`).
         """
         self.assertThat(
-            getattr(self.client, method)(*args),
+            getattr(self.client, method.replace("-", "_"))(*args),
             succeeded(Always()),
         )
         headers = {
             b'Accept-Encoding': [b'gzip'],
             b'Authorization': [b'Bearer fake token'],
             b'Connection': [b'close'],
             b'Host': [b'invalid.'],
@@ -74,15 +74,15 @@
         headers.update(extra_headers)
 
         self.assertThat(
             self.api_calls,
             Equals([
                 (req_kind,
                  req_url,
-                 {},
+                 expected_query_args,
                  headers,
                  body,
                 ),
             ])
         )
 
     def test_tahoe_objects(self):
@@ -133,14 +133,28 @@
         return self._client_method_request(
             "list_invites",
             ("folder_name", ),
             b"GET",
             "http://invalid./experimental/magic-folder/folder_name/invites",
         )
 
+    def test_recent_changes(self):
+        """
+        The .../magic-folder/../recent-changes API works"
+        """
+        return self._client_method_request(
+            "recent-changes",
+            ("folder_name", 25),
+            b"GET",
+            "http://invalid./v1/magic-folder/folder_name/recent-changes",
+            expected_query_args={
+                b"number": [b"25"],
+            }
+        )
+
     def test_join(self):
         """
         The /join API works
         """
         folder_dir = FilePath(self.mktemp()).asTextMode()
         body = json.dumps(
             {
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_common.py` & `magic-folder-23.5.0/src/magic_folder/test/test_common.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_config.py` & `magic-folder-23.5.0/src/magic_folder/test/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     APIError,
     InvalidMagicFolderName,
     NoSuchMagicFolder,
 )
 from ..config import (
     Conflict,
     LocalSnapshotMissingParent,
+    LocalSnapshotRequiresParent,
     RemoteSnapshotWithoutPathState,
     SQLite3DatabaseLocation,
     MagicFolderConfig,
     endpoint_description_to_http_api_root,
     create_global_configuration,
     create_testing_configuration,
     load_global_configuration,
@@ -657,14 +658,64 @@
         with ExpectedException(LocalSnapshotMissingParent):
             self.db.store_local_snapshot(
                 snapshots[1],
                 PathState(42, seconds_to_ns(42), seconds_to_ns(42)),
             )
 
     @given(
+        content1=binary(min_size=1),
+        content2=binary(min_size=1),
+        filename=magic_folder_filenames(),
+        stash_subdir=path_segments(),
+    )
+    def test_store_snapshot_wrong_parent(self, content1, content2, filename, stash_subdir):
+        """
+        If we already have a local-snapshot for a relpath it is an error
+        to add one that doesn't include that snapshot as a parent.
+        """
+        data1 = BytesIO(content1)
+
+        snapshots = []
+
+        d = create_snapshot(
+            relpath=filename,
+            author=self.author,
+            data_producer=data1,
+            snapshot_stash_dir=self.stash,
+            parents=[],
+            cooperator=self.uncooperator,
+        )
+        d.addCallback(snapshots.append)
+
+        # now modify the same file and create a new local snapshot
+        data2 = BytesIO(content2)
+        d = create_snapshot(
+            relpath=filename,
+            author=self.author,
+            data_producer=data2,
+            snapshot_stash_dir=self.stash,
+            parents=[],  # ...but don't include the correct parent
+            cooperator=self.uncooperator,
+        )
+        d.addCallback(snapshots.append)
+
+        # the first snapshot goes into the database
+        self.db.store_local_snapshot(
+            snapshots[0],
+            PathState(42, seconds_to_ns(42), seconds_to_ns(42)),
+        )
+        # trying to serialize this one is an error: it must have
+        # snapshots[0] as a parent to be valid
+        with ExpectedException(LocalSnapshotRequiresParent, ".*at least one parent.*"):
+            self.db.store_local_snapshot(
+                snapshots[1],
+                PathState(42, seconds_to_ns(42), seconds_to_ns(42)),
+            )
+
+    @given(
         local_snapshots(),
     )
     def test_delete_all_local_snapshots_for(self, snapshot):
         """
         After a local snapshot is deleted from the database,
         ``MagicFolderConfig.get_local_snapshot`` raises ``KeyError`` for that
         snapshot's path.
@@ -1213,15 +1264,15 @@
             self.db.get_recent_remotesnapshot_paths(20),
             AfterPreprocessing(
                 lambda data: [
                     (t[0], int(t[1])) for t in data
                 ],
                 Equals([
                     ("foo_{}".format(x), x)
-                    for x in range(34, 4, -1)  # newest to oldest
+                    for x in range(34, 14, -1)  # newest to oldest
                 ])
             )
         )
 
 
 class ConflictTests(SyncTestCase):
     """
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_download.py` & `magic-folder-23.5.0/src/magic_folder/test/test_download.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     RemoteSnapshot,
     sign_snapshot,
     format_filenode,
     create_snapshot,
     write_snapshot_to_tahoe,
 )
 from ..status import (
-    WebSocketStatusService,
+    EventsWebSocketStatusService,
 )
 from ..tahoe_client import (
     create_tahoe_client,
 )
 from ..testing.web import (
     create_fake_tahoe_root,
     create_tahoe_treq_client,
@@ -446,15 +446,15 @@
             None,
         )
         self.http_client = create_tahoe_treq_client(self.root)
         self.tahoe_client = create_tahoe_client(
             DecodedURL.from_text("http://invalid./"),
             self.http_client,
         )
-        self.status_service = WebSocketStatusService(reactor, self._global_config)
+        self.status_service = EventsWebSocketStatusService(reactor, self._global_config)
         self.service = MagicFolder.from_config(
             reactor,
             self.tahoe_client,
             "default",
             self._global_config,
             self.status_service,
         )
@@ -1520,28 +1520,22 @@
         yield top_service._loop()
         yield self.file_factory.finish()
 
         # status system should report our error
         self.assertThat(
             loads(self.alice.global_service.status_service._marshal_state()),
             ContainsDict({
-                "state": ContainsDict({
-                    "folders": ContainsDict({
-                        "default": ContainsDict({
-                            "errors": AfterPreprocessing(
-                                lambda errors: errors[0],
-                                ContainsDict({
-                                    "summary": Equals(
-                                        "Failed to overwrite file 'foo': [Errno 13] Permission denied"
-                                    ),
-                                }),
-                            ),
-                        }),
-                    }),
-                }),
+                "events": AfterPreprocessing(
+                    lambda events: events[1],
+                    ContainsDict({
+                        "summary": Equals(
+                            "Failed to overwrite file 'foo': [Errno 13] Permission denied"
+                        )
+                    })
+                )
             })
         )
 
         self.assertThat(
             self.eliot_logger.flush_tracebacks(OSError),
             MatchesListwise([
                 matches_flushed_traceback(OSError, r"\[Errno 13\] Permission denied")
@@ -1615,28 +1609,22 @@
         )
         yield top_service._loop()
 
         # status system should report our error
         self.assertThat(
             loads(self.alice.global_service.status_service._marshal_state()),
             ContainsDict({
-                "state": ContainsDict({
-                    "folders": ContainsDict({
-                        "default": ContainsDict({
-                            "errors": AfterPreprocessing(
-                                lambda errors: errors[0],
-                                ContainsDict({
-                                    "summary": Equals(
-                                        "Failed to download snapshot for 'foo'."
-                                    )
-                                }),
-                            ),
-                        }),
-                    }),
-                }),
+                "events": AfterPreprocessing(
+                    lambda events: events[1],
+                    ContainsDict({
+                        "summary": Equals(
+                            "Failed to download snapshot for 'foo'."
+                        )
+                    })
+                )
             })
         )
 
         self.assertThat(
             self.eliot_logger.flush_tracebacks(Exception),
             MatchesListwise([
                 matches_flushed_traceback(Exception, "the network is down"),
@@ -1695,28 +1683,22 @@
         )
         yield top_service._loop()
 
         # status system should report our error
         self.assertThat(
             loads(self.alice.global_service.status_service._marshal_state()),
             ContainsDict({
-                "state": ContainsDict({
-                    "folders": ContainsDict({
-                        "default": ContainsDict({
-                            "errors": AfterPreprocessing(
-                                lambda errors: errors[0],
-                                ContainsDict({
-                                    "summary": Equals(
-                                        "Error updating personal DMD: Couldn't add foo to directory. Error code 500"
-                                    )
-                                }),
-                            ),
-                        }),
-                    }),
-                }),
+                "events": AfterPreprocessing(
+                    lambda events: events[1],
+                    ContainsDict({
+                        "summary": Equals(
+                            "Error updating personal DMD: Couldn't add foo to directory. Error code 500"
+                        )
+                    })
+                )
             })
         )
 
         self.assertThat(
             self.eliot_logger.flush_tracebacks(Exception),
             MatchesListwise([
                 matches_flushed_traceback(Exception, "Couldn't add foo to directory. Error code 500")
@@ -1776,28 +1758,22 @@
         yield mf.found_new_remote(remote_snapshot)
         yield mf.when_idle()
 
         # status system should report our error
         self.assertThat(
             loads(carol.global_service.status_service._marshal_state()),
             ContainsDict({
-                "state": ContainsDict({
-                    "folders": ContainsDict({
-                        "default": ContainsDict({
-                            "errors": AfterPreprocessing(
-                                lambda errors: errors[0],
-                                ContainsDict({
-                                    "summary": Equals(
-                                        "Cancelled: some_file"
-                                    )
-                                }),
-                            ),
-                        }),
-                    }),
-                }),
+                "events": AfterPreprocessing(
+                    lambda events: events[1],
+                    ContainsDict({
+                        "summary": Equals(
+                            "Cancelled: some_file"
+                        )
+                    })
+                )
             })
         )
 
     # XXX NOTE if this name gets longer, the resulting temp-paths can
     # become "too long" on windows causing failures
     @inline_callbacks
     def test_cancel1(self):
@@ -1860,28 +1836,22 @@
         yield mf.found_new_remote(parent)
         yield mf.when_idle()
 
         # status system should report our error
         self.assertThat(
             loads(carol.global_service.status_service._marshal_state()),
             ContainsDict({
-                "state": ContainsDict({
-                    "folders": ContainsDict({
-                        "default": ContainsDict({
-                            "errors": AfterPreprocessing(
-                                lambda errors: errors[0],
-                                ContainsDict({
-                                    "summary": Equals(
-                                        "Cancelled: a_file"
-                                    )
-                                }),
-                            ),
-                        }),
-                    }),
-                }),
+                "events": AfterPreprocessing(
+                    lambda events: events[1],
+                    ContainsDict({
+                        "summary": Equals(
+                            "Cancelled: a_file"
+                        )
+                    })
+                )
             })
         )
 
 
 class AsyncFilesystemModificationTests(AsyncTestCase):
     """
     Tests for LocalMagicFolderFilesystem that are async
@@ -2000,7 +1970,116 @@
                 ),
                 AfterPreprocessing(
                     lambda f: f.getContent(),
                     Equals(b"pre-existing file")
                 )
             )
         )
+
+
+class RemoteScannerTests(AsyncTestCase):
+    """
+    Tests relating to polling the remote
+    """
+
+    def setUp(self):
+        super(RemoteScannerTests, self).setUp()
+
+        self.alice_magic_path = FilePath(self.mktemp())
+        self.alice_magic_path.makedirs()
+        self.alice = MagicFolderNode.create(
+            reactor,
+            FilePath(self.mktemp()),
+            folders={
+                "default": {
+                    "magic-path": self.alice_magic_path,
+                    "author-name": "alice",
+                    "admin": True,
+                    "poll-interval": 100,
+                    "scan-interval": 100,
+                },
+            },
+            start_folder_services=True,
+        )
+
+        self.file_factory = self.alice.global_service.getServiceNamed("magic-folder-default").file_factory
+        self.remote_cache = self.file_factory._remote_cache
+        self.state_path = self.alice.global_config._get_state_path("default")
+        self.alice_config = self.alice.global_config.get_magic_folder("default")
+        self.alice_author = self.alice_config.author
+        self.filesystem = InMemoryMagicFolderFilesystem()
+        self.file_factory._magic_fs = self.filesystem
+        self.carol_author = create_local_author("carol")
+
+    def tearDown(self):
+        super(RemoteScannerTests, self).tearDown()
+        return self.alice.cleanup()
+
+    @inline_callbacks
+    def test_redundant_update(self):
+        """
+        Give the updater an update taht's the ancestor of the current
+        snapshot (i.e. an out-of-date participant)
+        """
+
+        parent_cap = random_immutable(directory=True)
+        parent = RemoteSnapshot(
+            relpath="foo",
+            author=self.alice_author,
+            metadata={"modification_time": 0},
+            capability=parent_cap,
+            parents_raw=[],
+            content_cap=random_immutable(),
+            metadata_cap=random_immutable(),
+        )
+        parent_content = b"parent" * 1000
+        self.remote_cache._cached_snapshots[parent_cap.danger_real_capability_string()] = parent
+        # we've 'seen' this file before so we must have the path locally
+        local_path = self.alice_magic_path.child("foo")
+        local_path.setContent(parent_content)
+        self.alice_config.store_downloaded_snapshot("foo", parent, get_pathinfo(local_path).state)
+
+        cap0 = random_immutable(directory=True)
+        remote0 = RemoteSnapshot(
+            relpath="foo",
+            author=self.carol_author,
+            metadata={"modification_time": 0},
+            capability=cap0,
+            parents_raw=[parent_cap.danger_real_capability_string()],
+            content_cap=random_immutable(),
+            metadata_cap=random_immutable(),
+        )
+        self.remote_cache._cached_snapshots[cap0.danger_real_capability_string()] = remote0
+        self.alice_config.store_downloaded_snapshot("foo", remote0, get_pathinfo(local_path).state)
+
+        # set up a plausible 2-participant situation
+        tahoe_client = self.alice.tahoe_client
+        collective = yield tahoe_client.create_mutable_directory()
+        alice_personal = yield tahoe_client.create_mutable_directory()
+        carol_personal = yield tahoe_client.create_mutable_directory()
+        yield tahoe_client.add_entry_to_mutable_directory(collective, "carol", carol_personal)
+        # carol is on "parent", we are on "remote0" (the child)
+        yield tahoe_client.add_entry_to_mutable_directory(carol_personal, "foo", parent.capability)
+        yield tahoe_client.add_entry_to_mutable_directory(alice_personal, "foo", remote0.capability)
+
+        alice_participants = participants_from_collective(
+            collective,
+            alice_personal,
+            tahoe_client,
+        )
+
+        # run a scan, but "carol" is on the old (parent) snapshot
+        top_service = RemoteScannerService(
+            Clock(),
+            self.alice_config,
+            alice_participants,
+            self.file_factory,
+            self.remote_cache,
+            self.alice.global_service.status_service,
+        )
+        yield top_service._loop()
+
+        # we should have seen "carol's" out-of-date remote and ignored it
+        self.assertThat(
+            self.filesystem.actions,
+            Equals([])
+        )
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_eliotutil.py` & `magic-folder-23.5.0/src/magic_folder/test/test_eliotutil.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_endpoints.py` & `magic-folder-23.5.0/src/magic_folder/test/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_foo.py` & `magic-folder-23.5.0/src/magic_folder/test/test_foo.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_invite.py` & `magic-folder-23.5.0/src/magic_folder/test/test_invite.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     validate_versions,
     accept_invite,
 )
 from ..service import (
     MagicFolderService,
 )
 from ..status import (
-    WebSocketStatusService,
+    EventsWebSocketStatusService,
 )
 
 from magic_folder.snapshot import (
     create_local_author,
 )
 from magic_folder.tahoe_client import (
     create_tahoe_client,
@@ -576,15 +576,15 @@
             }).encode("utf8"),
 
             json.dumps({
                 "success": True,
             }).encode("utf8"),
         ])
 
-        self.global_status = WebSocketStatusService(
+        self.global_status = EventsWebSocketStatusService(
             self.reactor,
             self.global_config,
         )
 
         self.service = MagicFolderService(
             self.reactor,
             self.global_config,
@@ -790,15 +790,15 @@
             }).encode("utf8"),
 
             json.dumps({
                 "success": True,
             }).encode("utf8"),
         ])
 
-        self.global_status = WebSocketStatusService(
+        self.global_status = EventsWebSocketStatusService(
             self.reactor,
             self.global_config,
         )
 
         self.service = MagicFolderService(
             self.reactor,
             self.global_config,
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_local_snapshot.py` & `magic-folder-23.5.0/src/magic_folder/test/test_local_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 )
 from ..config import (
     create_global_configuration,
     create_testing_configuration,
 )
 from ..status import (
     FolderStatus,
-    WebSocketStatusService,
+    EventsWebSocketStatusService,
 )
 from ..util.file import (
     seconds_to_ns,
 )
 from ..util.capabilities import (
     random_immutable,
     random_dircap,
@@ -67,32 +67,33 @@
 from .matchers import matches_failure
 from .strategies import (
     path_segments,
     relative_paths,
     absolute_paths,
 )
 
+
 @attr.s
 class MemorySnapshotCreator(object):
     """
     A way to test LocalSnapshotService with an in-memory database.
 
     :ivar [FilePath] processed: All of the paths passed to ``store_local_snapshot``,
         in the order they were passed.
     """
     processed = attr.ib(default=attr.Factory(list))
 
-    def store_local_snapshot(self, path, local_snapshot=None):
+    def create_local_snapshot(self, path, local_snapshot=None):
         Message.log(
             message_type=u"memory-snapshot-creator:store-local-snapshot",
             path=path.path,
             local_snapshot=local_snapshot,
         )
         self.processed.append(path)
-
+        # XXX real code returns a LocalSnapshot?
 
 class LocalSnapshotServiceTests(SyncTestCase):
     """
     Tests for ``LocalSnapshotService``.
     """
     def setup_example(self):
         """
@@ -113,15 +114,15 @@
             create_local_author("author"),
             random_immutable(directory=True),
             random_dircap(),
             60,
             None,
         )
 
-        self.status = WebSocketStatusService(reactor, self._global_config)
+        self.status = EventsWebSocketStatusService(reactor, self._global_config)
         self.snapshot_creator = MemorySnapshotCreator()
         self.snapshot_service = LocalSnapshotService(
             config=self.magic_config,
             snapshot_creator=self.snapshot_creator,
             status=FolderStatus(self.magic_config.name, self.status),
         )
 
@@ -304,15 +305,15 @@
             content = data_strategy.draw(binary())
             file.setContent(content)
 
             files.append((file, filename, content))
 
         for (file, filename, _unused) in files:
             self.assertThat(
-                self.snapshot_creator.store_local_snapshot(file),
+                self.snapshot_creator.create_local_snapshot(file),
                 succeeded(Always())
             )
 
         self.assertThat(self.db.get_all_localsnapshot_paths(), HasLength(len(files)))
         for (file, filename, content) in files:
             stored_snapshot = self.db.get_local_snapshot(filename)
             stored_content = stored_snapshot.content_path.getContent()
@@ -337,26 +338,26 @@
         should refer to the existing snapshot as a parent.
         """
         foo = self.magic.child(filename)
         foo.setContent(content1)
 
         # make sure the store_local_snapshot() succeeds
         self.assertThat(
-            self.snapshot_creator.store_local_snapshot(foo),
+            self.snapshot_creator.create_local_snapshot(foo),
             succeeded(Always()),
         )
 
         stored_snapshot1 = self.db.get_local_snapshot(filename)
 
         # now modify the file with some new content.
         foo.setContent(content2)
 
         # make sure the second call succeeds as well
         self.assertThat(
-            self.snapshot_creator.store_local_snapshot(foo),
+            self.snapshot_creator.create_local_snapshot(foo),
             succeeded(Always()),
         )
         stored_snapshot2 = self.db.get_local_snapshot(filename)
 
         self.assertThat(
             stored_snapshot2.parents_local[0],
             MatchesStructure(
@@ -372,24 +373,24 @@
         Create a snapshot and then a deletion snapshot of it.
         """
         foo = self.magic.child(filename)
         foo.setContent(content)
 
         # make sure the store_local_snapshot() succeeds
         self.assertThat(
-            self.snapshot_creator.store_local_snapshot(foo),
+            self.snapshot_creator.create_local_snapshot(foo),
             succeeded(Always()),
         )
 
         # delete the file
         foo.remove()
 
         # store a new snapshot
         self.assertThat(
-            self.snapshot_creator.store_local_snapshot(foo),
+            self.snapshot_creator.create_local_snapshot(foo),
             succeeded(Always()),
         )
         stored_snapshot2 = self.db.get_local_snapshot(filename)
 
         self.assertThat(
             stored_snapshot2.is_delete(),
             Equals(True),
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_magic_folder_service.py` & `magic-folder-23.5.0/src/magic_folder/test/test_magic_folder_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # See COPYING for details.
 
 """
 Tests for the Twisted service which is responsible for a single
 magic-folder.
 """
 
-import attr
 from twisted.python.filepath import (
     FilePath,
 )
 from twisted.application.service import (
     Service,
     MultiService,
 )
@@ -25,41 +24,38 @@
     Is,
     Always,
     Equals,
 )
 from testtools.twistedsupport import (
     succeeded,
 )
-from zope.interface import (
-    implementer,
-)
 from ..magic_folder import (
     MagicFolder,
     LocalSnapshotService,
 )
 from ..magic_file import (
     MagicFileFactory,
 )
 from ..config import (
     create_testing_configuration,
 )
 from ..status import (
     FolderStatus,
-    WebSocketStatusService,
+    EventsWebSocketStatusService,
 )
 from ..snapshot import (
     create_local_author,
     LocalSnapshot,
 )
 from ..downloader import (
     InMemoryMagicFolderFilesystem,
 )
 from ..participants import (
-    IParticipants,
     SnapshotEntry,
+    static_participants,
 )
 from ..util.capabilities import (
     random_immutable,
     random_dircap,
 )
 from ..util.file import (
     PathState,
@@ -89,15 +85,15 @@
         local_snapshot_service = Service()
         tahoe_client = object()
         reactor = object()
         name = u"local-snapshot-service-test"
         config = object()
         participants = object()
         uploader = Service()
-        status_service = WebSocketStatusService(reactor, None)
+        status_service = EventsWebSocketStatusService(reactor, None)
         folder_status = FolderStatus(name, status_service)
         magic_folder = MagicFolder(
             client=tahoe_client,
             config=config,
             name=name,
             invite_manager=Service(),
             local_snapshot_service=local_snapshot_service,
@@ -150,15 +146,15 @@
         )
 
         target_path = magic_path.preauthChild(relative_target_path)
         target_path.parent().makedirs(ignoreExistingDirectory=True)
         target_path.setContent(content)
 
         clock = task.Clock()
-        status_service = WebSocketStatusService(clock, global_config)
+        status_service = EventsWebSocketStatusService(clock, global_config)
         folder_status = FolderStatus(u"foldername", status_service)
         local_snapshot_creator = MemorySnapshotCreator()
         clock = task.Clock()
         local_snapshot_service = LocalSnapshotService(
             mf_config,
             local_snapshot_creator,
             folder_status,
@@ -205,29 +201,14 @@
 
         self.assertThat(
             local_snapshot_creator.processed,
             Equals([target_path]),
         )
 
 
-from .test_magic_file import (
-    _FakeParticipant,
-    _FakeWriteableParticipant,
-)
-
-@implementer(IParticipants)
-@attr.s
-class _FakeParticipants:
-    writer = attr.ib()
-    our_participants = attr.ib()
-
-    def list(self):
-        return self.our_participants
-
-
 class LocalStateTests(SyncTestCase):
     """
     Tests for ``MagicFolder.check_local_state``
     """
 
     def test_update_personal_dmd(self):
         """
@@ -263,27 +244,24 @@
             dict(),
             content_path=FilePath("snap content"),
             parents_local=[],
             parents_remote=[],
         )
         config.store_local_snapshot(snap, PathState(size=1234, mtime_ns=555, ctime_ns=555))
 
-        participants = _FakeParticipants(
-            _FakeWriteableParticipant(),
-            [
-                _FakeParticipant({
-                    "foo": SnapshotEntry(
-                        random_immutable(),
-                        {"version": 1}
-                    ),
-                }, is_self=True),
-            ],
+        participants = static_participants(
+            my_files={
+                "foo": SnapshotEntry(
+                    random_immutable(),
+                    {"version": 1}
+                ),
+            }
         )
         uploader = Service()
-        status_service = WebSocketStatusService(reactor, None)
+        status_service = EventsWebSocketStatusService(reactor, None)
         folder_status = FolderStatus(name, status_service)
         magic_folder = MagicFolder(
             client=tahoe_client,
             config=config,
             name=name,
             invite_manager=Service(),
             local_snapshot_service=local_snapshot_service,
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_magicpath.py` & `magic-folder-23.5.0/src/magic_folder/test/test_magicpath.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_participants.py` & `magic-folder-23.5.0/src/magic_folder/test/test_participants.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_pid.py` & `magic-folder-23.5.0/src/magic_folder/test/test_pid.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_scanner.py` & `magic-folder-23.5.0/src/magic_folder/test/test_scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,18 @@
     find_deleted_files,
 )
 from ..snapshot import (
     LocalSnapshot,
     RemoteSnapshot,
     create_local_author,
 )
-from ..status import FolderStatus, WebSocketStatusService
+from ..status import (
+    FolderStatus,
+    EventsWebSocketStatusService,
+)
 from ..util.file import (
     PathState,
     get_pathinfo,
     seconds_to_ns,
 )
 from ..util.capabilities import (
     random_dircap,
@@ -76,15 +79,15 @@
             FilePath(self.mktemp()),
             FilePath("dummy"),
         )
         self.collective_cap = random_dircap()
         self.personal_cap = random_dircap()
 
         self.clock = Clock()
-        self.status_service = WebSocketStatusService(self.clock, self._global_config)
+        self.status_service = EventsWebSocketStatusService(self.clock, self._global_config)
         self.folder_status = FolderStatus("default", self.status_service)
 
         self.config = self._global_config.create_magic_folder(
             "default",
             self.magic_path,
             self.author,
             self.collective_cap,
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_schema.py` & `magic-folder-23.5.0/src/magic_folder/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_service.py` & `magic-folder-23.5.0/src/magic_folder/test/test_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,30 +36,32 @@
     create_tahoe_treq_client,
 )
 
 from ..config import (
     create_global_configuration,
 )
 from ..service import MagicFolderService
-from ..status import WebSocketStatusService
+from ..status import (
+    EventsWebSocketStatusService,
+)
 from .fixtures import (
     NodeDirectory,
 )
 from .common import (
     SyncTestCase,
     AsyncTestCase,
 )
 from magic_folder.tahoe_client import (
     create_tahoe_client,
 )
 
 
 class TestTahoeMonitor(AsyncTestCase):
     """
-    Tests relating to ConnectedTahoeservice
+    Tests relating to ConnectedTahoeService
     """
 
     def setUp(self):
         super(TestTahoeMonitor, self).setUp()
 
         self.root = create_fake_tahoe_root()
         self.http_client = create_tahoe_treq_client(self.root)
@@ -79,18 +81,32 @@
             self.node.path,
             u"tcp:localhost:0",
         )
         self.reactor = MemoryReactorClock()
         self.service = MagicFolderService(
             self.reactor,
             self.config,
-            WebSocketStatusService(self.reactor, self.config),
+            EventsWebSocketStatusService(self.reactor, self.config),
             self.tahoe_client,
         )
 
+    @inline_callbacks
+    def test_wait_happy(self):
+        # do one before we start the service so it "actually" has to
+        # wait
+        d0 = self.service._tahoe_status_service.when_happy()
+        self.service.startService()
+        d1 = self.service._tahoe_status_service.when_happy()
+        yield d0
+        yield d1
+        self.assertThat(
+            self.service._tahoe_status_service.happy,
+            Equals(True)
+        )
+
     def test_welcome_fails(self):
         """
         if get_welcome() fails we should print a message
         """
 
         def fail(*args, **kw):
             raise Exception("fail")
@@ -138,15 +154,15 @@
             self.node.path,
             u"tcp:localhost:0",
         )
         self.reactor = MemoryReactorClock()
         self.service = MagicFolderService(
             self.reactor,
             self.config,
-            WebSocketStatusService(self.reactor, self.config),
+            EventsWebSocketStatusService(self.reactor, self.config),
             self.tahoe_client,
         )
         self.service._stdout = self.out = io.StringIO()
 
     @inline_callbacks
     def test_allocate_port(self):
         """
@@ -218,15 +234,15 @@
             self.node.path,
             u"tcp:localhost:5555",
         )
         clock = Clock()
         self.service = MagicFolderService(
             clock,
             self.config,
-            WebSocketStatusService(clock, self.config),
+            EventsWebSocketStatusService(clock, self.config),
             self.tahoe_client,
         )
 
     def test_add_folder(self):
         d = self.service.create_folder(
             u"test",
             u"alice",
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_snapshot.py` & `magic-folder-23.5.0/src/magic_folder/test/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_status.py` & `magic-folder-23.5.0/src/magic_folder/test/test_status.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from .common import (
     SyncTestCase,
     AsyncTestCase,
 )
 from ..status import (
     StatusFactory,
-    WebSocketStatusService,
+    EventsWebSocketStatusService,
 )
 from ..config import (
     create_testing_configuration,
 )
 
 
 class StatusServiceTests(SyncTestCase):
@@ -47,15 +47,15 @@
         self.tahoe_node_dir = FilePath(self.mktemp())
         self.tahoe_node_dir.makedirs()
 
         self.global_config = create_testing_configuration(
             self.basedir,
             self.tahoe_node_dir,
         )
-        self.service = WebSocketStatusService(
+        self.service = EventsWebSocketStatusService(
             self.clock,
             self.global_config,
         )
 
     def test_single_client(self):
         """
         With a single connected client, that client receives updates
@@ -64,61 +64,112 @@
 
         class ClientProtocol(object):
             def sendMessage(self, payload):
                 messages.append(json.loads(payload))
 
         self.service.client_connected(ClientProtocol())
         self.service.upload_queued("foo", "foo")
+        self.clock.advance(1)
         self.service.upload_started("foo", "foo")
+        self.clock.advance(1)
         self.service.upload_finished("foo", "foo")
 
         self.assertThat(
             messages,
-            Equals([{
-                "state": {
-                    "synchronizing": False,
-                    "folders": {},
-                }
-            }, {
-                "state": {
-                    "synchronizing": True,
-                    "folders": {},
-                }
-            }, {
-                "state": {
-                    "synchronizing": False,
-                    "folders": {},
-                }
-            }])
+            Equals([
+                {
+                    "events": [{
+                        "kind": "tahoe-connection-changed",
+                        "connected": 0,
+                        "desired": 0,
+                        "happy": False,
+                    }]
+                },
+                {
+                    "events": [{
+                        "kind": "upload-queued",
+                        "folder": "foo",
+                        "timestamp": 0.0,
+                        "relpath": "foo",
+                    }]
+                },
+                {
+                    "events": [{
+                        "kind": "upload-started",
+                        "folder": "foo",
+                        "timestamp": 1.0,
+                        "relpath": "foo",
+                    }]
+                },
+                {
+                    "events": [{
+                        "kind": "upload-finished",
+                        "folder": "foo",
+                        "timestamp": 2.0,
+                        "relpath": "foo",
+                    }]
+                },
+            ])
         )
 
     def test_offline_client(self):
         """
         A client gets the correct state when connecting
         """
         messages = []
 
         class ClientProtocol(object):
             def sendMessage(self, payload):
                 messages.append(json.loads(payload))
 
         self.service.upload_queued("foo", "foo")
         self.service.upload_started("foo", "foo")
+        self.service.download_queued("foo", "bar")
+        self.service.download_started("foo", "bar")
         self.assertThat(messages, Equals([]))
 
         # once connected, this client should get the proper state
         self.service.client_connected(ClientProtocol())
 
         self.assertThat(
             messages,
             Equals([{
-                "state": {
-                    "synchronizing": True,
-                    "folders": {},
-                }
+                "events": [
+                    {"folder": "foo", "kind": "folder-added"},
+                    {
+                        "folder": "foo",
+                        "kind": "upload-queued",
+                        "timestamp": 0.0,
+                        "relpath": "foo",
+                    },
+                    {
+                        "folder": "foo",
+                        "kind": "upload-started",
+                        "relpath": "foo",
+                        "timestamp": 0.0,
+                    },
+                    {
+                        "folder": "foo",
+                        "kind": "download-queued",
+                        "timestamp": 0.0,
+                        "relpath": "bar",
+                    },
+                    {
+                        "folder": "foo",
+                        "kind": "download-started",
+                        "relpath": "bar",
+                        "timestamp": 0.0,
+                    },
+                    {
+                        "connected": 0,
+                        "desired": 0,
+                        "happy": False,
+                        "kind": "tahoe-connection-changed"
+                    }
+                ]
             }])
         )
 
     def test_disconnect(self):
         """
         A client disconnecting and re-connecting gets correct state
         """
@@ -130,40 +181,82 @@
 
         client = ClientProtocol()
         self.service.client_connected(client)
         self.service.client_disconnected(client)
         self.assertThat(
             messages,
             Equals([{
-                "state": {
-                    "synchronizing": False,
-                    "folders": {},
-                }
+                "events": [
+                    {"connected": 0, "desired": 0, "happy": False, "kind": "tahoe-connection-changed"},
+                ]
             }])
         )
 
         # change our state
         self.service.upload_queued("foo", "foo")
 
         # re-connect the client; it should get the (latest) state as
         # well as the initial state it got on the first connect
         self.service.client_connected(client)
+
         self.assertThat(
             messages,
-            Equals([{
-                "state": {
-                    "synchronizing": False,
-                    "folders": {},
+            Equals([
+                {
+                    "events": [
+                        {"connected": 0, "desired": 0, "happy": False, "kind": "tahoe-connection-changed"},
+                    ]
+                },
+                {
+                    "events": [
+                        {"folder": "foo", "kind": "folder-added"},
+                        {"folder": "foo", "kind": "upload-queued", "timestamp": 0.0, "relpath": "foo"},
+                        {"connected": 0, "desired": 0, "happy": False, "kind": "tahoe-connection-changed"},
+                    ]
                 }
-            }, {
-                "state": {
-                    "synchronizing": True,
-                    "folders": {},
+            ])
+        )
+
+    def test_client_error(self):
+        """
+        We log an error if a message to a client fails to send
+        """
+        messages = []
+
+        class ClientProtocol(object):
+            def sendMessage(self, payload):
+                messages.append(json.loads(payload))
+                if len(messages) == 2:
+                    raise RuntimeError("loopback is broken?")
+
+        client = ClientProtocol()
+        self.service.client_connected(client)
+
+        # change our state
+        self.service.upload_queued("foo", "foo")
+
+        self.assertThat(
+            messages,
+            Equals([
+                {
+                    "events": [
+                        {"connected": 0, "desired": 0, "happy": False, "kind": "tahoe-connection-changed"}
+                    ]
+                },
+                {
+                    "events": [
+                        {"folder": "foo", "kind": "upload-queued", "timestamp": 0.0, "relpath": "foo"}
+                    ]
+                },
+                {
+                    "events": [
+                        {"folder": None, "kind": "error-occurred", "summary": "Failed to send status: loopback is broken?", "timestamp": 0.0}
+                    ]
                 }
-            }])
+            ])
         )
 
 
 class WebSocketTests(AsyncTestCase):
     """
     Tests relating to the actual WebSocket protocol of the status
     serice
@@ -176,15 +269,15 @@
         self.tahoe_node_dir = FilePath(self.mktemp())
         self.tahoe_node_dir.makedirs()
         self.global_config = create_testing_configuration(
             FilePath(self.mktemp()),
             self.tahoe_node_dir,
         )
 
-        self.service = WebSocketStatusService(
+        self.service = EventsWebSocketStatusService(
             self.reactor,
             self.global_config,
         )
         self.factory = StatusFactory(self.service)
         self.agent = create_memory_agent(
             self.reactor,
             self.pumper,
@@ -212,40 +305,37 @@
         # upon open, we should receive the current state
         proto = yield self.agent.open("ws://127.0.0.1:2/v1/status", {}, TestProto)
         self.pumper._flush()
         self.assertThat(
             messages,
             Equals([
                 {
-                    "state": {
-                        "synchronizing": False,
-                        "folders": {},
-                    }
+                    "events": [
+                        {"connected": 0, "desired": 0, "happy": False, "kind": "tahoe-connection-changed"},
+                    ]
                 }
             ])
         )
 
         # if we change the state, we should receive an update
         self.service.upload_queued("foo", "foo")
         self.pumper._flush()
         self.assertThat(
             messages,
             Equals([
                 {
-                    "state": {
-                        "synchronizing": False,
-                        "folders": {},
-                    }
+                    "events": [
+                        {"connected": 0, "desired": 0, "happy": False, "kind": "tahoe-connection-changed"},
+                    ]
                 },
                 {
-                    "state": {
-                        "synchronizing": True,
-                        "folders": {},
-                    }
-                }
+                    "events": [
+                        {"folder": "foo", "kind": "upload-queued", "timestamp": 0.0, "relpath": "foo"}
+                    ]
+                },
             ])
         )
         proto.dropConnection()
         yield proto.is_closed
 
     def test_send_message(self):
         """
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_strategies.py` & `magic-folder-23.5.0/src/magic_folder/test/test_strategies.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_tahoe_client.py` & `magic-folder-23.5.0/src/magic_folder/test/test_tahoe_client.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_testing.py` & `magic-folder-23.5.0/src/magic_folder/test/test_testing.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_upload.py` & `magic-folder-23.5.0/src/magic_folder/test/test_upload.py`

 * *Files 22% similar despite different names*

```diff
@@ -523,28 +523,20 @@
         yield mf.create_update()
         yield mf.when_idle()
 
         # status system should report our error
         self.assertThat(
             loads(alice.global_service.status_service._marshal_state()),
             ContainsDict({
-                "state": ContainsDict({
-                    "folders": ContainsDict({
-                        "default": ContainsDict({
-                            "errors": AfterPreprocessing(
-                                lambda errors: errors[0],
-                                ContainsDict({
-                                    "summary": Equals(
-                                        "Error updating personal DMD: Couldn't add random_local_file to directory. Error code 500"
-                                    )
-                                }),
-                            ),
-                        }),
-                    }),
-                }),
+                "events": AfterPreprocessing(
+                    lambda errors: [error["summary"] for error in errors if error["kind"] == "error-occurred"],
+                    Equals([
+                        "Error updating personal DMD: Couldn't add random_local_file to directory. Error code 500",
+                    ]),
+                )
             })
         )
 
         self.assertThat(
             self.eliot_logger.flush_tracebacks(Exception),
             MatchesListwise([
                 matches_flushed_traceback(Exception, "Couldn't add random_local_file to directory. Error code 500")
@@ -593,28 +585,20 @@
         yield mf.create_update()
         yield mf.when_idle()
 
         # status system should report our error
         self.assertThat(
             loads(alice.global_service.status_service._marshal_state()),
             ContainsDict({
-                "state": ContainsDict({
-                    "folders": ContainsDict({
-                        "default": ContainsDict({
-                            "errors": AfterPreprocessing(
-                                lambda errors: errors[0],
-                                ContainsDict({
-                                    "summary": Equals(
-                                        "Cancelled: random_local_file"
-                                    )
-                                }),
-                            ),
-                        }),
-                    }),
-                }),
+                "events": AfterPreprocessing(
+                    lambda errors: [error["summary"] for error in errors if error["kind"] == "error-occurred"],
+                    Equals([
+                        "Cancelled: random_local_file",
+                    ]),
+                )
             })
         )
         self.assertThat(
             self.eliot_logger.flush_tracebacks(CancelledError),
             MatchesListwise([
                 matches_flushed_traceback(CancelledError),
             ]),
@@ -665,28 +649,20 @@
         yield mf.create_update()
         yield mf.when_idle()
 
         # status system should report our error
         self.assertThat(
             loads(alice.global_service.status_service._marshal_state()),
             ContainsDict({
-                "state": ContainsDict({
-                    "folders": ContainsDict({
-                        "default": ContainsDict({
-                            "errors": AfterPreprocessing(
-                                lambda errors: errors[0],
-                                ContainsDict({
-                                    "summary": Equals(
-                                        "Cancelled: a_local_file"
-                                    )
-                                }),
-                            ),
-                        }),
-                    }),
-                }),
+                "events": AfterPreprocessing(
+                    lambda errors: [error["summary"] for error in errors if error["kind"] == "error-occurred"],
+                    Equals([
+                        "Cancelled: a_local_file",
+                    ]),
+                )
             })
         )
 
     @inline_callbacks
     def test_update_dmd_fails_then_succeeds(self):
         """
         Some attempts to update the Personal DMD fail, then stop failing.
@@ -746,27 +722,21 @@
         yield mf.create_update()
         yield mf.when_idle()
 
         # status system should report our error
         self.assertThat(
             loads(alice.global_service.status_service._marshal_state()),
             ContainsDict({
-                "state": ContainsDict({
-                    "folders": ContainsDict({
-                        "default": ContainsDict({
-                            "errors": AfterPreprocessing(
-                                lambda errors: [error["summary"] for error in errors],
-                                Equals([
-                                    "Error updating personal DMD: bad stuff",
-                                    "Error updating personal DMD: bad stuff",
-                                ]),
-                            ),
-                        }),
-                    }),
-                }),
+                "events": AfterPreprocessing(
+                    lambda errors: [error["summary"] for error in errors if error["kind"] == "error-occurred"],
+                    Equals([
+                        "Error updating personal DMD: bad stuff",
+                        "Error updating personal DMD: bad stuff",
+                    ]),
+                )
             })
         )
         # ...as should the logger
         self.assertThat(
             self.eliot_logger.flush_tracebacks(Exception),
             AfterPreprocessing(
                 lambda errors: [err["reason"] for err in errors],
@@ -840,27 +810,21 @@
         yield mf.create_update()
         yield mf.when_idle()
 
         # status system should report our error
         self.assertThat(
             loads(alice.global_service.status_service._marshal_state()),
             ContainsDict({
-                "state": ContainsDict({
-                    "folders": ContainsDict({
-                        "default": ContainsDict({
-                            "errors": AfterPreprocessing(
-                                lambda errors: [error["summary"] for error in errors],
-                                Equals([
-                                    "Error uploading danger: bad stuff",
-                                    "Error uploading danger: bad stuff",
-                                ]),
-                            ),
-                        }),
-                    }),
-                }),
+                "events": AfterPreprocessing(
+                    lambda errors: [error["summary"] for error in errors if error["kind"] == "error-occurred"],
+                    Equals([
+                        "Error uploading danger: bad stuff",
+                        "Error uploading danger: bad stuff",
+                    ]),
+                )
             })
         )
         # ...as should the logger
         # XXX why does this only return _one_ error -- should be two!
         self.assertThat(
             self.eliot_logger.flush_tracebacks(Exception),
             AfterPreprocessing(
```

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_util_database.py` & `magic-folder-23.5.0/src/magic_folder/test/test_util_database.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_util_file.py` & `magic-folder-23.5.0/src/magic_folder/test/test_util_file.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_util_twisted.py` & `magic-folder-23.5.0/src/magic_folder/test/test_util_twisted.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/test/test_web.py` & `magic-folder-23.5.0/src/magic_folder/test/test_web.py`

 * *Files 0% similar despite different names*

```diff
@@ -1979,14 +1979,38 @@
                                 "last-upload-duration": None,
                             },
                         ]),
                     )
                 ),
             )
         )
+        self.assertThat(
+            authorized_request(
+                node.http_client,
+                AUTH_TOKEN,
+                u"GET",
+                self.url.child("default", "recent-changes"),
+            ),
+            succeeded(
+                matches_response(
+                    code_matcher=Equals(200),
+                    body_matcher=AfterPreprocessing(
+                        loads,
+                        Equals([
+                            {
+                                "conflicted": False,
+                                "last-updated": 42,
+                                "modified": 1,
+                                "relpath": "foo",
+                            }
+                        ])
+                    )
+                )
+            )
+        )
 
 
 class ConflictStatusTests(SyncTestCase):
     """
     Tests relating to the '/v1/magic-folder/<folder>/conflicts` API
     """
     url = DecodedURL.from_text(u"http://example.invalid./v1/magic-folder")
```

### Comparing `magic-folder-23.3.1/src/magic_folder/testing/web.py` & `magic-folder-23.5.0/src/magic_folder/testing/web.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/uploader.py` & `magic-folder-23.5.0/src/magic_folder/uploader.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 from .status import (
     FolderStatus,
 )
 from .config import (
     MagicFolderConfig,
 )
 from .util.file import get_pathinfo
+from .util.capabilities import (
+    random_immutable,
+)
 
 
 SNAPSHOT_CREATOR_PROCESS_ITEM = ActionType(
     u"magic-folder:local-snapshot-creator:processing-item",
     [RELPATH],
     [],
     u"Local snapshot creator is processing an input.",
@@ -87,15 +90,15 @@
     _author = attr.ib(validator=attr.validators.instance_of(LocalAuthor))  # LocalAuthor instance
     _stash_dir = attr.ib(validator=attr.validators.instance_of(FilePath))
     _magic_dir = attr.ib(validator=attr.validators.instance_of(FilePath))
     _tahoe_client = attr.ib()
     _cooperator = attr.ib(default=None)
 
     @inline_callbacks
-    def store_local_snapshot(self, path):
+    def create_local_snapshot(self, path):
         """
         Convert `path` into a LocalSnapshot and persist it to disk. If
         `path` does not exist, the this is a 'delete' (and we must
         'know' about the file already).
 
         :param FilePath path: a single file inside our magic-folder dir
 
@@ -174,20 +177,22 @@
     When told about local files (that must exist in `.magic_path` or below) we
     deliver it to the snapshot creator.
     """
     _config = attr.ib(validator=attr.validators.instance_of(MagicFolderConfig))
     _snapshot_creator = attr.ib()
     _status = attr.ib(validator=attr.validators.instance_of(FolderStatus))
     _queue = attr.ib(default=attr.Factory(DeferredQueue))
+    _service_d = attr.ib(default=None)
 
     def startService(self):
         """
         Start a periodic loop that looks for work and does it.
         """
         service.Service.startService(self)
+        assert self._service_d is None, "already started"
         self._service_d = self._process_queue()
 
     @inline_callbacks
     def _process_queue(self):
         """
         Wait for a single item from the queue and process it, forever.
         """
@@ -195,15 +200,15 @@
             try:
                 (path, d) = yield self._queue.get()
             except CancelledError:
                 return
 
             try:
                 with PROCESS_FILE_QUEUE(relpath=path.path):
-                    snap = yield self._snapshot_creator.store_local_snapshot(path)
+                    snap = yield self._snapshot_creator.create_local_snapshot(path)
                     d.callback(snap)
             except CancelledError:
                 d.cancel()
                 return
             except Exception:
                 d.errback()
                 write_traceback()
@@ -365,7 +370,33 @@
         # we could check if this one is already queued -- that should be
         # impossible
 
         # add file into the queue
         d = Deferred()
         self._queue.put((snapshot, d))
         return d
+
+
+@attr.s
+@implementer(service.IService)
+class InMemoryUploaderService(service.Service):
+    """
+    For testing.
+
+    An UploaderService that doesn't actually talk to Tahoe-LAFS
+    """
+
+    _uploads = attr.ib(validator=attr.validators.instance_of(list))
+
+    @inline_callbacks
+    def upload_snapshot(self, snapshot):
+        rel = self._uploads.pop(0)
+
+        class FakeRemoteSnapshot(object):
+            relpath = rel
+            author = object()#SnapshotAuthor()
+            metadata = dict()
+            capability = random_immutable(directory=True)
+            parents_raw = []
+            content_cap = random_immutable(directory=False)
+            metadata_cap = random_immutable(directory=False)
+        returnValue(FakeRemoteSnapshot())
```

### Comparing `magic-folder-23.3.1/src/magic_folder/util/capabilities.py` & `magic-folder-23.5.0/src/magic_folder/util/capabilities.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/util/database.py` & `magic-folder-23.5.0/src/magic_folder/util/database.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/util/eliotutil.py` & `magic-folder-23.5.0/src/magic_folder/util/eliotutil.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/util/encoding.py` & `magic-folder-23.5.0/src/magic_folder/util/encoding.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/util/file.py` & `magic-folder-23.5.0/src/magic_folder/util/file.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/util/observer.py` & `magic-folder-23.5.0/src/magic_folder/util/observer.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/util/twisted.py` & `magic-folder-23.5.0/src/magic_folder/util/twisted.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/util/wrap.py` & `magic-folder-23.5.0/src/magic_folder/util/wrap.py`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/src/magic_folder/web.py` & `magic-folder-23.5.0/src/magic_folder/web.py`

 * *Files 5% similar despite different names*

```diff
@@ -433,14 +433,39 @@
 
         yield folder_service.add_snapshot(path)
 
         request.setResponseCode(http.CREATED)
         _application_json(request)
         returnValue(b"{}")
 
+    @app.route("/magic-folder/<string:folder_name>/recent-changes", methods=['GET'])
+    def recent_changes(request, folder_name):
+        """
+        Respond with the recent ``number?=` of files, ordered by their
+        most-recent change.
+        """
+        number = int(request.args.get("number", ["30"])[0])
+        folder = global_config.get_magic_folder(folder_name)
+        recents = folder.get_recent_remotesnapshot_paths(number)
+        most_recent = [
+            {
+                "relpath": relpath,
+                # XXX nothing in the status API dumps this information
+                # -- maybe it should? in upload-queued? and
+                # download-finished?  ...but also nothing except the
+                # CLI used the "recent" in the state-based API
+                "modified": timestamp,
+                "last-updated": last_updated,
+                "conflicted": bool(len(folder.list_conflicts_for(relpath))),
+            }
+            for relpath, timestamp, last_updated
+            in recents
+        ]
+        return json.dumps(most_recent).encode("utf8")
+
     @app.route("/magic-folder", methods=["GET"])
     def list_folders(request):
         """
         Render a list of Magic Folders and some of their details, encoded as JSON.
         """
         include_secret_information = int(request.args.get(b"include_secret_information", [0])[0])
         _application_json(request)  # set reply headers
```

### Comparing `magic-folder-23.3.1/src/magic_folder.egg-info/PKG-INFO` & `magic-folder-23.5.0/src/magic_folder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-folder
-Version: 23.3.1
+Version: 23.5.0
 Summary: Tahoe-LAFS-based file synchronization
 Home-page: https://github.com/LeastAuthority/magic-folder/
 Author: the Tahoe-LAFS developers, the Magic-Folder developers
 Author-email: tahoe-dev@tahoe-lafs.org
 License: GNU GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `magic-folder-23.3.1/src/magic_folder.egg-info/SOURCES.txt` & `magic-folder-23.5.0/src/magic_folder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -342,14 +342,15 @@
 integration/test_general_cli.py
 integration/test_invite.py
 integration/test_kitties.py
 integration/test_list.py
 integration/test_magic_folder.py
 integration/test_magic_folder.py.orig
 integration/test_magic_folder.py.rej
+integration/test_multiuser.py
 integration/test_same_files.py
 integration/test_status.py
 integration/test_synchronize.py
 integration/test_tahoe_objects.py
 integration/util.py
 integration/util.py.orig
 integration/util.py.rej
```

### Comparing `magic-folder-23.3.1/src/magic_folder.egg-info/requires.txt` & `magic-folder-23.5.0/src/magic_folder.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `magic-folder-23.3.1/tox.ini` & `magic-folder-23.5.0/tox.ini`

 * *Files identical despite different names*

