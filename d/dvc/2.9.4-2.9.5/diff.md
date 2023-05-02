# Comparing `tmp/dvc-2.9.4.tar.gz` & `tmp/dvc-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/dvc/dvc/dist/tmpnfzwlseh/dvc-2.9.4.tar", last modified: Wed Feb 16 10:58:37 2022, max compression
+gzip compressed data, was "/home/runner/work/dvc/dvc/dist/tmpylbi2mzu/dvc-2.9.5.tar", last modified: Mon Feb 21 02:27:12 2022, max compression
```

## Comparing `dvc-2.9.4.tar` & `dvc-2.9.5.tar`

### file list

```diff
@@ -1,661 +1,661 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/
--rw-r--r--   0 runner    (1001) docker     (116)      154 2022-02-16 10:56:58.000000 dvc-2.9.4/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (116)      263 2022-02-16 10:56:58.000000 dvc-2.9.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/.dvc/
--rw-r--r--   0 runner    (1001) docker     (116)      113 2022-02-16 10:56:58.000000 dvc-2.9.4/.dvc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)       70 2022-02-16 10:56:58.000000 dvc-2.9.4/.dvc/config
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-02-16 10:56:58.000000 dvc-2.9.4/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (116)       32 2022-02-16 10:56:58.000000 dvc-2.9.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/.github/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-02-16 10:56:58.000000 dvc-2.9.4/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (116)       63 2022-02-16 10:56:58.000000 dvc-2.9.4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)     1296 2022-02-16 10:56:58.000000 dvc-2.9.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (116)      189 2022-02-16 10:56:58.000000 dvc-2.9.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (116)       84 2022-02-16 10:56:58.000000 dvc-2.9.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (116)      395 2022-02-16 10:56:58.000000 dvc-2.9.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (116)      273 2022-02-16 10:56:58.000000 dvc-2.9.4/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (116)      183 2022-02-16 10:56:58.000000 dvc-2.9.4/.github/mergify.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1020 2022-02-16 10:56:58.000000 dvc-2.9.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      554 2022-02-16 10:56:58.000000 dvc-2.9.4/.github/workflows/benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     4786 2022-02-16 10:56:58.000000 dvc-2.9.4/.github/workflows/packages.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     2533 2022-02-16 10:56:58.000000 dvc-2.9.4/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      359 2022-02-16 10:56:58.000000 dvc-2.9.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      238 2022-02-16 10:56:58.000000 dvc-2.9.4/.mailmap
--rw-r--r--   0 runner    (1001) docker     (116)     2110 2022-02-16 10:56:58.000000 dvc-2.9.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      631 2022-02-16 10:56:58.000000 dvc-2.9.4/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      322 2022-02-16 10:56:58.000000 dvc-2.9.4/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (116)     3348 2022-02-16 10:56:58.000000 dvc-2.9.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)       95 2022-02-16 10:56:58.000000 dvc-2.9.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (116)    11350 2022-02-16 10:56:58.000000 dvc-2.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      103 2022-02-16 10:56:58.000000 dvc-2.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    13942 2022-02-16 10:58:37.000000 dvc-2.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    12661 2022-02-16 10:56:58.000000 dvc-2.9.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (116)       51 2022-02-16 10:56:58.000000 dvc-2.9.4/bin/dvc
--rw-r--r--   0 runner    (1001) docker     (116)       53 2022-02-16 10:56:58.000000 dvc-2.9.4/bin/dvc.bat
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/
--rw-r--r--   0 runner    (1001) docker     (116)      165 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      148 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4365 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/_debug.py
--rw-r--r--   0 runner    (1001) docker     (116)      142 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/_dvc_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     5091 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/analytics.py
--rw-r--r--   0 runner    (1001) docker     (116)     4122 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/api.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/cli/
--rw-r--r--   0 runner    (1001) docker     (116)     3649 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      697 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (116)     4943 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (116)      954 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/commands/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3453 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (116)     2554 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)     3708 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (116)     3029 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (116)     2211 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (116)     3031 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/completion.py
--rw-r--r--   0 runner    (1001) docker     (116)     7055 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     2078 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (116)     3663 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (116)    11637 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/data_sync.py
--rw-r--r--   0 runner    (1001) docker     (116)     1514 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (116)     6419 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/commands/experiments/
--rw-r--r--   0 runner    (1001) docker     (116)     1200 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1221 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (116)     1006 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (116)     3754 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (116)     1112 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/exec_run.py
--rw-r--r--   0 runner    (1001) docker     (116)     3996 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/gc.py
--rw-r--r--   0 runner    (1001) docker     (116)     5707 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/init.py
--rw-r--r--   0 runner    (1001) docker     (116)     2352 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (116)     2787 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (116)     2869 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/push.py
--rw-r--r--   0 runner    (1001) docker     (116)     1593 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (116)     4331 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (116)    19727 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (116)     1780 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/freeze.py
--rw-r--r--   0 runner    (1001) docker     (116)     4501 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/gc.py
--rw-r--r--   0 runner    (1001) docker     (116)     2753 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/get.py
--rw-r--r--   0 runner    (1001) docker     (116)     1451 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/get_url.py
--rw-r--r--   0 runner    (1001) docker     (116)     4469 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/git_hook.py
--rw-r--r--   0 runner    (1001) docker     (116)     2792 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/imp.py
--rw-r--r--   0 runner    (1001) docker     (116)     3269 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (116)     2928 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (116)     1083 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (116)     2776 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/live.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (116)     2491 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1348 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/ls/ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (116)    17045 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/machine.py
--rw-r--r--   0 runner    (1001) docker     (116)     7508 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     1392 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/move.py
--rw-r--r--   0 runner    (1001) docker     (116)     3667 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/params.py
--rw-r--r--   0 runner    (1001) docker     (116)    11089 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/plots.py
--rw-r--r--   0 runner    (1001) docker     (116)     9583 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/remote.py
--rw-r--r--   0 runner    (1001) docker     (116)     1278 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (116)     4962 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/repro.py
--rw-r--r--   0 runner    (1001) docker     (116)      762 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/root.py
--rw-r--r--   0 runner    (1001) docker     (116)     3005 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (116)    10436 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/stage.py
--rw-r--r--   0 runner    (1001) docker     (116)     2787 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (116)     1214 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/unprotect.py
--rw-r--r--   0 runner    (1001) docker     (116)     2218 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (116)      908 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (116)    13694 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/compare.py
--rw-r--r--   0 runner    (1001) docker     (116)     9721 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     9040 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (116)     3003 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/daemon.py
--rw-r--r--   0 runner    (1001) docker     (116)     7955 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/dagascii.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/data/
--rw-r--r--   0 runner    (1001) docker     (116)      814 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6366 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/checkout.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/data/db/
--rw-r--r--   0 runner    (1001) docker     (116)     2365 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3750 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/db/index.py
--rw-r--r--   0 runner    (1001) docker     (116)     5481 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/db/local.py
--rw-r--r--   0 runner    (1001) docker     (116)     2750 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/db/reference.py
--rw-r--r--   0 runner    (1001) docker     (116)     3254 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/diff.py
--rw-r--r--   0 runner    (1001) docker     (116)     1255 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/gc.py
--rw-r--r--   0 runner    (1001) docker     (116)     1224 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/meta.py
--rw-r--r--   0 runner    (1001) docker     (116)     3796 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/reference.py
--rw-r--r--   0 runner    (1001) docker     (116)     1171 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/slow_link_detection.py
--rw-r--r--   0 runner    (1001) docker     (116)    10372 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/stage.py
--rw-r--r--   0 runner    (1001) docker     (116)     5979 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/status.py
--rw-r--r--   0 runner    (1001) docker     (116)     5430 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/transfer.py
--rw-r--r--   0 runner    (1001) docker     (116)     7551 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data/tree.py
--rw-r--r--   0 runner    (1001) docker     (116)     4932 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/data_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/dependency/
--rw-r--r--   0 runner    (1001) docker     (116)     2264 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      944 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     5015 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/dependency/param.py
--rw-r--r--   0 runner    (1001) docker     (116)     6830 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/dependency/repo.py
--rw-r--r--   0 runner    (1001) docker     (116)    12662 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (116)      396 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/env.py
--rw-r--r--   0 runner    (1001) docker     (116)     9844 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     8290 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/external_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/fs/
--rw-r--r--   0 runner    (1001) docker     (116)     3927 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1277 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/_callback.py
--rw-r--r--   0 runner    (1001) docker     (116)     5712 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/azure.py
--rw-r--r--   0 runner    (1001) docker     (116)    10930 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     6250 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/dvc.py
--rw-r--r--   0 runner    (1001) docker     (116)     7601 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/fsspec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (116)     9731 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/gdrive.py
--rw-r--r--   0 runner    (1001) docker     (116)     1621 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/git.py
--rw-r--r--   0 runner    (1001) docker     (116)      720 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/gs.py
--rw-r--r--   0 runner    (1001) docker     (116)     2882 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/hdfs.py
--rw-r--r--   0 runner    (1001) docker     (116)     4581 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/http.py
--rw-r--r--   0 runner    (1001) docker     (116)      167 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/https.py
--rw-r--r--   0 runner    (1001) docker     (116)     5055 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/local.py
--rw-r--r--   0 runner    (1001) docker     (116)      901 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/memory.py
--rw-r--r--   0 runner    (1001) docker     (116)      985 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/oss.py
--rw-r--r--   0 runner    (1001) docker     (116)     2408 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/path.py
--rw-r--r--   0 runner    (1001) docker     (116)     1354 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/pool.py
--rw-r--r--   0 runner    (1001) docker     (116)    16392 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/repo.py
--rw-r--r--   0 runner    (1001) docker     (116)     7785 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/s3.py
--rw-r--r--   0 runner    (1001) docker     (116)     4364 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/ssh.py
--rw-r--r--   0 runner    (1001) docker     (116)     4547 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     3116 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/webdav.py
--rw-r--r--   0 runner    (1001) docker     (116)     1575 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/fs/webhdfs.py
--rw-r--r--   0 runner    (1001) docker     (116)      923 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/hash_info.py
--rw-r--r--   0 runner    (1001) docker     (116)    13236 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/ignore.py
--rw-r--r--   0 runner    (1001) docker     (116)     4145 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/info.py
--rw-r--r--   0 runner    (1001) docker     (116)     1134 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/istextfile.py
--rw-r--r--   0 runner    (1001) docker     (116)     5016 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/lock.py
--rw-r--r--   0 runner    (1001) docker     (116)     8845 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/machine/
--rw-r--r--   0 runner    (1001) docker     (116)     6738 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/machine/backend/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/machine/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1611 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/machine/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     3288 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/machine/backend/terraform.py
--rw-r--r--   0 runner    (1001) docker     (116)      122 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/objects/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16425 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/objects/db.py
--rw-r--r--   0 runner    (1001) docker     (116)      236 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/objects/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)     2186 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/objects/file.py
--rw-r--r--   0 runner    (1001) docker     (116)    30231 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/parsing/
--rw-r--r--   0 runner    (1001) docker     (116)    15258 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16710 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/parsing/context.py
--rw-r--r--   0 runner    (1001) docker     (116)     4451 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/parsing/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1158 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/parsing/versions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2598 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/pathspec_math.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/proc/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      705 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/proc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     4964 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/proc/manager.py
--rw-r--r--   0 runner    (1001) docker     (116)     5057 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/proc/process.py
--rw-r--r--   0 runner    (1001) docker     (116)     5007 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/progress.py
--rw-r--r--   0 runner    (1001) docker     (116)     1257 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc/render/
--rw-r--r--   0 runner    (1001) docker     (116)      107 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1720 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/render/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     5803 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/render/data.py
--rw-r--r--   0 runner    (1001) docker     (116)     3207 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/render/html.py
--rw-r--r--   0 runner    (1001) docker     (116)     3073 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/render/image.py
--rw-r--r--   0 runner    (1001) docker     (116)     3010 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/render/plotly.py
--rw-r--r--   0 runner    (1001) docker     (116)     2004 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/render/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     3187 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/render/vega.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/repo/
--rw-r--r--   0 runner    (1001) docker     (116)    15551 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8038 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/add.py
--rw-r--r--   0 runner    (1001) docker     (116)     1840 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/brancher.py
--rw-r--r--   0 runner    (1001) docker     (116)     2853 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/checkout.py
--rw-r--r--   0 runner    (1001) docker     (116)     2313 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/collect.py
--rw-r--r--   0 runner    (1001) docker     (116)     1860 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/commit.py
--rw-r--r--   0 runner    (1001) docker     (116)      519 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/destroy.py
--rw-r--r--   0 runner    (1001) docker     (116)     7102 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (116)    29474 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2541 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (116)     5082 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     1870 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1131 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (116)     1295 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/repo/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    21717 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/executor/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     5301 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/executor/local.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/repo/experiments/executor/manager/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/executor/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9094 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/executor/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     3433 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/executor/manager/local.py
--rw-r--r--   0 runner    (1001) docker     (116)     3335 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/executor/manager/ssh.py
--rw-r--r--   0 runner    (1001) docker     (116)     9213 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/executor/ssh.py
--rw-r--r--   0 runner    (1001) docker     (116)     1232 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/gc.py
--rw-r--r--   0 runner    (1001) docker     (116)     8555 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/init.py
--rw-r--r--   0 runner    (1001) docker     (116)     1276 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (116)     2256 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (116)     2234 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/push.py
--rw-r--r--   0 runner    (1001) docker     (116)     3074 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (116)      867 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (116)     6259 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (116)     6332 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/experiments/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     2489 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/fetch.py
--rw-r--r--   0 runner    (1001) docker     (116)      401 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/freeze.py
--rw-r--r--   0 runner    (1001) docker     (116)     2323 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/gc.py
--rw-r--r--   0 runner    (1001) docker     (116)     1918 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/get.py
--rw-r--r--   0 runner    (1001) docker     (116)      470 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/get_url.py
--rw-r--r--   0 runner    (1001) docker     (116)     4286 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/graph.py
--rw-r--r--   0 runner    (1001) docker     (116)      247 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/imp.py
--rw-r--r--   0 runner    (1001) docker     (116)     2068 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (116)     9796 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/index.py
--rw-r--r--   0 runner    (1001) docker     (116)     2554 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/init.py
--rw-r--r--   0 runner    (1001) docker     (116)     2349 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/install.py
--rw-r--r--   0 runner    (1001) docker     (116)     1557 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/live.py
--rw-r--r--   0 runner    (1001) docker     (116)     2462 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/ls.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/repo/metrics/
--rw-r--r--   0 runner    (1001) docker     (116)      322 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      562 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/metrics/diff.py
--rw-r--r--   0 runner    (1001) docker     (116)     3481 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/metrics/show.py
--rw-r--r--   0 runner    (1001) docker     (116)     2206 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/move.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/repo/params/
--rw-r--r--   0 runner    (1001) docker     (116)      305 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      559 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/params/diff.py
--rw-r--r--   0 runner    (1001) docker     (116)     4301 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/params/show.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (116)     8754 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      580 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/plots/diff.py
--rw-r--r--   0 runner    (1001) docker     (116)    20092 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/plots/template.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/repo/plots/templates/
--rw-r--r--   0 runner    (1001) docker     (116)     3000 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/plots/templates/confusion.json
--rw-r--r--   0 runner    (1001) docker     (116)     3145 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/plots/templates/confusion_normalized.json
--rw-r--r--   0 runner    (1001) docker     (116)     3655 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/plots/templates/linear.json
--rw-r--r--   0 runner    (1001) docker     (116)     3266 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/plots/templates/scatter.json
--rw-r--r--   0 runner    (1001) docker     (116)      714 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/plots/templates/simple.json
--rw-r--r--   0 runner    (1001) docker     (116)      889 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/plots/templates/smooth.json
--rw-r--r--   0 runner    (1001) docker     (116)     1144 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/pull.py
--rw-r--r--   0 runner    (1001) docker     (116)     1889 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/push.py
--rw-r--r--   0 runner    (1001) docker     (116)      354 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/remove.py
--rw-r--r--   0 runner    (1001) docker     (116)     8369 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/reproduce.py
--rw-r--r--   0 runner    (1001) docker     (116)      758 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/run.py
--rw-r--r--   0 runner    (1001) docker     (116)     4619 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/scm_context.py
--rw-r--r--   0 runner    (1001) docker     (116)    16732 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/stage.py
--rw-r--r--   0 runner    (1001) docker     (116)     3574 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/status.py
--rw-r--r--   0 runner    (1001) docker     (116)     1456 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/trie.py
--rw-r--r--   0 runner    (1001) docker     (116)      830 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/repo/update.py
--rw-r--r--   0 runner    (1001) docker     (116)     4796 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/rwlock.py
--rw-r--r--   0 runner    (1001) docker     (116)     4049 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/schema.py
--rw-r--r--   0 runner    (1001) docker     (116)      285 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/scheme.py
--rw-r--r--   0 runner    (1001) docker     (116)     5175 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/scm.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/stage/
--rw-r--r--   0 runner    (1001) docker     (116)    21857 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8387 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/stage/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)     1516 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/stage/decorators.py
--rw-r--r--   0 runner    (1001) docker     (116)     2650 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/stage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1293 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/stage/imports.py
--rw-r--r--   0 runner    (1001) docker     (116)     6851 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/stage/loader.py
--rw-r--r--   0 runner    (1001) docker     (116)     4362 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/stage/monitor.py
--rw-r--r--   0 runner    (1001) docker     (116)      417 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/stage/params.py
--rw-r--r--   0 runner    (1001) docker     (116)     4798 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/stage/run.py
--rw-r--r--   0 runner    (1001) docker     (116)     6522 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/stage/serialize.py
--rw-r--r--   0 runner    (1001) docker     (116)     9456 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/stage/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     5033 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/state.py
--rw-r--r--   0 runner    (1001) docker     (116)     3816 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/system.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/testing/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2017 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/testing/cloud.py
--rw-r--r--   0 runner    (1001) docker     (116)       65 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     6049 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (116)    10002 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/testing/path_info.py
--rw-r--r--   0 runner    (1001) docker     (116)      554 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/testing/test_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     2945 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/testing/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (116)     4166 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/testing/test_workspace.py
--rw-r--r--   0 runner    (1001) docker     (116)     8595 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/testing/tmp_dir.py
--rw-r--r--   0 runner    (1001) docker     (116)      295 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/types.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/ui/
--rw-r--r--   0 runner    (1001) docker     (116)     8269 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2414 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/ui/pager.py
--rw-r--r--   0 runner    (1001) docker     (116)     5577 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/ui/prompt.py
--rw-r--r--   0 runner    (1001) docker     (116)     3200 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/ui/table.py
--rw-r--r--   0 runner    (1001) docker     (116)     5458 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/utils/
--rw-r--r--   0 runner    (1001) docker     (116)       10 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)    14335 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      844 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/_benedict.py
--rw-r--r--   0 runner    (1001) docker     (116)       12 2022-02-16 10:58:24.000000 dvc-2.9.4/dvc/utils/build.py
--rw-r--r--   0 runner    (1001) docker     (116)     1804 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (116)     5267 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (116)      613 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/conversions.py
--rw-r--r--   0 runner    (1001) docker     (116)      813 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (116)     2384 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/diff.py
--rw-r--r--   0 runner    (1001) docker     (116)      189 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/flatten.py
--rw-r--r--   0 runner    (1001) docker     (116)     6839 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (116)      787 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (116)      172 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/pkg.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/dvc/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (116)     1042 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2310 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/serialize/_common.py
--rw-r--r--   0 runner    (1001) docker     (116)      895 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/serialize/_json.py
--rw-r--r--   0 runner    (1001) docker     (116)     5235 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/serialize/_py.py
--rw-r--r--   0 runner    (1001) docker     (116)     1344 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/serialize/_toml.py
--rw-r--r--   0 runner    (1001) docker     (116)     1922 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/serialize/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (116)     1148 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/stream.py
--rw-r--r--   0 runner    (1001) docker     (116)     9295 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (116)     2824 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/table.py
--rw-r--r--   0 runner    (1001) docker     (116)     1046 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/utils/threadpool.py
--rw-r--r--   0 runner    (1001) docker     (116)      196 2022-02-16 10:56:58.000000 dvc-2.9.4/dvc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    13942 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    15393 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       37 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-16 10:57:46.000000 dvc-2.9.4/dvc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)     3019 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2022-02-16 10:58:36.000000 dvc-2.9.4/dvc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-02-16 10:56:58.000000 dvc-2.9.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/build-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2912 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/build.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      257 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/build_package.sh
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/scripts/fpm/
--rw-r--r--   0 runner    (1001) docker     (116)       28 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/fpm/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)       59 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/fpm/after-install.sh
--rw-r--r--   0 runner    (1001) docker     (116)       36 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/fpm/after-remove.sh
--rw-r--r--   0 runner    (1001) docker     (116)     2260 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/fpm/build.py
--rw-r--r--   0 runner    (1001) docker     (116)     1403 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/fpm/notarize.py
--rw-r--r--   0 runner    (1001) docker     (116)     1087 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/fpm/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/scripts/innosetup/
--rw-r--r--   0 runner    (1001) docker     (116)       64 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/innosetup/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     2686 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/innosetup/addSymLinkPermissions.ps1
--rw-r--r--   0 runner    (1001) docker     (116)     1153 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/innosetup/addsymlink.iss
--rw-r--r--   0 runner    (1001) docker     (116)      934 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/innosetup/build.py
--rw-r--r--   0 runner    (1001) docker     (116)       62 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/innosetup/dvc.ico.dvc
--rw-r--r--   0 runner    (1001) docker     (116)       67 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/innosetup/dvc_left.bmp.dvc
--rw-r--r--   0 runner    (1001) docker     (116)       65 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/innosetup/dvc_up.bmp.dvc
--rw-r--r--   0 runner    (1001) docker     (116)     6681 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/innosetup/modpath.iss
--rw-r--r--   0 runner    (1001) docker     (116)     2324 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/innosetup/setup.iss
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/scripts/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (116)       28 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/pyinstaller/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      521 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/pyinstaller/build.py
--rw-r--r--   0 runner    (1001) docker     (116)      380 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/pyinstaller/entitlements.plist
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/scripts/pyinstaller/hooks/
--rw-r--r--   0 runner    (1001) docker     (116)      662 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/pyinstaller/hooks/hook-dvc.py
--rw-r--r--   0 runner    (1001) docker     (116)       65 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/pyinstaller/hooks/hook-dvc.system.py
--rw-r--r--   0 runner    (1001) docker     (116)      353 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
--rw-r--r--   0 runner    (1001) docker     (116)      129 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
--rw-r--r--   0 runner    (1001) docker     (116)      178 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/pyinstaller/hooks/hook-google_compute_engine.logger.py
--rw-r--r--   0 runner    (1001) docker     (116)      292 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/pyinstaller/hooks/hook-googleapiclient.model.py
--rw-r--r--   0 runner    (1001) docker     (116)      176 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/pyinstaller/hooks/hook-pydrive2.py
--rw-r--r--   0 runner    (1001) docker     (116)      958 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/pyinstaller/sign.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      257 2022-02-16 10:56:58.000000 dvc-2.9.4/scripts/pypi_upload.sh
--rw-r--r--   0 runner    (1001) docker     (116)     3653 2022-02-16 10:58:37.000000 dvc-2.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-02-16 10:56:58.000000 dvc-2.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     1450 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      584 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5364 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/basic_env.py
--rw-r--r--   0 runner    (1001) docker     (116)     6448 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     4678 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/dir_helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)      293 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/func/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      840 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/func/experiments/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2653 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/func/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5067 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/experiments/executor/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (116)     9169 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/experiments/test_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (116)      999 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/experiments/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (116)    23097 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/experiments/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (116)     4095 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/experiments/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (116)    13000 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/experiments/test_init.py
--rw-r--r--   0 runner    (1001) docker     (116)    11362 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/experiments/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (116)     4502 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (116)    22212 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/experiments/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/func/machine/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1324 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/machine/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     5373 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/machine/test_machine_config.py
--rw-r--r--   0 runner    (1001) docker     (116)      800 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/machine/test_machine_status.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/func/metrics/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5660 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/metrics/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (116)     8383 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/metrics/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/func/objects/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/func/objects/db/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/objects/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2770 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/objects/db/test_index.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/func/params/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6491 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/params/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (116)     4907 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/params/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/func/parsing/
--rw-r--r--   0 runner    (1001) docker     (116)     1469 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9617 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/parsing/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (116)    15175 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/parsing/test_foreach.py
--rw-r--r--   0 runner    (1001) docker     (116)     7713 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/parsing/test_interpolated_entry.py
--rw-r--r--   0 runner    (1001) docker     (116)     6132 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/parsing/test_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/func/plots/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1441 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (116)     2855 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/plots/test_modify.py
--rw-r--r--   0 runner    (1001) docker     (116)     8855 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/plots/test_show.py
--rw-r--r--   0 runner    (1001) docker     (116)    34281 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_add.py
--rw-r--r--   0 runner    (1001) docker     (116)     1724 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (116)     6432 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     4317 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (116)    30043 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (116)     6429 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     6230 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (116)    10046 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    15142 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_data_cloud.py
--rw-r--r--   0 runner    (1001) docker     (116)    17519 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (116)    10871 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (116)     7878 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_external_repo.py
--rw-r--r--   0 runner    (1001) docker     (116)    10858 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (116)    12435 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (116)    10591 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_get.py
--rw-r--r--   0 runner    (1001) docker     (116)     1126 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (116)    13381 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (116)    19313 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_import.py
--rw-r--r--   0 runner    (1001) docker     (116)     7698 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (116)     3209 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_init.py
--rw-r--r--   0 runner    (1001) docker     (116)     5582 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_install.py
--rw-r--r--   0 runner    (1001) docker     (116)     8753 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_live.py
--rw-r--r--   0 runner    (1001) docker     (116)      913 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (116)     7079 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (116)    17664 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (116)     5133 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_merge_driver.py
--rw-r--r--   0 runner    (1001) docker     (116)     8297 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_move.py
--rw-r--r--   0 runner    (1001) docker     (116)     6428 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_odb.py
--rw-r--r--   0 runner    (1001) docker     (116)    15556 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (116)     3178 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (116)     1289 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (116)     8788 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_repo_index.py
--rw-r--r--   0 runner    (1001) docker     (116)    37964 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (116)    14978 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_repro_multistage.py
--rw-r--r--   0 runner    (1001) docker     (116)      340 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_root.py
--rw-r--r--   0 runner    (1001) docker     (116)     5766 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_run_cache.py
--rw-r--r--   0 runner    (1001) docker     (116)    11561 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_run_multistage.py
--rw-r--r--   0 runner    (1001) docker     (116)    30285 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_run_single_stage.py
--rw-r--r--   0 runner    (1001) docker     (116)      602 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (116)     1839 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_scm_context.py
--rw-r--r--   0 runner    (1001) docker     (116)     9641 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (116)    15585 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_stage_load.py
--rw-r--r--   0 runner    (1001) docker     (116)     2352 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_state.py
--rw-r--r--   0 runner    (1001) docker     (116)     3941 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_status.py
--rw-r--r--   0 runner    (1001) docker     (116)     1196 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_unprotect.py
--rw-r--r--   0 runner    (1001) docker     (116)    11945 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_update.py
--rw-r--r--   0 runner    (1001) docker     (116)     1139 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      599 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/func/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      896 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/utils/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (116)     9083 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/func/utils/test_strict_yaml.py
--rw-r--r--   0 runner    (1001) docker     (116)     1412 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/pylint_plugin_disable.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/remotes/
--rw-r--r--   0 runner    (1001) docker     (116)      316 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/remotes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/remotes/git-init/
--rw-r--r--   0 runner    (1001) docker     (116)       35 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/remotes/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (116)     1430 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/remotes/git_server.py
--rw-r--r--   0 runner    (1001) docker     (116)     1679 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/remotes/user.key
--rw-r--r--   0 runner    (1001) docker     (116)      394 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/remotes/user.key.pub
--rw-r--r--   0 runner    (1001) docker     (116)      924 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/remotes_env.sample
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/command/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/command/ls/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3171 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/ls/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (116)     2134 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/ls/test_ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (116)     2781 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_add.py
--rw-r--r--   0 runner    (1001) docker     (116)      674 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (116)     1255 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (116)     1400 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_compat_flag.py
--rw-r--r--   0 runner    (1001) docker     (116)      889 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_config.py
--rw-r--r--   0 runner    (1001) docker     (116)     4542 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (116)     2741 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_data_sync.py
--rw-r--r--   0 runner    (1001) docker     (116)      604 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (116)    11023 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (116)    24047 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (116)     1011 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_get.py
--rw-r--r--   0 runner    (1001) docker     (116)      369 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (116)      563 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_git_hook.py
--rw-r--r--   0 runner    (1001) docker     (116)     1484 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_imp.py
--rw-r--r--   0 runner    (1001) docker     (116)     3590 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_imp_url.py
--rw-r--r--   0 runner    (1001) docker     (116)      961 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_live.py
--rw-r--r--   0 runner    (1001) docker     (116)     4928 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_machine.py
--rw-r--r--   0 runner    (1001) docker     (116)     4240 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     2045 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_params.py
--rw-r--r--   0 runner    (1001) docker     (116)    10158 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (116)      988 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (116)     4230 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_run.py
--rw-r--r--   0 runner    (1001) docker     (116)     2523 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (116)     3180 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_status.py
--rw-r--r--   0 runner    (1001) docker     (116)     1276 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/command/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      320 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/dependency/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (116)     6223 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/dependency/test_params.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/fs/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2600 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/fs/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (116)      506 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/fs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (116)     7481 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/fs/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (116)     1203 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/fs/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (116)      481 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/fs/test_hdfs.py
--rw-r--r--   0 runner    (1001) docker     (116)      733 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/fs/test_path.py
--rw-r--r--   0 runner    (1001) docker     (116)    21724 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/fs/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (116)     4281 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/fs/test_repo_info.py
--rw-r--r--   0 runner    (1001) docker     (116)     3922 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/fs/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (116)     4643 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/fs/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (116)     1401 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/fs/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/machine/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1096 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/machine/test_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/objects/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/objects/db/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/objects/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3952 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/objects/db/test_local.py
--rw-r--r--   0 runner    (1001) docker     (116)     6260 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/objects/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/output/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3898 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/output/test_load.py
--rw-r--r--   0 runner    (1001) docker     (116)     2122 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/output/test_local.py
--rw-r--r--   0 runner    (1001) docker     (116)     3345 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/output/test_output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/proc/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3691 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/proc/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (116)     1466 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/proc/test_process.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/remote/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3619 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/remote/test_base.py
--rw-r--r--   0 runner    (1001) docker     (116)     1940 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/remote/test_gdrive.py
--rw-r--r--   0 runner    (1001) docker     (116)     2109 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/remote/test_http.py
--rw-r--r--   0 runner    (1001) docker     (116)     1210 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/remote/test_index.py
--rw-r--r--   0 runner    (1001) docker     (116)      576 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/remote/test_oss.py
--rw-r--r--   0 runner    (1001) docker     (116)     2103 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/remote/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (116)     1324 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/remote/test_slow_link_detection.py
--rw-r--r--   0 runner    (1001) docker     (116)     3323 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/remote/test_webdav.py
--rw-r--r--   0 runner    (1001) docker     (116)     1621 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/remote/test_webhdfs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/render/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4552 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/render/test_data.py
--rw-r--r--   0 runner    (1001) docker     (116)     1095 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/render/test_html.py
--rw-r--r--   0 runner    (1001) docker     (116)     2061 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/render/test_image.py
--rw-r--r--   0 runner    (1001) docker     (116)     4234 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/render/test_parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (116)     2570 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/render/test_render.py
--rw-r--r--   0 runner    (1001) docker     (116)      275 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/render/test_renderer.py
--rw-r--r--   0 runner    (1001) docker     (116)    10726 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/render/test_vega.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/repo/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1547 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/repo/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1456 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/repo/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (116)     2229 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/repo/plots/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (116)     3700 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/repo/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (116)      714 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/repo/test_reproduce.py
--rw-r--r--   0 runner    (1001) docker     (116)      335 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/repo/test_run.py
--rw-r--r--   0 runner    (1001) docker     (116)     4410 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/repo/test_scm_context.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/scm/
--rw-r--r--   0 runner    (1001) docker     (116)     1814 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/scm/test_scm.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/stage/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6829 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/stage/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (116)     8582 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/stage/test_loader_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (116)      574 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/stage/test_run.py
--rw-r--r--   0 runner    (1001) docker     (116)     5588 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/stage/test_serialize_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (116)     7211 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/stage/test_serialize_pipeline_lock.py
--rw-r--r--   0 runner    (1001) docker     (116)     4373 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/stage/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (116)      624 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/stage/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     4309 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (116)      307 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (116)    14096 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (116)     1914 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    12487 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_context.py
--rw-r--r--   0 runner    (1001) docker     (116)     1025 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (116)     4012 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (116)     2871 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_external_repo.py
--rw-r--r--   0 runner    (1001) docker     (116)     8856 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (116)      520 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (116)     4299 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_info.py
--rw-r--r--   0 runner    (1001) docker     (116)     3061 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (116)     3427 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (116)     9107 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (116)      819 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     1240 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_params.py
--rw-r--r--   0 runner    (1001) docker     (116)     3747 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (116)      896 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (116)     1418 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (116)      339 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (116)      354 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_run.py
--rw-r--r--   0 runner    (1001) docker     (116)     2553 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_rwlock.py
--rw-r--r--   0 runner    (1001) docker     (116)    10239 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_tabular_data.py
--rw-r--r--   0 runner    (1001) docker     (116)     5319 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/ui/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1714 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/ui/test_console.py
--rw-r--r--   0 runner    (1001) docker     (116)     2747 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/ui/test_pager.py
--rw-r--r--   0 runner    (1001) docker     (116)     4514 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/ui/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (116)     4624 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/ui/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/unit/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1221 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/utils/serialize/test_python.py
--rw-r--r--   0 runner    (1001) docker     (116)      629 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/utils/serialize/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (116)      513 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/utils/test_cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (116)     5888 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/utils/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (116)      728 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/utils/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1358 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/utils/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (116)     7261 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/utils/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (116)     2090 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/utils/test_humanize.py
--rw-r--r--   0 runner    (1001) docker     (116)     2203 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/utils/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (116)     6723 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/unit/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-16 10:58:37.000000 dvc-2.9.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (116)     1913 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      524 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (116)      749 2022-02-16 10:56:58.000000 dvc-2.9.4/tests/utils/scriptify.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/
+-rw-r--r--   0 runner    (1001) docker     (116)      154 2022-02-21 02:25:05.000000 dvc-2.9.5/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      263 2022-02-21 02:25:05.000000 dvc-2.9.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/.dvc/
+-rw-r--r--   0 runner    (1001) docker     (116)      113 2022-02-21 02:25:05.000000 dvc-2.9.5/.dvc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)       70 2022-02-21 02:25:05.000000 dvc-2.9.5/.dvc/config
+-rw-r--r--   0 runner    (1001) docker     (116)       23 2022-02-21 02:25:05.000000 dvc-2.9.5/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       32 2022-02-21 02:25:05.000000 dvc-2.9.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (116)       23 2022-02-21 02:25:05.000000 dvc-2.9.5/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (116)       63 2022-02-21 02:25:05.000000 dvc-2.9.5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (116)     1296 2022-02-21 02:25:05.000000 dvc-2.9.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (116)      189 2022-02-21 02:25:05.000000 dvc-2.9.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       84 2022-02-21 02:25:05.000000 dvc-2.9.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (116)      395 2022-02-21 02:25:05.000000 dvc-2.9.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (116)      273 2022-02-21 02:25:05.000000 dvc-2.9.5/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      183 2022-02-21 02:25:05.000000 dvc-2.9.5/.github/mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1020 2022-02-21 02:25:05.000000 dvc-2.9.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)      554 2022-02-21 02:25:05.000000 dvc-2.9.5/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     4786 2022-02-21 02:25:05.000000 dvc-2.9.5/.github/workflows/packages.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     2533 2022-02-21 02:25:05.000000 dvc-2.9.5/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      359 2022-02-21 02:25:05.000000 dvc-2.9.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      238 2022-02-21 02:25:05.000000 dvc-2.9.5/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (116)     2110 2022-02-21 02:25:05.000000 dvc-2.9.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      631 2022-02-21 02:25:05.000000 dvc-2.9.5/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      322 2022-02-21 02:25:05.000000 dvc-2.9.5/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (116)     3348 2022-02-21 02:25:05.000000 dvc-2.9.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (116)       95 2022-02-21 02:25:05.000000 dvc-2.9.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (116)    11350 2022-02-21 02:25:05.000000 dvc-2.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2022-02-21 02:25:05.000000 dvc-2.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    13942 2022-02-21 02:27:12.000000 dvc-2.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    12661 2022-02-21 02:25:05.000000 dvc-2.9.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (116)       51 2022-02-21 02:25:05.000000 dvc-2.9.5/bin/dvc
+-rw-r--r--   0 runner    (1001) docker     (116)       53 2022-02-21 02:25:05.000000 dvc-2.9.5/bin/dvc.bat
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/
+-rw-r--r--   0 runner    (1001) docker     (116)      165 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      148 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4365 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (116)      142 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/_dvc_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5091 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4122 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/api.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/cli/
+-rw-r--r--   0 runner    (1001) docker     (116)     3649 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      697 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4943 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (116)      954 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/commands/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3453 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2554 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3708 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3029 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2211 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3031 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/completion.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7055 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2078 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3663 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11637 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1514 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6419 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/commands/experiments/
+-rw-r--r--   0 runner    (1001) docker     (116)     1200 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1221 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1006 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3754 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1112 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/exec_run.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3996 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/gc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5656 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/init.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2352 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2787 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2869 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/push.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1593 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4331 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19727 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1780 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4501 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/gc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2753 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/get.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1451 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4469 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2792 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/imp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3269 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2928 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1083 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2776 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/live.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (116)     2491 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1348 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/ls/ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17045 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/machine.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7508 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1392 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/move.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3667 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/params.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11089 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/plots.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9583 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/remote.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1278 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4962 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/repro.py
+-rw-r--r--   0 runner    (1001) docker     (116)      762 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/root.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3005 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10436 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/stage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2787 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1214 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2218 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (116)      908 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13694 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/compare.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9721 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9040 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3003 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7955 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/dagascii.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/data/
+-rw-r--r--   0 runner    (1001) docker     (116)      814 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6366 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/checkout.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/data/db/
+-rw-r--r--   0 runner    (1001) docker     (116)     2365 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3750 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/db/index.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5481 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/db/local.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2750 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/db/reference.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3254 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1255 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/gc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1224 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/meta.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3796 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/reference.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1171 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/slow_link_detection.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10372 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/stage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6138 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/status.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5455 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7551 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data/tree.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4932 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/data_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/dependency/
+-rw-r--r--   0 runner    (1001) docker     (116)     2264 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      944 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5015 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/dependency/param.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6830 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/dependency/repo.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12662 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (116)      396 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/env.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9844 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8290 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/external_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/fs/
+-rw-r--r--   0 runner    (1001) docker     (116)     3927 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1277 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/_callback.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5712 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/azure.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10916 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6083 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7857 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/fsspec_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9731 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1275 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/git.py
+-rw-r--r--   0 runner    (1001) docker     (116)      720 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/gs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2882 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/hdfs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4581 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/http.py
+-rw-r--r--   0 runner    (1001) docker     (116)      167 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/https.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5037 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/local.py
+-rw-r--r--   0 runner    (1001) docker     (116)      901 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/memory.py
+-rw-r--r--   0 runner    (1001) docker     (116)      985 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/oss.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2408 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/path.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1354 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/pool.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15947 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/repo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7785 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/s3.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4364 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4547 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3116 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/webdav.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1575 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/fs/webhdfs.py
+-rw-r--r--   0 runner    (1001) docker     (116)      923 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/hash_info.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13236 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4145 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/info.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1134 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5016 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/lock.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8845 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/machine/
+-rw-r--r--   0 runner    (1001) docker     (116)     6738 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/machine/backend/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/machine/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1611 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/machine/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3288 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/machine/backend/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (116)      122 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/objects/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16475 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/objects/db.py
+-rw-r--r--   0 runner    (1001) docker     (116)      236 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/objects/errors.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2186 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/objects/file.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30231 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/parsing/
+-rw-r--r--   0 runner    (1001) docker     (116)    15258 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16710 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/parsing/context.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4451 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/parsing/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1158 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/parsing/versions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2598 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/pathspec_math.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/proc/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      705 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/proc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4964 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/proc/manager.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5057 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/proc/process.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5007 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/progress.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1257 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/render/
+-rw-r--r--   0 runner    (1001) docker     (116)      107 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1720 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/render/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5803 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/render/data.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3207 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/render/html.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3073 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/render/image.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3010 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/render/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2004 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/render/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3187 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/render/vega.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/repo/
+-rw-r--r--   0 runner    (1001) docker     (116)    15551 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8038 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/add.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1840 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2853 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2313 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/collect.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1860 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/commit.py
+-rw-r--r--   0 runner    (1001) docker     (116)      519 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7102 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (116)    29474 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2541 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5082 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1870 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1131 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1295 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/repo/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21717 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/executor/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5301 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/executor/local.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/repo/experiments/executor/manager/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/executor/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9094 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/executor/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3433 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/executor/manager/local.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3335 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/executor/manager/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9213 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/executor/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1232 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/gc.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10101 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/init.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1276 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2256 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2234 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/push.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3074 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (116)      867 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6259 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6332 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/experiments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2489 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (116)      401 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2334 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/gc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1918 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/get.py
+-rw-r--r--   0 runner    (1001) docker     (116)      470 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4286 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (116)      247 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/imp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2068 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9796 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/index.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2554 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/init.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2349 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/install.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1557 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/live.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2316 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/ls.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/repo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (116)      322 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      562 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/metrics/diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3481 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/metrics/show.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2206 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/move.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/repo/params/
+-rw-r--r--   0 runner    (1001) docker     (116)      305 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      559 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/params/diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4301 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/params/show.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (116)     8754 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      580 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/plots/diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20092 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/plots/template.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/repo/plots/templates/
+-rw-r--r--   0 runner    (1001) docker     (116)     3000 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/plots/templates/confusion.json
+-rw-r--r--   0 runner    (1001) docker     (116)     3145 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/plots/templates/confusion_normalized.json
+-rw-r--r--   0 runner    (1001) docker     (116)     3655 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/plots/templates/linear.json
+-rw-r--r--   0 runner    (1001) docker     (116)     3266 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/plots/templates/scatter.json
+-rw-r--r--   0 runner    (1001) docker     (116)      714 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/plots/templates/simple.json
+-rw-r--r--   0 runner    (1001) docker     (116)      889 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/plots/templates/smooth.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1144 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/pull.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1889 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/push.py
+-rw-r--r--   0 runner    (1001) docker     (116)      354 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/remove.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8369 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (116)      758 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/run.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4619 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16732 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/stage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3574 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/status.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1456 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/trie.py
+-rw-r--r--   0 runner    (1001) docker     (116)      830 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/repo/update.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4796 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4049 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/schema.py
+-rw-r--r--   0 runner    (1001) docker     (116)      285 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5175 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/scm.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/stage/
+-rw-r--r--   0 runner    (1001) docker     (116)    21857 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8387 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/stage/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1516 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/stage/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2650 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/stage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1293 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/stage/imports.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6851 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/stage/loader.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4362 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/stage/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (116)      417 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/stage/params.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4798 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/stage/run.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6522 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/stage/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9456 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/stage/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5033 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/state.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3816 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/system.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/testing/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2017 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/testing/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (116)       65 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6049 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10002 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/testing/path_info.py
+-rw-r--r--   0 runner    (1001) docker     (116)      554 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/testing/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2945 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/testing/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4166 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/testing/test_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8595 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/testing/tmp_dir.py
+-rw-r--r--   0 runner    (1001) docker     (116)      295 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/types.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/ui/
+-rw-r--r--   0 runner    (1001) docker     (116)     8269 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2414 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/ui/pager.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5577 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/ui/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3200 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/ui/table.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5458 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)       10 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)    14335 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      844 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/_benedict.py
+-rw-r--r--   0 runner    (1001) docker     (116)       12 2022-02-21 02:27:00.000000 dvc-2.9.5/dvc/utils/build.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1804 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5267 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (116)      613 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (116)      813 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2384 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)      189 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6839 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (116)      787 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (116)      172 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/pkg.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (116)     1042 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2310 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/serialize/_common.py
+-rw-r--r--   0 runner    (1001) docker     (116)      895 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/serialize/_json.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5235 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/serialize/_py.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1344 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/serialize/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1922 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/serialize/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1148 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/stream.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9295 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2824 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/table.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1046 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/utils/threadpool.py
+-rw-r--r--   0 runner    (1001) docker     (116)      196 2022-02-21 02:25:05.000000 dvc-2.9.5/dvc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    13942 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    15393 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       37 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-21 02:26:22.000000 dvc-2.9.5/dvc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)     3019 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        4 2022-02-21 02:27:12.000000 dvc-2.9.5/dvc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-02-21 02:25:05.000000 dvc-2.9.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (116)       17 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/build-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     2912 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/build.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      257 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/build_package.sh
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/scripts/fpm/
+-rw-r--r--   0 runner    (1001) docker     (116)       28 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/fpm/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/fpm/after-install.sh
+-rw-r--r--   0 runner    (1001) docker     (116)       36 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/fpm/after-remove.sh
+-rw-r--r--   0 runner    (1001) docker     (116)     2260 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/fpm/build.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1403 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/fpm/notarize.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1087 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/fpm/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/scripts/innosetup/
+-rw-r--r--   0 runner    (1001) docker     (116)       64 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/innosetup/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)     2686 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/innosetup/addSymLinkPermissions.ps1
+-rw-r--r--   0 runner    (1001) docker     (116)     1153 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/innosetup/addsymlink.iss
+-rw-r--r--   0 runner    (1001) docker     (116)      934 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/innosetup/build.py
+-rw-r--r--   0 runner    (1001) docker     (116)       62 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/innosetup/dvc.ico.dvc
+-rw-r--r--   0 runner    (1001) docker     (116)       67 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/innosetup/dvc_left.bmp.dvc
+-rw-r--r--   0 runner    (1001) docker     (116)       65 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/innosetup/dvc_up.bmp.dvc
+-rw-r--r--   0 runner    (1001) docker     (116)     6681 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/innosetup/modpath.iss
+-rw-r--r--   0 runner    (1001) docker     (116)     2324 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/innosetup/setup.iss
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/scripts/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (116)       28 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/pyinstaller/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      521 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/pyinstaller/build.py
+-rw-r--r--   0 runner    (1001) docker     (116)      380 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/pyinstaller/entitlements.plist
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/scripts/pyinstaller/hooks/
+-rw-r--r--   0 runner    (1001) docker     (116)      662 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/pyinstaller/hooks/hook-dvc.py
+-rw-r--r--   0 runner    (1001) docker     (116)       65 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/pyinstaller/hooks/hook-dvc.system.py
+-rw-r--r--   0 runner    (1001) docker     (116)      353 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
+-rw-r--r--   0 runner    (1001) docker     (116)      129 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
+-rw-r--r--   0 runner    (1001) docker     (116)      178 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/pyinstaller/hooks/hook-google_compute_engine.logger.py
+-rw-r--r--   0 runner    (1001) docker     (116)      292 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/pyinstaller/hooks/hook-googleapiclient.model.py
+-rw-r--r--   0 runner    (1001) docker     (116)      176 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/pyinstaller/hooks/hook-pydrive2.py
+-rw-r--r--   0 runner    (1001) docker     (116)      958 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/pyinstaller/sign.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      257 2022-02-21 02:25:05.000000 dvc-2.9.5/scripts/pypi_upload.sh
+-rw-r--r--   0 runner    (1001) docker     (116)     3653 2022-02-21 02:27:12.000000 dvc-2.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-02-21 02:25:05.000000 dvc-2.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)     1450 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      584 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5364 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/basic_env.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6448 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4678 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/dir_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)      293 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      840 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/func/experiments/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2653 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/func/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5067 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/experiments/executor/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9169 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/experiments/test_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (116)      999 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/experiments/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23097 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/experiments/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4095 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/experiments/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13936 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/experiments/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11362 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/experiments/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4502 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22212 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/experiments/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/func/machine/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1324 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/machine/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5373 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/machine/test_machine_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)      800 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/machine/test_machine_status.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/func/metrics/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5660 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/metrics/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8383 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/metrics/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/func/objects/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/func/objects/db/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/objects/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2770 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/objects/db/test_index.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/func/params/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6491 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/params/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4907 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/params/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/func/parsing/
+-rw-r--r--   0 runner    (1001) docker     (116)     1469 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9617 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/parsing/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15175 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/parsing/test_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7713 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/parsing/test_interpolated_entry.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6132 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/parsing/test_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/func/plots/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1441 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2855 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/plots/test_modify.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8855 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/plots/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (116)    34281 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1724 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6432 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4317 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30043 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6429 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6230 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10046 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16383 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_data_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17519 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10871 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7878 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_external_repo.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10858 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12435 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10591 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1126 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13381 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19313 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7698 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3209 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5582 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8753 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_live.py
+-rw-r--r--   0 runner    (1001) docker     (116)      913 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7079 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17664 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5133 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_merge_driver.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8297 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_move.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6428 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_odb.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15556 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3178 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1289 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8788 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_repo_index.py
+-rw-r--r--   0 runner    (1001) docker     (116)    37964 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14978 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_repro_multistage.py
+-rw-r--r--   0 runner    (1001) docker     (116)      340 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_root.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5766 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_run_cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11561 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_run_multistage.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30285 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_run_single_stage.py
+-rw-r--r--   0 runner    (1001) docker     (116)      602 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1839 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9641 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15585 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_stage_load.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2352 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3941 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1196 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11945 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1139 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      599 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/func/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      896 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/utils/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9083 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/func/utils/test_strict_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1412 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/pylint_plugin_disable.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/remotes/
+-rw-r--r--   0 runner    (1001) docker     (116)      316 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/remotes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/remotes/git-init/
+-rw-r--r--   0 runner    (1001) docker     (116)       35 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/remotes/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (116)     1430 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/remotes/git_server.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1679 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/remotes/user.key
+-rw-r--r--   0 runner    (1001) docker     (116)      394 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/remotes/user.key.pub
+-rw-r--r--   0 runner    (1001) docker     (116)      924 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/remotes_env.sample
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/command/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/command/ls/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3171 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/ls/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2134 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/ls/test_ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2781 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (116)      674 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1255 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1400 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_compat_flag.py
+-rw-r--r--   0 runner    (1001) docker     (116)      889 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4542 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2741 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (116)      604 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11023 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24047 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1011 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (116)      369 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (116)      563 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1484 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_imp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3590 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (116)      961 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_live.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4928 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4240 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2045 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10158 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (116)      988 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4230 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2523 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3180 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1276 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/command/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      320 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/dependency/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6223 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/dependency/test_params.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/fs/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2600 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/fs/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (116)      506 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/fs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7577 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/fs/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1203 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/fs/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (116)      481 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/fs/test_hdfs.py
+-rw-r--r--   0 runner    (1001) docker     (116)      733 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/fs/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21502 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/fs/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4281 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/fs/test_repo_info.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3922 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/fs/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4643 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/fs/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1401 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/fs/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/machine/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1096 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/machine/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/objects/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/objects/db/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/objects/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3952 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/objects/db/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6260 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/objects/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/output/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3898 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/output/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2122 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/output/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3345 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/output/test_output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/proc/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3691 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/proc/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1466 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/proc/test_process.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/remote/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3629 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/remote/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1940 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/remote/test_gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2109 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/remote/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1210 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/remote/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (116)      576 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/remote/test_oss.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2103 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/remote/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1324 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/remote/test_slow_link_detection.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3323 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/remote/test_webdav.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1621 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/remote/test_webhdfs.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/render/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4552 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/render/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1095 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/render/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2061 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/render/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4234 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/render/test_parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2570 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/render/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (116)      275 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/render/test_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10726 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/render/test_vega.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/repo/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1547 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/repo/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1456 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/repo/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2229 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/repo/plots/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3700 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/repo/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (116)      714 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/repo/test_reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (116)      335 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/repo/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4410 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/repo/test_scm_context.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/scm/
+-rw-r--r--   0 runner    (1001) docker     (116)     1814 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/scm/test_scm.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/stage/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6829 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/stage/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8582 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/stage/test_loader_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (116)      574 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/stage/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5588 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/stage/test_serialize_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7211 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/stage/test_serialize_pipeline_lock.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4373 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/stage/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (116)      624 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/stage/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4309 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (116)      307 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14096 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1914 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12487 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1025 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4012 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2871 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_external_repo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8856 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (116)      520 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4299 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3061 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3427 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9107 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (116)      819 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1240 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3747 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (116)      896 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1418 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (116)      339 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (116)      354 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2553 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10239 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_tabular_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5319 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/ui/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1714 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/ui/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2747 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/ui/test_pager.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4514 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/ui/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4624 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/ui/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/unit/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1221 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/utils/serialize/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (116)      629 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/utils/serialize/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (116)      513 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/utils/test_cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5888 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/utils/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (116)      728 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/utils/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1358 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/utils/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7261 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/utils/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2090 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/utils/test_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2203 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/utils/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6723 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/unit/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-21 02:27:12.000000 dvc-2.9.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)     1913 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      524 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (116)      749 2022-02-21 02:25:05.000000 dvc-2.9.5/tests/utils/scriptify.py
```

### Comparing `dvc-2.9.4/.github/ISSUE_TEMPLATE/bug_report.md` & `dvc-2.9.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/.github/release-drafter.yml` & `dvc-2.9.5/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/.github/workflows/benchmarks.yaml` & `dvc-2.9.5/.github/workflows/benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/.github/workflows/packages.yaml` & `dvc-2.9.5/.github/workflows/packages.yaml`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/.github/workflows/tests.yaml` & `dvc-2.9.5/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/.pre-commit-config.yaml` & `dvc-2.9.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/.pre-commit-hooks.yaml` & `dvc-2.9.5/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/CODE_OF_CONDUCT.md` & `dvc-2.9.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/LICENSE` & `dvc-2.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/PKG-INFO` & `dvc-2.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 2.9.4
+Version: 2.9.5
 Summary: Git for data scientists - manage your code and data together
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc
 Author: Dmitry Petrov
 Author-email: dmitry@dvc.org
 Maintainer: Iterative
 Maintainer-email: support@dvc.org
```

