# Comparing `tmp/datamol-0.9.7.tar.gz` & `tmp/datamol-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamol-0.9.7.tar", last modified: Fri Apr 14 22:59:25 2023, max compression
+gzip compressed data, was "datamol-0.9.8.tar", last modified: Fri Apr 14 23:02:44 2023, max compression
```

## Comparing `datamol-0.9.7.tar` & `datamol-0.9.8.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.938113 datamol-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-14 22:59:12.000000 datamol-0.9.7/.authors.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.906113 datamol-0.9.7/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-14 22:57:37.000000 datamol-0.9.7/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-14 22:57:37.000000 datamol-0.9.7/.devcontainer/bashrc
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-14 22:57:37.000000 datamol-0.9.7/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.906113 datamol-0.9.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 22:57:37.000000 datamol-0.9.7/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-14 22:57:37.000000 datamol-0.9.7/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 22:57:37.000000 datamol-0.9.7/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-14 22:57:37.000000 datamol-0.9.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 22:57:37.000000 datamol-0.9.7/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.906113 datamol-0.9.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-14 22:57:37.000000 datamol-0.9.7/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 22:57:37.000000 datamol-0.9.7/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-14 22:57:37.000000 datamol-0.9.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-14 22:57:37.000000 datamol-0.9.7/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 22:57:37.000000 datamol-0.9.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-14 22:59:12.000000 datamol-0.9.7/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-14 22:59:12.000000 datamol-0.9.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26231 2023-04-14 22:59:12.000000 datamol-0.9.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-04-14 22:57:37.000000 datamol-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-14 22:59:25.938113 datamol-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-04-14 22:57:37.000000 datamol-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.906113 datamol-0.9.7/binder/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 22:57:37.000000 datamol-0.9.7/binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 22:57:37.000000 datamol-0.9.7/binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 22:57:37.000000 datamol-0.9.7/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.910113 datamol-0.9.7/datamol/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/_sanifix4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.910113 datamol-0.9.7/datamol/conformers/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/conformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/conformers/_conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/conformers/_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.910113 datamol-0.9.7/datamol/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   160134 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/data/cdk2.sdf
--rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/data/freesolv.csv
--rw-r--r--   0 runner    (1001) docker     (123)   124841 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/data/reactions.json
--rw-r--r--   0 runner    (1001) docker     (123)   245735 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/data/solubility.test.sdf
--rw-r--r--   0 runner    (1001) docker     (123)  1376487 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/data/solubility.train.sdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.914113 datamol-0.9.7/datamol/descriptors/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/descriptors/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/descriptors/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/fp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.914113 datamol-0.9.7/datamol/fragment/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/fragment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/fragment/_assemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/fragment/_fragment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.914113 datamol-0.9.7/datamol/isomers/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/isomers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/isomers/_enumerate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/isomers/_structural.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/mcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43876 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/mol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/molar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.914113 datamol-0.9.7/datamol/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/predictors/esol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.914113 datamol-0.9.7/datamol/reactions/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/reactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/reactions/_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/reactions/_reactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.914113 datamol-0.9.7/datamol/scaffold/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/scaffold/_fuzzy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.918113 datamol-0.9.7/datamol/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/utils/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/utils/perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.918113 datamol-0.9.7/datamol/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/viz/_circle_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/viz/_conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19046 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/viz/_lasso_highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/viz/_substructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/viz/_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-14 22:57:37.000000 datamol-0.9.7/datamol/viz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.910113 datamol-0.9.7/datamol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-14 22:59:25.000000 datamol-0.9.7/datamol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-14 22:59:25.000000 datamol-0.9.7/datamol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:59:25.000000 datamol-0.9.7/datamol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-14 22:59:25.000000 datamol-0.9.7/datamol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 22:59:25.000000 datamol-0.9.7/datamol.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.918113 datamol-0.9.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.922113 datamol-0.9.7/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.align.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.cluster.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.conformers.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.convert.md
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.data.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.descriptors.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.fp.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.fragment.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.graph.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.io.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.isomers.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.log.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.mol.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.molar.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.reactions.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.scaffold.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.similarity.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/api/datamol.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.902113 datamol-0.9.7/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.922113 datamol-0.9.7/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/assets/css/custom-datamol.css
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/assets/css/tweak-width.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.922113 datamol-0.9.7/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/contribute.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.922113 datamol-0.9.7/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/images/logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/images/logo-title.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.926113 datamol-0.9.7/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)   298565 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/Aligning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   174933 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/Clustering.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    94833 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/Conformers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   180458 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/Descriptors.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/Filesystem.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   297941 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/Fragment.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   210862 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/Fuzzy_Scaffolds.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42846 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/Preprocessing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    89360 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/Reactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   151601 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/Scaffolds.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   521054 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/The_Basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   181122 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/Visualization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.930113 datamol-0.9.7/docs/tutorials/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1345316 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/data/ReactionBlock.rxn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.930113 datamol-0.9.7/docs/tutorials/images/
--rw-r--r--   0 runner    (1001) docker     (123)   141008 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/images/Aligning_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    76455 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/images/Aligning_2.png
--rw-r--r--   0 runner    (1001) docker     (123)   310889 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/images/Conformers_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/images/Descriptors_1.png
--rw-r--r--   0 runner    (1001) docker     (123)   422734 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/images/Fragment_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    67840 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/images/Fragment_2.png
--rw-r--r--   0 runner    (1001) docker     (123)    34879 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/images/Fragment_3.png
--rw-r--r--   0 runner    (1001) docker     (123)   333241 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/images/Preprocess_1.png
--rw-r--r--   0 runner    (1001) docker     (123)   102167 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/tutorials/images/Scaffolds_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-14 22:57:37.000000 datamol-0.9.7/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 22:57:37.000000 datamol-0.9.7/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-14 22:57:37.000000 datamol-0.9.7/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.934113 datamol-0.9.7/news/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 22:57:37.000000 datamol-0.9.7/news/TEMPLATE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-14 22:57:37.000000 datamol-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-14 22:57:37.000000 datamol-0.9.7/rever.xsh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 22:59:25.938113 datamol-0.9.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.938113 datamol-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:59:25.938113 datamol-0.9.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/data/TUBB3-observations-last-broken.sdf
--rw-r--r--   0 runner    (1001) docker     (123)    30331 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/data/TUBB3-observations.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/data/TUBB3-observations.sdf.gz
--rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/data/freesolv.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28227 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/data/freesolv.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/data/test.mol2
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_datamol_import_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_fragment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_isomers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_mcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_mol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_molar.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_predictors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_utils_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_utils_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_utils_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_viz_lasso_highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 22:57:37.000000 datamol-0.9.7/tests/test_viz_substrcture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.336417 datamol-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-14 23:02:33.000000 datamol-0.9.8/.authors.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.308417 datamol-0.9.8/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-14 23:01:55.000000 datamol-0.9.8/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-14 23:01:55.000000 datamol-0.9.8/.devcontainer/bashrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-14 23:01:55.000000 datamol-0.9.8/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.308417 datamol-0.9.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 23:01:55.000000 datamol-0.9.8/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-14 23:01:55.000000 datamol-0.9.8/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 23:01:55.000000 datamol-0.9.8/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-14 23:01:55.000000 datamol-0.9.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 23:01:55.000000 datamol-0.9.8/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.308417 datamol-0.9.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-14 23:01:55.000000 datamol-0.9.8/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 23:01:55.000000 datamol-0.9.8/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-14 23:01:55.000000 datamol-0.9.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-14 23:01:55.000000 datamol-0.9.8/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 23:01:55.000000 datamol-0.9.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-14 23:02:33.000000 datamol-0.9.8/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-14 23:02:33.000000 datamol-0.9.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26292 2023-04-14 23:02:33.000000 datamol-0.9.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-04-14 23:01:55.000000 datamol-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-14 23:02:44.336417 datamol-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-04-14 23:01:55.000000 datamol-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.308417 datamol-0.9.8/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 23:01:55.000000 datamol-0.9.8/binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 23:01:55.000000 datamol-0.9.8/binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 23:01:55.000000 datamol-0.9.8/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.312417 datamol-0.9.8/datamol/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/_sanifix4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.312417 datamol-0.9.8/datamol/conformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/conformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/conformers/_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/conformers/_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.312417 datamol-0.9.8/datamol/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160134 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/data/cdk2.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/data/freesolv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   124841 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/data/reactions.json
+-rw-r--r--   0 runner    (1001) docker     (123)   245735 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/data/solubility.test.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)  1376487 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/data/solubility.train.sdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.316417 datamol-0.9.8/datamol/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/descriptors/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/descriptors/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/fp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.316417 datamol-0.9.8/datamol/fragment/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/fragment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/fragment/_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/fragment/_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.316417 datamol-0.9.8/datamol/isomers/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/isomers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/isomers/_enumerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/isomers/_structural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/mcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43876 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/molar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.316417 datamol-0.9.8/datamol/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/predictors/esol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.316417 datamol-0.9.8/datamol/reactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/reactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/reactions/_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/reactions/_reactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.316417 datamol-0.9.8/datamol/scaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/scaffold/_fuzzy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.316417 datamol-0.9.8/datamol/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/utils/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/utils/perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.320417 datamol-0.9.8/datamol/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/viz/_circle_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/viz/_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19046 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/viz/_lasso_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/viz/_substructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/viz/_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-14 23:01:55.000000 datamol-0.9.8/datamol/viz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.312417 datamol-0.9.8/datamol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-14 23:02:44.000000 datamol-0.9.8/datamol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-14 23:02:44.000000 datamol-0.9.8/datamol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:02:44.000000 datamol-0.9.8/datamol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-14 23:02:44.000000 datamol-0.9.8/datamol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 23:02:44.000000 datamol-0.9.8/datamol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.320417 datamol-0.9.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.320417 datamol-0.9.8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.align.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.cluster.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.conformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.convert.md
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.data.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.descriptors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.fp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.fragment.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.graph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.io.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.isomers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.log.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.mol.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.molar.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.reactions.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.scaffold.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.similarity.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/api/datamol.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.304417 datamol-0.9.8/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.320417 datamol-0.9.8/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/assets/css/custom-datamol.css
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/assets/css/tweak-width.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.320417 datamol-0.9.8/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/contribute.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.320417 datamol-0.9.8/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/images/logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/images/logo-title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.324417 datamol-0.9.8/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   298565 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/Aligning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   174933 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/Clustering.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    94833 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/Conformers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   180458 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/Descriptors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/Filesystem.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   297941 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/Fragment.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   210862 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/Fuzzy_Scaffolds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42846 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/Preprocessing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    89360 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/Reactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   151601 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/Scaffolds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   521054 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/The_Basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   181122 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/Visualization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.328417 datamol-0.9.8/docs/tutorials/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1345316 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/data/ReactionBlock.rxn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.332417 datamol-0.9.8/docs/tutorials/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   141008 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/images/Aligning_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76455 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/images/Aligning_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   310889 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/images/Conformers_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/images/Descriptors_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   422734 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/images/Fragment_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67840 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/images/Fragment_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34879 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/images/Fragment_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   333241 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/images/Preprocess_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   102167 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/tutorials/images/Scaffolds_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-14 23:01:55.000000 datamol-0.9.8/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 23:01:55.000000 datamol-0.9.8/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-14 23:01:55.000000 datamol-0.9.8/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.332417 datamol-0.9.8/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 23:01:55.000000 datamol-0.9.8/news/TEMPLATE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-14 23:01:55.000000 datamol-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-14 23:01:55.000000 datamol-0.9.8/rever.xsh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 23:02:44.336417 datamol-0.9.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.332417 datamol-0.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:02:44.336417 datamol-0.9.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/data/TUBB3-observations-last-broken.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)    30331 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/data/TUBB3-observations.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/data/TUBB3-observations.sdf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/data/freesolv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28227 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/data/freesolv.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/data/test.mol2
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_datamol_import_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_isomers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_mcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_molar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_predictors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_utils_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_utils_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_utils_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_viz_lasso_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 23:01:55.000000 datamol-0.9.8/tests/test_viz_substrcture.py
```

### Comparing `datamol-0.9.7/.authors.yml` & `datamol-0.9.8/.authors.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/.devcontainer/Dockerfile` & `datamol-0.9.8/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/.devcontainer/devcontainer.json` & `datamol-0.9.8/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/.github/CODE_OF_CONDUCT.md` & `datamol-0.9.8/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/.github/workflows/code-check.yml` & `datamol-0.9.8/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/.github/workflows/doc.yml` & `datamol-0.9.8/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/.github/workflows/release.yml` & `datamol-0.9.8/.github/workflows/release.yml`

 * *Files 5% similar despite different names*

```diff
@@ -102,8 +102,9 @@
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
           packages-dir: dist/
 
       - name: Create GitHub Release
         uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
         with:
