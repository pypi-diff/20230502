# Comparing `tmp/flux-python-0.46.0rc1.tar.gz` & `tmp/flux-python-0.48.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-python-0.46.0rc1.tar", last modified: Tue May  2 13:27:35 2023, max compression
+gzip compressed data, was "flux-python-0.48.0rc0.tar", last modified: Tue May  2 18:24:22 2023, max compression
```

## Comparing `flux-python-0.46.0rc1.tar` & `flux-python-0.48.0rc0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.104492 flux-python-0.46.0rc1/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      186 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6099 2023-05-02 13:27:35.104492 flux-python-0.46.0rc1/PKG-INFO
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4317 2023-05-02 13:27:21.000000 flux-python-0.46.0rc1/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.092492 flux-python-0.46.0rc1/flux/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/.gitignore
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26956 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26465 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/Makefile.in
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      668 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.092492 flux-python-0.46.0rc1/flux/cli/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    27800 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/cli/_fortune.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      754 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/constants.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.092492 flux-python-0.46.0rc1/flux/constraint/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17451 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/constraint/parser.out
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2862 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/constraint/parsetab.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.092492 flux-python-0.46.0rc1/flux/core/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/core/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    12153 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/core/handle.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      815 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/core/inner.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1309 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/core/trampoline.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     5167 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/core/watchers.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      567 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/debugged.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7721 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/future.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6219 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/hostlist.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    10040 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/idset.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1674 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/importer.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/job/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3059 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/JobID.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    35872 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/Jobspec.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1189 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      597 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/_wrapper.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7170 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/event.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    26007 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/executor.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/job/frobnicator/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      460 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/frobnicator/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4929 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/frobnicator/frobnicator.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/job/frobnicator/plugins/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1938 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/frobnicator/plugins/constraints.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3088 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/frobnicator/plugins/defaults.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    21558 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/info.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2449 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/kill.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1104 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/kvs.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    10098 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/list.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3580 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/stats.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4598 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/submit.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/job/validator/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      452 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/validator/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/job/validator/plugins/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1710 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/validator/plugins/feasibility.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1755 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/validator/plugins/jobspec.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1427 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/validator/plugins/require-instance.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1408 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/validator/plugins/schema.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7594 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/validator/validator.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6988 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/job/wait.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     9456 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/kvs.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2629 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/memoized_property.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     5394 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/message.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    11771 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/progress.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/resource/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7954 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/resource/ResourceSet.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2767 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/resource/ResourceSetImplementation.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4408 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/resource/Rlist.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      533 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/resource/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2663 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/resource/list.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2474 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/rpc.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3691 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/security.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/uri/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      470 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/uri/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/uri/resolvers/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2490 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/uri/resolvers/jobid.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3468 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/uri/resolvers/lsf.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3916 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/uri/resolvers/pid.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3357 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/uri/resolvers/slurm.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6461 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/uri/uri.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    36871 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/util.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.096492 flux-python-0.46.0rc1/flux/utils/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      201 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.100492 flux-python-0.46.0rc1/flux/utils/parsedatetime/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)   105234 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4652 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/context.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       61 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/parsedatetime.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.100492 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      719 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4611 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/base.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3130 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/de_DE.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      380 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/en_AU.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      157 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/en_US.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      959 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/es.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6090 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/fr_FR.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4566 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/icu.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2998 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/nl_NL.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1128 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/pt_BR.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4577 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/ru_RU.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      485 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/parsedatetime/warns.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.100492 flux-python-0.46.0rc1/flux/utils/tomli/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1072 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/tomli/LICENSE
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      294 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/tomli/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    21649 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/tomli/_parser.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2813 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/tomli/_re.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      126 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/tomli/_types.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       26 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/utils/tomli/py.typed
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    12713 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/flux/wrapper.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.104492 flux-python-0.46.0rc1/flux_python.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6099 2023-05-02 13:27:35.000000 flux-python-0.46.0rc1/flux_python.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2825 2023-05-02 13:27:35.000000 flux-python-0.46.0rc1/flux_python.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 13:27:35.000000 flux-python-0.46.0rc1/flux_python.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 13:16:43.000000 flux-python-0.46.0rc1/flux_python.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       58 2023-05-02 13:27:35.000000 flux-python-0.46.0rc1/flux_python.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       15 2023-05-02 13:27:35.000000 flux-python-0.46.0rc1/flux_python.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-02 13:27:35.104492 flux-python-0.46.0rc1/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    14019 2023-05-02 13:23:29.000000 flux-python-0.46.0rc1/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 13:27:35.104492 flux-python-0.46.0rc1/src/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1386 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/_core_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)   134746 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_core_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)    54595 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_core_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1241 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/_hostlist_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4739 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_hostlist_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1524 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_hostlist_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1667 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/_idset_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4483 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_idset_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1876 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_idset_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2177 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/_rlist_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    21389 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_rlist_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4552 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_rlist_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1533 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/_security_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5186 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_security_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2048 2023-05-02 13:27:26.000000 flux-python-0.46.0rc1/src/_security_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      516 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/callbacks.h
--rwxrwxr-x   0 vscode    (1000) vscode    (1000)     2804 2023-05-02 05:33:04.000000 flux-python-0.46.0rc1/src/make_clean_header.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.098467 flux-python-0.48.0rc0/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      186 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6108 2023-05-02 18:24:22.098467 flux-python-0.48.0rc0/PKG-INFO
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4326 2023-05-02 18:19:53.000000 flux-python-0.48.0rc0/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.082467 flux-python-0.48.0rc0/flux/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/.gitignore
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26956 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26465 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/Makefile.in
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      668 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.082467 flux-python-0.48.0rc0/flux/cli/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    27800 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/cli/_fortune.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      754 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/constants.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.082467 flux-python-0.48.0rc0/flux/constraint/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17451 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/constraint/parser.out
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2862 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/constraint/parsetab.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.082467 flux-python-0.48.0rc0/flux/core/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/core/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    12153 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/core/handle.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      815 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/core/inner.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1309 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/core/trampoline.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     5167 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/core/watchers.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      567 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/debugged.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7721 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/future.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6219 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/hostlist.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    10040 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/idset.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1674 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/importer.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.086467 flux-python-0.48.0rc0/flux/job/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3059 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/JobID.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    35872 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/Jobspec.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1189 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      597 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/_wrapper.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7170 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/event.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    26007 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/executor.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.086467 flux-python-0.48.0rc0/flux/job/frobnicator/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      460 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/frobnicator/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4929 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/frobnicator/frobnicator.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.086467 flux-python-0.48.0rc0/flux/job/frobnicator/plugins/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1938 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/frobnicator/plugins/constraints.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3088 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/frobnicator/plugins/defaults.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    21558 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/info.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2449 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/kill.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1104 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/kvs.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    10098 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/list.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3580 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/stats.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4598 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/submit.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.086467 flux-python-0.48.0rc0/flux/job/validator/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      452 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/validator/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.090467 flux-python-0.48.0rc0/flux/job/validator/plugins/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1710 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/validator/plugins/feasibility.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1755 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/validator/plugins/jobspec.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1427 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/validator/plugins/require-instance.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1408 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/validator/plugins/schema.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7594 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/validator/validator.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6988 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/wait.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     9456 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/kvs.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2629 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/memoized_property.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     5394 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/message.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    11771 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/progress.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.090467 flux-python-0.48.0rc0/flux/resource/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7954 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/resource/ResourceSet.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2767 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/resource/ResourceSetImplementation.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4408 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/resource/Rlist.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      533 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/resource/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2663 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/resource/list.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2474 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/rpc.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3691 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/security.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.090467 flux-python-0.48.0rc0/flux/uri/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      470 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/uri/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.090467 flux-python-0.48.0rc0/flux/uri/resolvers/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2490 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/uri/resolvers/jobid.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3468 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/uri/resolvers/lsf.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3916 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/uri/resolvers/pid.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3357 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/uri/resolvers/slurm.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6461 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/uri/uri.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    36871 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/util.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.090467 flux-python-0.48.0rc0/flux/utils/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      201 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.094467 flux-python-0.48.0rc0/flux/utils/parsedatetime/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)   105234 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4652 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/context.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       61 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/parsedatetime.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.094467 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      719 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4611 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/base.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3130 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      380 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/en_AU.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      157 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/en_US.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      959 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/es.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6090 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4566 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2998 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1128 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4577 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      485 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/warns.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.098467 flux-python-0.48.0rc0/flux/utils/tomli/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1072 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/tomli/LICENSE
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      294 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/tomli/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    21649 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/tomli/_parser.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2813 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/tomli/_re.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      126 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/tomli/_types.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       26 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/tomli/py.typed
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    12713 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/wrapper.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.098467 flux-python-0.48.0rc0/flux_python.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6108 2023-05-02 18:24:22.000000 flux-python-0.48.0rc0/flux_python.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2825 2023-05-02 18:24:22.000000 flux-python-0.48.0rc0/flux_python.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 18:24:22.000000 flux-python-0.48.0rc0/flux_python.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 13:16:43.000000 flux-python-0.48.0rc0/flux_python.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       58 2023-05-02 18:24:22.000000 flux-python-0.48.0rc0/flux_python.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       15 2023-05-02 18:24:22.000000 flux-python-0.48.0rc0/flux_python.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-02 18:24:22.098467 flux-python-0.48.0rc0/setup.cfg
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    14019 2023-05-02 14:05:24.000000 flux-python-0.48.0rc0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.098467 flux-python-0.48.0rc0/src/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1386 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/_core_build.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)   134328 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_core_clean.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    54497 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_core_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1241 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/_hostlist_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4739 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_hostlist_clean.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1524 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_hostlist_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1667 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/_idset_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4483 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_idset_clean.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1876 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_idset_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2177 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/_rlist_build.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    21443 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_rlist_clean.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4552 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_rlist_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1533 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/_security_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5186 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_security_clean.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2048 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_security_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      516 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/callbacks.h
+-rwxrwxr-x   0 vscode    (1000) vscode    (1000)     2804 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/make_clean_header.py
```

### Comparing `flux-python-0.46.0rc1/PKG-INFO` & `flux-python-0.48.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-python
-Version: 0.46.0rc1
+Version: 0.48.0rc0
 Summary: Python bindings for the flux resource manager API
 Home-page: https://github.com/flux-framework/flux-python
 License: UNKNOWN
 Description: # Flux Python Bindings
         
         > 🐍️ You called me?
         