### Comparing `dvc-2.9.4/README.rst` & `dvc-2.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/_debug.py` & `dvc-2.9.5/dvc/_debug.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/analytics.py` & `dvc-2.9.5/dvc/analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/api.py` & `dvc-2.9.5/dvc/api.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/cli/__init__.py` & `dvc-2.9.5/dvc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/cli/command.py` & `dvc-2.9.5/dvc/cli/command.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/cli/parser.py` & `dvc-2.9.5/dvc/cli/parser.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/cli/utils.py` & `dvc-2.9.5/dvc/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/add.py` & `dvc-2.9.5/dvc/commands/add.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/cache.py` & `dvc-2.9.5/dvc/commands/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/check_ignore.py` & `dvc-2.9.5/dvc/commands/check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/checkout.py` & `dvc-2.9.5/dvc/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/commit.py` & `dvc-2.9.5/dvc/commands/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/completion.py` & `dvc-2.9.5/dvc/commands/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/config.py` & `dvc-2.9.5/dvc/commands/config.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/daemon.py` & `dvc-2.9.5/dvc/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/dag.py` & `dvc-2.9.5/dvc/commands/dag.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/data_sync.py` & `dvc-2.9.5/dvc/commands/data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/destroy.py` & `dvc-2.9.5/dvc/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/diff.py` & `dvc-2.9.5/dvc/commands/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/experiments/__init__.py` & `dvc-2.9.5/dvc/commands/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/experiments/apply.py` & `dvc-2.9.5/dvc/commands/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/experiments/branch.py` & `dvc-2.9.5/dvc/commands/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/experiments/diff.py` & `dvc-2.9.5/dvc/commands/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/experiments/exec_run.py` & `dvc-2.9.5/dvc/commands/experiments/exec_run.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/experiments/gc.py` & `dvc-2.9.5/dvc/commands/experiments/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/experiments/init.py` & `dvc-2.9.5/dvc/commands/experiments/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
             defaults=defaults,
             overrides=cli_args,
             interactive=self.args.interactive,
             force=self.args.force,
         )
 
         text = ui.rich_text.assemble(
-            "\n" if self.args.interactive else "",
             "Created ",
             (self.args.name, "bright_blue"),
             " stage in ",
             ("dvc.yaml", "green"),
             ".",
         )
         if not self.args.run:
```

### Comparing `dvc-2.9.4/dvc/commands/experiments/ls.py` & `dvc-2.9.5/dvc/commands/experiments/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/experiments/pull.py` & `dvc-2.9.5/dvc/commands/experiments/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/experiments/push.py` & `dvc-2.9.5/dvc/commands/experiments/push.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/experiments/remove.py` & `dvc-2.9.5/dvc/commands/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/experiments/run.py` & `dvc-2.9.5/dvc/commands/experiments/run.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/experiments/show.py` & `dvc-2.9.5/dvc/commands/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/freeze.py` & `dvc-2.9.5/dvc/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/gc.py` & `dvc-2.9.5/dvc/commands/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/get.py` & `dvc-2.9.5/dvc/commands/get.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/get_url.py` & `dvc-2.9.5/dvc/commands/get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/git_hook.py` & `dvc-2.9.5/dvc/commands/git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/imp.py` & `dvc-2.9.5/dvc/commands/imp.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/imp_url.py` & `dvc-2.9.5/dvc/commands/imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/init.py` & `dvc-2.9.5/dvc/commands/init.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/install.py` & `dvc-2.9.5/dvc/commands/install.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/live.py` & `dvc-2.9.5/dvc/commands/live.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/ls/__init__.py` & `dvc-2.9.5/dvc/commands/ls/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/ls/ls_colors.py` & `dvc-2.9.5/dvc/commands/ls/ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/machine.py` & `dvc-2.9.5/dvc/commands/machine.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/metrics.py` & `dvc-2.9.5/dvc/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/move.py` & `dvc-2.9.5/dvc/commands/move.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/params.py` & `dvc-2.9.5/dvc/commands/params.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/plots.py` & `dvc-2.9.5/dvc/commands/plots.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/remote.py` & `dvc-2.9.5/dvc/commands/remote.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/remove.py` & `dvc-2.9.5/dvc/commands/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/repro.py` & `dvc-2.9.5/dvc/commands/repro.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/root.py` & `dvc-2.9.5/dvc/commands/root.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/run.py` & `dvc-2.9.5/dvc/commands/run.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/stage.py` & `dvc-2.9.5/dvc/commands/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/status.py` & `dvc-2.9.5/dvc/commands/status.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/unprotect.py` & `dvc-2.9.5/dvc/commands/unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/update.py` & `dvc-2.9.5/dvc/commands/update.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/commands/version.py` & `dvc-2.9.5/dvc/commands/version.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/compare.py` & `dvc-2.9.5/dvc/compare.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/config.py` & `dvc-2.9.5/dvc/config.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/config_schema.py` & `dvc-2.9.5/dvc/config_schema.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/daemon.py` & `dvc-2.9.5/dvc/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/dagascii.py` & `dvc-2.9.5/dvc/dagascii.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/__init__.py` & `dvc-2.9.5/dvc/data/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/checkout.py` & `dvc-2.9.5/dvc/data/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/db/__init__.py` & `dvc-2.9.5/dvc/data/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/db/index.py` & `dvc-2.9.5/dvc/data/db/index.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/db/local.py` & `dvc-2.9.5/dvc/data/db/local.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/db/reference.py` & `dvc-2.9.5/dvc/data/db/reference.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/diff.py` & `dvc-2.9.5/dvc/data/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/gc.py` & `dvc-2.9.5/dvc/data/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/meta.py` & `dvc-2.9.5/dvc/data/meta.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/reference.py` & `dvc-2.9.5/dvc/data/reference.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/slow_link_detection.py` & `dvc-2.9.5/dvc/data/slow_link_detection.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/stage.py` & `dvc-2.9.5/dvc/data/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data/status.py` & `dvc-2.9.5/dvc/data/status.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,34 +23,34 @@
 class CompareStatusResult(NamedTuple):
     ok: Set["HashInfo"]
     missing: Set["HashInfo"]
     new: Set["HashInfo"]
     deleted: Set["HashInfo"]
 
 