+          tag_name: ${{ inputs.release-version }}
           body: "See [CHANGELOGS.rst](https://github.com/datamol-io/datamol/blob/main/CHANGELOG.rst)."
```

### Comparing `datamol-0.9.7/.github/workflows/test.yml` & `datamol-0.9.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/.gitignore` & `datamol-0.9.8/.gitignore`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/.mailmap` & `datamol-0.9.8/.mailmap`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/CHANGELOG.rst` & `datamol-0.9.8/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 ==================
 Datamol Changelogs
 ==================
 
 .. current developments
 
+v0.9.8
+====================
+
+**Authors:**
+
+* Hadrien Mary
+
+
+
 v0.9.7
 ====================
 
 **Authors:**
 
 * Hadrien Mary
```

### Comparing `datamol-0.9.7/LICENSE` & `datamol-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/PKG-INFO` & `datamol-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamol
-Version: 0.9.7
+Version: 0.9.8
 Summary: A python library to work with molecules. Built on top of RDKit.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol
 Project-URL: Bug Tracker, https://github.com/datamol-io/datamol/issues
 Project-URL: Documentation, https://docs.datamol.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datamol Version: 0.9.7 Summary: A python library to
+Metadata-Version: 2.1 Name: datamol Version: 0.9.8 Summary: A python library to
 work with molecules. Built on top of RDKit. Author-email: Hadrien Mary
 valencediscovery.com> License: Apache Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol Project-URL:
 Bug Tracker, https://github.com/datamol-io/datamol/issues Project-URL:
 Documentation, https://docs.datamol.io Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
