# Comparing `tmp/st4sd-runtime-core-2.0.0a9.dev3.tar.gz` & `tmp/st4sd-runtime-core-2.0.0a9.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/st4sd-runtime-core-2.0.0a9.dev3.tar", last modified: Fri Apr 28 14:42:18 2023, max compression
+gzip compressed data, was "dist/st4sd-runtime-core-2.0.0a9.dev4.tar", last modified: Tue May  2 09:26:21 2023, max compression
```

## Comparing `st4sd-runtime-core-2.0.0a9.dev3.tar` & `st4sd-runtime-core-2.0.0a9.dev4.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/.github/
--rw-rw-r--   0 root         (0) root         (0)      127 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/.github/dco.yml
--rw-rw-r--   0 root         (0) root         (0)     1799 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/.gitignore
--rw-rw-r--   0 root         (0) root         (0)     8059 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/.travis.yml
--rw-rw-r--   0 root         (0) root         (0)       77 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/.whitesource
--rw-rw-r--   0 root         (0) root         (0)     3347 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/CODE_OF_CONDUCT.md
--rw-rw-r--   0 root         (0) root         (0)     2643 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/CONTRIBUTING.md
--rw-rw-r--   0 root         (0) root         (0)     2445 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/Dockerfile
--rw-rw-r--   0 root         (0) root         (0)    10774 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/LICENSE.md
--rw-rw-r--   0 root         (0) root         (0)      439 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/MAINTAINERS.md
--rw-r--r--   0 root         (0) root         (0)     4097 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3334 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/README.MD
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/
--rw-rw-r--   0 root         (0) root         (0)      180 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/creation_payload.json
--rwxrwxr-x   0 root         (0) root         (0)      292 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/skopeo_copy.sh
--rw-rw-r--   0 root         (0) root         (0)      635 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/st4sd-runtime-core-image.deploy
--rw-rw-r--   0 root         (0) root         (0)     1426 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/st4sd-runtime-core-multiarch.deploy
--rw-rw-r--   0 root         (0) root         (0)      291 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/st4sd-runtime-core-release-tag.deploy
--rwxrwxr-x   0 root         (0) root         (0)     2445 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/triggerExternalBuild.sh
--rw-rw-r--   0 root         (0) root         (0)     2442 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/py310.Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    35722 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/appenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/
--rw-rw-r--   0 root         (0) root         (0)      112 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2342 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/api.py
--rw-rw-r--   0 root         (0) root         (0)     2411 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     2891 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/context.py
--rw-rw-r--   0 root         (0) root         (0)      266 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/exit_codes.py
--rw-rw-r--   0 root         (0) root         (0)     1899 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/git.py
--rw-rw-r--   0 root         (0) root         (0)     5140 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/login.py
--rw-rw-r--   0 root         (0) root         (0)    18250 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/package.py
--rw-rw-r--   0 root         (0) root         (0)    31124 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/pvep_schema.jsonschema
--rw-rw-r--   0 root         (0) root         (0)     2300 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/stp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3003 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/codes.py
--rw-rw-r--   0 root         (0) root         (0)    82296 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/conf.py
--rw-rw-r--   0 root         (0) root         (0)   148053 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/data.py
--rw-rw-r--   0 root         (0) root         (0)    44154 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/errors.py
--rw-rw-r--   0 root         (0) root         (0)    57316 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/executors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/__init__.py
--rw-rw-r--   0 root         (0) root         (0)   126138 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/cwl.py
--rw-rw-r--   0 root         (0) root         (0)    85741 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/dosini.py
--rw-rw-r--   0 root         (0) root         (0)   257676 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/flowir.py
--rw-rw-r--   0 root         (0) root         (0)   146796 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/
--rw-rw-r--   0 root         (0) root         (0)      683 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4236 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/hooks.py
--rw-rw-r--   0 root         (0) root         (0)    36110 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/interface.py
--rw-rw-r--   0 root         (0) root         (0)     2394 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/utils.py
--rw-rw-r--   0 root         (0) root         (0)     5562 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/interface.py
--rw-rw-r--   0 root         (0) root         (0)    67317 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package/
--rw-rw-r--   0 root         (0) root         (0)      544 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package/README.MD
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package/conf/
--rw-rw-r--   0 root         (0) root         (0)      376 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package/conf/flowir_package.yaml
--rw-rw-r--   0 root         (0) root         (0)     6144 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package.tar
--rw-rw-r--   0 root         (0) root         (0)      630 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/rewrite-rules.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      753 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/docker.py
--rw-rw-r--   0 root         (0) root         (0)   114992 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/k8s.py
--rw-rw-r--   0 root         (0) root         (0)     5188 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/localtask.py
--rw-rw-r--   0 root         (0) root         (0)   113109 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/lsf.py
--rwxrwxr-x   0 root         (0) root         (0)     1414 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/stage-out.sh
--rw-rw-r--   0 root         (0) root         (0)    13277 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/task_simulator.py
--rw-rw-r--   0 root         (0) root         (0)    34639 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backends.py
--rw-rw-r--   0 root         (0) root         (0)    23603 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backends_base.py
--rw-rw-r--   0 root         (0) root         (0)   118126 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/control.py
--rw-rw-r--   0 root         (0) root         (0)   104583 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/engine.py
--rw-rw-r--   0 root         (0) root         (0)     5429 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    26290 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/cwl.py
--rw-rw-r--   0 root         (0) root         (0)     9481 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/cwl_cmdline.py
--rw-rw-r--   0 root         (0) root         (0)     8089 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/js.py
--rw-rw-r--   0 root         (0) root         (0)    20080 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/monitor.py
--rw-rw-r--   0 root         (0) root         (0)    68147 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/optimizer.py
--rw-rw-r--   0 root         (0) root         (0)    34954 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/output.py
--rw-rw-r--   0 root         (0) root         (0)    45119 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/span.py
--rw-rw-r--   0 root         (0) root         (0)    35543 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/status.py
--rw-rw-r--   0 root         (0) root         (0)     5622 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3879 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/container_image_cache.py
--rw-rw-r--   0 root         (0) root         (0)     4089 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/rx.py
--rw-rw-r--   0 root         (0) root         (0)     5384 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/s3.py
--rw-rw-r--   0 root         (0) root         (0)    36584 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/service/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/service/__init__.py
--rw-rw-r--   0 root         (0) root         (0)   259382 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/service/db.py
--rw-rw-r--   0 root         (0) root         (0)     8206 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/service/errors.py
--rw-rw-r--   0 root         (0) root         (0)     7089 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/settings.py
--rw-rw-r--   0 root         (0) root         (0)     6441 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/
--rw-rw-r--   0 root         (0) root         (0)      104 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/README
--rw-rw-r--   0 root         (0) root         (0)      317 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    58393 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/data.py
--rw-rw-r--   0 root         (0) root         (0)     4705 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/fsearch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4097 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4567 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/requirement_files/
--rw-rw-r--   0 root         (0) root         (0)      133 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/requirement_files/requirements_base_3.7.txt
--rw-rw-r--   0 root         (0) root         (0)      423 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/requirement_files/requirements_base_3.txt
--rw-rw-r--   0 root         (0) root         (0)       18 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/requirement_files/requirements_deploy.txt
--rw-rw-r--   0 root         (0) root         (0)       94 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/requirement_files/requirements_lsf.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/
--rwxrwxr-x   0 root         (0) root         (0)     7054 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/ccommand.py
--rwxrwxr-x   0 root         (0) root         (0)    11413 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/cexecute.py
--rwxrwxr-x   0 root         (0) root         (0)     1239 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/checkpackage.py
--rwxrwxr-x   0 root         (0) root         (0)     4286 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/ctest.py
--rwxrwxr-x   0 root         (0) root         (0)     2567 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/ecreate.py
--rwxrwxr-x   0 root         (0) root         (0)     4196 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/eflowir.py
--rwxrwxr-x   0 root         (0) root         (0)     8094 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/einputs.py
--rwxrwxr-x   0 root         (0) root         (0)     8246 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/einspect.py
--rwxrwxr-x   0 root         (0) root         (0)   106886 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/elaunch.py
--rwxrwxr-x   0 root         (0) root         (0)    17228 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/ememo.py
--rwxrwxr-x   0 root         (0) root         (0)    46741 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/epatch-apply.py
--rwxrwxr-x   0 root         (0) root         (0)    33324 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/epatch.py
--rwxrwxr-x   0 root         (0) root         (0)    17371 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/etest.py
--rwxrwxr-x   0 root         (0) root         (0)    10419 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/ewrap.py
--rwxrwxr-x   0 root         (0) root         (0)      821 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/expstatus.sh
--rw-rw-r--   0 root         (0) root         (0)     3840 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/k8srun.py
--rwxrwxr-x   0 root         (0) root         (0)   106886 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/launchexperiment.py
--rwxrwxr-x   0 root         (0) root         (0)    14013 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/lsfsub.py
--rwxrwxr-x   0 root         (0) root         (0)      262 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/stp
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     4693 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10844 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/conftest.py
--rw-rw-r--   0 root         (0) root         (0)    11290 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/dont_test_cwl.py
--rw-rw-r--   0 root         (0) root         (0)     4541 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/reactive_testutils.py
--rw-rw-r--   0 root         (0) root         (0)    14765 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/saltcurve_paragon.py
--rw-rw-r--   0 root         (0) root         (0)    11225 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_array_variables.py
--rw-rw-r--   0 root         (0) root         (0)     6643 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_command.py
--rw-rw-r--   0 root         (0) root         (0)     7643 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_component.py
--rw-rw-r--   0 root         (0) root         (0)     2432 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_container_image_uri_manipulation.py
--rw-rw-r--   0 root         (0) root         (0)    44829 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_control.py
--rw-rw-r--   0 root         (0) root         (0)     4840 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_data.py
--rw-rw-r--   0 root         (0) root         (0)     5588 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_db.py
--rw-rw-r--   0 root         (0) root         (0)    40697 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_dosini.py
--rw-rw-r--   0 root         (0) root         (0)    35269 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_dowhile.py
--rw-rw-r--   0 root         (0) root         (0)    30930 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_engines.py
--rw-rw-r--   0 root         (0) root         (0)    57435 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_flowir.py
--rw-rw-r--   0 root         (0) root         (0)    17145 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_graph.py
--rw-rw-r--   0 root         (0) root         (0)     3286 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_identifier.py
--rw-rw-r--   0 root         (0) root         (0)    22435 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_interface.py
--rw-rw-r--   0 root         (0) root         (0)     6059 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_k8s.py
--rw-rw-r--   0 root         (0) root         (0)     2467 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_memoization.py
--rw-rw-r--   0 root         (0) root         (0)    13525 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_package_load.py
--rw-rw-r--   0 root         (0) root         (0)     1673 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_service.py
--rw-rw-r--   0 root         (0) root         (0)     2085 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_settings.py
--rw-rw-r--   0 root         (0) root         (0)     5739 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/utils.py
--rw-rw-r--   0 root         (0) root         (0)     3119 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/.github/
+-rw-rw-r--   0 root         (0) root         (0)      127 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/.github/dco.yml
+-rw-rw-r--   0 root         (0) root         (0)     1799 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)     8059 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/.travis.yml
+-rw-rw-r--   0 root         (0) root         (0)       77 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/.whitesource
+-rw-rw-r--   0 root         (0) root         (0)     3347 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 root         (0) root         (0)     2643 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/CONTRIBUTING.md
+-rw-rw-r--   0 root         (0) root         (0)     2445 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/Dockerfile
+-rw-rw-r--   0 root         (0) root         (0)    10774 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/LICENSE.md
+-rw-rw-r--   0 root         (0) root         (0)      439 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/MAINTAINERS.md
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3334 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/README.MD
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/deploy/
+-rw-rw-r--   0 root         (0) root         (0)      180 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/deploy/creation_payload.json
+-rwxrwxr-x   0 root         (0) root         (0)      292 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/deploy/skopeo_copy.sh
+-rw-rw-r--   0 root         (0) root         (0)      635 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/deploy/st4sd-runtime-core-image.deploy
+-rw-rw-r--   0 root         (0) root         (0)     1426 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/deploy/st4sd-runtime-core-multiarch.deploy
+-rw-rw-r--   0 root         (0) root         (0)      291 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/deploy/st4sd-runtime-core-release-tag.deploy
+-rwxrwxr-x   0 root         (0) root         (0)     2445 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/deploy/triggerExternalBuild.sh
+-rw-rw-r--   0 root         (0) root         (0)     2442 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/py310.Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    35722 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/appenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/
+-rw-rw-r--   0 root         (0) root         (0)      112 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2342 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/api.py
+-rw-rw-r--   0 root         (0) root         (0)     2411 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     2891 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/context.py
+-rw-rw-r--   0 root         (0) root         (0)      266 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/exit_codes.py
+-rw-rw-r--   0 root         (0) root         (0)     1899 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/git.py
+-rw-rw-r--   0 root         (0) root         (0)     5140 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/login.py
+-rw-rw-r--   0 root         (0) root         (0)    18250 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/package.py
+-rw-rw-r--   0 root         (0) root         (0)    31124 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/pvep_schema.jsonschema
+-rw-rw-r--   0 root         (0) root         (0)     2300 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/stp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3003 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/codes.py
+-rw-rw-r--   0 root         (0) root         (0)    82296 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/conf.py
+-rw-rw-r--   0 root         (0) root         (0)   148053 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/data.py
+-rw-rw-r--   0 root         (0) root         (0)    44154 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/errors.py
+-rw-rw-r--   0 root         (0) root         (0)    57316 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/executors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/frontends/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/frontends/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)   126138 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/frontends/cwl.py
+-rw-rw-r--   0 root         (0) root         (0)    85741 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/frontends/dosini.py
+-rw-rw-r--   0 root         (0) root         (0)   257676 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/frontends/flowir.py
+-rw-rw-r--   0 root         (0) root         (0)   147639 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/hooks/
+-rw-rw-r--   0 root         (0) root         (0)      683 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/hooks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4236 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/hooks/hooks.py
+-rw-rw-r--   0 root         (0) root         (0)    36110 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/hooks/interface.py
+-rw-rw-r--   0 root         (0) root         (0)     2394 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/hooks/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5562 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/interface.py
+-rw-rw-r--   0 root         (0) root         (0)    67317 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/resources/Template.package/
+-rw-rw-r--   0 root         (0) root         (0)      544 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/resources/Template.package/README.MD
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/resources/Template.package/conf/
+-rw-rw-r--   0 root         (0) root         (0)      376 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/resources/Template.package/conf/flowir_package.yaml
+-rw-rw-r--   0 root         (0) root         (0)     6144 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/resources/Template.package.tar
+-rw-rw-r--   0 root         (0) root         (0)      630 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/rewrite-rules.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      753 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/docker.py
+-rw-rw-r--   0 root         (0) root         (0)   114992 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/k8s.py
+-rw-rw-r--   0 root         (0) root         (0)     5188 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/localtask.py
+-rw-rw-r--   0 root         (0) root         (0)   113109 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/lsf.py
+-rwxrwxr-x   0 root         (0) root         (0)     1414 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/stage-out.sh
+-rw-rw-r--   0 root         (0) root         (0)    13277 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/task_simulator.py
+-rw-rw-r--   0 root         (0) root         (0)    34639 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backends.py
+-rw-rw-r--   0 root         (0) root         (0)    23603 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backends_base.py
+-rw-rw-r--   0 root         (0) root         (0)   118126 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/control.py
+-rw-rw-r--   0 root         (0) root         (0)   104583 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/engine.py
+-rw-rw-r--   0 root         (0) root         (0)     5429 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/interpreters/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/interpreters/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    26290 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/interpreters/cwl.py
+-rw-rw-r--   0 root         (0) root         (0)     9481 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/interpreters/cwl_cmdline.py
+-rw-rw-r--   0 root         (0) root         (0)     8089 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/interpreters/js.py
+-rw-rw-r--   0 root         (0) root         (0)    20080 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/monitor.py
+-rw-rw-r--   0 root         (0) root         (0)    68147 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/optimizer.py
+-rw-rw-r--   0 root         (0) root         (0)    34954 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/output.py
+-rw-rw-r--   0 root         (0) root         (0)    45119 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/span.py
+-rw-rw-r--   0 root         (0) root         (0)    35543 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/status.py
+-rw-rw-r--   0 root         (0) root         (0)     5622 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/utilities/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3879 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/utilities/container_image_cache.py
+-rw-rw-r--   0 root         (0) root         (0)     4089 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/utilities/rx.py
+-rw-rw-r--   0 root         (0) root         (0)     5384 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/utilities/s3.py
+-rw-rw-r--   0 root         (0) root         (0)    36584 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/service/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/service/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)   259382 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/service/db.py
+-rw-rw-r--   0 root         (0) root         (0)     8206 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/service/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     7089 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/settings.py
+-rw-rw-r--   0 root         (0) root         (0)     6441 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/utilities/
+-rw-rw-r--   0 root         (0) root         (0)      104 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/utilities/README
+-rw-rw-r--   0 root         (0) root         (0)      317 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    58393 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/utilities/data.py
+-rw-rw-r--   0 root         (0) root         (0)     4705 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/python/experiment/utilities/fsearch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/st4sd_runtime_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/st4sd_runtime_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/st4sd_runtime_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/st4sd_runtime_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/st4sd_runtime_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/python/st4sd_runtime_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/requirement_files/
+-rw-rw-r--   0 root         (0) root         (0)      133 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/requirement_files/requirements_base_3.7.txt
+-rw-rw-r--   0 root         (0) root         (0)      423 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/requirement_files/requirements_base_3.txt
+-rw-rw-r--   0 root         (0) root         (0)       18 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/requirement_files/requirements_deploy.txt
+-rw-rw-r--   0 root         (0) root         (0)       94 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/requirement_files/requirements_lsf.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/
+-rwxrwxr-x   0 root         (0) root         (0)     7054 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/ccommand.py
+-rwxrwxr-x   0 root         (0) root         (0)    11413 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/cexecute.py
+-rwxrwxr-x   0 root         (0) root         (0)     1239 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/checkpackage.py
+-rwxrwxr-x   0 root         (0) root         (0)     4286 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/ctest.py
+-rwxrwxr-x   0 root         (0) root         (0)     2567 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/ecreate.py
+-rwxrwxr-x   0 root         (0) root         (0)     4196 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/eflowir.py
+-rwxrwxr-x   0 root         (0) root         (0)     8094 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/einputs.py
+-rwxrwxr-x   0 root         (0) root         (0)     8246 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/einspect.py
+-rwxrwxr-x   0 root         (0) root         (0)   106886 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/elaunch.py
+-rwxrwxr-x   0 root         (0) root         (0)    17228 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/ememo.py
+-rwxrwxr-x   0 root         (0) root         (0)    46741 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/epatch-apply.py
+-rwxrwxr-x   0 root         (0) root         (0)    33324 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/epatch.py
+-rwxrwxr-x   0 root         (0) root         (0)    17371 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/etest.py
+-rwxrwxr-x   0 root         (0) root         (0)    10419 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/ewrap.py
+-rwxrwxr-x   0 root         (0) root         (0)      821 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/expstatus.sh
+-rw-rw-r--   0 root         (0) root         (0)     3840 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/k8srun.py
+-rwxrwxr-x   0 root         (0) root         (0)   106886 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/launchexperiment.py
+-rwxrwxr-x   0 root         (0) root         (0)    14013 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/lsfsub.py
+-rwxrwxr-x   0 root         (0) root         (0)      262 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/scripts/stp
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     4693 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:26:21.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10844 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/conftest.py
+-rw-rw-r--   0 root         (0) root         (0)    11290 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/dont_test_cwl.py
+-rw-rw-r--   0 root         (0) root         (0)     4541 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/reactive_testutils.py
+-rw-rw-r--   0 root         (0) root         (0)    14765 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/saltcurve_paragon.py
+-rw-rw-r--   0 root         (0) root         (0)    11225 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_array_variables.py
+-rw-rw-r--   0 root         (0) root         (0)     6643 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_command.py
+-rw-rw-r--   0 root         (0) root         (0)     7643 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_component.py
+-rw-rw-r--   0 root         (0) root         (0)     2432 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_container_image_uri_manipulation.py
+-rw-rw-r--   0 root         (0) root         (0)    44829 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_control.py
+-rw-rw-r--   0 root         (0) root         (0)     4840 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_data.py
+-rw-rw-r--   0 root         (0) root         (0)     5588 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_db.py
+-rw-rw-r--   0 root         (0) root         (0)    40697 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_dosini.py
+-rw-rw-r--   0 root         (0) root         (0)    35269 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_dowhile.py
+-rw-rw-r--   0 root         (0) root         (0)    30930 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_engines.py
+-rw-rw-r--   0 root         (0) root         (0)    57435 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_flowir.py
+-rw-rw-r--   0 root         (0) root         (0)    18304 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_graph.py
+-rw-rw-r--   0 root         (0) root         (0)     3286 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_identifier.py
+-rw-rw-r--   0 root         (0) root         (0)    22435 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_interface.py
+-rw-rw-r--   0 root         (0) root         (0)     6059 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_k8s.py
+-rw-rw-r--   0 root         (0) root         (0)     2467 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_memoization.py
+-rw-rw-r--   0 root         (0) root         (0)    13525 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_package_load.py
+-rw-rw-r--   0 root         (0) root         (0)     1673 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_service.py
+-rw-rw-r--   0 root         (0) root         (0)     2085 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/test_settings.py
+-rw-rw-r--   0 root         (0) root         (0)     5739 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tests/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3119 2023-05-02 09:22:39.000000 st4sd-runtime-core-2.0.0a9.dev4/tox.ini
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/.gitignore` & `st4sd-runtime-core-2.0.0a9.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/.travis.yml` & `st4sd-runtime-core-2.0.0a9.dev4/.travis.yml`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/CODE_OF_CONDUCT.md` & `st4sd-runtime-core-2.0.0a9.dev4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/CONTRIBUTING.md` & `st4sd-runtime-core-2.0.0a9.dev4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/Dockerfile` & `st4sd-runtime-core-2.0.0a9.dev4/Dockerfile`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/LICENSE.md` & `st4sd-runtime-core-2.0.0a9.dev4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/PKG-INFO` & `st4sd-runtime-core-2.0.0a9.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st4sd-runtime-core
-Version: 2.0.0a9.dev3
+Version: 2.0.0a9.dev4
 Summary: A tool for creating and deploying computational experiments
 Home-page: https://github.com/st4sd/st4sd-runtime-core
 Author: Michael A. Johnston
 Author-email: michaelj@ie.ibm.com
 License: Apache 2.0
 Keywords: hpc kubernetes openshift lsf workflows experiments computational-chemistry simulation science
 Classifier: Development Status :: 4 - Beta
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/README.MD` & `st4sd-runtime-core-2.0.0a9.dev4/README.MD`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/deploy/st4sd-runtime-core-image.deploy` & `st4sd-runtime-core-2.0.0a9.dev4/deploy/st4sd-runtime-core-image.deploy`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/deploy/st4sd-runtime-core-multiarch.deploy` & `st4sd-runtime-core-2.0.0a9.dev4/deploy/st4sd-runtime-core-multiarch.deploy`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/deploy/triggerExternalBuild.sh` & `st4sd-runtime-core-2.0.0a9.dev4/deploy/triggerExternalBuild.sh`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/py310.Dockerfile` & `st4sd-runtime-core-2.0.0a9.dev4/py310.Dockerfile`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/appenv.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/appenv.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/api.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/api.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/configuration.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/context.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/context.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/git.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/git.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/login.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/login.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/package.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/package.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/pvep_schema.jsonschema` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/pvep_schema.jsonschema`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/stp.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/cli/stp.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/codes.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/codes.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/conf.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/conf.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/data.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/data.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/errors.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/errors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/executors.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/executors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/cwl.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/frontends/cwl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/dosini.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/frontends/dosini.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/flowir.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/frontends/flowir.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/graph.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1081,29 +1081,22 @@
         comp_with_platform = self.workflowGraphRef().configurationForNode(
             self.identification.identifier, raw=True,
             omitDefault=False, is_primitive=True)
 
         comp_vars = OrderedDict(comp_no_platform.get('variables', {}))
 
         all_var_refs = experiment.model.frontends.flowir.FlowIR.discover_references_to_variables(comp_with_platform)
-        parameters = [{'name': name} for name in sorted(set(all_var_refs).difference(comp_vars))]
 
-        command = comp_with_platform.get('command', {})
-
-        # VV: In the new DSL environment is either a dictionary of key: value items OR a reference to a parameter
-        if 'environment' in command:
-            # VV: We can generate a parameter, call it "env-vars" and assign the environment to it so that
-            # callers of this component can update the environment. If the component already has such a variable
-            # then just use the entire environment as is with no way to override it.
+        # VV: Order of parameters:
+        # 1. reference parameters
+        # 2. parameters which define values of variables (e.g. platform)
+        # 3. the env-var parameter
+        parameters = []
 
-            if any(filter(lambda x: x['name'] == 'env-vars', parameters)):
-                command['environment'] = self.environment
-            else:
-                parameters.append({'name': 'env-vars', 'default': self.environment})
-                command['environment'] = "$(env-vars)s"
+        command = comp_with_platform.get('command', {})
 
         # VV: In the new DSL the references are auto-generated from parameters whose value follows the
         # <producer>[/fileref]:<method> schema. Need to auto-generate parameters for references and then rewrite
         # the instances of references in the arguments (because that's the only place that they can appear) so that
         # they look like parameter references (i.e. %(hello)s).
         # Use param<index of reference> for the name of the auto-generated parameter.
         # FIXME I cannot think of a way to fully handle a :copy reference - the developer may have used information
@@ -1129,14 +1122,28 @@
             arguments = arguments.replace(dref.absoluteReference, f'%({new_param})s')
             if dref.stageIndex == self.identification.stageIndex:
                 arguments = arguments.replace(dref.relativeReference, f'%({new_param})s')
 
         if arguments:
             command['arguments'] = arguments
 
+        parameters.extend([{'name': name} for name in sorted(set(all_var_refs).difference(comp_vars))])
+
+        # VV: In the new DSL environment is either a dictionary of key: value items OR a reference to a parameter
+        if 'environment' in command:
+            # VV: We can generate a parameter, call it "env-vars" and assign the environment to it so that
+            # callers of this component can update the environment. If the component already has such a variable
+            # then just use the entire environment as is with no way to override it.
+
+            if any(filter(lambda x: x['name'] == 'env-vars', parameters)):
+                command['environment'] = self.environment
+            else:
+                parameters.append({'name': 'env-vars', 'default': self.environment})
+                command['environment'] = "$(env-vars)s"
+
         signature=OrderedDict( (('name', self.identification.identifier), ('parameters', parameters)) )
         dsl = OrderedDict(( ('signature', signature), ))
 
         if comp_vars:
             dsl['variables'] = comp_vars
 
         dsl['command'] = command
@@ -2317,33 +2324,27 @@
     def dsl_workflow_blueprint(self):
         """Returns the workflow blueprint in the DSL of st4sd.
 
         This is a WIP method and subject to changes.
         """
         platform_vars = self._concrete.get_platform_variables()[experiment.model.frontends.flowir.FlowIR.LabelGlobal]
 
-        # VV: The arguments to the workflow are platform variables
-        # TODO we need a way to handle stage variables - they are basically different variables which
-        # happen to occupy the same name as the global platform variables but only for a subset of components
-        # those that belong in that certain stage index
-        parameters = [
-            {'name': name, "default": platform_vars[name]} for name in sorted(platform_vars)
-        ]
-
         graph = self.graph
 
         top_level_folders = self.configuration.top_level_folders
         app_deps = self.configuration.get_application_dependencies()
 
         # VV: References that do not point to components are parameters of workflow
         # Those that are pointing to `input` files should also be part of entrypoint.execute.args
         # Those that point to app-deps/data, etc should not be part of entrypoint but should have a default value
         #   (the reference string)
         known_param_refs = dict()
 
+        params_no_default = []
+        params_with_default = []
         # VV: Must visit references in the correct order
         for name in sorted(graph.nodes):
             spec: ComponentSpecification = graph.nodes[name]['componentSpecification']
             for ref in sorted(spec.rawDataReferences):
 
                 if ref in known_param_refs:
                     continue
@@ -2356,20 +2357,36 @@
                     # VV: This is a reference that points to a component, skip it
                     continue
 
                 num_param = len(known_param_refs)
                 param_name = f"param{num_param}"
 
                 if jobName.split("/")[0] != "input":
-                    parameters.append({'name': param_name, 'default': ref})
+                    params_with_default.append({'name': param_name, 'default': ref})
                 else:
-                    parameters.append({'name': param_name})
+                    params_no_default.append({'name': param_name})
 
                 known_param_refs[ref] = param_name
 
+        # VV: The order of parameters is:
+        # 1. parameters with no default values (e.g. input files)
+        # 2. parameters with default values that are references (e.g. application-dependencies)
+        # 3. parameters with default values that are variables
+
+        parameters = []
+        parameters.extend(sorted(params_no_default, key=lambda x: x['name']))
+        parameters.extend(sorted(params_with_default, key=lambda x: x['name']))
+
+        # VV: Variables which manifest as parameters with default values should be at the bottom of the parameter list
+        # VV: The arguments to the workflow are platform variables
+        # TODO we need a way to handle stage variables - they are basically different variables which
+        # happen to occupy the same name as the global platform variables but only for a subset of components
+        # those that belong in that certain stage index
+        parameters.extend([{'name': name, "default": platform_vars[name]} for name in sorted(platform_vars)])
+
         signature = OrderedDict((('name', "main"), ('parameters', parameters)))
         workflow = OrderedDict((('signature', signature),))
 
         workflow['steps'] = OrderedDict( ((name, name) for name in networkx.topological_sort(graph)) )
         workflow['execute'] = [
             {
                 'target': f"<{name}>",
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/__init__.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/hooks.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/hooks/hooks.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/interface.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/hooks/interface.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/utils.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/hooks/utils.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/interface.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/interface.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/storage.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/model/storage.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package/README.MD` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/resources/Template.package/README.MD`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package.tar` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/resources/Template.package.tar`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/rewrite-rules.json` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/rewrite-rules.json`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/docker.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/docker.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/k8s.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/k8s.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/localtask.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/localtask.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/lsf.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/lsf.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/stage-out.sh` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/stage-out.sh`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/task_simulator.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backend_interfaces/task_simulator.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backends.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backends.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backends_base.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/backends_base.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/control.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/control.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/engine.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/engine.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/errors.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/errors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/cwl.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/interpreters/cwl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/cwl_cmdline.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/interpreters/cwl_cmdline.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/js.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/interpreters/js.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/monitor.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/monitor.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/optimizer.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/optimizer.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/output.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/output.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/span.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/span.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/status.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/status.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/task.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/task.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/container_image_cache.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/utilities/container_image_cache.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/rx.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/utilities/rx.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/s3.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/utilities/s3.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/workflow.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/runtime/workflow.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/service/db.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/service/db.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/service/errors.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/service/errors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/settings.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/settings.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/test.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/test.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/data.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/utilities/data.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/fsearch.py` & `st4sd-runtime-core-2.0.0a9.dev4/python/experiment/utilities/fsearch.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/PKG-INFO` & `st4sd-runtime-core-2.0.0a9.dev4/python/st4sd_runtime_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st4sd-runtime-core
-Version: 2.0.0a9.dev3
+Version: 2.0.0a9.dev4
 Summary: A tool for creating and deploying computational experiments
 Home-page: https://github.com/st4sd/st4sd-runtime-core
 Author: Michael A. Johnston
 Author-email: michaelj@ie.ibm.com
 License: Apache 2.0
 Keywords: hpc kubernetes openshift lsf workflows experiments computational-chemistry simulation science
 Classifier: Development Status :: 4 - Beta
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/SOURCES.txt` & `st4sd-runtime-core-2.0.0a9.dev4/python/st4sd_runtime_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/ccommand.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/ccommand.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/cexecute.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/cexecute.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/checkpackage.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/checkpackage.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/ctest.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/ctest.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/ecreate.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/ecreate.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/eflowir.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/eflowir.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/einputs.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/einputs.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/einspect.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/einspect.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/elaunch.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/elaunch.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/ememo.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/ememo.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/epatch-apply.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/epatch-apply.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/epatch.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/epatch.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/etest.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/etest.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/ewrap.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/ewrap.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/expstatus.sh` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/expstatus.sh`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/k8srun.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/k8srun.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/launchexperiment.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/launchexperiment.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/scripts/lsfsub.py` & `st4sd-runtime-core-2.0.0a9.dev4/scripts/lsfsub.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/setup.py` & `st4sd-runtime-core-2.0.0a9.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/conftest.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/dont_test_cwl.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/dont_test_cwl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/reactive_testutils.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/reactive_testutils.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/saltcurve_paragon.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/saltcurve_paragon.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_array_variables.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_array_variables.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_command.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_component.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_container_image_uri_manipulation.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_container_image_uri_manipulation.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_control.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_data.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_db.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_dosini.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_dosini.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_dowhile.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_dowhile.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_engines.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_engines.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_flowir.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_flowir.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_graph.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,22 +153,22 @@
         name: dict(value) if isinstance(value, OrderedDict) else value for (name, value) in dsl.items()
     }
 
     assert dsl == {
         'signature': {
             'name': 'stage0.hello',
             'parameters': [
+                {'name': 'param0'},
+                {'name': 'param1'},
                 {
                     'name': 'env-vars',
                     'default': {
                         'FOO': 'bar'
                     }
                 },
-                {'name': 'param0'},
-                {'name': 'param1'}
             ]},
         'variables': {
             'name': 'wisdom'
         },
         'command': {'executable': 'sh', 'arguments': '-c "hello %(name)s; ls -lth %(param0)s %(param1)s"',
                     'resolvePath': True, 'expandArguments': 'none', 'interpreter': None, 'environment': '$(env-vars)s'},
         'resourceRequest': {'numberProcesses': 1, 'numberThreads': 1, 'ranksPerNode': 1, 'threadsPerCore': 1,
@@ -226,23 +226,23 @@
     dsl = spec.dsl_component_blueprint()
 
     dsl = {
         name: dict(value) if isinstance(value, OrderedDict) else value for (name, value) in dsl.items()
     }
 
     assert dsl['signature']['parameters'] == [
+        {'name': 'param0'},
+        {'name': 'param1'},
         {'name': 'from-platform'},
         {
             'name': 'env-vars',
             'default': {
                 'FOO': 'bar'
             }
         },
-        {'name': 'param0'},
-        {'name': 'param1'}
     ]
 
     assert dsl['variables'] == {
         'name': 'wisdom'
     }
 
 
@@ -292,17 +292,17 @@
     assert len(dsl['workflows']) == 1
 
     workflow = dsl['workflows'][0]
 
     assert workflow['signature'] == {
         'name': 'main',
         'parameters': [
-            {'name': 'from-platform', 'default': 'in-entrypoint'},
             {'name': 'param0', 'default': 'dataset:ref'},
             {'name': 'param1', 'default': 'fromManifest:ref'},
+            {'name': 'from-platform', 'default': 'in-entrypoint'},
         ]
     }
 
     assert workflow['steps'] == {'stage0.hello': 'stage0.hello'}
 
     assert workflow['execute'] == [
                 {
@@ -369,17 +369,17 @@
     assert len(dsl['workflows']) == 1
 
     workflow = dsl['workflows'][0]
 
     assert workflow['signature'] == {
         'name': 'main',
         'parameters': [
-            {'name': 'from-platform', 'default': 'in-entrypoint'},
             {'name': 'param0', 'default': 'dataset:ref'},
-            {'name': 'param1', 'default': 'fromManifest:ref'}
+            {'name': 'param1', 'default': 'fromManifest:ref'},
+            {'name': 'from-platform', 'default': 'in-entrypoint'},
         ]
     }
 
     assert workflow['steps'] == {
         'stage0.hello': 'stage0.hello',
         'stage0.consume': 'stage0.consume',
     }
@@ -439,18 +439,18 @@
     workflow = dsl['workflows'][0]
 
     workflow = {name: dict(value) if isinstance(value, OrderedDict) else value for (name, value) in workflow.items()}
 
     assert workflow['signature'] == {
         'name': 'main',
         'parameters': [
-            {'name': 'from-platform', 'default': 'in-entrypoint'},
+            {'name': 'param2'},
             {'name': 'param0', 'default': 'dataset:ref'},
             {'name': 'param1', 'default': 'fromManifest:ref'},
-            {'name': 'param2'}
+            {'name': 'from-platform', 'default': 'in-entrypoint'},
         ]
     }
 
     assert workflow['steps'] == {'stage0.hello': 'stage0.hello'}
 
     assert workflow['execute'] == [
         {
@@ -516,18 +516,18 @@
     assert len(dsl['workflows']) == 1
 
     workflow = dsl['workflows'][0]
 
     assert workflow['signature'] == {
         'name': 'main',
         'parameters': [
-            {'name': 'another-var', 'default': 'in-entrypoint'},
-            {'name': 'from-platform', 'default': 'in-entrypoint'},
             {'name': 'param0', 'default': 'dataset:ref'},
             {'name': 'param1', 'default': 'fromManifest:ref'},
+            {'name': 'another-var', 'default': 'in-entrypoint'},
+            {'name': 'from-platform', 'default': 'in-entrypoint'},
         ]
     }
 
     assert workflow['steps'] == {'stage0.hello': 'stage0.hello'}
 
     assert workflow['execute'] == [
                 {
@@ -536,7 +536,51 @@
                         'from-platform': '%(from-platform)s',
                         'another-var': '%(another-var)s',
                         'param0': '%(param0)s',
                         'param1': '%(param1)s'
                     }
                 }
             ]
+
+
+def test_graph_generate_new_dsl_workflow_one_component_param_order():
+    flowir = experiment.model.frontends.flowir.yaml_load("""
+        application-dependencies:
+          default:
+          - dataset
+        environments:
+          default:
+            my-env:
+              FOO: bar
+        
+        variables:
+          default:
+            global:
+              backend: kubernetes
+
+        components:
+        - name: hello
+          command:
+            executable: sh
+            arguments: -c "hello %(backend)s; ls -lth dataset:ref; cat input/msg.txt:ref"
+            expandArguments: "none"
+            environment: my-env
+          references:
+          - dataset:ref
+          - input/msg.txt:ref
+        """)
+    graph = experiment.model.graph.WorkflowGraph.graphFromFlowIR(flowir, {})
+
+    dsl = graph.to_dsl()
+
+    assert len(dsl['workflows']) == 1
+
+    workflow = dsl['workflows'][0]
+
+    assert workflow['signature'] == {
+        'name': 'main',
+        'parameters': [
+            {'name': 'param1'},
+            {'name': 'param0', 'default': 'dataset:ref'},
+            {'name': 'backend', 'default': 'kubernetes'}
+        ]
+    }
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_identifier.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_interface.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_k8s.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_k8s.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_memoization.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_memoization.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_package_load.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_package_load.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_service.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/test_settings.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tests/utils.py` & `st4sd-runtime-core-2.0.0a9.dev4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev3/tox.ini` & `st4sd-runtime-core-2.0.0a9.dev4/tox.ini`

 * *Files identical despite different names*