-def _indexed_dir_hashes(odb, index, dir_objs, name, cache_odb):
+def _indexed_dir_hashes(odb, index, dir_objs, name, cache_odb, jobs=None):
     # Validate our index by verifying all indexed .dir hashes
     # still exist on the remote
     dir_hashes = set(dir_objs.keys())
     indexed_dirs = set(index.dir_hashes())
     indexed_dir_exists = set()
     if indexed_dirs:
-        indexed_dir_exists.update(odb.list_hashes_exists(indexed_dirs))
+        indexed_dir_exists.update(odb.list_hashes_exists(indexed_dirs, jobs))
         missing_dirs = indexed_dirs.difference(indexed_dir_exists)
         if missing_dirs:
             logger.debug(
                 "Remote cache missing indexed .dir hashes '%s', "
                 "clearing remote index",
                 ", ".join(missing_dirs),
             )
             index.clear()
 
     # Check if non-indexed (new) dir hashes exist on remote
     dir_exists = dir_hashes.intersection(indexed_dir_exists)
-    dir_exists.update(odb.list_hashes_exists(dir_hashes - dir_exists))
+    dir_exists.update(odb.list_hashes_exists(dir_hashes - dir_exists, jobs))
 
     # If .dir hash exists in the ODB, assume directory contents
     # also exists
     for dir_hash in dir_exists:
         tree = dir_objs.get(dir_hash)
         if not tree:
             try:
@@ -72,14 +72,15 @@
 def status(
     odb: "ObjectDB",
     obj_ids: Iterable["HashInfo"],
     name: Optional[str] = None,
     index: Optional["ObjectDBIndexBase"] = None,
     cache_odb: Optional["ObjectDB"] = None,
     shallow: bool = True,
+    jobs: Optional[int] = None,
     **kwargs,
 ) -> "StatusResult":
     """Return status of whether or not the specified objects exist odb.
 
     If cache_odb is set, trees will be loaded from cache_odb instead of odb
     when needed.
 
@@ -117,57 +118,60 @@
     hashes: Set[str] = set(hash_infos.keys())
     exists: Set[str] = set()
 
     logger.debug("Collecting status from '%s'", odb.fs_path)
     if index and hashes:
         if dir_objs:
             exists = hashes.intersection(
-                _indexed_dir_hashes(odb, index, dir_objs, name, cache_odb)
+                _indexed_dir_hashes(
+                    odb, index, dir_objs, name, cache_odb, jobs=jobs
+                )
             )
             hashes.difference_update(exists)
         if hashes:
             exists.update(index.intersection(hashes))
             hashes.difference_update(exists)
 
     if hashes:
-        exists.update(odb.hashes_exist(hashes, name=odb.fs_path, **kwargs))
+        exists.update(odb.hashes_exist(hashes, name=odb.fs_path, jobs=jobs))
     return StatusResult(
         {hash_infos[hash_] for hash_ in exists},
         {hash_infos[hash_] for hash_ in (hashes - exists)},
     )
 
 
 def compare_status(
     src: "ObjectDB",
     dest: "ObjectDB",
     obj_ids: Iterable["HashInfo"],
     log_missing: bool = True,
     check_deleted: bool = True,
     src_index: Optional["ObjectDBIndexBase"] = None,
     dest_index: Optional["ObjectDBIndexBase"] = None,
+    jobs: Optional[int] = None,
     **kwargs,
 ) -> "CompareStatusResult":
     """Compare status for the specified objects between two ODBs.
 
     Status is returned as a tuple of:
         ok: hashes that exist in both src and dest
         missing: hashes that do not exist in neither src nor dest
         new: hashes that only exist in src
         deleted: hashes that only exist in dest
     """
     if "cache_odb" not in kwargs:
         kwargs["cache_odb"] = src
     dest_exists, dest_missing = status(
-        dest, obj_ids, index=dest_index, **kwargs
+        dest, obj_ids, index=dest_index, jobs=jobs, **kwargs
     )
     # for transfer operations we can skip src status check when all objects
     # already exist in dest
     if dest_missing or check_deleted:
         src_exists, src_missing = status(
-            src, obj_ids, index=src_index, **kwargs
+            src, obj_ids, index=src_index, jobs=jobs, **kwargs
         )
     else:
         src_exists = dest_exists
         src_missing = set()
     result = CompareStatusResult(
         src_exists & dest_exists,
         src_missing & dest_missing,
```

### Comparing `dvc-2.9.4/dvc/data/transfer.py` & `dvc-2.9.5/dvc/data/transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,17 @@
         "Preparing to transfer data from '%s' to '%s'",
         src.fs_path,
         dest.fs_path,
     )
     if src == dest:
         return 0
 
-    status = compare_status(src, dest, obj_ids, check_deleted=False, **kwargs)
+    status = compare_status(
+        src, dest, obj_ids, check_deleted=False, jobs=jobs, **kwargs
+    )
     if not status.new:
         return 0
 
     def func(hash_info: "HashInfo") -> None:
         obj = src.get(hash_info)
         return dest.add(
             obj.fs_path,
```

### Comparing `dvc-2.9.4/dvc/data/tree.py` & `dvc-2.9.5/dvc/data/tree.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/data_cloud.py` & `dvc-2.9.5/dvc/data_cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/dependency/__init__.py` & `dvc-2.9.5/dvc/dependency/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/dependency/base.py` & `dvc-2.9.5/dvc/dependency/base.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/dependency/param.py` & `dvc-2.9.5/dvc/dependency/param.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/dependency/repo.py` & `dvc-2.9.5/dvc/dependency/repo.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/dvcfile.py` & `dvc-2.9.5/dvc/dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/exceptions.py` & `dvc-2.9.5/dvc/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/external_repo.py` & `dvc-2.9.5/dvc/external_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/__init__.py` & `dvc-2.9.5/dvc/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/_callback.py` & `dvc-2.9.5/dvc/fs/_callback.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/azure.py` & `dvc-2.9.5/dvc/fs/azure.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/base.py` & `dvc-2.9.5/dvc/fs/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         """
         return True
 
     def iscopy(self, path):
         """Check if this file is an independent copy."""
         return False  # We can't be sure by default
 