@@ -26,30 +26,30 @@
         to have an environment ready to go with Flux (and Flux Security). You can follow
         the instructions in the DevContainer to build the Flux Python bindings.
         By default, this environment installs the latest flux-core.
         If you want to build a custom version with Flux core you can do:
         
         ```bash
         rm -rf ~/flux-core
-        export FLUX_VERSION=0.46.0
+        export FLUX_VERSION=0.48.0
         wget https://github.com/flux-framework/flux-core/releases/download/v${FLUX_VERSION}/flux-core-${FLUX_VERSION}.tar.gz
         tar -xzvf flux-core-${FLUX_VERSION}.tar.gz
         sudo mv flux-core-${FLUX_VERSION} ~/flux-core
         rm flux-core-${FLUX_VERSION}.tar.gz
         cd ~/flux-core
         ./configure --prefix=/usr/local
         make
         sudo make install
         ```
         
         And then build your custom wheel:
         
         ```bash
         $ cd /workspaces/flux-python
-        $ python3 setup.py sdist bdist_wheel --flux-root /home/vscode/flux-core --security-src /home/vscode/security --security-include /usr/local/include/flux/security --version 0.46.0-rc-0
+        $ python3 setup.py sdist bdist_wheel --flux-root /home/vscode/flux-core --security-src /home/vscode/security --security-include /usr/local/include/flux/security --version ${FLUX_VERSION}-rc-0
         ```
         
         And if you want to upload:
         
         ```bash
         $ twine upload dist/*.tar.gz
         ```
```

### Comparing `flux-python-0.46.0rc1/README.md` & `flux-python-0.48.0rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 to have an environment ready to go with Flux (and Flux Security). You can follow
 the instructions in the DevContainer to build the Flux Python bindings.
 By default, this environment installs the latest flux-core.
 If you want to build a custom version with Flux core you can do:
 
 ```bash
 rm -rf ~/flux-core
-export FLUX_VERSION=0.46.0
+export FLUX_VERSION=0.48.0
 wget https://github.com/flux-framework/flux-core/releases/download/v${FLUX_VERSION}/flux-core-${FLUX_VERSION}.tar.gz
 tar -xzvf flux-core-${FLUX_VERSION}.tar.gz
 sudo mv flux-core-${FLUX_VERSION} ~/flux-core
 rm flux-core-${FLUX_VERSION}.tar.gz
 cd ~/flux-core
 ./configure --prefix=/usr/local
 make
 sudo make install
 ```
 
 And then build your custom wheel:
 
 ```bash
 $ cd /workspaces/flux-python
-$ python3 setup.py sdist bdist_wheel --flux-root /home/vscode/flux-core --security-src /home/vscode/security --security-include /usr/local/include/flux/security --version 0.46.0-rc-0
+$ python3 setup.py sdist bdist_wheel --flux-root /home/vscode/flux-core --security-src /home/vscode/security --security-include /usr/local/include/flux/security --version ${FLUX_VERSION}-rc-0
 ```
 
 And if you want to upload:
 
 ```bash
 $ twine upload dist/*.tar.gz
 ```
```

### Comparing `flux-python-0.46.0rc1/flux/Makefile` & `flux-python-0.48.0rc0/flux/Makefile`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/Makefile.in` & `flux-python-0.48.0rc0/flux/Makefile.in`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/__init__.py` & `flux-python-0.48.0rc0/flux/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/cli/_fortune.py` & `flux-python-0.48.0rc0/flux/cli/_fortune.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/constants.py` & `flux-python-0.48.0rc0/flux/constants.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/constraint/parser.out` & `flux-python-0.48.0rc0/flux/constraint/parser.out`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/constraint/parsetab.py` & `flux-python-0.48.0rc0/flux/constraint/parsetab.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/core/handle.py` & `flux-python-0.48.0rc0/flux/core/handle.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/core/inner.py` & `flux-python-0.48.0rc0/flux/core/inner.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/core/trampoline.py` & `flux-python-0.48.0rc0/flux/core/trampoline.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/core/watchers.py` & `flux-python-0.48.0rc0/flux/core/watchers.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/debugged.py` & `flux-python-0.48.0rc0/flux/debugged.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/future.py` & `flux-python-0.48.0rc0/flux/future.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/hostlist.py` & `flux-python-0.48.0rc0/flux/hostlist.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/idset.py` & `flux-python-0.48.0rc0/flux/idset.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/importer.py` & `flux-python-0.48.0rc0/flux/importer.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/JobID.py` & `flux-python-0.48.0rc0/flux/job/JobID.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/Jobspec.py` & `flux-python-0.48.0rc0/flux/job/Jobspec.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/__init__.py` & `flux-python-0.48.0rc0/flux/job/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/_wrapper.py` & `flux-python-0.48.0rc0/flux/job/_wrapper.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/event.py` & `flux-python-0.48.0rc0/flux/job/event.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/executor.py` & `flux-python-0.48.0rc0/flux/job/executor.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/frobnicator/frobnicator.py` & `flux-python-0.48.0rc0/flux/job/frobnicator/frobnicator.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/frobnicator/plugins/constraints.py` & `flux-python-0.48.0rc0/flux/job/frobnicator/plugins/constraints.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/frobnicator/plugins/defaults.py` & `flux-python-0.48.0rc0/flux/job/frobnicator/plugins/defaults.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/info.py` & `flux-python-0.48.0rc0/flux/job/info.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/kill.py` & `flux-python-0.48.0rc0/flux/job/kill.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/kvs.py` & `flux-python-0.48.0rc0/flux/job/kvs.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/list.py` & `flux-python-0.48.0rc0/flux/job/list.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/stats.py` & `flux-python-0.48.0rc0/flux/job/stats.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/submit.py` & `flux-python-0.48.0rc0/flux/job/submit.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/validator/plugins/feasibility.py` & `flux-python-0.48.0rc0/flux/job/validator/plugins/feasibility.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/validator/plugins/jobspec.py` & `flux-python-0.48.0rc0/flux/job/validator/plugins/jobspec.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/validator/plugins/require-instance.py` & `flux-python-0.48.0rc0/flux/job/validator/plugins/require-instance.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/validator/plugins/schema.py` & `flux-python-0.48.0rc0/flux/job/validator/plugins/schema.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/validator/validator.py` & `flux-python-0.48.0rc0/flux/job/validator/validator.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/job/wait.py` & `flux-python-0.48.0rc0/flux/job/wait.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/kvs.py` & `flux-python-0.48.0rc0/flux/kvs.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/memoized_property.py` & `flux-python-0.48.0rc0/flux/memoized_property.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/message.py` & `flux-python-0.48.0rc0/flux/message.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/progress.py` & `flux-python-0.48.0rc0/flux/progress.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/resource/ResourceSet.py` & `flux-python-0.48.0rc0/flux/resource/ResourceSet.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/resource/ResourceSetImplementation.py` & `flux-python-0.48.0rc0/flux/resource/ResourceSetImplementation.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/resource/Rlist.py` & `flux-python-0.48.0rc0/flux/resource/Rlist.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/resource/__init__.py` & `flux-python-0.48.0rc0/flux/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/resource/list.py` & `flux-python-0.48.0rc0/flux/resource/list.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/rpc.py` & `flux-python-0.48.0rc0/flux/rpc.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/security.py` & `flux-python-0.48.0rc0/flux/security.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/uri/resolvers/jobid.py` & `flux-python-0.48.0rc0/flux/uri/resolvers/jobid.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/uri/resolvers/lsf.py` & `flux-python-0.48.0rc0/flux/uri/resolvers/lsf.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/uri/resolvers/pid.py` & `flux-python-0.48.0rc0/flux/uri/resolvers/pid.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/uri/resolvers/slurm.py` & `flux-python-0.48.0rc0/flux/uri/resolvers/slurm.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/uri/uri.py` & `flux-python-0.48.0rc0/flux/uri/uri.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/util.py` & `flux-python-0.48.0rc0/flux/util.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/parsedatetime/__init__.py` & `flux-python-0.48.0rc0/flux/utils/parsedatetime/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/parsedatetime/context.py` & `flux-python-0.48.0rc0/flux/utils/parsedatetime/context.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/__init__.py` & `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/base.py` & `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/base.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/de_DE.py` & `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/es.py` & `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/es.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/fr_FR.py` & `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/icu.py` & `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/nl_NL.py` & `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/pt_BR.py` & `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/parsedatetime/pdt_locales/ru_RU.py` & `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/tomli/LICENSE` & `flux-python-0.48.0rc0/flux/utils/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/tomli/_parser.py` & `flux-python-0.48.0rc0/flux/utils/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/utils/tomli/_re.py` & `flux-python-0.48.0rc0/flux/utils/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux/wrapper.py` & `flux-python-0.48.0rc0/flux/wrapper.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/flux_python.egg-info/PKG-INFO` & `flux-python-0.48.0rc0/flux_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-python
-Version: 0.46.0rc1
+Version: 0.48.0rc0
 Summary: Python bindings for the flux resource manager API
 Home-page: https://github.com/flux-framework/flux-python
 License: UNKNOWN
 Description: # Flux Python Bindings
         
         > 🐍️ You called me?
         
@@ -26,30 +26,30 @@
         to have an environment ready to go with Flux (and Flux Security). You can follow
         the instructions in the DevContainer to build the Flux Python bindings.
         By default, this environment installs the latest flux-core.
         If you want to build a custom version with Flux core you can do:
         
         ```bash
         rm -rf ~/flux-core