```

### Comparing `datamol-0.9.7/README.md` & `datamol-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/binder/environment.yml` & `datamol-0.9.8/binder/environment.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/__init__.py` & `datamol-0.9.8/datamol/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/_sanifix4.py` & `datamol-0.9.8/datamol/_sanifix4.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/_version.py` & `datamol-0.9.8/datamol/_version.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/align.py` & `datamol-0.9.8/datamol/align.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/cluster.py` & `datamol-0.9.8/datamol/cluster.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/conformers/_conformers.py` & `datamol-0.9.8/datamol/conformers/_conformers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/conformers/_features.py` & `datamol-0.9.8/datamol/conformers/_features.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/convert.py` & `datamol-0.9.8/datamol/convert.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/data/__init__.py` & `datamol-0.9.8/datamol/data/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/data/cdk2.sdf` & `datamol-0.9.8/datamol/data/cdk2.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/data/freesolv.csv` & `datamol-0.9.8/datamol/data/freesolv.csv`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/data/reactions.json` & `datamol-0.9.8/datamol/data/reactions.json`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/data/solubility.test.sdf` & `datamol-0.9.8/datamol/data/solubility.test.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/data/solubility.train.sdf` & `datamol-0.9.8/datamol/data/solubility.train.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/descriptors/__init__.py` & `datamol-0.9.8/datamol/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/descriptors/compute.py` & `datamol-0.9.8/datamol/descriptors/compute.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/descriptors/descriptors.py` & `datamol-0.9.8/datamol/descriptors/descriptors.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/fp.py` & `datamol-0.9.8/datamol/fp.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/fragment/_assemble.py` & `datamol-0.9.8/datamol/fragment/_assemble.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/fragment/_fragment.py` & `datamol-0.9.8/datamol/fragment/_fragment.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/graph.py` & `datamol-0.9.8/datamol/graph.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/io.py` & `datamol-0.9.8/datamol/io.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/isomers/_enumerate.py` & `datamol-0.9.8/datamol/isomers/_enumerate.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/isomers/_structural.py` & `datamol-0.9.8/datamol/isomers/_structural.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/log.py` & `datamol-0.9.8/datamol/log.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/mcs.py` & `datamol-0.9.8/datamol/mcs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/mol.py` & `datamol-0.9.8/datamol/mol.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/molar.py` & `datamol-0.9.8/datamol/molar.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/predictors/esol.py` & `datamol-0.9.8/datamol/predictors/esol.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/reactions/__init__.py` & `datamol-0.9.8/datamol/reactions/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/reactions/_attachments.py` & `datamol-0.9.8/datamol/reactions/_attachments.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/reactions/_reactions.py` & `datamol-0.9.8/datamol/reactions/_reactions.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/scaffold/_fuzzy.py` & `datamol-0.9.8/datamol/scaffold/_fuzzy.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/similarity.py` & `datamol-0.9.8/datamol/similarity.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/utils/decorators.py` & `datamol-0.9.8/datamol/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/utils/fs.py` & `datamol-0.9.8/datamol/utils/fs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/utils/jobs.py` & `datamol-0.9.8/datamol/utils/jobs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/utils/perf.py` & `datamol-0.9.8/datamol/utils/perf.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/utils/testing.py` & `datamol-0.9.8/datamol/utils/testing.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/viz/_circle_grid.py` & `datamol-0.9.8/datamol/viz/_circle_grid.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/viz/_conformers.py` & `datamol-0.9.8/datamol/viz/_conformers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/viz/_lasso_highlight.py` & `datamol-0.9.8/datamol/viz/_lasso_highlight.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/viz/_substructure.py` & `datamol-0.9.8/datamol/viz/_substructure.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/viz/_viz.py` & `datamol-0.9.8/datamol/viz/_viz.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol/viz/utils.py` & `datamol-0.9.8/datamol/viz/utils.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/datamol.egg-info/PKG-INFO` & `datamol-0.9.8/datamol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamol
-Version: 0.9.7
+Version: 0.9.8
 Summary: A python library to work with molecules. Built on top of RDKit.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol
 Project-URL: Bug Tracker, https://github.com/datamol-io/datamol/issues
 Project-URL: Documentation, https://docs.datamol.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datamol Version: 0.9.7 Summary: A python library to
