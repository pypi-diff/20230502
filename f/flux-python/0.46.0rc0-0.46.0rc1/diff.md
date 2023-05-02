# Comparing `tmp/flux-python-0.46.0rc0.tar.gz` & `tmp/flux-python-0.46.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-python-0.46.0rc0.tar", last modified: Tue May  2 13:16:43 2023, max compression
+gzip compressed data, was "flux-python-0.46.0rc1.tar", last modified: Tue May  2 13:27:35 2023, max compression
```

## Comparing `flux-python-0.46.0rc0.tar` & `flux-python-0.46.0rc1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.605673 flux-python-0.46.0rc0/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      186 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)      741 2023-05-02 13:16:43.605673 flux-python-0.46.0rc0/PKG-INFO
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3702 2023-05-02 13:14:19.000000 flux-python-0.46.0rc0/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.589673 flux-python-0.46.0rc0/flux/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/.gitignore
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26956 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26465 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/Makefile.in
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      668 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.589673 flux-python-0.46.0rc0/flux/cli/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    27800 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/cli/_fortune.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      754 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/constants.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.589673 flux-python-0.46.0rc0/flux/constraint/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17451 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/constraint/parser.out
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2862 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/constraint/parsetab.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.589673 flux-python-0.46.0rc0/flux/core/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/core/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    12153 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/core/handle.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      815 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/core/inner.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1309 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/core/trampoline.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     5167 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/core/watchers.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      567 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/debugged.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7721 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/future.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6219 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/hostlist.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    10040 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/idset.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1674 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/importer.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.593673 flux-python-0.46.0rc0/flux/job/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3059 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/JobID.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    35872 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/Jobspec.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1189 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      597 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/_wrapper.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7170 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/event.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    26007 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/executor.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.593673 flux-python-0.46.0rc0/flux/job/frobnicator/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      460 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/frobnicator/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4929 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/frobnicator/frobnicator.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.593673 flux-python-0.46.0rc0/flux/job/frobnicator/plugins/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1938 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/frobnicator/plugins/constraints.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3088 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/frobnicator/plugins/defaults.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    21558 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/info.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2449 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/kill.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1104 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/kvs.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    10098 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/list.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3580 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/stats.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4598 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/submit.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.593673 flux-python-0.46.0rc0/flux/job/validator/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      452 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/validator/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.597673 flux-python-0.46.0rc0/flux/job/validator/plugins/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1710 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/validator/plugins/feasibility.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1755 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/validator/plugins/jobspec.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1427 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/validator/plugins/require-instance.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1408 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/validator/plugins/schema.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7594 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/validator/validator.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6988 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/job/wait.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     9456 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/kvs.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2629 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/memoized_property.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     5394 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/message.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    11771 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/progress.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.597673 flux-python-0.46.0rc0/flux/resource/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7954 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/resource/ResourceSet.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2767 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/resource/ResourceSetImplementation.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4408 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/resource/Rlist.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      533 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/resource/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2663 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/resource/list.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2474 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/rpc.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3691 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/security.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.597673 flux-python-0.46.0rc0/flux/uri/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      470 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/uri/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.597673 flux-python-0.46.0rc0/flux/uri/resolvers/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2490 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/uri/resolvers/jobid.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3468 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/uri/resolvers/lsf.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3916 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/uri/resolvers/pid.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3357 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/uri/resolvers/slurm.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6461 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/uri/uri.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    36871 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/util.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.597673 flux-python-0.46.0rc0/flux/utils/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      201 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.597673 flux-python-0.46.0rc0/flux/utils/parsedatetime/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)   105234 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4652 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/context.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       61 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/parsedatetime.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.601673 flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      719 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4611 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/base.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3130 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      380 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/en_AU.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      157 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/en_US.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      959 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/es.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6090 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4566 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2998 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1128 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4577 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      485 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/parsedatetime/warns.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.601673 flux-python-0.46.0rc0/flux/utils/tomli/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1072 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/tomli/LICENSE
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      294 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/tomli/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    21649 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/tomli/_parser.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2813 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/tomli/_re.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      126 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/tomli/_types.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       26 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/utils/tomli/py.typed
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    12713 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/flux/wrapper.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.601673 flux-python-0.46.0rc0/flux_python.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      741 2023-05-02 13:16:43.000000 flux-python-0.46.0rc0/flux_python.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2825 2023-05-02 13:16:43.000000 flux-python-0.46.0rc0/flux_python.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 13:16:43.000000 flux-python-0.46.0rc0/flux_python.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 13:16:43.000000 flux-python-0.46.0rc0/flux_python.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       58 2023-05-02 13:16:43.000000 flux-python-0.46.0rc0/flux_python.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       15 2023-05-02 13:16:43.000000 flux-python-0.46.0rc0/flux_python.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-02 13:16:43.605673 flux-python-0.46.0rc0/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    13761 2023-05-02 13:16:41.000000 flux-python-0.46.0rc0/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:16:43.605673 flux-python-0.46.0rc0/src/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/src/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1386 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/src/_core_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)   134746 2023-05-02 13:16:34.000000 flux-python-0.46.0rc0/src/_core_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)    54595 2023-05-02 13:16:34.000000 flux-python-0.46.0rc0/src/_core_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1241 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/src/_hostlist_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4739 2023-05-02 13:16:34.000000 flux-python-0.46.0rc0/src/_hostlist_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1524 2023-05-02 13:16:34.000000 flux-python-0.46.0rc0/src/_hostlist_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1667 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/src/_idset_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4483 2023-05-02 13:16:34.000000 flux-python-0.46.0rc0/src/_idset_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1876 2023-05-02 13:16:34.000000 flux-python-0.46.0rc0/src/_idset_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2177 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/src/_rlist_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    21389 2023-05-02 13:16:34.000000 flux-python-0.46.0rc0/src/_rlist_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4552 2023-05-02 13:16:34.000000 flux-python-0.46.0rc0/src/_rlist_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1533 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/src/_security_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5186 2023-05-02 13:16:34.000000 flux-python-0.46.0rc0/src/_security_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2048 2023-05-02 13:16:34.000000 flux-python-0.46.0rc0/src/_security_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      516 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/src/callbacks.h
--rwxrwxr-x   0 vscode    (1000) vscode    (1000)     2804 2023-05-02 05:33:04.000000 flux-python-0.46.0rc0/src/make_clean_header.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.104492 flux-python-0.46.0rc1/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      186 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6099 2023-05-02 13:27:35.104492 flux-python-0.46.0rc1/PKG-INFO
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4317 2023-05-02 13:27:21.000000 flux-python-0.46.0rc1/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.092492 flux-python-0.46.0rc1/flux/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/.gitignore
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26956 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26465 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/Makefile.in
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      668 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.092492 flux-python-0.46.0rc1/flux/cli/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    27800 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/cli/_fortune.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      754 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/constants.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.092492 flux-python-0.46.0rc1/flux/constraint/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17451 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/constraint/parser.out
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2862 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/constraint/parsetab.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.092492 flux-python-0.46.0rc1/flux/core/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/core/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    12153 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/core/handle.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      815 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/core/inner.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1309 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/core/trampoline.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     5167 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/core/watchers.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      567 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/debugged.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7721 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/future.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6219 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/hostlist.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    10040 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/idset.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1674 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/importer.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/job/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3059 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/JobID.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    35872 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/Jobspec.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1189 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      597 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/_wrapper.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7170 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/event.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    26007 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/executor.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/job/frobnicator/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      460 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/frobnicator/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4929 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/frobnicator/frobnicator.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/job/frobnicator/plugins/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1938 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/frobnicator/plugins/constraints.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3088 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/frobnicator/plugins/defaults.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    21558 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/info.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2449 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/kill.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1104 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/kvs.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    10098 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/list.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3580 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/stats.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4598 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/submit.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/job/validator/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      452 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/validator/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/job/validator/plugins/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1710 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/validator/plugins/feasibility.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1755 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/validator/plugins/jobspec.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1427 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/validator/plugins/require-instance.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1408 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/validator/plugins/schema.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7594 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/validator/validator.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6988 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/wait.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     9456 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/kvs.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2629 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/memoized_property.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     5394 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/message.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    11771 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/progress.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/resource/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7954 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/resource/ResourceSet.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2767 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/resource/ResourceSetImplementation.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4408 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/resource/Rlist.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      533 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/resource/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2663 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/resource/list.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2474 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/rpc.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3691 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/security.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/uri/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      470 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/uri/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/uri/resolvers/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2490 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/uri/resolvers/jobid.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3468 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/uri/resolvers/lsf.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3916 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/uri/resolvers/pid.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3357 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/uri/resolvers/slurm.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6461 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/uri/uri.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    36871 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/util.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/utils/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      201 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.100492 flux-python-0.46.0rc1/flux/utils/parsedatetime/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)   105234 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4652 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/context.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       61 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/parsedatetime.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.100492 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      719 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4611 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/base.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3130 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/de_DE.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      380 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/en_AU.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      157 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/en_US.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      959 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/es.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6090 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/fr_FR.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4566 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/icu.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2998 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/nl_NL.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1128 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/pt_BR.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4577 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/ru_RU.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      485 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/warns.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.100492 flux-python-0.46.0rc1/flux/utils/tomli/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1072 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/tomli/LICENSE
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      294 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/tomli/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    21649 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/tomli/_parser.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2813 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/tomli/_re.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      126 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/tomli/_types.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       26 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/tomli/py.typed
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    12713 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/wrapper.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.104492 flux-python-0.46.0rc1/flux_python.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6099 2023-05-02 13:27:35.000000 flux-python-0.46.0rc1/flux_python.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2825 2023-05-02 13:27:35.000000 flux-python-0.46.0rc1/flux_python.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 13:27:35.000000 flux-python-0.46.0rc1/flux_python.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 13:16:43.000000 flux-python-0.46.0rc1/flux_python.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       58 2023-05-02 13:27:35.000000 flux-python-0.46.0rc1/flux_python.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       15 2023-05-02 13:27:35.000000 flux-python-0.46.0rc1/flux_python.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-02 13:27:35.104492 flux-python-0.46.0rc1/setup.cfg
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    14019 2023-05-02 13:23:29.000000 flux-python-0.46.0rc1/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.104492 flux-python-0.46.0rc1/src/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1386 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/_core_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   134746 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_core_clean.h
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    54595 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_core_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1241 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/_hostlist_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4739 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_hostlist_clean.h
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1524 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_hostlist_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1667 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/_idset_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4483 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_idset_clean.h
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1876 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_idset_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2177 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/_rlist_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    21389 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_rlist_clean.h
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4552 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_rlist_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1533 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/_security_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5186 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_security_clean.h
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2048 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_security_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      516 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/callbacks.h
+-rwxrwxr-x   0 vscode    (1000) vscode    (1000)     2804 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/make_clean_header.py
```

### Comparing `flux-python-0.46.0rc0/README.md` & `flux-python-0.46.0rc1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,56 @@
 # Flux Python Bindings
 