-        export FLUX_VERSION=0.46.0
+        export FLUX_VERSION=0.48.0
         wget https://github.com/flux-framework/flux-core/releases/download/v${FLUX_VERSION}/flux-core-${FLUX_VERSION}.tar.gz
         tar -xzvf flux-core-${FLUX_VERSION}.tar.gz
         sudo mv flux-core-${FLUX_VERSION} ~/flux-core
         rm flux-core-${FLUX_VERSION}.tar.gz
         cd ~/flux-core
         ./configure --prefix=/usr/local
         make
         sudo make install
         ```
         
         And then build your custom wheel:
         
         ```bash
         $ cd /workspaces/flux-python
-        $ python3 setup.py sdist bdist_wheel --flux-root /home/vscode/flux-core --security-src /home/vscode/security --security-include /usr/local/include/flux/security --version 0.46.0-rc-0
+        $ python3 setup.py sdist bdist_wheel --flux-root /home/vscode/flux-core --security-src /home/vscode/security --security-include /usr/local/include/flux/security --version ${FLUX_VERSION}-rc-0
         ```
         
         And if you want to upload:
         
         ```bash
         $ twine upload dist/*.tar.gz
         ```
```

### Comparing `flux-python-0.46.0rc1/flux_python.egg-info/SOURCES.txt` & `flux-python-0.48.0rc0/flux_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/setup.py` & `flux-python-0.48.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/_core_build.py` & `flux-python-0.48.0rc0/src/_core_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/_core_clean.h` & `flux-python-0.48.0rc0/src/_core_clean.h`

 * *Files 0% similar despite different names*

```diff
@@ -858,14 +858,20 @@
 /* if line buffered, second to last callback may not contain a full line */
 flux_watcher_t *flux_buffer_read_watcher_create (flux_reactor_t *r, int fd,
                                                  int size, flux_watcher_f cb,
                                                  int flags, void *arg);
 
 flux_buffer_t *flux_buffer_read_watcher_get_buffer (flux_watcher_t *w);
 
+/* Get next chunk of data from a buffered read watcher. Gets the next
+ * line if the watcher is line buffered.
+ */
+const char *flux_buffer_read_watcher_get_data (flux_watcher_t *w,
+                                               int *lenp);
+
 /* 'cb' only called after fd closed (FLUX_POLLOUT) or error (FLUX_POLLERR) */
 flux_watcher_t *flux_buffer_write_watcher_create (flux_reactor_t *r, int fd,
                                                   int size, flux_watcher_f cb,
                                                   int flags, void *arg);
 
 flux_buffer_t *flux_buffer_write_watcher_get_buffer (flux_watcher_t *w);
 
@@ -1438,14 +1444,25 @@
 void flux_log_set_redirect (flux_t *h, flux_log_f fun, void *arg);
 
 /* Convert errno to string.
  * Flux errno space includes POSIX errno + zeromq errors.
  */
 const char *flux_strerror (int errnum);
 
+/* Flux log function compatible with libutil llog interface
+ */
+void flux_llog (void *arg,
+                const char *file,
+                int line,
+                const char *func,
+                const char *subsys,
+                int level,
+                const char *fmt,
+                va_list ap);
+
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* !_FLUX_CORE_FLOG_H */
 
 /*
@@ -1994,15 +2011,16 @@
 void flux_conf_decref (const flux_conf_t *conf);
 
 /* Decode config-reload request, setting 'conf' to a config object
  * owned by 'msg'.
  */
 int flux_conf_reload_decode (const flux_msg_t *msg, const flux_conf_t **conf);
 
-/* Parse *.toml in 'path' directory.
+/* Parse TOML config in 'path' and return a new flux_conf_t on success.
+ * If path is a directory, then parse all files matching *.toml in path.
  */
 flux_conf_t *flux_conf_parse (const char *path, flux_error_t *error);
 
 /* Get/set config object cached in flux_t handle, with destructor.
  * Re-setting the object decrefs the old one.
  */
 const flux_conf_t *flux_get_conf (flux_t *h);
@@ -2136,17 +2154,17 @@
 
 /* Flux uses semantic versioning: <major>.<minor>.<patch>
  */
 
 /* The VERSION_STRING may include a "-N-hash" suffix from git describe
  * if this snapshot is not tagged.  This is not reflected in VERSION_PATCH.
  */
-#define FLUX_CORE_VERSION_STRING    "0.46.0"
+#define FLUX_CORE_VERSION_STRING    "0.48.0"
 #define FLUX_CORE_VERSION_MAJOR     0
-#define FLUX_CORE_VERSION_MINOR     46
+#define FLUX_CORE_VERSION_MINOR     48
 #define FLUX_CORE_VERSION_PATCH     0
 
 /* The version in 3 bytes, for numeric comparison.
  */
 #define FLUX_CORE_VERSION_HEX       ((FLUX_CORE_VERSION_MAJOR << 16) | \
                                      (FLUX_CORE_VERSION_MINOR << 8) | \
                                      (FLUX_CORE_VERSION_PATCH << 0))
@@ -3014,35 +3032,29 @@
  *  flux_subprocess_t: A subprocess is an instantiation of a command
  *   as a remote or local process. A subprocess has a state (e.g.
  *   initialized, starting, running, exited, completed), a PID, and
  *   a rank if running remotely.
  */
 typedef struct flux_subprocess flux_subprocess_t;
 