-    def walk(self, top, topdown=True, onerror=None, **kwargs):
+    def walk(self, top, topdown=True, **kwargs):
         """Return a generator with (root, dirs, files)."""
         raise NotImplementedError
 
     def find(self, path, prefix=None):
         """Return a generator with `str`s to all the files.
 
         Optional kwargs:
```

### Comparing `dvc-2.9.4/dvc/fs/dvc.py` & `dvc-2.9.5/dvc/fs/dvc.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         if cls != LocalFileSystem or os.path.isabs(path):
             fs = cls(**kwargs)
             return (cls.scheme, *fs.path.parts(fs_path))
 
         fs_key = "repo"
         key = self.path.parts(path)
-        if key == (".",):
+        if key == (".",) or key == ("",):
             key = ()
 
         return (fs_key, *key)
 
     def _get_fs_path(self, path: "AnyPath", remote=None):
         from dvc.config import NoRemoteError
 
@@ -128,26 +128,22 @@
         assert topdown
         dirs = list(dirs)
         yield root, dirs, files
 
         for dname in dirs:
             yield from self._walk(self.path.join(root, dname))
 
-    def walk(self, top, topdown=True, onerror=None, **kwargs):
+    def walk(self, top, topdown=True, **kwargs):
         assert topdown
         try:
             info = self.info(top)
         except FileNotFoundError:
-            if onerror is not None:
-                onerror(FileNotFoundError(top))
             return
 
         if info["type"] != "directory":
-            if onerror is not None:
-                onerror(NotADirectoryError(top))
             return
 
         yield from self._walk(top, topdown=topdown, **kwargs)
 
     def find(self, path, prefix=None):
         for root, _, files in self.walk(path):
             for fname in files:
```

### Comparing `dvc-2.9.4/dvc/fs/fsspec_wrapper.py` & `dvc-2.9.5/dvc/fs/fsspec_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,28 +45,19 @@
     def _prepare_credentials(
         self, **config: Dict[str, Any]  # pylint: disable=unused-argument
     ) -> Dict[str, Any]:
         """Prepare the arguments for authentication to the
         host filesystem"""
         return {}
 
-    def _isdir(self, path: AnyFSPath) -> bool:
-        return self.fs.isdir(path)
-
     def isdir(self, path: AnyFSPath) -> bool:
-        try:
-            return self._isdir(path)
-        except FileNotFoundError:
-            return False
+        return self.fs.isdir(path)
 
     def isfile(self, path: AnyFSPath) -> bool:
-        try:
-            return not self._isdir(path)
-        except FileNotFoundError:
-            return False
+        return self.fs.isfile(path)
 
     def is_empty(self, path: AnyFSPath) -> bool:
         entry = self.info(path)
         if entry["type"] == "directory":
             return not self.fs.ls(path)
         return entry["size"] == 0
 
@@ -141,14 +132,22 @@
         with self.open(to_info, "wb") as fdest:
             shutil.copyfileobj(
                 fobj,
                 fdest,
                 length=getattr(fdest, "blocksize", None),  # type: ignore
             )
 
+    def walk(
+        self,
+        top: AnyFSPath,
+        topdown: bool = True,
+        **kwargs: Any,
+    ):
+        return self.fs.walk(top, topdown=topdown, **kwargs)
+
 
 # pylint: disable=abstract-method
 class ObjectFSWrapper(FSSpecWrapper):
     TRAVERSE_PREFIX_LEN = 3
 
     def makedirs(self, path: AnyFSPath, **kwargs) -> None:
         # For object storages make this method a no-op. The original
@@ -168,14 +167,26 @@
         entry = self.info(path)
         return entry["type"] == "directory" or (
             entry["size"] == 0
             and entry["type"] == "file"
             and entry["name"].endswith("/")
         )
 
+    def isdir(self, path: AnyFSPath) -> bool:
+        try:
+            return self._isdir(path)
+        except FileNotFoundError:
+            return False
+
+    def isfile(self, path: AnyFSPath) -> bool:
+        try:
+            return not self._isdir(path)
+        except FileNotFoundError:
+            return False
+
     def find(self, path, prefix=None):
         if prefix:
             with_prefix = self.path.parent(path)
             files = self.fs.find(with_prefix, prefix=self.path.parts(path)[-1])
         else:
             with_prefix = path
             files = self.fs.find(path)
```

### Comparing `dvc-2.9.4/dvc/fs/gdrive.py` & `dvc-2.9.5/dvc/fs/gdrive.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/gs.py` & `dvc-2.9.5/dvc/fs/gs.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/hdfs.py` & `dvc-2.9.5/dvc/fs/hdfs.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/http.py` & `dvc-2.9.5/dvc/fs/http.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/local.py` & `dvc-2.9.5/dvc/fs/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,22 +47,23 @@
 
     def isdir(self, path) -> bool:
         return os.path.isdir(path)
 
     def iscopy(self, path):
         return not (System.is_symlink(path) or System.is_hardlink(path))
 
-    def walk(self, top, topdown=True, onerror=None, **kwargs):
+    def walk(self, top, topdown=True, **kwargs):
         """Directory fs generator.
 
         See `os.walk` for the docs. Differences:
         - no support for symlinks
         """
         for root, dirs, files in os.walk(
-            top, topdown=topdown, onerror=onerror
+            top,
+            topdown=topdown,
         ):
             yield os.path.normpath(root), dirs, files
 
     def find(self, path, prefix=None):
         for root, _, files in self.walk(path):
             for file in files:
                 # NOTE: os.path.join is ~5.5 times slower
```

### Comparing `dvc-2.9.4/dvc/fs/memory.py` & `dvc-2.9.5/dvc/fs/memory.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/oss.py` & `dvc-2.9.5/dvc/fs/oss.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/path.py` & `dvc-2.9.5/dvc/fs/path.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/pool.py` & `dvc-2.9.5/dvc/fs/pool.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/repo.py` & `dvc-2.9.5/dvc/fs/repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -400,64 +400,52 @@
             elif dirname in shared:
                 yield from self._walk(repo_walk, dvc_walk, dvcfiles=dvcfiles)
             elif dirname in dvc_set:
                 yield from self._dvc_walk(dvc_walk)
             elif dirname in repo_set:
                 yield from self._walk(repo_walk, None, dvcfiles=dvcfiles)
 
-    def walk(self, top, topdown=True, onerror=None, **kwargs):
+    def walk(self, top, topdown=True, **kwargs):
         """Walk and merge both DVC and repo fss.
 
         Args:
             top: path to walk from
             topdown: if True, fs will be walked from top down.
-            onerror: if set, onerror function will be called if an error
-                occurs (by default errors are ignored).
             dvcfiles: if True, dvcfiles will be included in the files list
                 for walked directories.
 
         Any kwargs will be passed into methods used for fetching and/or
         streaming DVC outs from remotes.
         """
         assert topdown
 
         if not self.exists(top):
-            if onerror is not None:
-                onerror(FileNotFoundError(top))
             return
 
         if not self.isdir(top):
-            if onerror is not None:
-                onerror(NotADirectoryError(top))
             return
 
         repo = self._get_repo(os.path.abspath(top))
         dvcfiles = kwargs.pop("dvcfiles", False)
 
         fs, dvc_fs, dvc_path = self._get_fs_pair(top)
         repo_exists = fs.exists(top)
 
-        repo_walk = repo.dvcignore.walk(
-            fs, top, topdown=topdown, onerror=onerror, **kwargs
-        )
+        repo_walk = repo.dvcignore.walk(fs, top, topdown=topdown, **kwargs)
 
         if not dvc_fs or (repo_exists and dvc_fs.isdvc(dvc_path)):
             yield from self._walk(repo_walk, None, dvcfiles=dvcfiles)
             return
 
         if not repo_exists:
-            yield from _wrap_walk(
-                dvc_fs, dvc_path, topdown=topdown, onerror=onerror, **kwargs
-            )
+            yield from _wrap_walk(dvc_fs, dvc_path, topdown=topdown, **kwargs)
 
         dvc_walk = None
         if dvc_fs.exists(dvc_path):
-            dvc_walk = _wrap_walk(
-                dvc_fs, dvc_path, topdown=topdown, onerror=onerror, **kwargs
-            )
+            dvc_walk = _wrap_walk(dvc_fs, dvc_path, topdown=topdown, **kwargs)
 
         yield from self._walk(repo_walk, dvc_walk, dvcfiles=dvcfiles)
 
     def find(self, path, prefix=None):
         for root, _, files in self.walk(path):
             for fname in files:
                 yield self.path.join(root, fname)
```

### Comparing `dvc-2.9.4/dvc/fs/s3.py` & `dvc-2.9.5/dvc/fs/s3.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/ssh.py` & `dvc-2.9.5/dvc/fs/ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/utils.py` & `dvc-2.9.5/dvc/fs/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/webdav.py` & `dvc-2.9.5/dvc/fs/webdav.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/fs/webhdfs.py` & `dvc-2.9.5/dvc/fs/webhdfs.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/hash_info.py` & `dvc-2.9.5/dvc/hash_info.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/ignore.py` & `dvc-2.9.5/dvc/ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/info.py` & `dvc-2.9.5/dvc/info.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/istextfile.py` & `dvc-2.9.5/dvc/istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/lock.py` & `dvc-2.9.5/dvc/lock.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/logger.py` & `dvc-2.9.5/dvc/logger.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/machine/__init__.py` & `dvc-2.9.5/dvc/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/machine/backend/base.py` & `dvc-2.9.5/dvc/machine/backend/base.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/machine/backend/terraform.py` & `dvc-2.9.5/dvc/machine/backend/terraform.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/objects/db.py` & `dvc-2.9.5/dvc/objects/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,15 +346,15 @@
         )
 
         if not self.fs.CAN_TRAVERSE:
             return self._list_hashes()
 
         remote_size, remote_hashes = self._estimate_remote_size(name=name)
         return self._list_hashes_traverse(
-            remote_size, remote_hashes, jobs, name
+            remote_size, remote_hashes, jobs=jobs, name=name
         )
 
     def _remove_unpacked_dir(self, hash_):
         pass
 
     def list_hashes_exists(self, hashes, jobs=None, name=None):
         """Return list of the specified hashes which exist in this fs.
@@ -453,10 +453,12 @@
             )
             return list(hashes & remote_hashes) + self.list_hashes_exists(
                 hashes - remote_hashes, jobs, name
             )
 
         logger.debug(f"Querying '{len(hashes)}' hashes via traverse")
         remote_hashes = set(
-            self._list_hashes_traverse(remote_size, remote_hashes, jobs, name)
+            self._list_hashes_traverse(
+                remote_size, remote_hashes, jobs=jobs, name=name
+            )
         )
         return list(hashes & set(remote_hashes))
```

### Comparing `dvc-2.9.4/dvc/objects/file.py` & `dvc-2.9.5/dvc/objects/file.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/output.py` & `dvc-2.9.5/dvc/output.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/parsing/__init__.py` & `dvc-2.9.5/dvc/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/parsing/context.py` & `dvc-2.9.5/dvc/parsing/context.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/parsing/interpolate.py` & `dvc-2.9.5/dvc/parsing/interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/parsing/versions.py` & `dvc-2.9.5/dvc/parsing/versions.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/pathspec_math.py` & `dvc-2.9.5/dvc/pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/proc/exceptions.py` & `dvc-2.9.5/dvc/proc/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/proc/manager.py` & `dvc-2.9.5/dvc/proc/manager.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/proc/process.py` & `dvc-2.9.5/dvc/proc/process.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/progress.py` & `dvc-2.9.5/dvc/progress.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/prompt.py` & `dvc-2.9.5/dvc/prompt.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/render/base.py` & `dvc-2.9.5/dvc/render/base.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/render/data.py` & `dvc-2.9.5/dvc/render/data.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/render/html.py` & `dvc-2.9.5/dvc/render/html.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/render/image.py` & `dvc-2.9.5/dvc/render/image.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/render/plotly.py` & `dvc-2.9.5/dvc/render/plotly.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/render/utils.py` & `dvc-2.9.5/dvc/render/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/render/vega.py` & `dvc-2.9.5/dvc/render/vega.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/__init__.py` & `dvc-2.9.5/dvc/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/add.py` & `dvc-2.9.5/dvc/repo/add.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/brancher.py` & `dvc-2.9.5/dvc/repo/brancher.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/checkout.py` & `dvc-2.9.5/dvc/repo/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/collect.py` & `dvc-2.9.5/dvc/repo/collect.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/commit.py` & `dvc-2.9.5/dvc/repo/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/destroy.py` & `dvc-2.9.5/dvc/repo/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/diff.py` & `dvc-2.9.5/dvc/repo/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/__init__.py` & `dvc-2.9.5/dvc/repo/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/apply.py` & `dvc-2.9.5/dvc/repo/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/base.py` & `dvc-2.9.5/dvc/repo/experiments/base.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/branch.py` & `dvc-2.9.5/dvc/repo/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/diff.py` & `dvc-2.9.5/dvc/repo/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/exceptions.py` & `dvc-2.9.5/dvc/repo/experiments/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/executor/base.py` & `dvc-2.9.5/dvc/repo/experiments/executor/base.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/executor/local.py` & `dvc-2.9.5/dvc/repo/experiments/executor/local.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/executor/manager/base.py` & `dvc-2.9.5/dvc/repo/experiments/executor/manager/base.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/executor/manager/local.py` & `dvc-2.9.5/dvc/repo/experiments/executor/manager/local.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/executor/manager/ssh.py` & `dvc-2.9.5/dvc/repo/experiments/executor/manager/ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/executor/ssh.py` & `dvc-2.9.5/dvc/repo/experiments/executor/ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/gc.py` & `dvc-2.9.5/dvc/repo/experiments/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/init.py` & `dvc-2.9.5/dvc/repo/experiments/init.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,23 @@
     Optional,
     TextIO,
     Tuple,
     Union,
     cast,
 )
 
-from funcy import compact, lremove
+from funcy import compact, lremove, lsplit
 from rich.rule import Rule
 from rich.syntax import Syntax
 
 from dvc.exceptions import DvcException
 from dvc.stage import PipelineStage
 from dvc.stage.serialize import to_pipeline_file
 from dvc.types import OptStr