+Metadata-Version: 2.1 Name: datamol Version: 0.9.8 Summary: A python library to
 work with molecules. Built on top of RDKit. Author-email: Hadrien Mary
 valencediscovery.com> License: Apache Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol Project-URL:
 Bug Tracker, https://github.com/datamol-io/datamol/issues Project-URL:
 Documentation, https://docs.datamol.io Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
```

### Comparing `datamol-0.9.7/datamol.egg-info/SOURCES.txt` & `datamol-0.9.8/datamol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/assets/css/custom-datamol.css` & `datamol-0.9.8/docs/assets/css/custom-datamol.css`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/assets/css/custom.css` & `datamol-0.9.8/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/contribute.md` & `datamol-0.9.8/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/images/logo-black.png` & `datamol-0.9.8/docs/images/logo-black.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/images/logo-black.svg` & `datamol-0.9.8/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/images/logo-title.svg` & `datamol-0.9.8/docs/images/logo-title.svg`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/images/logo.png` & `datamol-0.9.8/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/images/logo.svg` & `datamol-0.9.8/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/index.md` & `datamol-0.9.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/Aligning.ipynb` & `datamol-0.9.8/docs/tutorials/Aligning.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/Clustering.ipynb` & `datamol-0.9.8/docs/tutorials/Clustering.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/Conformers.ipynb` & `datamol-0.9.8/docs/tutorials/Conformers.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/Descriptors.ipynb` & `datamol-0.9.8/docs/tutorials/Descriptors.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/Filesystem.ipynb` & `datamol-0.9.8/docs/tutorials/Filesystem.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/Fragment.ipynb` & `datamol-0.9.8/docs/tutorials/Fragment.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/Fuzzy_Scaffolds.ipynb` & `datamol-0.9.8/docs/tutorials/Fuzzy_Scaffolds.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/Preprocessing.ipynb` & `datamol-0.9.8/docs/tutorials/Preprocessing.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/Reactions.ipynb` & `datamol-0.9.8/docs/tutorials/Reactions.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/Scaffolds.ipynb` & `datamol-0.9.8/docs/tutorials/Scaffolds.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/The_Basics.ipynb` & `datamol-0.9.8/docs/tutorials/The_Basics.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/Visualization.ipynb` & `datamol-0.9.8/docs/tutorials/Visualization.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf` & `datamol-0.9.8/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/data/ReactionBlock.rxn` & `datamol-0.9.8/docs/tutorials/data/ReactionBlock.rxn`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/images/Aligning_1.png` & `datamol-0.9.8/docs/tutorials/images/Aligning_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/images/Aligning_2.png` & `datamol-0.9.8/docs/tutorials/images/Aligning_2.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/images/Conformers_1.png` & `datamol-0.9.8/docs/tutorials/images/Conformers_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/images/Descriptors_1.png` & `datamol-0.9.8/docs/tutorials/images/Descriptors_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/images/Fragment_1.png` & `datamol-0.9.8/docs/tutorials/images/Fragment_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/images/Fragment_2.png` & `datamol-0.9.8/docs/tutorials/images/Fragment_2.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/images/Fragment_3.png` & `datamol-0.9.8/docs/tutorials/images/Fragment_3.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/images/Preprocess_1.png` & `datamol-0.9.8/docs/tutorials/images/Preprocess_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/tutorials/images/Scaffolds_1.png` & `datamol-0.9.8/docs/tutorials/images/Scaffolds_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/docs/usage.md` & `datamol-0.9.8/docs/usage.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/env.yml` & `datamol-0.9.8/env.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/mkdocs.yml` & `datamol-0.9.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/pyproject.toml` & `datamol-0.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/conftest.py` & `datamol-0.9.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/data/TUBB3-observations-last-broken.sdf` & `datamol-0.9.8/tests/data/TUBB3-observations-last-broken.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/data/TUBB3-observations.sdf` & `datamol-0.9.8/tests/data/TUBB3-observations.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/data/TUBB3-observations.sdf.gz` & `datamol-0.9.8/tests/data/TUBB3-observations.sdf.gz`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/data/freesolv.csv` & `datamol-0.9.8/tests/data/freesolv.csv`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/data/freesolv.xlsx` & `datamol-0.9.8/tests/data/freesolv.xlsx`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/data/test.mol2` & `datamol-0.9.8/tests/data/test.mol2`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_align.py` & `datamol-0.9.8/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_cluster.py` & `datamol-0.9.8/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_conformers.py` & `datamol-0.9.8/tests/test_conformers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_convert.py` & `datamol-0.9.8/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_data.py` & `datamol-0.9.8/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_datamol_import_time.py` & `datamol-0.9.8/tests/test_datamol_import_time.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_descriptors.py` & `datamol-0.9.8/tests/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_fp.py` & `datamol-0.9.8/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_fragment.py` & `datamol-0.9.8/tests/test_fragment.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_graph.py` & `datamol-0.9.8/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_io.py` & `datamol-0.9.8/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_isomers.py` & `datamol-0.9.8/tests/test_isomers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_log.py` & `datamol-0.9.8/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_mcs.py` & `datamol-0.9.8/tests/test_mcs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_mol.py` & `datamol-0.9.8/tests/test_mol.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_molar.py` & `datamol-0.9.8/tests/test_molar.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_notebooks.py` & `datamol-0.9.8/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_predictors.py` & `datamol-0.9.8/tests/test_predictors.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_reactions.py` & `datamol-0.9.8/tests/test_reactions.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_scaffold.py` & `datamol-0.9.8/tests/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_similarity.py` & `datamol-0.9.8/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_utils_fs.py` & `datamol-0.9.8/tests/test_utils_fs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_utils_jobs.py` & `datamol-0.9.8/tests/test_utils_jobs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_viz.py` & `datamol-0.9.8/tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_viz_lasso_highlight.py` & `datamol-0.9.8/tests/test_viz_lasso_highlight.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.7/tests/test_viz_substrcture.py` & `datamol-0.9.8/tests/test_viz_substrcture.py`

 * *Files identical despite different names*