-/*  flux_subprocess_server_t: Handler for a subprocess remote server */
-typedef struct flux_subprocess_server flux_subprocess_server_t;
-
 /*
  * Subprocess states, on changes, will lead to calls to
  * on_state_change below.
  *
  * Possible state changes:
  *
  * init -> running
- * init -> exec failed
  * running -> exited
  * any state -> failed
  */
 typedef enum {
     FLUX_SUBPROCESS_INIT,         /* initial state */
-    FLUX_SUBPROCESS_EXEC_FAILED,  /* exec(2) has failed, only for rexec() */
     FLUX_SUBPROCESS_RUNNING,      /* exec(2) has been called */
     FLUX_SUBPROCESS_EXITED,       /* process has exited */
-    FLUX_SUBPROCESS_FAILED,       /* internal failure, catch all for
-                                   * all other errors */
+    FLUX_SUBPROCESS_FAILED,       /* exec failure or other non-child error */
     FLUX_SUBPROCESS_STOPPED,      /* process was stopped */
 } flux_subprocess_state_t;
 
 /*
  * Subprocess flags
  */
 enum {
@@ -3072,16 +3084,15 @@
 /*
  *  Functions for event-driven subprocess handling:
  *
  */
 typedef struct {
     flux_subprocess_f on_completion;    /* Process exited and all I/O
                                          * complete, will not be
-                                         * called if EXEC_FAILED or
-                                         * FAILED states reached.
+                                         * called if FAILED state reached.
                                          */
     flux_subprocess_state_f on_state_change;  /* Process state change        */
     flux_subprocess_output_f on_channel_out; /* Read from channel when ready */
     flux_subprocess_output_f on_stdout; /* Read of stdout is ready           */
     flux_subprocess_output_f on_stderr; /* Read of stderr is ready           */
 } flux_subprocess_ops_t;
 
@@ -3093,61 +3104,14 @@
     flux_subprocess_hook_f pre_exec;
     void *pre_exec_arg;
     flux_subprocess_hook_f post_fork;
     void *post_fork_arg;
 } flux_subprocess_hooks_t;
 
 /*
- *  General support:
- */
-
-/*  Start a subprocess server on the handle `h`. Registers message
- *   handlers, etc for remote execution.
- */
-flux_subprocess_server_t *flux_subprocess_server_start (flux_t *h,
-                                                        const char *local_uri,
-                                                        uint32_t rank);
-
-
-typedef int (*flux_subprocess_server_auth_f) (const flux_msg_t *msg,
-                                              void *arg);
-
-/*   Register an authorization function to the subprocess server
- *
- *   The registered function should return 0 to allow the request to
- *    proceed, and -1 with errno set to deny the request.
- */
-void flux_subprocess_server_set_auth_cb (flux_subprocess_server_t *s,
-                                         flux_subprocess_server_auth_f fn,
-                                         void *arg);
-
-/*  Stop a subprocess server / cleanup flux_subprocess_server_t.  Will
- *  send a SIGKILL to all remaining subprocesses.
- */
-void flux_subprocess_server_stop (flux_subprocess_server_t *s);
-
-/* Send all subprocesses signal and wait up to wait_time seconds for
- * all subprocesses to complete.  This is typically called to send
- * SIGTERM before calling flux_subprocess_server_stop(), allowing
- * users to send a signal to inform subprocesses to complete / cleanup
- * before they are sent SIGKILL.
- *
- * This function will enter the reactor to wait for subprocesses to
- * complete, should only be called on cleanup path when primary
- * reactor has exited.
- */
-int flux_subprocess_server_subprocesses_kill (flux_subprocess_server_t *s,
-                                              int signum,
-                                              double wait_time);
-
-/* Terminate all subprocesses started by a sender id */
-int flux_subprocess_server_terminate_by_uuid (flux_subprocess_server_t *s,
-                                              const char *id);
-
-/*
  * Convenience Functions:
  */
 
 /*  General output callback that will send output from the subprocess
  *  to stdout or stderr.  Set the `on_stdout` and/or `on_stderr`
  *  callbacks in flux_subprocess_ops_t and this function will output
  *  to stdout/stderr respectively.  You can also set 'on_channel_out'
@@ -3459,16 +3423,15 @@
 
 /*  Return string value of state of subprocess
  */
 const char *flux_subprocess_state_string (flux_subprocess_state_t state);
 
 int flux_subprocess_rank (flux_subprocess_t *p);
 
-/* Returns the errno causing the FLUX_SUBPROCESS_EXEC_FAILED or
- * FLUX_SUBPROCESS_FAILED states to be reached.
+/* Returns the errno causing the FLUX_SUBPROCESS_FAILED states to be reached.
  */
 int flux_subprocess_fail_errno (flux_subprocess_t *p);
 
 /* Returns exit status as returned from wait(2).  Works only for
  * FLUX_SUBPROCESS_EXITED state. */
 int flux_subprocess_status (flux_subprocess_t *p);
 
@@ -3500,14 +3463,31 @@
 
 /*
  *  Return pointer to any context associated with `p` under `name`. If
  *   no such context exists, then NULL is returned.
  */
 void *flux_subprocess_aux_get (flux_subprocess_t *p, const char *name);
 
+typedef void (*subprocess_log_f) (void *arg,
+                                  const char *file,
+                                  int line,
+                                  const char *func,
+                                  const char *subsys,
+                                  int level,
+                                  const char *fmt,
+                                  va_list args);
+
+/* Set default internal logging function.
+ */
+int flux_set_default_subprocess_log (flux_t *h,
+                                     subprocess_log_f log_fn,
+                                     void *log_data);
+
+
+
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* !_FLUX_CORE_SUBPROCESS_H */
 /************************************************************\
  * Copyright 2018 Lawrence Livermore National Security, LLC
@@ -3757,14 +3737,28 @@
  *     "exception_type"?s,     exception type (if exception)
  *     "exception_note"?s      exception note (if exception)
  *   }
  *
  */
 int flux_job_result_get_unpack (flux_future_t *f, const char *fmt, ...);
 