+from dvc.utils import humanize
 from dvc.utils.serialize import dumps_yaml
 
 if TYPE_CHECKING:
     from dvc.repo import Repo
     from dvc.dvcfile import DVCFile
     from rich.tree import Tree
 
@@ -75,26 +76,34 @@
 
     try:
         yield
     finally:
         logging.disable(previous_level)
 
 
-def build_workspace_tree(workspace: Dict[str, str]) -> "Tree":
+def build_workspace_tree(workspace: Dict[str, str], label: str) -> "Tree":
     from rich.tree import Tree
 
-    tree = Tree(
-        "DVC assumes the following workspace structure:",
-        highlight=True,
-    )
+    tree = Tree(label, highlight=True)
     for value in sorted(workspace.values()):
         tree.add(f"[green]{value}[/green]")
     return tree
 
 
+def display_workspace_tree(
+    workspace: Dict[str, str], label: str, stderr: bool = False
+) -> None:
+    d = workspace.copy()
+    d.pop("cmd", None)
+
+    if d:
+        ui.write(build_workspace_tree(d, label), styled=True, stderr=stderr)
+    ui.write(styled=True, stderr=stderr)
+
+
 PIPELINE_FILE_LINK = "https://s.dvc.org/g/pipeline-files"
 
 
 def init_interactive(
     name: str,
     defaults: Dict[str, str],
     provided: Dict[str, str],
@@ -140,17 +149,17 @@
     if not prompts:
         return ret
 
     ui.error_write(
         "Enter the paths for dependencies and outputs of the command.",
         styled=True,
     )
-    if workspace:
-        ui.error_write(build_workspace_tree(workspace), styled=True)
-    ui.error_write(styled=True)
+
+    tree_label = "Using experiment project structure:"
+    display_workspace_tree(workspace, tree_label, stderr=True)
     ret.update(
         compact(
             _prompts(prompts, defaults, validator=validator, stream=stream)
         )
     )
     return ret
 
@@ -188,21 +197,53 @@
             suffices = {
                 errno.EISDIR: "is a directory",
                 errno.ENOENT: "does not exist",
             }
             raise InvalidResponse(msg_format.format(value, suffices[e.errno]))
     elif key in ("code", "data"):
         if not os.path.exists(value):
-            return value, (
-                f"[yellow]'{value}' does not exist in the workspace. "
-                '"exp run" may fail.[/]'
+            typ = "file" if is_file(value) else "directory"
+            return (
+                value,
+                f"[yellow]'{value}' does not exist, "
+                f"the {typ} will be created. ",
             )
     return value
 
 
+def is_file(path: str) -> bool:
+    _, ext = os.path.splitext(path)
+    return bool(ext)
+
+
+def init_deps(stage: PipelineStage) -> None:
+    from funcy import rpartial
+
+    from dvc.dependency import ParamsDependency
+    from dvc.fs.local import localfs
+
+    new_deps = [dep for dep in stage.deps if not dep.exists]
+    params, deps = lsplit(rpartial(isinstance, ParamsDependency), new_deps)
+
+    if new_deps:
+        paths = map("[green]{0}[/]".format, new_deps)
+        ui.write(f"Created {humanize.join(paths)}.", styled=True)
+
+    # always create a file for params, detect file/folder based on extension
+    # for other dependencies
+    dirs = [dep.fs_path for dep in deps if not is_file(dep.fs_path)]
+    files = [dep.fs_path for dep in deps + params if is_file(dep.fs_path)]
+    for path in dirs:
+        localfs.makedirs(path)
+    for path in files:
+        localfs.makedirs(localfs.path.parent(path), exist_ok=True)
+        with localfs.open(path, "w", encoding="utf-8"):
+            pass
+
+
 def init(
     repo: "Repo",
     name: str = "train",
     type: str = "default",  # pylint: disable=redefined-builtin
     defaults: Dict[str, str] = None,
     overrides: Dict[str, str] = None,
     interactive: bool = False,
@@ -274,23 +315,30 @@
         ui.error_write(Rule(style="green"), styled=True)
         _yaml = dumps_yaml(to_pipeline_file(cast(PipelineStage, stage)))
         syn = Syntax(_yaml, "yaml", theme="ansi_dark")
         ui.error_write(syn, styled=True)
 
     from dvc.ui.prompt import Confirm
 
-    if not interactive or Confirm.ask(
+    if interactive and not Confirm.ask(
         "Do you want to add the above contents to dvc.yaml?",
         console=ui.error_console,
         default=True,
         stream=stream,
     ):
-        with _disable_logging(), repo.scm_context(autostage=True, quiet=True):
-            stage.dump(update_lock=False)
-            stage.ignore_outs()
-            if params:
-                repo.scm_context.track_file(params)
-    else:
         raise DvcException("Aborting ...")
 
+    if interactive:
+        ui.error_write()  # add a newline after the prompts
+
+    with _disable_logging(), repo.scm_context(autostage=True, quiet=True):
+        stage.dump(update_lock=False)
+        stage.ignore_outs()
+        if not interactive:
+            label = "Using experiment project structure:"
+            display_workspace_tree(context, label)
+        init_deps(stage)
+        if params:
+            repo.scm_context.track_file(params)
+
     assert isinstance(stage, PipelineStage)
     return stage
```

### Comparing `dvc-2.9.4/dvc/repo/experiments/ls.py` & `dvc-2.9.5/dvc/repo/experiments/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/pull.py` & `dvc-2.9.5/dvc/repo/experiments/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/push.py` & `dvc-2.9.5/dvc/repo/experiments/push.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/remove.py` & `dvc-2.9.5/dvc/repo/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/run.py` & `dvc-2.9.5/dvc/repo/experiments/run.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/show.py` & `dvc-2.9.5/dvc/repo/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/experiments/utils.py` & `dvc-2.9.5/dvc/repo/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/fetch.py` & `dvc-2.9.5/dvc/repo/fetch.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/gc.py` & `dvc-2.9.5/dvc/repo/gc.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,12 +78,12 @@
         if not removed:
             logger.info(f"No unused '{scheme}' cache to remove.")
 
     if not cloud:
         return
 
     odb = self.cloud.get_remote_odb(remote, "gc -c")
-    removed = ogc(odb, used_obj_ids)
+    removed = ogc(odb, used_obj_ids, jobs=jobs)
     if removed:
         get_index(odb).clear()
     else:
         logger.info("No unused cache to remove from remote.")
```

### Comparing `dvc-2.9.4/dvc/repo/get.py` & `dvc-2.9.5/dvc/repo/get.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/graph.py` & `dvc-2.9.5/dvc/repo/graph.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/imp_url.py` & `dvc-2.9.5/dvc/repo/imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/index.py` & `dvc-2.9.5/dvc/repo/index.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/init.py` & `dvc-2.9.5/dvc/repo/init.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/install.py` & `dvc-2.9.5/dvc/repo/install.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/live.py` & `dvc-2.9.5/dvc/repo/live.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/ls.py` & `dvc-2.9.5/dvc/repo/ls.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,31 +43,24 @@
             info["path"] = path
             ret_list.append(info)
         ret_list.sort(key=lambda f: f["path"])
         return ret_list
 
 
 def _ls(repo, fs_path, recursive=None, dvc_only=False):
-    def onerror(exc):
-        raise exc
-
     fs = repo.repo_fs
     infos = []
-    try:
-        for root, dirs, files in fs.walk(
-            fs_path, onerror=onerror, dvcfiles=True
-        ):
-            entries = chain(files, dirs) if not recursive else files
-            infos.extend(fs.path.join(root, entry) for entry in entries)
-            if not recursive:
-                break
-    except NotADirectoryError:
+    for root, dirs, files in fs.walk(fs_path, dvcfiles=True):
+        entries = chain(files, dirs) if not recursive else files
+        infos.extend(fs.path.join(root, entry) for entry in entries)
+        if not recursive:
+            break
+
+    if not infos and fs.isfile(fs_path):
         infos.append(fs_path)
-    except FileNotFoundError:
-        return {}
 
     ret = {}
     for info in infos:
         try:
             _info = fs.info(info)
         except FileNotFoundError:
             # broken symlink
```

### Comparing `dvc-2.9.4/dvc/repo/metrics/diff.py` & `dvc-2.9.5/dvc/repo/metrics/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/metrics/show.py` & `dvc-2.9.5/dvc/repo/metrics/show.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/move.py` & `dvc-2.9.5/dvc/repo/move.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/params/diff.py` & `dvc-2.9.5/dvc/repo/params/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/params/show.py` & `dvc-2.9.5/dvc/repo/params/show.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/plots/__init__.py` & `dvc-2.9.5/dvc/repo/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/plots/diff.py` & `dvc-2.9.5/dvc/repo/plots/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/plots/template.py` & `dvc-2.9.5/dvc/repo/plots/template.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/plots/templates/confusion.json` & `dvc-2.9.5/dvc/repo/plots/templates/confusion.json`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/plots/templates/confusion_normalized.json` & `dvc-2.9.5/dvc/repo/plots/templates/confusion_normalized.json`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/plots/templates/linear.json` & `dvc-2.9.5/dvc/repo/plots/templates/linear.json`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/plots/templates/scatter.json` & `dvc-2.9.5/dvc/repo/plots/templates/scatter.json`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/plots/templates/simple.json` & `dvc-2.9.5/dvc/repo/plots/templates/simple.json`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/plots/templates/smooth.json` & `dvc-2.9.5/dvc/repo/plots/templates/smooth.json`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/pull.py` & `dvc-2.9.5/dvc/repo/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/push.py` & `dvc-2.9.5/dvc/repo/push.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/reproduce.py` & `dvc-2.9.5/dvc/repo/reproduce.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/run.py` & `dvc-2.9.5/dvc/repo/run.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/scm_context.py` & `dvc-2.9.5/dvc/repo/scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/stage.py` & `dvc-2.9.5/dvc/repo/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/status.py` & `dvc-2.9.5/dvc/repo/status.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/trie.py` & `dvc-2.9.5/dvc/repo/trie.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/repo/update.py` & `dvc-2.9.5/dvc/repo/update.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/rwlock.py` & `dvc-2.9.5/dvc/rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/schema.py` & `dvc-2.9.5/dvc/schema.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/scm.py` & `dvc-2.9.5/dvc/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/stage/__init__.py` & `dvc-2.9.5/dvc/stage/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/stage/cache.py` & `dvc-2.9.5/dvc/stage/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/stage/decorators.py` & `dvc-2.9.5/dvc/stage/decorators.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/stage/exceptions.py` & `dvc-2.9.5/dvc/stage/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/stage/imports.py` & `dvc-2.9.5/dvc/stage/imports.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/stage/loader.py` & `dvc-2.9.5/dvc/stage/loader.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/stage/monitor.py` & `dvc-2.9.5/dvc/stage/monitor.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/stage/run.py` & `dvc-2.9.5/dvc/stage/run.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/stage/serialize.py` & `dvc-2.9.5/dvc/stage/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/stage/utils.py` & `dvc-2.9.5/dvc/stage/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/state.py` & `dvc-2.9.5/dvc/state.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/system.py` & `dvc-2.9.5/dvc/system.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/testing/cloud.py` & `dvc-2.9.5/dvc/testing/cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/testing/fixtures.py` & `dvc-2.9.5/dvc/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/testing/path_info.py` & `dvc-2.9.5/dvc/testing/path_info.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/testing/test_api.py` & `dvc-2.9.5/dvc/testing/test_api.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/testing/test_remote.py` & `dvc-2.9.5/dvc/testing/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/testing/test_workspace.py` & `dvc-2.9.5/dvc/testing/test_workspace.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/testing/tmp_dir.py` & `dvc-2.9.5/dvc/testing/tmp_dir.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/ui/__init__.py` & `dvc-2.9.5/dvc/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/ui/pager.py` & `dvc-2.9.5/dvc/ui/pager.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/ui/prompt.py` & `dvc-2.9.5/dvc/ui/prompt.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/ui/table.py` & `dvc-2.9.5/dvc/ui/table.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/updater.py` & `dvc-2.9.5/dvc/updater.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/__init__.py` & `dvc-2.9.5/dvc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/_benedict.py` & `dvc-2.9.5/dvc/utils/_benedict.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/cli_parse.py` & `dvc-2.9.5/dvc/utils/cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/collections.py` & `dvc-2.9.5/dvc/utils/collections.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/conversions.py` & `dvc-2.9.5/dvc/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/decorators.py` & `dvc-2.9.5/dvc/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/diff.py` & `dvc-2.9.5/dvc/utils/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/fs.py` & `dvc-2.9.5/dvc/utils/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/humanize.py` & `dvc-2.9.5/dvc/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/serialize/__init__.py` & `dvc-2.9.5/dvc/utils/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/serialize/_common.py` & `dvc-2.9.5/dvc/utils/serialize/_common.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/serialize/_json.py` & `dvc-2.9.5/dvc/utils/serialize/_json.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/serialize/_py.py` & `dvc-2.9.5/dvc/utils/serialize/_py.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/serialize/_toml.py` & `dvc-2.9.5/dvc/utils/serialize/_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/serialize/_yaml.py` & `dvc-2.9.5/dvc/utils/serialize/_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/stream.py` & `dvc-2.9.5/dvc/utils/stream.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/strictyaml.py` & `dvc-2.9.5/dvc/utils/strictyaml.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/table.py` & `dvc-2.9.5/dvc/utils/table.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc/utils/threadpool.py` & `dvc-2.9.5/dvc/utils/threadpool.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc.egg-info/PKG-INFO` & `dvc-2.9.5/dvc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 2.9.4
+Version: 2.9.5
 Summary: Git for data scientists - manage your code and data together
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc
 Author: Dmitry Petrov
 Author-email: dmitry@dvc.org
 Maintainer: Iterative
 Maintainer-email: support@dvc.org
```

### Comparing `dvc-2.9.4/dvc.egg-info/SOURCES.txt` & `dvc-2.9.5/dvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/dvc.egg-info/requires.txt` & `dvc-2.9.5/dvc.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 pytest-lazy-fixture==0.6.3
 flaky==3.7.0
 mock==4.0.3
 pytest-timeout==2.1.0
 rangehttpserver==1.2.0
 mock-ssh-server==0.9.1
 wget==3.2
-filelock==3.4.2
+filelock==3.5.1
 wsgidav==4.0.1
 crc32c==2.2.post0
 xmltodict==0.12.0
 google-compute-engine==2.8.13
 google-cloud-storage==2.1.0
 dvclive[image]==0.5.1
 hdfs==2.6.0
@@ -151,15 +151,15 @@
 pytest-lazy-fixture==0.6.3
 flaky==3.7.0
 mock==4.0.3
 pytest-timeout==2.1.0
 rangehttpserver==1.2.0
 mock-ssh-server==0.9.1
 wget==3.2
-filelock==3.4.2
+filelock==3.5.1
 wsgidav==4.0.1
 crc32c==2.2.post0
 xmltodict==0.12.0
 google-compute-engine==2.8.13
 google-cloud-storage==2.1.0
 dvclive[image]==0.5.1
 hdfs==2.6.0
```

### Comparing `dvc-2.9.4/pyproject.toml` & `dvc-2.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/scripts/build.py` & `dvc-2.9.5/scripts/build.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/scripts/fpm/build.py` & `dvc-2.9.5/scripts/fpm/build.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/scripts/fpm/notarize.py` & `dvc-2.9.5/scripts/fpm/notarize.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/scripts/fpm/sign.py` & `dvc-2.9.5/scripts/fpm/sign.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/scripts/innosetup/addSymLinkPermissions.ps1` & `dvc-2.9.5/scripts/innosetup/addSymLinkPermissions.ps1`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/scripts/innosetup/addsymlink.iss` & `dvc-2.9.5/scripts/innosetup/addsymlink.iss`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/scripts/innosetup/build.py` & `dvc-2.9.5/scripts/innosetup/build.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/scripts/innosetup/modpath.iss` & `dvc-2.9.5/scripts/innosetup/modpath.iss`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/scripts/innosetup/setup.iss` & `dvc-2.9.5/scripts/innosetup/setup.iss`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/scripts/pyinstaller/build.py` & `dvc-2.9.5/scripts/pyinstaller/build.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/scripts/pyinstaller/hooks/hook-dvc.py` & `dvc-2.9.5/scripts/pyinstaller/hooks/hook-dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/scripts/pyinstaller/sign.py` & `dvc-2.9.5/scripts/pyinstaller/sign.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/setup.cfg` & `dvc-2.9.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 	pytest-docker==0.10.3; python_version < '3.10' or sys_platform != 'win32'
 	flaky==3.7.0
 	mock==4.0.3
 	pytest-timeout==2.1.0
 	rangehttpserver==1.2.0
 	mock-ssh-server==0.9.1
 	wget==3.2
-	filelock==3.4.2
+	filelock==3.5.1
 	wsgidav==4.0.1
 	crc32c==2.2.post0
 	xmltodict==0.12.0
 	google-compute-engine==2.8.13
 	google-cloud-storage==2.1.0
 	dvclive[image]==0.5.1
 	hdfs==2.6.0
```

### Comparing `dvc-2.9.4/tests/__init__.py` & `dvc-2.9.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/__main__.py` & `dvc-2.9.5/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/basic_env.py` & `dvc-2.9.5/tests/basic_env.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/conftest.py` & `dvc-2.9.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/dir_helpers.py` & `dvc-2.9.5/tests/dir_helpers.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/conftest.py` & `dvc-2.9.5/tests/func/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/experiments/conftest.py` & `dvc-2.9.5/tests/func/experiments/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/experiments/executor/test_ssh.py` & `dvc-2.9.5/tests/func/experiments/executor/test_ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/experiments/test_checkpoints.py` & `dvc-2.9.5/tests/func/experiments/test_checkpoints.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/experiments/test_diff.py` & `dvc-2.9.5/tests/func/experiments/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/experiments/test_experiments.py` & `dvc-2.9.5/tests/func/experiments/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/experiments/test_gc.py` & `dvc-2.9.5/tests/func/experiments/test_gc.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/experiments/test_init.py` & `dvc-2.9.5/tests/func/experiments/test_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,16 @@
                 "metrics": [{"metrics.json": {"cache": False}}],
                 "outs": ["models"],
                 "params": ["foo"],
                 "plots": [{"plots": {"cache": False}}],
             }
         }
     }
+    assert (tmp_dir / "data").read_text() == "data"
+    assert (tmp_dir / "src").is_dir()
 
 
 @pytest.mark.parametrize("interactive", [True, False])
 def test_when_stage_already_exists_with_same_name(tmp_dir, dvc, interactive):
     (tmp_dir / "dvc.yaml").dump({"stages": {"train": {"cmd": "test"}}})
     with pytest.raises(DuplicateStageName) as exc:
         init(
@@ -138,14 +140,16 @@
                 # so it creates checkpoint-based output.
                 "outs": [{"models": {"checkpoint": True}}],
                 "params": ["foo"],
                 "plots": [{"plots": {"cache": False}}],
             }
         }
     }