+> 🐍️ You called me?
+
 Hello! You've found the flux Python bindings, an experiment to build and deploy
 Flux to Pypi without needing to store code alongside Flux. The goal of
 this experiment is to test them separately. This was originally developed
 at [vsoch/flux-python](https://github.com/vsoch/flux-python) and has 
-been ported here to automate more officially.
+been ported here to automate more officially. The following guides might be useful
+to you:
 
+ - ⭐️ [Flux Framework Documentation](https://flux-framework.readthedocs.io)
+ - ⭐️ [Flux Projects](https://flux-framework.org)
+ - ⭐️ [Tutorials](https://flux-framework.readthedocs.io/en/latest/tutorials/index.html)
+ 
+ 
 ## Development
 
-We provide a [.devcontainer](.devcontainer) environment you can open in VSCode
+We provide a [.devcontainer](https://github.com/flux-framework/flux-python/tree/main/.devcontainer) environment you can open in VSCode
 to have an environment ready to go with Flux (and Flux Security). You can follow
 the instructions in the DevContainer to build the Flux Python bindings.
+By default, this environment installs the latest flux-core.
+If you want to build a custom version with Flux core you can do:
+
+```bash
+rm -rf ~/flux-core
+export FLUX_VERSION=0.46.0
+wget https://github.com/flux-framework/flux-core/releases/download/v${FLUX_VERSION}/flux-core-${FLUX_VERSION}.tar.gz
+tar -xzvf flux-core-${FLUX_VERSION}.tar.gz
+sudo mv flux-core-${FLUX_VERSION} ~/flux-core
+rm flux-core-${FLUX_VERSION}.tar.gz
+cd ~/flux-core
+./configure --prefix=/usr/local
+make
+sudo make install
+```
+
+And then build your custom wheel:
+
+```bash
+$ cd /workspaces/flux-python
+$ python3 setup.py sdist bdist_wheel --flux-root /home/vscode/flux-core --security-src /home/vscode/security --security-include /usr/local/include/flux/security --version 0.46.0-rc-0
+```
+
+And if you want to upload:
+
+```bash
+$ twine upload dist/*.tar.gz
+```
 
 ### Building Modules
 
 We will need to build the tarball providing paths to the flux-core and flux-security
 sources. This can be improved upon to just be one path if all the dependencies
 are provided with the flux install (and we don't need the source). Note
 that we also provide a custom version for the pypi package:
@@ -50,19 +86,14 @@
 $ ipython
 ```
 ```python
 import flux
 flux.Flux()
 ```
 
-More coming soon! We still need to:
-
- - [ ] some version checking
- - [ ] ability to build .tar.gz (needed flux deps to be removed)
-
 ### Automation
 
 In order to (eventually) support a workflow to check for a release, get the release's
 flux assets and build, we have a [workflow script](.github/scripts/check_releases.py) that will:
 
 - Get the latest flux releases
 - Compare to the latest pypi releases
@@ -75,43 +106,21 @@
 $ export GITHUB_TOKEN=xxxxxxxxxxxxx
 $ python .github/scripts/check_releases.py flux-framework --version 0.46.0
 ```
 
 That basically checks if there should be a build. It will use the container provided
 here to install a custom version of flux core that builds the release.
 
-#### DevContainer
-
-We provide a Development Container for VSCode, and if you want to build a custom version 
-with Flux core you can do:
-
-```bash
-rm -rf ~/flux-core
-export FLUX_VERSION=0.46.0
-wget https://github.com/flux-framework/flux-core/releases/download/v${FLUX_VERSION}/flux-core-${FLUX_VERSION}.tar.gz
-tar -xzvf flux-core-${FLUX_VERSION}.tar.gz
-sudo mv flux-core-${FLUX_VERSION} ~/flux-core
-rm flux-core-${FLUX_VERSION}.tar.gz
-cd ~/flux-core
-./configure --prefix=/usr/local
-make
-sudo make install
-```
-
-And then build your custom wheel:
+### Work in Progress
 
-```bash
-$ cd /workspaces/flux-python
-$ python3 setup.py sdist bdist_wheel --flux-root /home/vscode/flux-core --security-src /home/vscode/security --security-include /usr/local/include/flux/security --version 0.46.0-rc-0
-```
-
-And if you want to upload:
+@vsoch wants to try installing her test releases to a system somewhere, and figure
+out this issue with buidling a wheel (or maybe we don't want wheels after all):
 
-```bash
-$ twine upload dist/*
-```
+> HTTPError: 400 Bad Request from https://upload.pypi.org/legacy/        
+>         Binary wheel 'flux_python-0.46.0rc0-cp38-cp38-linux_x86_64.whl' has an 
+>         unsupported platform tag 'linux_x86_64'. 
 
 #### Release
 
 SPDX-License-Identifier: LGPL-3.0
 
 LLNL-CODE-764420
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flux-python-0.46.0rc0/flux/Makefile` & `flux-python-0.46.0rc1/flux/Makefile`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/Makefile.in` & `flux-python-0.46.0rc1/flux/Makefile.in`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/__init__.py` & `flux-python-0.46.0rc1/flux/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/cli/_fortune.py` & `flux-python-0.46.0rc1/flux/cli/_fortune.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/constants.py` & `flux-python-0.46.0rc1/flux/constants.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/constraint/parser.out` & `flux-python-0.46.0rc1/flux/constraint/parser.out`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/constraint/parsetab.py` & `flux-python-0.46.0rc1/flux/constraint/parsetab.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/core/handle.py` & `flux-python-0.46.0rc1/flux/core/handle.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/core/inner.py` & `flux-python-0.46.0rc1/flux/core/inner.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/core/trampoline.py` & `flux-python-0.46.0rc1/flux/core/trampoline.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/core/watchers.py` & `flux-python-0.46.0rc1/flux/core/watchers.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/debugged.py` & `flux-python-0.46.0rc1/flux/debugged.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/future.py` & `flux-python-0.46.0rc1/flux/future.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/hostlist.py` & `flux-python-0.46.0rc1/flux/hostlist.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/idset.py` & `flux-python-0.46.0rc1/flux/idset.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/importer.py` & `flux-python-0.46.0rc1/flux/importer.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/JobID.py` & `flux-python-0.46.0rc1/flux/job/JobID.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/Jobspec.py` & `flux-python-0.46.0rc1/flux/job/Jobspec.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/__init__.py` & `flux-python-0.46.0rc1/flux/job/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/_wrapper.py` & `flux-python-0.46.0rc1/flux/job/_wrapper.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/event.py` & `flux-python-0.46.0rc1/flux/job/event.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/executor.py` & `flux-python-0.46.0rc1/flux/job/executor.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/frobnicator/frobnicator.py` & `flux-python-0.46.0rc1/flux/job/frobnicator/frobnicator.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/frobnicator/plugins/constraints.py` & `flux-python-0.46.0rc1/flux/job/frobnicator/plugins/constraints.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/frobnicator/plugins/defaults.py` & `flux-python-0.46.0rc1/flux/job/frobnicator/plugins/defaults.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/info.py` & `flux-python-0.46.0rc1/flux/job/info.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/kill.py` & `flux-python-0.46.0rc1/flux/job/kill.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/kvs.py` & `flux-python-0.46.0rc1/flux/job/kvs.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/list.py` & `flux-python-0.46.0rc1/flux/job/list.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/stats.py` & `flux-python-0.46.0rc1/flux/job/stats.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/submit.py` & `flux-python-0.46.0rc1/flux/job/submit.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/validator/plugins/feasibility.py` & `flux-python-0.46.0rc1/flux/job/validator/plugins/feasibility.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/validator/plugins/jobspec.py` & `flux-python-0.46.0rc1/flux/job/validator/plugins/jobspec.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/validator/plugins/require-instance.py` & `flux-python-0.46.0rc1/flux/job/validator/plugins/require-instance.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/validator/plugins/schema.py` & `flux-python-0.46.0rc1/flux/job/validator/plugins/schema.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/validator/validator.py` & `flux-python-0.46.0rc1/flux/job/validator/validator.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/job/wait.py` & `flux-python-0.46.0rc1/flux/job/wait.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/kvs.py` & `flux-python-0.46.0rc1/flux/kvs.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/memoized_property.py` & `flux-python-0.46.0rc1/flux/memoized_property.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/message.py` & `flux-python-0.46.0rc1/flux/message.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/progress.py` & `flux-python-0.46.0rc1/flux/progress.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/resource/ResourceSet.py` & `flux-python-0.46.0rc1/flux/resource/ResourceSet.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/resource/ResourceSetImplementation.py` & `flux-python-0.46.0rc1/flux/resource/ResourceSetImplementation.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/resource/Rlist.py` & `flux-python-0.46.0rc1/flux/resource/Rlist.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/resource/__init__.py` & `flux-python-0.46.0rc1/flux/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/resource/list.py` & `flux-python-0.46.0rc1/flux/resource/list.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/rpc.py` & `flux-python-0.46.0rc1/flux/rpc.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/security.py` & `flux-python-0.46.0rc1/flux/security.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/uri/resolvers/jobid.py` & `flux-python-0.46.0rc1/flux/uri/resolvers/jobid.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/uri/resolvers/lsf.py` & `flux-python-0.46.0rc1/flux/uri/resolvers/lsf.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/uri/resolvers/pid.py` & `flux-python-0.46.0rc1/flux/uri/resolvers/pid.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/uri/resolvers/slurm.py` & `flux-python-0.46.0rc1/flux/uri/resolvers/slurm.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/uri/uri.py` & `flux-python-0.46.0rc1/flux/uri/uri.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/util.py` & `flux-python-0.46.0rc1/flux/util.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/parsedatetime/__init__.py` & `flux-python-0.46.0rc1/flux/utils/parsedatetime/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/parsedatetime/context.py` & `flux-python-0.46.0rc1/flux/utils/parsedatetime/context.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py` & `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/base.py` & `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/base.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py` & `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/de_DE.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/es.py` & `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/es.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py` & `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/fr_FR.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py` & `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/icu.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py` & `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/nl_NL.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py` & `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/pt_BR.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py` & `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/ru_RU.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/tomli/LICENSE` & `flux-python-0.46.0rc1/flux/utils/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/tomli/_parser.py` & `flux-python-0.46.0rc1/flux/utils/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/utils/tomli/_re.py` & `flux-python-0.46.0rc1/flux/utils/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux/wrapper.py` & `flux-python-0.46.0rc1/flux/wrapper.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/flux_python.egg-info/SOURCES.txt` & `flux-python-0.46.0rc1/flux_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/setup.py` & `flux-python-0.46.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,20 @@
 # Metadata
 package_name = "flux-python"
 package_version = "0.46.0"
 package_description = "Python bindings for the flux resource manager API"
 package_url = "https://github.com/flux-framework/flux-python"
 package_keywords = "flux, job manager, orchestration, hpc"
 
+try:
+    with open("README.md") as filey:
+        package_long_description = filey.read()
+except Exception:
+    package_long_description = description
+
 # Setup variables for dependencies
 cffi_dep = "cffi>=1.1"
 
 # src/bindings/python
 here = os.path.dirname(os.path.abspath(__file__))
 
 # top level with src, etc (/code here)
@@ -422,14 +428,16 @@
 
     # This assumes relative location of Flux install
     # Now with cffi for final install
     _setup(
         name=package_name,
         version=package_version,
         description=package_description,
+        long_description=package_long_description,
+        long_description_content_type="text/markdown",
         keywords=package_keywords,
         url=package_url,
         setup_requires=[cffi_dep],
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         install_requires=[cffi_dep],
```

### Comparing `flux-python-0.46.0rc0/src/_core_build.py` & `flux-python-0.46.0rc1/src/_core_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_core_clean.h` & `flux-python-0.46.0rc1/src/_core_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_core_preproc.h` & `flux-python-0.46.0rc1/src/_core_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_hostlist_build.py` & `flux-python-0.46.0rc1/src/_hostlist_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_hostlist_clean.h` & `flux-python-0.46.0rc1/src/_hostlist_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_hostlist_preproc.h` & `flux-python-0.46.0rc1/src/_hostlist_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_idset_build.py` & `flux-python-0.46.0rc1/src/_idset_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_idset_clean.h` & `flux-python-0.46.0rc1/src/_idset_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_idset_preproc.h` & `flux-python-0.46.0rc1/src/_idset_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_rlist_build.py` & `flux-python-0.46.0rc1/src/_rlist_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_rlist_clean.h` & `flux-python-0.46.0rc1/src/_rlist_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_rlist_preproc.h` & `flux-python-0.46.0rc1/src/_rlist_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_security_build.py` & `flux-python-0.46.0rc1/src/_security_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_security_clean.h` & `flux-python-0.46.0rc1/src/_security_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/_security_preproc.h` & `flux-python-0.46.0rc1/src/_security_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/callbacks.h` & `flux-python-0.46.0rc1/src/callbacks.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc0/src/make_clean_header.py` & `flux-python-0.46.0rc1/src/make_clean_header.py`

 * *Files identical despite different names*