+
+/*  Get remaining time in floating point seconds for the current job or
+ *  enclosing instancce (i.e., if the current process is associated with
+ *  a flux instance, but is not part of a parallel job).
+ *
+ *  Returns 0 on success with timeleft assigned to the remaining time.
+ *  If there is no expiration in the current context (e.g. the job has
+ *  no timelimit), then timeleft is set to infinity. If the job is not
+ *  in RUN state, or the job has expired, then timeleft is set to 0.
+ *
+ *  Returns -1 with error string assinged to 'errp' on failure.
+ */
+int flux_job_timeleft (flux_t *h, flux_error_t *errp, double *timeleft);
+
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* !_FLUX_CORE_JOB_H */
 
 /*
```

### Comparing `flux-python-0.46.0rc1/src/_core_preproc.h` & `flux-python-0.48.0rc0/src/_core_preproc.h`

 * *Files 1% similar despite different names*

```diff
@@ -605,20 +605,26 @@
 flux_watcher_t *flux_buffer_read_watcher_create (flux_reactor_t *r, int fd,
                                                  int size, flux_watcher_f cb,
                                                  int flags, void *arg);
 
 flux_buffer_t *flux_buffer_read_watcher_get_buffer (flux_watcher_t *w);
 
 
+
+
+const char *flux_buffer_read_watcher_get_data (flux_watcher_t *w,
+                                               int *lenp);
+
+
 flux_watcher_t *flux_buffer_write_watcher_create (flux_reactor_t *r, int fd,
                                                   int size, flux_watcher_f cb,
                                                   int flags, void *arg);
 
 flux_buffer_t *flux_buffer_write_watcher_get_buffer (flux_watcher_t *w);
-# 881 "/workspaces/flux-python/src/_core_clean.h"
+# 887 "/workspaces/flux-python/src/_core_clean.h"
 int flux_buffer_write_watcher_close (flux_watcher_t *w);
 
 
 int flux_buffer_write_watcher_is_closed (flux_watcher_t *w, int *close_err);
 
 
 
@@ -688,27 +694,27 @@
 
 
 struct flux_watcher_ops {
     void (*start) (flux_watcher_t *w);
     void (*stop) (flux_watcher_t *w);
     void (*destroy) (flux_watcher_t *w);
 };
-# 966 "/workspaces/flux-python/src/_core_clean.h"
+# 972 "/workspaces/flux-python/src/_core_clean.h"
 flux_watcher_t * flux_watcher_create (flux_reactor_t *r, size_t data_size,
                                       struct flux_watcher_ops *ops,
                                       flux_watcher_f fn, void *arg);
 
 
 
 void * flux_watcher_get_data (flux_watcher_t *w);
 
 
 
 struct flux_watcher_ops * flux_watcher_get_ops (flux_watcher_t *w);
-# 1005 "/workspaces/flux-python/src/_core_clean.h"
+# 1011 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_msg_handler flux_msg_handler_t;
 
 typedef void (*flux_msg_handler_f)(flux_t *h, flux_msg_handler_t *mh,
                                    const flux_msg_t *msg, void *arg);
 
 flux_msg_handler_t *flux_msg_handler_create (flux_t *h,
                                              const struct flux_match match,
@@ -741,15 +747,15 @@
                              void *arg,
                              flux_msg_handler_t **msg_handlers[]);
 void flux_msg_handler_delvec (flux_msg_handler_t *msg_handlers[]);
 
 
 
 int flux_dispatch_requeue (flux_t *h);
-# 1076 "/workspaces/flux-python/src/_core_clean.h"
+# 1082 "/workspaces/flux-python/src/_core_clean.h"
 typedef flux_t *(connector_init_f)(const char *uri,
                                    int flags,
                                    flux_error_t *errp);
 
 struct flux_handle_ops {
     int (*setopt)(void *impl, const char *option,
                           const void *val, size_t len);
@@ -762,32 +768,32 @@
     int (*reconnect)(void *impl);
 
     void (*impl_destroy)(void *impl);
 };
 
 flux_t *flux_handle_create (void *impl, const struct flux_handle_ops *ops, int flags);
 void flux_handle_destroy (flux_t *hp);
-# 1127 "/workspaces/flux-python/src/_core_clean.h"
+# 1133 "/workspaces/flux-python/src/_core_clean.h"
 struct flux_msglist *flux_msglist_create (void);
 void flux_msglist_destroy (struct flux_msglist *l);
 
 int flux_msglist_push (struct flux_msglist *l, const flux_msg_t *msg);
 int flux_msglist_append (struct flux_msglist *l, const flux_msg_t *msg);
 void flux_msglist_delete (struct flux_msglist *l);
 const flux_msg_t *flux_msglist_pop (struct flux_msglist *l);
 
 const flux_msg_t *flux_msglist_first (struct flux_msglist *l);
 const flux_msg_t *flux_msglist_next (struct flux_msglist *l);
 const flux_msg_t *flux_msglist_last (struct flux_msglist *l);
 
 int flux_msglist_count (struct flux_msglist *l);
-# 1148 "/workspaces/flux-python/src/_core_clean.h"
+# 1154 "/workspaces/flux-python/src/_core_clean.h"
 int flux_msglist_pollevents (struct flux_msglist *l);
 int flux_msglist_pollfd (struct flux_msglist *l);
-# 1184 "/workspaces/flux-python/src/_core_clean.h"
+# 1190 "/workspaces/flux-python/src/_core_clean.h"
 int flux_request_decode (const flux_msg_t *msg, const char **topic,
                          const char **s);
 
 
 
 
 
@@ -810,18 +816,18 @@
 
 
 
 
 
 flux_msg_t *flux_request_encode_raw (const char *topic,
                                      const void *data, int len);
-# 1250 "/workspaces/flux-python/src/_core_clean.h"
+# 1256 "/workspaces/flux-python/src/_core_clean.h"
 int flux_response_decode (const flux_msg_t *msg, const char **topic,
                           const char **s);
-# 1261 "/workspaces/flux-python/src/_core_clean.h"
+# 1267 "/workspaces/flux-python/src/_core_clean.h"
 int flux_response_decode_raw (const flux_msg_t *msg, const char **topic,
                               const void **data, int *len);
 
 
 
 
 
@@ -868,19 +874,19 @@
 
 
 
 
 
 int flux_respond_error (flux_t *h, const flux_msg_t *request,
                         int errnum, const char *errstr);
-# 1343 "/workspaces/flux-python/src/_core_clean.h"
+# 1349 "/workspaces/flux-python/src/_core_clean.h"
 flux_msg_t *flux_control_encode (int type, int status);
 
 int flux_control_decode (const flux_msg_t *msg, int *type, int *status);
-# 1404 "/workspaces/flux-python/src/_core_clean.h"
+# 1410 "/workspaces/flux-python/src/_core_clean.h"
 typedef void (*flux_log_f)(const char *buf, int len, void *arg);
 
 
 
 
 void flux_log_set_appname (flux_t *h, const char *s);
 
@@ -913,15 +919,26 @@
 
 void flux_log_set_redirect (flux_t *h, flux_log_f fun, void *arg);
 
 
 
 
 const char *flux_strerror (int errnum);
-# 1463 "/workspaces/flux-python/src/_core_clean.h"
+
+
+
+void flux_llog (void *arg,
+                const char *file,
+                int line,
+                const char *func,
+                const char *subsys,
+                int level,
+                const char *fmt,
+                va_list ap);
+# 1480 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_future flux_future_t;
 
 typedef void (*flux_continuation_f)(flux_future_t *f, void *arg);
 
 int flux_future_then (flux_future_t *f, double timeout,
                       flux_continuation_f cb, void *arg);
 
@@ -979,15 +996,15 @@
 
 int flux_future_push (flux_future_t *cf, const char *name, flux_future_t *f);
 
 const char * flux_future_first_child (flux_future_t *cf);
 const char * flux_future_next_child (flux_future_t *cf);
 
 flux_future_t *flux_future_get_child (flux_future_t *cf, const char *name);
-# 1541 "/workspaces/flux-python/src/_core_clean.h"
+# 1558 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_future_and_then (flux_future_t *f,
                                      flux_continuation_f cb, void *arg);
 
 
 
 
 flux_future_t *flux_future_or_then (flux_future_t *f,
@@ -1007,15 +1024,15 @@
                                  const char *errstr);
 
 
 
 int flux_future_fulfill_next (flux_future_t *prev,
                               void *result,
                               flux_free_f free_fn);
-# 1583 "/workspaces/flux-python/src/_core_clean.h"
+# 1600 "/workspaces/flux-python/src/_core_clean.h"
 enum {
     FLUX_RPC_NORESPONSE = 1,
     FLUX_RPC_STREAMING = 2,
 };
 
 flux_future_t *flux_rpc (flux_t *h, const char *topic, const char *s,
                          uint32_t nodeid, int flags);
@@ -1045,17 +1062,17 @@
 
 
 uint32_t flux_rpc_get_matchtag (flux_future_t *f);
 
 
 
 uint32_t flux_rpc_get_nodeid (flux_future_t *f);
-# 1652 "/workspaces/flux-python/src/_core_clean.h"
+# 1669 "/workspaces/flux-python/src/_core_clean.h"
 int flux_panic (flux_t *h, uint32_t nodeid, int flags, const char *reason);
-# 1681 "/workspaces/flux-python/src/_core_clean.h"
+# 1698 "/workspaces/flux-python/src/_core_clean.h"
 enum event_flags {
     FLUX_EVENT_PRIVATE = 1,
 };
 
 
 
 int flux_event_subscribe (flux_t *h, const char *topic);
@@ -1128,15 +1145,15 @@
                                        const char *topic, int flags,
                                        const void *data, int len);
 
 
 
 
 int flux_event_publish_get_seq (flux_future_t *f, int *seq);
-# 1796 "/workspaces/flux-python/src/_core_clean.h"
+# 1813 "/workspaces/flux-python/src/_core_clean.h"
 enum {
     FLUX_MODSTATE_INIT = 0,
     FLUX_MODSTATE_RUNNING = 1,
     FLUX_MODSTATE_FINALIZING = 2,
     FLUX_MODSTATE_EXITED = 3,
 };
 
@@ -1170,15 +1187,15 @@
 
 
 
 
 
 
 int flux_module_set_running (flux_t *h);
-# 1885 "/workspaces/flux-python/src/_core_clean.h"
+# 1902 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_attr_get (flux_t *h, const char *name);
 
 
 
 
 
 
@@ -1205,26 +1222,26 @@
 const char *flux_get_hostbyrank (flux_t *h, uint32_t rank);
 
 
 
 
 
 int flux_get_rankbyhost (flux_t *h, const char *host);
-# 1933 "/workspaces/flux-python/src/_core_clean.h"
+# 1950 "/workspaces/flux-python/src/_core_clean.h"
 char *flux_hostmap_lookup (flux_t *h,
                            const char *targets,
                            flux_error_t *errp);
 
 
 
 
 
 
 int flux_get_instance_starttime (flux_t *h, double *starttime);
-# 1971 "/workspaces/flux-python/src/_core_clean.h"
+# 1988 "/workspaces/flux-python/src/_core_clean.h"
 enum flux_conf_flags {
     FLUX_CONF_INSTALLED=0,
     FLUX_CONF_INTREE=1,
     FLUX_CONF_AUTO=2,
 };
 
 
@@ -1249,14 +1266,15 @@
 
 
 
 int flux_conf_reload_decode (const flux_msg_t *msg, const flux_conf_t **conf);
 
 
 
+
 flux_conf_t *flux_conf_parse (const char *path, flux_error_t *error);
 
 
 
 
 const flux_conf_t *flux_get_conf (flux_t *h);
 int flux_set_conf (flux_t *h, const flux_conf_t *conf);
@@ -1268,30 +1286,30 @@
                        flux_error_t *error,
                        const char *fmt,
                        va_list ap);
 
 int flux_conf_unpack (const flux_conf_t *conf,
                       flux_error_t *error,
                       const char *fmt, ...);
-# 2054 "/workspaces/flux-python/src/_core_clean.h"
+# 2072 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_barrier (flux_t *h, const char *name, int nprocs);
-# 2097 "/workspaces/flux-python/src/_core_clean.h"
+# 2115 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_service_register (flux_t *h, const char *name);
-# 2109 "/workspaces/flux-python/src/_core_clean.h"
+# 2127 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_service_unregister (flux_t *h, const char *name);
-# 2161 "/workspaces/flux-python/src/_core_clean.h"
+# 2179 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_core_version_string (void);
 
 
 
 
 
 
 int flux_core_version (int *major, int *minor, int *patch);
-# 2199 "/workspaces/flux-python/src/_core_clean.h"
+# 2217 "/workspaces/flux-python/src/_core_clean.h"
 enum {
     FLUX_PLUGIN_RTLD_LAZY = 1,
     FLUX_PLUGIN_RTLD_NOW = 2,
     FLUX_PLUGIN_RTLD_GLOBAL = 4,
     FLUX_PLUGIN_RTLD_DEEPBIND = 8,
 };
 
@@ -1361,15 +1379,15 @@
 
 
 
 
 int flux_plugin_register (flux_plugin_t *p,
                           const char *name,
                           const struct flux_plugin_handler t[]);
-# 2286 "/workspaces/flux-python/src/_core_clean.h"
+# 2304 "/workspaces/flux-python/src/_core_clean.h"
 int flux_plugin_aux_set (flux_plugin_t *p,
                          const char *key,
                          void *val,
                          flux_free_f free_fn);
 
 
 
@@ -1423,22 +1441,22 @@
 int flux_plugin_arg_vpack (flux_plugin_arg_t *args, int flags,
                            const char *fmt, va_list ap);
 
 int flux_plugin_arg_unpack (flux_plugin_arg_t *args, int flags,
                             const char *fmt, ...);
 int flux_plugin_arg_vunpack (flux_plugin_arg_t *args, int flags,
                              const char *fmt, va_list ap);
-# 2355 "/workspaces/flux-python/src/_core_clean.h"
+# 2373 "/workspaces/flux-python/src/_core_clean.h"
 int flux_plugin_call (flux_plugin_t *p, const char *name,
                       flux_plugin_arg_t *args);
-# 2365 "/workspaces/flux-python/src/_core_clean.h"
+# 2383 "/workspaces/flux-python/src/_core_clean.h"
 int flux_plugin_load_dso (flux_plugin_t *p, const char *path);
-# 2398 "/workspaces/flux-python/src/_core_clean.h"
+# 2416 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_sync_create (flux_t *h, double minimum);
-# 2430 "/workspaces/flux-python/src/_core_clean.h"
+# 2448 "/workspaces/flux-python/src/_core_clean.h"
 bool flux_disconnect_match (const flux_msg_t *msg1, const flux_msg_t *msg2);
 
 
 
 
 int flux_msglist_disconnect (struct flux_msglist *l, const flux_msg_t *msg);
 
@@ -1450,15 +1468,15 @@
 
 
 
 
 int flux_msglist_cancel (flux_t *h,
                          struct flux_msglist *l,
                          const flux_msg_t *msg);
-# 2499 "/workspaces/flux-python/src/_core_clean.h"
+# 2517 "/workspaces/flux-python/src/_core_clean.h"
 void flux_stats_count (flux_t *h, const char *name, ssize_t count);
 
 
 
 
 void flux_stats_gauge_set (flux_t *h, const char *name, ssize_t value);
 
@@ -1486,18 +1504,18 @@
 
 void flux_stats_set_prefix (flux_t *h, const char *fmt, ...);
 
 
 
 
 bool flux_stats_enabled (flux_t *h, const char *metric);
-# 2582 "/workspaces/flux-python/src/_core_clean.h"
+# 2600 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_kvsdir flux_kvsdir_t;
 typedef struct flux_kvsitr flux_kvsitr_t;
-# 2597 "/workspaces/flux-python/src/_core_clean.h"
+# 2615 "/workspaces/flux-python/src/_core_clean.h"
 flux_kvsdir_t *flux_kvsdir_create (flux_t *handle, const char *rootref,
                                    const char *key, const char *json_str);
 void flux_kvsdir_destroy (flux_kvsdir_t *dir);
 
 flux_kvsdir_t *flux_kvsdir_copy (const flux_kvsdir_t *dir);
 void flux_kvsdir_incref (flux_kvsdir_t *dir);
 
@@ -1535,15 +1553,15 @@
 void *flux_kvsdir_handle (const flux_kvsdir_t *dir);
 const char *flux_kvsdir_rootref (const flux_kvsdir_t *dir);
 
 
 
 
 char *flux_kvsdir_key_at (const flux_kvsdir_t *dir, const char *key);
-# 2670 "/workspaces/flux-python/src/_core_clean.h"
+# 2688 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_lookup (flux_t *h, const char *ns, int flags,
                                 const char *key);
 flux_future_t *flux_kvs_lookupat (flux_t *h, int flags, const char *key,
                                   const char *treeobj);
 
 int flux_kvs_lookup_get (flux_future_t *f, const char **value);
 int flux_kvs_lookup_get_unpack (flux_future_t *f, const char *fmt, ...);
@@ -1558,22 +1576,22 @@
 
 
 
 
 
 
 int flux_kvs_lookup_cancel (flux_future_t *f);
-# 2720 "/workspaces/flux-python/src/_core_clean.h"
+# 2738 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_getroot (flux_t *h, const char *ns, int flags);
-# 2729 "/workspaces/flux-python/src/_core_clean.h"
+# 2747 "/workspaces/flux-python/src/_core_clean.h"
 int flux_kvs_getroot_get_treeobj (flux_future_t *f, const char **treeobj);
 int flux_kvs_getroot_get_blobref (flux_future_t *f, const char **blobref);
 int flux_kvs_getroot_get_sequence (flux_future_t *f, int *seq);
 int flux_kvs_getroot_get_owner (flux_future_t *f, uint32_t *owner);
-# 2761 "/workspaces/flux-python/src/_core_clean.h"
+# 2779 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_kvs_txn flux_kvs_txn_t;
 
 flux_kvs_txn_t *flux_kvs_txn_create (void);
 void flux_kvs_txn_destroy (flux_kvs_txn_t *txn);
 
 int flux_kvs_txn_put (flux_kvs_txn_t *txn, int flags,
                       const char *key, const char *value);
@@ -1595,15 +1613,15 @@
 
 int flux_kvs_txn_unlink (flux_kvs_txn_t *txn, int flags,
                          const char *key);
 
 int flux_kvs_txn_symlink (flux_kvs_txn_t *txn, int flags,
                           const char *key, const char *ns,
                           const char *target);
-# 2839 "/workspaces/flux-python/src/_core_clean.h"
+# 2857 "/workspaces/flux-python/src/_core_clean.h"
 enum kvs_commit_flags {
     FLUX_KVS_NO_MERGE = 1,
     FLUX_KVS_TXN_COMPACT = 2,
     FLUX_KVS_SYNC = 4,
 };
 
 flux_future_t *flux_kvs_commit (flux_t *h, const char *ns, int flags,
@@ -1613,41 +1631,41 @@
                                const char *name, int nprocs,
                                flux_kvs_txn_t *txn);
 
 
 int flux_kvs_commit_get_treeobj (flux_future_t *f, const char **treeobj);
 int flux_kvs_commit_get_rootref (flux_future_t *f, const char **rootref);
 int flux_kvs_commit_get_sequence (flux_future_t *f, int *rootseq);
-# 2895 "/workspaces/flux-python/src/_core_clean.h"
+# 2913 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_copy (flux_t *h,
                               const char *srcns,
                               const char *srckey,
                               const char *dstns,
                               const char *dstkey,
                               int commit_flags);
-# 2912 "/workspaces/flux-python/src/_core_clean.h"
+# 2930 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_move (flux_t *h,
                               const char *srcns,
                               const char *srckey,
                               const char *dstns,
                               const char *dstkey,
                               int commit_flags);
-# 2935 "/workspaces/flux-python/src/_core_clean.h"
+# 2953 "/workspaces/flux-python/src/_core_clean.h"
 enum kvs_op {
     FLUX_KVS_READDIR = 1,
     FLUX_KVS_READLINK = 2,
     FLUX_KVS_WATCH = 4,
     FLUX_KVS_WAITCREATE = 8,
     FLUX_KVS_TREEOBJ = 16,
     FLUX_KVS_APPEND = 32,
     FLUX_KVS_WATCH_FULL = 64,
     FLUX_KVS_WATCH_UNIQ = 128,
     FLUX_KVS_WATCH_APPEND = 256
 };
-# 2956 "/workspaces/flux-python/src/_core_clean.h"
+# 2974 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_namespace_create (flux_t *h, const char *ns,
                                           uint32_t owner, int flags);
 flux_future_t *flux_kvs_namespace_create_with (flux_t *h, const char *ns,
                                                const char *rootref,
                                                uint32_t owner, int flags);
 flux_future_t *flux_kvs_namespace_remove (flux_t *h, const char *ns);
 
@@ -1660,35 +1678,30 @@
 
 
 
 
 
 
 int flux_kvs_dropcache (flux_t *h);
-# 3011 "/workspaces/flux-python/src/_core_clean.h"
+# 3029 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_command flux_cmd_t;
 
 
 
 
 
 
 
 typedef struct flux_subprocess flux_subprocess_t;
-
-
-typedef struct flux_subprocess_server flux_subprocess_server_t;
-# 3035 "/workspaces/flux-python/src/_core_clean.h"
+# 3049 "/workspaces/flux-python/src/_core_clean.h"
 typedef enum {
     FLUX_SUBPROCESS_INIT,
-    FLUX_SUBPROCESS_EXEC_FAILED,
     FLUX_SUBPROCESS_RUNNING,
     FLUX_SUBPROCESS_EXITED,
     FLUX_SUBPROCESS_FAILED,
-
     FLUX_SUBPROCESS_STOPPED,
 } flux_subprocess_state_t;
 
 
 
 
 enum {
@@ -1720,15 +1733,14 @@
 
 
 typedef struct {
     flux_subprocess_f on_completion;
 
 
 
-
     flux_subprocess_state_f on_state_change;
     flux_subprocess_output_f on_channel_out;
     flux_subprocess_output_f on_stdout;
     flux_subprocess_output_f on_stderr;
 } flux_subprocess_ops_t;
 
 
@@ -1737,47 +1749,17 @@
 
 typedef struct {
     flux_subprocess_hook_f pre_exec;
     void *pre_exec_arg;
     flux_subprocess_hook_f post_fork;
     void *post_fork_arg;
 } flux_subprocess_hooks_t;
-# 3106 "/workspaces/flux-python/src/_core_clean.h"
-flux_subprocess_server_t *flux_subprocess_server_start (flux_t *h,
-                                                        const char *local_uri,
-                                                        uint32_t rank);
-
-
-typedef int (*flux_subprocess_server_auth_f) (const flux_msg_t *msg,
-                                              void *arg);
-
-
-
-
-
-
-void flux_subprocess_server_set_auth_cb (flux_subprocess_server_t *s,
-                                         flux_subprocess_server_auth_f fn,
-                                         void *arg);
-
-
-
-
-void flux_subprocess_server_stop (flux_subprocess_server_t *s);
-# 3138 "/workspaces/flux-python/src/_core_clean.h"
-int flux_subprocess_server_subprocesses_kill (flux_subprocess_server_t *s,
-                                              int signum,
-                                              double wait_time);
-
-
-int flux_subprocess_server_terminate_by_uuid (flux_subprocess_server_t *s,
-                                              const char *id);
-# 3156 "/workspaces/flux-python/src/_core_clean.h"
+# 3120 "/workspaces/flux-python/src/_core_clean.h"
 void flux_standard_output (flux_subprocess_t *p, const char *stream);
-# 3165 "/workspaces/flux-python/src/_core_clean.h"
+# 3129 "/workspaces/flux-python/src/_core_clean.h"
 flux_cmd_t * flux_cmd_create (int argc, char *argv[], char **env);
 
 
 
 
 flux_cmd_t * flux_cmd_copy (const flux_cmd_t *cmd);
 
@@ -1843,34 +1825,34 @@
 const char *flux_cmd_getenv (const flux_cmd_t *cmd, const char *name);
 
 
 
 
 int flux_cmd_setcwd (flux_cmd_t *cmd, const char *cwd);
 const char *flux_cmd_getcwd (const flux_cmd_t *cmd);
-# 3251 "/workspaces/flux-python/src/_core_clean.h"
+# 3215 "/workspaces/flux-python/src/_core_clean.h"
 int flux_cmd_add_channel (flux_cmd_t *cmd, const char *name);
-# 3301 "/workspaces/flux-python/src/_core_clean.h"
+# 3265 "/workspaces/flux-python/src/_core_clean.h"
 int flux_cmd_setopt (flux_cmd_t *cmd, const char *var, const char *val);
 const char *flux_cmd_getopt (flux_cmd_t *cmd, const char *var);
-# 3324 "/workspaces/flux-python/src/_core_clean.h"
+# 3288 "/workspaces/flux-python/src/_core_clean.h"
 flux_subprocess_t *flux_exec (flux_t *h, int flags,
                               const flux_cmd_t *cmd,
                               const flux_subprocess_ops_t *ops,
                               const flux_subprocess_hooks_t *hooks);
 
 flux_subprocess_t *flux_local_exec (flux_reactor_t *r, int flags,
                                     const flux_cmd_t *cmd,
                                     const flux_subprocess_ops_t *ops,
                                     const flux_subprocess_hooks_t *hooks);
 
 flux_subprocess_t *flux_rexec (flux_t *h, int rank, int flags,
                                const flux_cmd_t *cmd,
                                const flux_subprocess_ops_t *ops);
-# 3346 "/workspaces/flux-python/src/_core_clean.h"
+# 3310 "/workspaces/flux-python/src/_core_clean.h"
 int flux_subprocess_stream_start (flux_subprocess_t *p, const char *stream);
 int flux_subprocess_stream_stop (flux_subprocess_t *p, const char *stream);
 int flux_subprocess_stream_status (flux_subprocess_t *p, const char *stream);
 
 
 
 
@@ -1882,33 +1864,33 @@
 
 
 
 
 
 
 int flux_subprocess_close (flux_subprocess_t *p, const char *stream);
-# 3377 "/workspaces/flux-python/src/_core_clean.h"
+# 3341 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_subprocess_read (flux_subprocess_t *p,
                                   const char *stream,
                                   int len, int *lenp);
-# 3392 "/workspaces/flux-python/src/_core_clean.h"
+# 3356 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_subprocess_read_line (flux_subprocess_t *p,
                                        const char *stream,
                                        int *lenp);
 
 
 
 
 const char *flux_subprocess_read_trimmed_line (flux_subprocess_t *p,
                                                const char *stream,
                                                int *lenp);
-# 3412 "/workspaces/flux-python/src/_core_clean.h"
+# 3376 "/workspaces/flux-python/src/_core_clean.h"
 int flux_subprocess_read_stream_closed (flux_subprocess_t *p,
                                         const char *stream);
-# 3431 "/workspaces/flux-python/src/_core_clean.h"
+# 3395 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_subprocess_getline (flux_subprocess_t *p,
                                      const char *stream,
                                      int *lenp);
 
 
 
 
@@ -1920,26 +1902,25 @@
 
 
 
 
 
 void flux_subprocess_ref (flux_subprocess_t *p);
 void flux_subprocess_unref (flux_subprocess_t *p);
-# 3458 "/workspaces/flux-python/src/_core_clean.h"
+# 3422 "/workspaces/flux-python/src/_core_clean.h"
 flux_subprocess_state_t flux_subprocess_state (flux_subprocess_t *p);
 
 
 
 const char *flux_subprocess_state_string (flux_subprocess_state_t state);
 
 int flux_subprocess_rank (flux_subprocess_t *p);
 
 
 
-
 int flux_subprocess_fail_errno (flux_subprocess_t *p);
 
 
 
 int flux_subprocess_status (flux_subprocess_t *p);
 
 
@@ -1969,15 +1950,30 @@
                              const char *name, void *ctx, flux_free_f free);
 
 
 
 
 
 void *flux_subprocess_aux_get (flux_subprocess_t *p, const char *name);
-# 3530 "/workspaces/flux-python/src/_core_clean.h"
+
+typedef void (*subprocess_log_f) (void *arg,
+                                  const char *file,
+                                  int line,
+                                  const char *func,
+                                  const char *subsys,
+                                  int level,
+                                  const char *fmt,
+                                  va_list args);
+
+
+
+int flux_set_default_subprocess_log (flux_t *h,
+                                     subprocess_log_f log_fn,
+                                     void *log_data);
+# 3510 "/workspaces/flux-python/src/_core_clean.h"
 enum job_submit_flags {
     FLUX_JOB_PRE_SIGNED = 1,
     FLUX_JOB_DEBUG = 2,
     FLUX_JOB_WAITABLE = 4,
     FLUX_JOB_NOVALIDATE = 8,
 };
 
@@ -2031,18 +2027,18 @@
 
 typedef uint64_t flux_jobid_t;
 
 
 
 
 int flux_job_id_parse (const char *s, flux_jobid_t *id);
-# 3600 "/workspaces/flux-python/src/_core_clean.h"
+# 3580 "/workspaces/flux-python/src/_core_clean.h"
 int flux_job_id_encode (flux_jobid_t id, const char *type,
                         char *buf, size_t bufsz);
-# 3611 "/workspaces/flux-python/src/_core_clean.h"
+# 3591 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_job_statetostr (flux_job_state_t state, const char *fmt);
 
 
 
 
 int flux_job_strtostate (const char *s, flux_job_state_t *state);
 
@@ -2070,15 +2066,15 @@
 
 
 flux_future_t *flux_job_wait (flux_t *h, flux_jobid_t id);
 int flux_job_wait_get_status (flux_future_t *f,
                               bool *success,
                               const char **errstr);
 int flux_job_wait_get_id (flux_future_t *f, flux_jobid_t *id);
-# 3664 "/workspaces/flux-python/src/_core_clean.h"
+# 3644 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_job_list (flux_t *h,
                               int max_entries,
                               const char *attrs_json_str,
                               uint32_t userid,
                               int states);
 
 
@@ -2151,17 +2147,19 @@
 
 flux_future_t *flux_job_result (flux_t *h, flux_jobid_t id, int flags);
 
 
 
 int flux_job_result_get (flux_future_t *f,
                          const char **json_str);
-# 3762 "/workspaces/flux-python/src/_core_clean.h"
+# 3742 "/workspaces/flux-python/src/_core_clean.h"
 int flux_job_result_get_unpack (flux_future_t *f, const char *fmt, ...);
-# 3787 "/workspaces/flux-python/src/_core_clean.h"
+# 3756 "/workspaces/flux-python/src/_core_clean.h"
+int flux_job_timeleft (flux_t *h, flux_error_t *errp, double *timeleft);
+# 3781 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_jobspec1 flux_jobspec1_t;
 typedef flux_error_t flux_jobspec1_error_t;
 
 
 
 
 
@@ -2251,34 +2249,34 @@
 
 
 
 
 
 flux_jobspec1_t *flux_jobspec1_decode (const char *s,
                                        flux_jobspec1_error_t *error);
-# 3898 "/workspaces/flux-python/src/_core_clean.h"
+# 3892 "/workspaces/flux-python/src/_core_clean.h"
 flux_jobspec1_t *flux_jobspec1_from_command (int argc,
                                              char **argv,
                                              char **env,
                                              int ntasks,
                                              int cores_per_task,
                                              int gpus_per_task,
                                              int nnodes,
                                              double duration);
 
 
 void flux_jobspec1_destroy (flux_jobspec1_t *jobspec);
-# 3918 "/workspaces/flux-python/src/_core_clean.h"
+# 3912 "/workspaces/flux-python/src/_core_clean.h"
 extern "Python" void message_handler_wrapper(flux_t *, flux_msg_handler_t *, const flux_msg_t *, void *);
 
 
 extern "Python" void timeout_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 extern "Python" void fd_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 extern "Python" void signal_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 
 
 extern "Python" void continuation_callback(flux_future_t *, void *);
-# 3944 "/workspaces/flux-python/src/_core_clean.h"
+# 3938 "/workspaces/flux-python/src/_core_clean.h"
 extern int MPIR_being_debugged;
 extern void MPIR_Breakpoint (void);
 extern int get_mpir_being_debugged (void);
 extern void set_mpir_being_debugged (int v);
```

### Comparing `flux-python-0.46.0rc1/src/_hostlist_build.py` & `flux-python-0.48.0rc0/src/_hostlist_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/_hostlist_clean.h` & `flux-python-0.48.0rc0/src/_hostlist_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/_hostlist_preproc.h` & `flux-python-0.48.0rc0/src/_hostlist_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/_idset_build.py` & `flux-python-0.48.0rc0/src/_idset_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/_idset_clean.h` & `flux-python-0.48.0rc0/src/_idset_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/_idset_preproc.h` & `flux-python-0.48.0rc0/src/_idset_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/_rlist_build.py` & `flux-python-0.48.0rc0/src/_rlist_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/_rlist_clean.h` & `flux-python-0.48.0rc0/src/_rlist_clean.h`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 #if HAVE_CONFIG_H
 /* config/config.h.  Generated from config.h.in by configure.  */
 /* config/config.h.in.  Generated from configure.ac by autoheader.  */
 
 /* Define if building universal (internal helper macro) */
 /* #undef AC_APPLE_UNIVERSAL_BUILD */
 