+    assert (tmp_dir / "src").is_dir()
+    assert (tmp_dir / "data").is_dir()
 
 
 def test_when_params_is_omitted_in_interactive_mode(tmp_dir, scm, dvc):
     (tmp_dir / "params.yaml").dump({"foo": 1})
     inp = io.StringIO("python script.py\nscript.py\ndata\nmodels\nn")
 
     init(
@@ -160,14 +164,16 @@
                 "metrics": [{"metrics.json": {"cache": False}}],
                 "outs": ["models"],
                 "plots": [{"plots": {"cache": False}}],
             }
         }
     }
     assert not (tmp_dir / "dvc.lock").exists()
+    assert (tmp_dir / "script.py").read_text() == ""
+    assert (tmp_dir / "data").is_dir()
     scm._reset()
     assert scm.is_tracked("dvc.yaml")
     assert not scm.is_tracked("params.yaml")
     assert scm.is_tracked(".gitignore")
     assert scm.is_ignored("models")
 
 
@@ -190,55 +196,51 @@
                 "metrics": [{"metrics.json": {"cache": False}}],
                 "outs": ["models"],
                 "params": ["foo"],
                 "plots": [{"plots": {"cache": False}}],
             }
         }
     }
+    assert (tmp_dir / "script.py").read_text() == ""
+    assert (tmp_dir / "data").is_dir()
 
     out, err = capsys.readouterr()
     assert (
         "Path to a parameters file [params.yaml, n to omit]: "
         "'params.json' does not exist. "
         "Please retry with an existing parameters file.\n"
         "Path to a parameters file [params.yaml, n to omit]: "
         "'data' is a directory. "
         "Please retry with an existing parameters file.\n"
         "Path to a parameters file [params.yaml, n to omit]:"
     ) in err
-    assert not out
+    assert out == "Created script.py.\n"
 
 
 def test_init_with_no_defaults_interactive(tmp_dir, dvc):
-    inp = io.StringIO(
-        "python script.py\n"
-        "script.py\n"
-        "data\n"
-        "model\n"
-        "n\n"
-        "metric\n"
-        "n\n"
-    )
+    inp = io.StringIO("script.py\n" "data\n" "model\n" "n\n" "metric\n" "n\n")
     init(
         dvc,
         defaults={},
         overrides={"cmd": "python script.py"},
         interactive=True,
         stream=inp,
     )
     assert (tmp_dir / "dvc.yaml").parse() == {
         "stages": {
             "train": {
                 "cmd": "python script.py",
-                "deps": ["python script.py", "script.py"],
+                "deps": ["data", "script.py"],
                 "metrics": [{"metric": {"cache": False}}],
-                "outs": ["data"],
+                "outs": ["model"],
             }
         }
     }
+    assert (tmp_dir / "script.py").read_text() == ""
+    assert (tmp_dir / "data").is_dir()
 
 
 @pytest.mark.parametrize(
     "interactive, overrides, inp",
     [
         (False, {"cmd": "python script.py", "code": "script.py"}, None),
         (
@@ -254,17 +256,15 @@
                 "plots\n"
                 "y"
             ),
         ),
     ],
     ids=["non-interactive", "interactive"],
 )
-def test_init_interactive_default(
-    tmp_dir, scm, dvc, interactive, overrides, inp, capsys
-):
+def test_init_default(tmp_dir, scm, dvc, interactive, overrides, inp, capsys):
     (tmp_dir / "params.yaml").dump({"foo": {"bar": 1}})
 
     init(
         dvc,
         interactive=interactive,
         defaults=CmdExperimentsInit.DEFAULTS,
         overrides=overrides,
@@ -280,25 +280,29 @@
                 "outs": ["models"],
                 "params": ["foo"],
                 "plots": [{"plots": {"cache": False}}],
             }
         }
     }
     assert not (tmp_dir / "dvc.lock").exists()
+    assert (tmp_dir / "script.py").read_text() == ""
+    assert (tmp_dir / "data").is_dir()
     scm._reset()
     assert scm.is_tracked("dvc.yaml")
     assert scm.is_tracked("params.yaml")
     assert scm.is_tracked(".gitignore")
     assert scm.is_ignored("models")
     out, err = capsys.readouterr()
 
     if interactive:
-        assert "'script.py' does not exist in the workspace." in err
-        assert "'data' does not exist in the workspace." in err
-    assert not out
+        assert "'script.py' does not exist, the file will be created." in err
+        assert "'data' does not exist, the directory will be created." in err
+    else:
+        assert "Using experiment project structure: " in out
+    assert "Created script.py and data" in out
 
 
 @pytest.mark.timeout(5, func_only=True)
 @pytest.mark.parametrize(
     "interactive, overrides, inp",
     [
         (False, {"cmd": "python script.py", "code": "script.py"}, None),
@@ -361,25 +365,30 @@
                 "live": {"dvclive": {"html": True, "summary": True}},
                 "outs": [{"models": {"checkpoint": True}}],
                 "params": ["foo"],
             }
         }
     }
     assert not (tmp_dir / "dvc.lock").exists()
+    assert (tmp_dir / "script.py").read_text() == ""
+    assert (tmp_dir / "data").is_dir()
     scm._reset()
     assert scm.is_tracked("dvc.yaml")
     assert scm.is_tracked("params.yaml")
     assert scm.is_tracked(".gitignore")
     assert scm.is_ignored("models")
 
     out, err = capsys.readouterr()
+
     if interactive:
-        assert "'script.py' does not exist in the workspace." in err
-        assert "'data' does not exist in the workspace." in err
-    assert not out
+        assert "'script.py' does not exist, the file will be created." in err
+        assert "'data' does not exist, the directory will be created." in err
+    else:
+        assert "Using experiment project structure: " in out
+    assert "Created script.py and data" in out
 
 
 @pytest.mark.parametrize(
     "interactive, inp",
     [
         (False, None),
         (True, io.StringIO()),
@@ -406,14 +415,16 @@
                 "metrics": [{"m": {"cache": False}}],
                 "outs": [{"models": {"checkpoint": True}}],
                 "params": ["foo"],
                 "plots": [{"p": {"cache": False}}],
             }
         }
     }
+    assert (tmp_dir / "src").is_dir()
+    assert (tmp_dir / "data").is_dir()
 
 
 @pytest.mark.parametrize(
     "interactive, inp",
     [
         (False, None),
         (True, io.StringIO()),
@@ -439,7 +450,9 @@
                 "metrics": [{"metrics.json": {"cache": False}}],
                 "outs": [{"models": {"checkpoint": True}}],
                 "params": ["foo"],
                 "plots": [{"plots": {"cache": False}}],
             }
         }
     }
+    assert (tmp_dir / "src").is_dir()
+    assert (tmp_dir / "data").is_dir()
```

### Comparing `dvc-2.9.4/tests/func/experiments/test_remote.py` & `dvc-2.9.5/tests/func/experiments/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/experiments/test_remove.py` & `dvc-2.9.5/tests/func/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/experiments/test_show.py` & `dvc-2.9.5/tests/func/experiments/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/machine/conftest.py` & `dvc-2.9.5/tests/func/machine/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/machine/test_machine_config.py` & `dvc-2.9.5/tests/func/machine/test_machine_config.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/machine/test_machine_status.py` & `dvc-2.9.5/tests/func/machine/test_machine_status.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/metrics/test_diff.py` & `dvc-2.9.5/tests/func/metrics/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/metrics/test_show.py` & `dvc-2.9.5/tests/func/metrics/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/objects/db/test_index.py` & `dvc-2.9.5/tests/func/objects/db/test_index.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/params/test_diff.py` & `dvc-2.9.5/tests/func/params/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/params/test_show.py` & `dvc-2.9.5/tests/func/params/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/parsing/__init__.py` & `dvc-2.9.5/tests/func/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/parsing/test_errors.py` & `dvc-2.9.5/tests/func/parsing/test_errors.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/parsing/test_foreach.py` & `dvc-2.9.5/tests/func/parsing/test_foreach.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/parsing/test_interpolated_entry.py` & `dvc-2.9.5/tests/func/parsing/test_interpolated_entry.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/parsing/test_resolver.py` & `dvc-2.9.5/tests/func/parsing/test_resolver.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/plots/test_diff.py` & `dvc-2.9.5/tests/func/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/plots/test_modify.py` & `dvc-2.9.5/tests/func/plots/test_modify.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/plots/test_show.py` & `dvc-2.9.5/tests/func/plots/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_add.py` & `dvc-2.9.5/tests/func/test_add.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_analytics.py` & `dvc-2.9.5/tests/func/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_api.py` & `dvc-2.9.5/tests/func/test_api.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_check_ignore.py` & `dvc-2.9.5/tests/func/test_check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_checkout.py` & `dvc-2.9.5/tests/func/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_cli.py` & `dvc-2.9.5/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_commit.py` & `dvc-2.9.5/tests/func/test_commit.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_config.py` & `dvc-2.9.5/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_data_cloud.py` & `dvc-2.9.5/tests/func/test_data_cloud.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 import shutil
 
 import pytest
 from flaky.flaky_decorator import flaky
 
 import dvc as dvc_module
 from dvc.cli import main
+from dvc.data.db.local import LocalObjectDB
 from dvc.external_repo import clean_repos
+from dvc.objects.db import ObjectDB
 from dvc.stage.exceptions import StageNotFound
 from dvc.testing.test_remote import (  # noqa, pylint: disable=unused-import
     TestRemote,
 )
 from dvc.utils.fs import remove
 
 
-def test_cloud_cli(tmp_dir, dvc, remote):
-    args = ["-v", "-j", "2"]
+def test_cloud_cli(tmp_dir, dvc, remote, mocker):
+    jobs = 2
+    args = ["-v", "-j", str(jobs)]
 
     (stage,) = tmp_dir.dvc_gen("foo", "foo")
     cache = stage.outs[0].cache_path
 
     (stage_dir,) = tmp_dir.dvc_gen(
         {
             "data_dir": {
@@ -30,54 +33,93 @@
             }
         }
     )
     assert stage_dir is not None
     cache_dir = stage_dir.outs[0].cache_path
 
     # FIXME check status output
+    hashes_exist = mocker.spy(LocalObjectDB, "hashes_exist")
 
     assert main(["push"] + args) == 0
     assert os.path.exists(cache)
     assert os.path.isfile(cache)
     assert os.path.isfile(cache_dir)
+    assert hashes_exist.called
+    assert all(
+        _kwargs["jobs"] == jobs
+        for (_args, _kwargs) in hashes_exist.call_args_list
+    )
 
     remove(dvc.odb.local.cache_dir)
+    hashes_exist.reset_mock()
 
     assert main(["fetch"] + args) == 0
     assert os.path.exists(cache)
     assert os.path.isfile(cache)
     assert os.path.isfile(cache_dir)
+    assert hashes_exist.called
+    assert all(
+        _kwargs["jobs"] == jobs
+        for (_args, _kwargs) in hashes_exist.call_args_list
+    )
+
+    hashes_exist.reset_mock()
 
     assert main(["pull"] + args) == 0
     assert os.path.exists(cache)
     assert os.path.isfile(cache)
     assert os.path.isfile(cache_dir)
     assert os.path.isfile("foo")
     assert os.path.isdir("data_dir")
+    assert hashes_exist.called
+    assert all(
+        _kwargs["jobs"] == jobs
+        for (_args, _kwargs) in hashes_exist.call_args_list
+    )
 
     with open(cache, encoding="utf-8") as fd:
         assert fd.read() == "foo"
     assert os.path.isfile(cache_dir)
 
     # NOTE: http doesn't support gc yet
     if remote.url.startswith("http"):
         return
 
+    hashes_exist.reset_mock()
+
+    _list_hashes_traverse = mocker.spy(ObjectDB, "_list_hashes_traverse")
     # NOTE: check if remote gc works correctly on directories
     assert main(["gc", "-cw", "-f"] + args) == 0
+    assert _list_hashes_traverse.called
+    assert all(
+        _kwargs["jobs"] == 2
+        for (_args, _kwargs) in hashes_exist.call_args_list
+    )
     shutil.move(dvc.odb.local.cache_dir, dvc.odb.local.cache_dir + ".back")
 
     assert main(["fetch"] + args) == 0
 
+    assert hashes_exist.called
+    assert all(
+        _kwargs["jobs"] == jobs
+        for (_args, _kwargs) in hashes_exist.call_args_list
+    )
+
+    hashes_exist.reset_mock()
     assert main(["pull", "-f"] + args) == 0
     assert os.path.exists(cache)
     assert os.path.isfile(cache)
     assert os.path.isfile(cache_dir)
     assert os.path.isfile("foo")
     assert os.path.isdir("data_dir")
+    assert hashes_exist.called
+    assert all(
+        _kwargs["jobs"] == jobs
+        for (_args, _kwargs) in hashes_exist.call_args_list
+    )
 
 
 def test_data_cloud_error_cli(dvc):
     f = "non-existing-file"
     assert main(["status", "-c", f])
     assert main(["push", f])
     assert main(["pull", f])
```

### Comparing `dvc-2.9.4/tests/func/test_diff.py` & `dvc-2.9.5/tests/func/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_dvcfile.py` & `dvc-2.9.5/tests/func/test_dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_external_repo.py` & `dvc-2.9.5/tests/func/test_external_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_fs.py` & `dvc-2.9.5/tests/func/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_gc.py` & `dvc-2.9.5/tests/func/test_gc.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_get.py` & `dvc-2.9.5/tests/func/test_get.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_get_url.py` & `dvc-2.9.5/tests/func/test_get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_ignore.py` & `dvc-2.9.5/tests/func/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_import.py` & `dvc-2.9.5/tests/func/test_import.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_import_url.py` & `dvc-2.9.5/tests/func/test_import_url.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_init.py` & `dvc-2.9.5/tests/func/test_init.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_install.py` & `dvc-2.9.5/tests/func/test_install.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_live.py` & `dvc-2.9.5/tests/func/test_live.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_lock.py` & `dvc-2.9.5/tests/func/test_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_lockfile.py` & `dvc-2.9.5/tests/func/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_ls.py` & `dvc-2.9.5/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_merge_driver.py` & `dvc-2.9.5/tests/func/test_merge_driver.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_move.py` & `dvc-2.9.5/tests/func/test_move.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_odb.py` & `dvc-2.9.5/tests/func/test_odb.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_remote.py` & `dvc-2.9.5/tests/func/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_remove.py` & `dvc-2.9.5/tests/func/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_repo.py` & `dvc-2.9.5/tests/func/test_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_repo_index.py` & `dvc-2.9.5/tests/func/test_repo_index.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_repro.py` & `dvc-2.9.5/tests/func/test_repro.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_repro_multistage.py` & `dvc-2.9.5/tests/func/test_repro_multistage.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_run_cache.py` & `dvc-2.9.5/tests/func/test_run_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_run_multistage.py` & `dvc-2.9.5/tests/func/test_run_multistage.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_run_single_stage.py` & `dvc-2.9.5/tests/func/test_run_single_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_scm.py` & `dvc-2.9.5/tests/func/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_scm_context.py` & `dvc-2.9.5/tests/func/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_stage.py` & `dvc-2.9.5/tests/func/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_stage_load.py` & `dvc-2.9.5/tests/func/test_stage_load.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_state.py` & `dvc-2.9.5/tests/func/test_state.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_status.py` & `dvc-2.9.5/tests/func/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_unprotect.py` & `dvc-2.9.5/tests/func/test_unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_update.py` & `dvc-2.9.5/tests/func/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_utils.py` & `dvc-2.9.5/tests/func/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/test_version.py` & `dvc-2.9.5/tests/func/test_version.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/utils/test_fs.py` & `dvc-2.9.5/tests/func/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/func/utils/test_strict_yaml.py` & `dvc-2.9.5/tests/func/utils/test_strict_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/pylint_plugin_disable.py` & `dvc-2.9.5/tests/pylint_plugin_disable.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/remotes/git_server.py` & `dvc-2.9.5/tests/remotes/git_server.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/remotes/user.key` & `dvc-2.9.5/tests/remotes/user.key`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/remotes_env.sample` & `dvc-2.9.5/tests/remotes_env.sample`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/ls/test_ls.py` & `dvc-2.9.5/tests/unit/command/ls/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/ls/test_ls_colors.py` & `dvc-2.9.5/tests/unit/command/ls/test_ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_add.py` & `dvc-2.9.5/tests/unit/command/test_add.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_cache.py` & `dvc-2.9.5/tests/unit/command/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_checkout.py` & `dvc-2.9.5/tests/unit/command/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_compat_flag.py` & `dvc-2.9.5/tests/unit/command/test_compat_flag.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_config.py` & `dvc-2.9.5/tests/unit/command/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_dag.py` & `dvc-2.9.5/tests/unit/command/test_dag.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_data_sync.py` & `dvc-2.9.5/tests/unit/command/test_data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_debug.py` & `dvc-2.9.5/tests/unit/command/test_debug.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_diff.py` & `dvc-2.9.5/tests/unit/command/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_experiments.py` & `dvc-2.9.5/tests/unit/command/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_get.py` & `dvc-2.9.5/tests/unit/command/test_get.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_git_hook.py` & `dvc-2.9.5/tests/unit/command/test_git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_imp.py` & `dvc-2.9.5/tests/unit/command/test_imp.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_imp_url.py` & `dvc-2.9.5/tests/unit/command/test_imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_live.py` & `dvc-2.9.5/tests/unit/command/test_live.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_machine.py` & `dvc-2.9.5/tests/unit/command/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_metrics.py` & `dvc-2.9.5/tests/unit/command/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_params.py` & `dvc-2.9.5/tests/unit/command/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_plots.py` & `dvc-2.9.5/tests/unit/command/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_repro.py` & `dvc-2.9.5/tests/unit/command/test_repro.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_run.py` & `dvc-2.9.5/tests/unit/command/test_run.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_stage.py` & `dvc-2.9.5/tests/unit/command/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_status.py` & `dvc-2.9.5/tests/unit/command/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/command/test_update.py` & `dvc-2.9.5/tests/unit/command/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/dependency/test_params.py` & `dvc-2.9.5/tests/unit/dependency/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/fs/test_azure.py` & `dvc-2.9.5/tests/unit/fs/test_azure.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/fs/test_dvc.py` & `dvc-2.9.5/tests/unit/fs/test_dvc.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,28 @@
 from dvc.config import NoRemoteError
 from dvc.data.stage import stage
 from dvc.fs.dvc import DvcFileSystem
 from dvc.hash_info import HashInfo
 from dvc.utils.fs import remove
 
 
+@pytest.mark.parametrize(
+    "path, key",
+    [
+        ("", ("repo",)),
+        (".", ("repo",)),
+        ("foo", ("repo", "foo")),
+        (os.path.join("dir", "foo"), ("repo", "dir", "foo")),
+    ],
+)
+def test_get_key(tmp_dir, dvc, path, key):
+    fs = DvcFileSystem(repo=dvc)
+    assert fs._get_key(path) == key
+
+
 def test_exists(tmp_dir, dvc):
     tmp_dir.gen("foo", "foo")
     dvc.add("foo")
     (tmp_dir / "foo").unlink()
 
     fs = DvcFileSystem(repo=dvc)
     assert fs.exists("foo")
@@ -177,34 +191,27 @@
         for entry in dirs + files:
             actual.append(os.path.join(root, entry))
 
     assert set(actual) == set(expected)
     assert len(actual) == len(expected)
 
 
-def test_walk_onerror(tmp_dir, dvc):
-    def onerror(exc):
-        raise exc
-
-    tmp_dir.dvc_gen("foo", "foo")
+def test_walk_missing(tmp_dir, dvc):
     fs = DvcFileSystem(repo=dvc)
 
-    # path does not exist
     for _ in fs.walk("dir"):
         pass
-    with pytest.raises(OSError):
-        for _ in fs.walk("dir", onerror=onerror):
-            pass
 
-    # path is not a directory
+
+def test_walk_not_a_dir(tmp_dir, dvc):
+    tmp_dir.dvc_gen("foo", "foo")
+    fs = DvcFileSystem(repo=dvc)
+
     for _ in fs.walk("foo"):
         pass
-    with pytest.raises(OSError):
-        for _ in fs.walk("foo", onerror=onerror):
-            pass
 
 
 def test_isdvc(tmp_dir, dvc):
     tmp_dir.gen({"foo": "foo", "bar": "bar"})
     dvc.add("foo")
     fs = DvcFileSystem(repo=dvc)
     assert fs.isdvc("foo")
```

### Comparing `dvc-2.9.4/tests/unit/fs/test_fs.py` & `dvc-2.9.5/tests/unit/fs/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/fs/test_path.py` & `dvc-2.9.5/tests/unit/fs/test_path.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/fs/test_repo.py` & `dvc-2.9.5/tests/unit/fs/test_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,34 +287,27 @@
         for entry in dirs + files:
             actual.append(os.path.join(root, entry))
 
     assert set(actual) == set(expected)
     assert len(actual) == len(expected)
 
 
-def test_walk_onerror(tmp_dir, dvc):
-    def onerror(exc):
-        raise exc
-
-    tmp_dir.dvc_gen("foo", "foo")
+def test_walk_missing(tmp_dir, dvc):
     fs = RepoFileSystem(repo=dvc)
 
-    # path does not exist
     for _ in fs.walk("dir"):
         pass
-    with pytest.raises(OSError):
-        for _ in fs.walk("dir", onerror=onerror):
-            pass
 
-    # path is not a directory
+
+def test_walk_not_a_dir(tmp_dir, dvc):
+    tmp_dir.dvc_gen("foo", "foo")
+    fs = RepoFileSystem(repo=dvc)
+
     for _ in fs.walk("foo"):
         pass
-    with pytest.raises(OSError):
-        for _ in fs.walk("foo", onerror=onerror):
-            pass
 
 
 def test_isdvc(tmp_dir, dvc):
     tmp_dir.gen({"foo": "foo", "bar": "bar", "dir": {"baz": "baz"}})
     dvc.add("foo")
     dvc.add("dir")
     fs = RepoFileSystem(repo=dvc)
```

### Comparing `dvc-2.9.4/tests/unit/fs/test_repo_info.py` & `dvc-2.9.5/tests/unit/fs/test_repo_info.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/fs/test_s3.py` & `dvc-2.9.5/tests/unit/fs/test_s3.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/fs/test_ssh.py` & `dvc-2.9.5/tests/unit/fs/test_ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/fs/test_tree.py` & `dvc-2.9.5/tests/unit/fs/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/machine/test_machine.py` & `dvc-2.9.5/tests/unit/machine/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/objects/db/test_local.py` & `dvc-2.9.5/tests/unit/objects/db/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/objects/test_tree.py` & `dvc-2.9.5/tests/unit/objects/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/output/test_load.py` & `dvc-2.9.5/tests/unit/output/test_load.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/output/test_local.py` & `dvc-2.9.5/tests/unit/output/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/output/test_output.py` & `dvc-2.9.5/tests/unit/output/test_output.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/proc/test_manager.py` & `dvc-2.9.5/tests/unit/proc/test_manager.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/proc/test_process.py` & `dvc-2.9.5/tests/unit/proc/test_process.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/remote/test_base.py` & `dvc-2.9.5/tests/unit/remote/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
     with mock.patch.object(odb, "_list_hashes", return_value=list(range(256))):
         hashes = list(range(1000000))
         odb.hashes_exist(hashes)
         object_exists.assert_not_called()
         traverse.assert_called_with(
             256 * pow(16, odb.fs.TRAVERSE_PREFIX_LEN),
             set(range(256)),
-            None,
-            None,
+            jobs=None,
+            name=None,
         )
 
 
 @mock.patch.object(ObjectDB, "_list_hashes", return_value=[])
 @mock.patch.object(ObjectDB, "_path_to_hash", side_effect=lambda x: x)
 def test_list_hashes_traverse(_path_to_hash, list_hashes, dvc):
     odb = ObjectDB(FileSystem(), None)
```

### Comparing `dvc-2.9.4/tests/unit/remote/test_gdrive.py` & `dvc-2.9.5/tests/unit/remote/test_gdrive.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/remote/test_http.py` & `dvc-2.9.5/tests/unit/remote/test_http.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/remote/test_index.py` & `dvc-2.9.5/tests/unit/remote/test_index.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/remote/test_oss.py` & `dvc-2.9.5/tests/unit/remote/test_oss.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/remote/test_remote.py` & `dvc-2.9.5/tests/unit/remote/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/remote/test_slow_link_detection.py` & `dvc-2.9.5/tests/unit/remote/test_slow_link_detection.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/remote/test_webdav.py` & `dvc-2.9.5/tests/unit/remote/test_webdav.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/remote/test_webhdfs.py` & `dvc-2.9.5/tests/unit/remote/test_webhdfs.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/render/test_data.py` & `dvc-2.9.5/tests/unit/render/test_data.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/render/test_html.py` & `dvc-2.9.5/tests/unit/render/test_html.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/render/test_image.py` & `dvc-2.9.5/tests/unit/render/test_image.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/render/test_parallel_coordinates.py` & `dvc-2.9.5/tests/unit/render/test_parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/render/test_render.py` & `dvc-2.9.5/tests/unit/render/test_render.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/render/test_vega.py` & `dvc-2.9.5/tests/unit/render/test_vega.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/repo/experiments/test_utils.py` & `dvc-2.9.5/tests/unit/repo/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/repo/plots/test_diff.py` & `dvc-2.9.5/tests/unit/repo/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/repo/plots/test_templates.py` & `dvc-2.9.5/tests/unit/repo/plots/test_templates.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/repo/test_repo.py` & `dvc-2.9.5/tests/unit/repo/test_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/repo/test_reproduce.py` & `dvc-2.9.5/tests/unit/repo/test_reproduce.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/repo/test_scm_context.py` & `dvc-2.9.5/tests/unit/repo/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/scm/test_scm.py` & `dvc-2.9.5/tests/unit/scm/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/stage/test_cache.py` & `dvc-2.9.5/tests/unit/stage/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/stage/test_loader_pipeline_file.py` & `dvc-2.9.5/tests/unit/stage/test_loader_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/stage/test_run.py` & `dvc-2.9.5/tests/unit/stage/test_run.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/stage/test_serialize_pipeline_file.py` & `dvc-2.9.5/tests/unit/stage/test_serialize_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/stage/test_serialize_pipeline_lock.py` & `dvc-2.9.5/tests/unit/stage/test_serialize_pipeline_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/stage/test_stage.py` & `dvc-2.9.5/tests/unit/stage/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/stage/test_utils.py` & `dvc-2.9.5/tests/unit/stage/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_analytics.py` & `dvc-2.9.5/tests/unit/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_compare.py` & `dvc-2.9.5/tests/unit/test_compare.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_config.py` & `dvc-2.9.5/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_context.py` & `dvc-2.9.5/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_daemon.py` & `dvc-2.9.5/tests/unit/test_daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_dvcfile.py` & `dvc-2.9.5/tests/unit/test_dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_external_repo.py` & `dvc-2.9.5/tests/unit/test_external_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_ignore.py` & `dvc-2.9.5/tests/unit/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_imports.py` & `dvc-2.9.5/tests/unit/test_imports.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_info.py` & `dvc-2.9.5/tests/unit/test_info.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_interpolate.py` & `dvc-2.9.5/tests/unit/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_lockfile.py` & `dvc-2.9.5/tests/unit/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_logger.py` & `dvc-2.9.5/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_metrics.py` & `dvc-2.9.5/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_params.py` & `dvc-2.9.5/tests/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_pathspec_math.py` & `dvc-2.9.5/tests/unit/test_pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_plots.py` & `dvc-2.9.5/tests/unit/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_progress.py` & `dvc-2.9.5/tests/unit/test_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_rwlock.py` & `dvc-2.9.5/tests/unit/test_rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_tabular_data.py` & `dvc-2.9.5/tests/unit/test_tabular_data.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/test_updater.py` & `dvc-2.9.5/tests/unit/test_updater.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/ui/test_console.py` & `dvc-2.9.5/tests/unit/ui/test_console.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/ui/test_pager.py` & `dvc-2.9.5/tests/unit/ui/test_pager.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/ui/test_prompt.py` & `dvc-2.9.5/tests/unit/ui/test_prompt.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/ui/test_table.py` & `dvc-2.9.5/tests/unit/ui/test_table.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/utils/serialize/test_python.py` & `dvc-2.9.5/tests/unit/utils/serialize/test_python.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/utils/serialize/test_yaml.py` & `dvc-2.9.5/tests/unit/utils/serialize/test_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/utils/test_cli_parse.py` & `dvc-2.9.5/tests/unit/utils/test_cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/utils/test_collections.py` & `dvc-2.9.5/tests/unit/utils/test_collections.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/utils/test_conversions.py` & `dvc-2.9.5/tests/unit/utils/test_conversions.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/utils/test_decorators.py` & `dvc-2.9.5/tests/unit/utils/test_decorators.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/utils/test_fs.py` & `dvc-2.9.5/tests/unit/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/utils/test_humanize.py` & `dvc-2.9.5/tests/unit/utils/test_humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/utils/test_stream.py` & `dvc-2.9.5/tests/unit/utils/test_stream.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/unit/utils/test_utils.py` & `dvc-2.9.5/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/utils/__init__.py` & `dvc-2.9.5/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/utils/asserts.py` & `dvc-2.9.5/tests/utils/asserts.py`

 * *Files identical despite different names*

### Comparing `dvc-2.9.4/tests/utils/scriptify.py` & `dvc-2.9.5/tests/utils/scriptify.py`

 * *Files identical despite different names*