+/* assume broken locale configuration and disable non-ascii characters */
+/* #undef ASSUME_BROKEN_LOCALE */
+
 /* code coverage support */
 /* #undef CODE_COVERAGE_ENABLED */
 
 /* deepbind is unsupported with asan, musl and so-forth */
 #define FLUX_DEEPBIND RTLD_DEEPBIND
 
 /* big endian */
@@ -95,17 +98,14 @@
 
 /* Define to 1 if you have the `jemalloc' library (-ljemalloc). */
 /* #undef HAVE_LIBJEMALLOC */
 
 /* Define to 1 if you have the `m' library (-lm). */
 #define HAVE_LIBM 1
 
-/* Enable PMIx bootstrap */
-/* #undef HAVE_LIBPMIX */
-
 /* Define to 1 if you have the `rt' library (-lrt). */
 /* #undef HAVE_LIBRT */
 
 /* Define to 1 if you have the `s3' library (-ls3). */
 /* #undef HAVE_LIBS3 */
 
 /* Define if you have libsystemd */
@@ -294,24 +294,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT ""
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "flux-core"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "flux-core 0.46.0"
+#define PACKAGE_STRING "flux-core 0.48.0"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "flux-core"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "0.46.0"
+#define PACKAGE_VERSION "0.48.0"
 
 /* Define remote shell program to be used by the ssh:// connector */
 #define PATH_SSH "/usr/bin/rsh"
 
 /* The python interpreter flux is configured with */
 #define PYTHON_INTERPRETER "/usr/bin/python3"
 
@@ -336,15 +336,15 @@
 /* The number of bytes in type uintptr_t */
 #define SIZEOF_UINTPTR_T 8
 
 /* Define to 1 if you have the ANSI C header files. */
 #define STDC_HEADERS 1
 
 /* Version number of package */
-#define VERSION "0.46.0"
+#define VERSION "0.48.0"
 
 /* build with jemalloc */
 /* #undef WITH_JEMALLOC */
 
 /* build with Google-perftools malloc */
 /* #undef WITH_TCMALLOC */
```

### Comparing `flux-python-0.46.0rc1/src/_rlist_preproc.h` & `flux-python-0.48.0rc0/src/_rlist_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/_security_build.py` & `flux-python-0.48.0rc0/src/_security_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/_security_clean.h` & `flux-python-0.48.0rc0/src/_security_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/_security_preproc.h` & `flux-python-0.48.0rc0/src/_security_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/callbacks.h` & `flux-python-0.48.0rc0/src/callbacks.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.46.0rc1/src/make_clean_header.py` & `flux-python-0.48.0rc0/src/make_clean_header.py`

 * *Files identical despite different names*

