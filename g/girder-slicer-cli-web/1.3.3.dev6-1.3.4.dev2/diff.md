# Comparing `tmp/girder-slicer-cli-web-1.3.3.dev6.tar.gz` & `tmp/girder-slicer-cli-web-1.3.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-slicer-cli-web-1.3.3.dev6.tar", last modified: Tue May  2 12:24:22 2023, max compression
+gzip compressed data, was "girder-slicer-cli-web-1.3.4.dev2.tar", last modified: Tue May  2 15:20:12 2023, max compression
```

## Comparing `girder-slicer-cli-web-1.3.3.dev6.tar` & `girder-slicer-cli-web-1.3.4.dev2.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.594419 girder-slicer-cli-web-1.3.3.dev6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.562419 girder-slicer-cli-web-1.3.3.dev6/.circleci/
--rw-r--r--   0 root         (0) root         (0)     7841 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)     4002 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/.dockerignore
--rw-r--r--   0 root         (0) root         (0)      406 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/.editorconfig
--rw-r--r--   0 root         (0) root         (0)     1734 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/LICENSE
--rw-r--r--   0 root         (0) root         (0)    16189 2023-05-02 12:24:22.594419 girder-slicer-cli-web-1.3.3.dev6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15141 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/README.rst
--rw-r--r--   0 root         (0) root         (0)      461 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/codecov.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.562419 girder-slicer-cli-web-1.3.3.dev6/docs/
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/docs/worker_management.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.562419 girder-slicer-cli-web-1.3.3.dev6/example-average-color/
--rw-r--r--   0 root         (0) root         (0)     4002 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-average-color/.dockerignore
--rw-r--r--   0 root         (0) root         (0)      259 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-average-color/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      885 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-average-color/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.562419 girder-slicer-cli-web-1.3.3.dev6/example-average-color/average_color/
--rw-r--r--   0 root         (0) root         (0)     1515 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-average-color/average_color/average_color.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-average-color/average_color/average_color.xml
--rw-r--r--   0 root         (0) root         (0)       50 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-average-color/cli_list.json
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-average-color/cli_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.566419 girder-slicer-cli-web-1.3.3.dev6/example-girder-requests/
--rw-r--r--   0 root         (0) root         (0)      289 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-girder-requests/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      507 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-girder-requests/README.rst
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-girder-requests/cli_list.json
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-girder-requests/cli_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.566419 girder-slicer-cli-web-1.3.3.dev6/example-girder-requests/girder_requests/
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-girder-requests/girder_requests/girder_requests.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/example-girder-requests/girder_requests/girder_requests.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.566419 girder-slicer-cli-web-1.3.3.dev6/girder_slicer_cli_web.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16189 2023-05-02 12:24:22.000000 girder-slicer-cli-web-1.3.3.dev6/girder_slicer_cli_web.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6030 2023-05-02 12:24:22.000000 girder-slicer-cli-web-1.3.3.dev6/girder_slicer_cli_web.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 12:24:22.000000 girder-slicer-cli-web-1.3.3.dev6/girder_slicer_cli_web.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-02 12:24:22.000000 girder-slicer-cli-web-1.3.3.dev6/girder_slicer_cli_web.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 12:23:45.000000 girder-slicer-cli-web-1.3.3.dev6/girder_slicer_cli_web.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-02 12:24:22.000000 girder-slicer-cli-web-1.3.3.dev6/girder_slicer_cli_web.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-02 12:24:22.000000 girder-slicer-cli-web-1.3.3.dev6/girder_slicer_cli_web.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-02 12:24:22.594419 girder-slicer-cli-web-1.3.3.dev6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2898 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.566419 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/
--rw-r--r--   0 root         (0) root         (0)     1344 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3506 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/cli_list_entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2501 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/cli_utils.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/config.py
--rw-r--r--   0 root         (0) root         (0)     6649 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/ctk_cli_adjustment.py
--rw-r--r--   0 root         (0) root         (0)    15903 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/docker_resource.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/girder_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.570419 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/girder_worker_plugin/
--rw-r--r--   0 root         (0) root         (0)     1018 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/girder_worker_plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/girder_worker_plugin/cli_progress.py
--rw-r--r--   0 root         (0) root         (0)     3834 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/girder_worker_plugin/direct_docker_run.py
--rw-r--r--   0 root         (0) root         (0)    12039 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/image_job.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.570419 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/models/
--rw-r--r--   0 root         (0) root         (0)      208 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10452 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/models/docker_image.py
--rw-r--r--   0 root         (0) root         (0)      810 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/models/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3314 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/models/json_to_xml.py
--rw-r--r--   0 root         (0) root         (0)     2340 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/models/parser.py
--rw-r--r--   0 root         (0) root         (0)    32185 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/models/schema.json
--rw-r--r--   0 root         (0) root         (0)    14268 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/prepare_task.py
--rw-r--r--   0 root         (0) root         (0)    25904 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/rest_slicer_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.570419 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/
--rw-r--r--   0 root         (0) root         (0)      404 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/JobStatus.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.570419 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/collections/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/collections/WidgetCollection.js
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/collections/index.js
--rw-r--r--   0 root         (0) root         (0)       78 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/events.js
--rw-r--r--   0 root         (0) root         (0)      299 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/index.js
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.570419 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/models/
--rw-r--r--   0 root         (0) root         (0)     9732 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/models/WidgetModel.js
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/models/index.js
--rw-r--r--   0 root         (0) root         (0)     3996 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.574419 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/
--rw-r--r--   0 root         (0) root         (0)      540 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/constraints.js
--rw-r--r--   0 root         (0) root         (0)      610 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/convert.js
--rw-r--r--   0 root         (0) root         (0)      671 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/defaultValue.js
--rw-r--r--   0 root         (0) root         (0)      894 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/group.js
--rw-r--r--   0 root         (0) root         (0)      384 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/index.js
--rw-r--r--   0 root         (0) root         (0)      506 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/panel.js
--rw-r--r--   0 root         (0) root         (0)     2521 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/param.js
--rw-r--r--   0 root         (0) root         (0)     1595 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/parse.js
--rw-r--r--   0 root         (0) root         (0)      921 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/widget.js
--rw-r--r--   0 root         (0) root         (0)      404 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/routes.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.574419 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/stylesheets/
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/stylesheets/configView.styl
--rw-r--r--   0 root         (0) root         (0)      926 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/stylesheets/controlWidget.styl
--rw-r--r--   0 root         (0) root         (0)      112 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/stylesheets/controlsPanel.styl
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/stylesheets/outputParameterDialog.styl
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/stylesheets/panel.styl
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/stylesheets/panelGroup.styl
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/stylesheets/slicerUI.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.574419 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/
--rw-r--r--   0 root         (0) root         (0)      173 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/booleanWidget.pug
--rw-r--r--   0 root         (0) root         (0)      115 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/colorWidget.pug
--rw-r--r--   0 root         (0) root         (0)     2165 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/configView.pug
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/controlsPanel.pug
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/enumerationWidget.pug
--rw-r--r--   0 root         (0) root         (0)     1305 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/fileWidget.pug
--rw-r--r--   0 root         (0) root         (0)      621 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/jobsListWidget.pug
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/outputParameterDialog.pug
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/panel.pug
--rw-r--r--   0 root         (0) root         (0)      529 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/panelGroup.pug
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/rangeWidget.pug
--rw-r--r--   0 root         (0) root         (0)     2921 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/regionWidget.pug
--rw-r--r--   0 root         (0) root         (0)      308 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/slicerUI.pug
--rw-r--r--   0 root         (0) root         (0)      735 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/uploadImageDialog.pug
--rw-r--r--   0 root         (0) root         (0)      569 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/widget.pug
--rw-r--r--   0 root         (0) root         (0)     1642 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/utils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.578419 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/
--rw-r--r--   0 root         (0) root         (0)     4761 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/CollectionView.js
--rw-r--r--   0 root         (0) root         (0)     7145 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/ConfigView.js
--rw-r--r--   0 root         (0) root         (0)    17436 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/ControlWidget.js
--rw-r--r--   0 root         (0) root         (0)     1542 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/ControlsPanel.js
--rw-r--r--   0 root         (0) root         (0)    11455 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/ItemSelectorWidget.js
--rw-r--r--   0 root         (0) root         (0)     4584 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/ItemView.js
--rw-r--r--   0 root         (0) root         (0)     3798 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/JobsListWidget.js
--rw-r--r--   0 root         (0) root         (0)      799 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/JobsPanel.js
--rw-r--r--   0 root         (0) root         (0)      532 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/OutputParameterDialog.js
--rw-r--r--   0 root         (0) root         (0)     1150 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/Panel.js
--rw-r--r--   0 root         (0) root         (0)     8397 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/PanelGroup.js
--rw-r--r--   0 root         (0) root         (0)      394 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/index.js
--rw-r--r--   0 root         (0) root         (0)      872 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/utils.js
--rw-r--r--   0 root         (0) root         (0)     7791 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/worker_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.578419 girder-slicer-cli-web-1.3.3.dev6/small-docker/
--rw-r--r--   0 root         (0) root         (0)     4002 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/.dockerignore
--rw-r--r--   0 root         (0) root         (0)      719 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.578419 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example1/
--rw-r--r--   0 root         (0) root         (0)    10493 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example1/Example1.json
--rw-r--r--   0 root         (0) root         (0)      681 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example1/Example1.py
--rw-r--r--   0 root         (0) root         (0)    10227 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example1/Example1.xml
--rw-r--r--   0 root         (0) root         (0)     7115 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example1/Example1.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.578419 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example2/
--rw-r--r--   0 root         (0) root         (0)     1041 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example2/Example2.json
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example2/Example2.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example2/Example2.xml
--rw-r--r--   0 root         (0) root         (0)      639 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example2/Example2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.590419 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example3/
--rw-r--r--   0 root         (0) root         (0)     1034 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example3/Example3.json
--rw-r--r--   0 root         (0) root         (0)      621 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example3/Example3.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example3/Example3.xml
--rw-r--r--   0 root         (0) root         (0)      626 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/Example3/Example3.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.590419 girder-slicer-cli-web-1.3.3.dev6/small-docker/ExampleProgress/
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/ExampleProgress/ExampleProgress.json
--rw-r--r--   0 root         (0) root         (0)      884 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/ExampleProgress/ExampleProgress.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/ExampleProgress/progress_helper.py
--rw-r--r--   0 root         (0) root         (0)      523 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/cli_list.json
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/small-docker/cli_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.590419 girder-slicer-cli-web-1.3.3.dev6/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10287 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.590419 girder-slicer-cli-web-1.3.3.dev6/tests/data/
--rw-r--r--   0 root         (0) root         (0)     3850 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/data/ExampleSpec.xml
--rw-r--r--   0 root         (0) root         (0)      301 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/data/girder_worker.cfg
--rw-r--r--   0 root         (0) root         (0)     1442 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/data/parser_params_advanced.json
--rw-r--r--   0 root         (0) root         (0)     1183 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/data/parser_params_advanced.xml
--rw-r--r--   0 root         (0) root         (0)      775 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/data/parser_params_advanced.yaml
--rw-r--r--   0 root         (0) root         (0)      232 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/data/parser_params_simple.json
--rw-r--r--   0 root         (0) root         (0)      218 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/data/parser_params_simple.xml
--rw-r--r--   0 root         (0) root         (0)      109 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/data/parser_params_simple.yaml
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/data/parser_simple.json
--rw-r--r--   0 root         (0) root         (0)      319 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/data/parser_simple.xml
--rw-r--r--   0 root         (0) root         (0)      152 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/data/parser_simple.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.594419 girder-slicer-cli-web-1.3.3.dev6/tests/girder_worker_plugin/
--rw-r--r--   0 root         (0) root         (0)     2761 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/girder_worker_plugin/test_cli_progress.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/girder_worker_plugin/test_direct_docker_run.py
--rw-r--r--   0 root         (0) root         (0)     4961 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/test_batch.py
--rw-r--r--   0 root         (0) root         (0)      762 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     6041 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/test_docker.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/test_load.py
--rw-r--r--   0 root         (0) root         (0)     5923 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/test_parser.py
--rw-r--r--   0 root         (0) root         (0)    10504 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/test_rest_slicer_cli.py
--rw-r--r--   0 root         (0) root         (0)      867 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/test_web_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.594419 girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/
--rw-r--r--   0 root         (0) root         (0)      237 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/.eslintrc
--rw-r--r--   0 root         (0) root         (0)     2410 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/configViewSpec.js
--rw-r--r--   0 root         (0) root         (0)     4543 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/containerViewSpec.js
--rw-r--r--   0 root         (0) root         (0)     6091 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/dockerTaskSpec.js
--rw-r--r--   0 root         (0) root         (0)     9822 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/itemSelectorWidgetSpec.js
--rw-r--r--   0 root         (0) root         (0)     2503 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/panelGroupSpec.js
--rw-r--r--   0 root         (0) root         (0)    27393 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/parseSpec.js
--rw-r--r--   0 root         (0) root         (0)    43069 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/widgetSpec.js
--rw-r--r--   0 root         (0) root         (0)     2508 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/tox.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:24:22.594419 girder-slicer-cli-web-1.3.3.dev6/utils/
--rw-r--r--   0 root         (0) root         (0)     3879 2023-05-02 12:23:34.000000 girder-slicer-cli-web-1.3.3.dev6/utils/xmltojson.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.556704 girder-slicer-cli-web-1.3.4.dev2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.516704 girder-slicer-cli-web-1.3.4.dev2/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     7841 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)      406 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    16189 2023-05-02 15:20:12.556704 girder-slicer-cli-web-1.3.4.dev2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15141 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      461 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.516704 girder-slicer-cli-web-1.3.4.dev2/docs/
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/docs/worker_management.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.516704 girder-slicer-cli-web-1.3.4.dev2/example-average-color/
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-average-color/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)      259 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-average-color/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      885 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-average-color/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.516704 girder-slicer-cli-web-1.3.4.dev2/example-average-color/average_color/
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-average-color/average_color/average_color.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-average-color/average_color/average_color.xml
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-average-color/cli_list.json
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-average-color/cli_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.516704 girder-slicer-cli-web-1.3.4.dev2/example-girder-requests/
+-rw-r--r--   0 root         (0) root         (0)      289 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-girder-requests/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      507 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-girder-requests/README.rst
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-girder-requests/cli_list.json
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-girder-requests/cli_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.516704 girder-slicer-cli-web-1.3.4.dev2/example-girder-requests/girder_requests/
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-girder-requests/girder_requests/girder_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/example-girder-requests/girder_requests/girder_requests.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.520704 girder-slicer-cli-web-1.3.4.dev2/girder_slicer_cli_web.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16189 2023-05-02 15:20:12.000000 girder-slicer-cli-web-1.3.4.dev2/girder_slicer_cli_web.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6030 2023-05-02 15:20:12.000000 girder-slicer-cli-web-1.3.4.dev2/girder_slicer_cli_web.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 15:20:12.000000 girder-slicer-cli-web-1.3.4.dev2/girder_slicer_cli_web.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-02 15:20:12.000000 girder-slicer-cli-web-1.3.4.dev2/girder_slicer_cli_web.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 15:19:30.000000 girder-slicer-cli-web-1.3.4.dev2/girder_slicer_cli_web.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-02 15:20:12.000000 girder-slicer-cli-web-1.3.4.dev2/girder_slicer_cli_web.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-02 15:20:12.000000 girder-slicer-cli-web-1.3.4.dev2/girder_slicer_cli_web.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-02 15:20:12.556704 girder-slicer-cli-web-1.3.4.dev2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.524704 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3506 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/cli_list_entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/config.py
+-rw-r--r--   0 root         (0) root         (0)     6649 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/ctk_cli_adjustment.py
+-rw-r--r--   0 root         (0) root         (0)    15903 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/docker_resource.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/girder_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.524704 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/girder_worker_plugin/
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/girder_worker_plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/girder_worker_plugin/cli_progress.py
+-rw-r--r--   0 root         (0) root         (0)     3834 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/girder_worker_plugin/direct_docker_run.py
+-rw-r--r--   0 root         (0) root         (0)    12039 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/image_job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.528704 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/models/
+-rw-r--r--   0 root         (0) root         (0)      208 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10452 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/models/docker_image.py
+-rw-r--r--   0 root         (0) root         (0)      810 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/models/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3314 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/models/json_to_xml.py
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/models/parser.py
+-rw-r--r--   0 root         (0) root         (0)    32185 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/models/schema.json
+-rw-r--r--   0 root         (0) root         (0)    14268 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/prepare_task.py
+-rw-r--r--   0 root         (0) root         (0)    25904 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/rest_slicer_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.528704 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/
+-rw-r--r--   0 root         (0) root         (0)      404 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/JobStatus.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.528704 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/collections/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/collections/WidgetCollection.js
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/collections/index.js
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/events.js
+-rw-r--r--   0 root         (0) root         (0)      299 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/index.js
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.528704 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/models/
+-rw-r--r--   0 root         (0) root         (0)     9732 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/models/WidgetModel.js
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/models/index.js
+-rw-r--r--   0 root         (0) root         (0)     3996 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.532704 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/
+-rw-r--r--   0 root         (0) root         (0)      540 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/constraints.js
+-rw-r--r--   0 root         (0) root         (0)      610 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/convert.js
+-rw-r--r--   0 root         (0) root         (0)      671 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/defaultValue.js
+-rw-r--r--   0 root         (0) root         (0)      894 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/group.js
+-rw-r--r--   0 root         (0) root         (0)      384 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/index.js
+-rw-r--r--   0 root         (0) root         (0)      506 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/panel.js
+-rw-r--r--   0 root         (0) root         (0)     2521 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/param.js
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/parse.js
+-rw-r--r--   0 root         (0) root         (0)      921 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/widget.js
+-rw-r--r--   0 root         (0) root         (0)      404 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/routes.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.532704 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/stylesheets/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/stylesheets/configView.styl
+-rw-r--r--   0 root         (0) root         (0)      926 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/stylesheets/controlWidget.styl
+-rw-r--r--   0 root         (0) root         (0)      112 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/stylesheets/controlsPanel.styl
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/stylesheets/outputParameterDialog.styl
+-rw-r--r--   0 root         (0) root         (0)      662 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/stylesheets/panel.styl
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/stylesheets/panelGroup.styl
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/stylesheets/slicerUI.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.536704 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/booleanWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      115 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/colorWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/configView.pug
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/controlsPanel.pug
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/enumerationWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/fileWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      621 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/jobsListWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/outputParameterDialog.pug
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/panel.pug
+-rw-r--r--   0 root         (0) root         (0)      529 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/panelGroup.pug
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/rangeWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/regionWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      308 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/slicerUI.pug
+-rw-r--r--   0 root         (0) root         (0)      735 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/uploadImageDialog.pug
+-rw-r--r--   0 root         (0) root         (0)      569 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/widget.pug
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/utils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.540704 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/
+-rw-r--r--   0 root         (0) root         (0)     4761 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/CollectionView.js
+-rw-r--r--   0 root         (0) root         (0)     7145 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/ConfigView.js
+-rw-r--r--   0 root         (0) root         (0)    17436 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/ControlWidget.js
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/ControlsPanel.js
+-rw-r--r--   0 root         (0) root         (0)    11455 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/ItemSelectorWidget.js
+-rw-r--r--   0 root         (0) root         (0)     4584 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/ItemView.js
+-rw-r--r--   0 root         (0) root         (0)     3798 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/JobsListWidget.js
+-rw-r--r--   0 root         (0) root         (0)      799 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/JobsPanel.js
+-rw-r--r--   0 root         (0) root         (0)      532 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/OutputParameterDialog.js
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/Panel.js
+-rw-r--r--   0 root         (0) root         (0)     8424 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/PanelGroup.js
+-rw-r--r--   0 root         (0) root         (0)      394 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/index.js
+-rw-r--r--   0 root         (0) root         (0)      872 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/utils.js
+-rw-r--r--   0 root         (0) root         (0)     7791 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/worker_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.544704 girder-slicer-cli-web-1.3.4.dev2/small-docker/
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)      719 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.544704 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example1/
+-rw-r--r--   0 root         (0) root         (0)    10493 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example1/Example1.json
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example1/Example1.py
+-rw-r--r--   0 root         (0) root         (0)    10227 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example1/Example1.xml
+-rw-r--r--   0 root         (0) root         (0)     7115 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example1/Example1.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.544704 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example2/
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example2/Example2.json
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example2/Example2.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example2/Example2.xml
+-rw-r--r--   0 root         (0) root         (0)      639 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example2/Example2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.544704 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example3/
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example3/Example3.json
+-rw-r--r--   0 root         (0) root         (0)      621 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example3/Example3.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example3/Example3.xml
+-rw-r--r--   0 root         (0) root         (0)      626 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/Example3/Example3.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.548704 girder-slicer-cli-web-1.3.4.dev2/small-docker/ExampleProgress/
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/ExampleProgress/ExampleProgress.json
+-rw-r--r--   0 root         (0) root         (0)      884 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/ExampleProgress/ExampleProgress.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/ExampleProgress/progress_helper.py
+-rw-r--r--   0 root         (0) root         (0)      523 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/cli_list.json
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/small-docker/cli_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.548704 girder-slicer-cli-web-1.3.4.dev2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10287 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.552704 girder-slicer-cli-web-1.3.4.dev2/tests/data/
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/data/ExampleSpec.xml
+-rw-r--r--   0 root         (0) root         (0)      301 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/data/girder_worker.cfg
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/data/parser_params_advanced.json
+-rw-r--r--   0 root         (0) root         (0)     1183 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/data/parser_params_advanced.xml
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/data/parser_params_advanced.yaml
+-rw-r--r--   0 root         (0) root         (0)      232 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/data/parser_params_simple.json
+-rw-r--r--   0 root         (0) root         (0)      218 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/data/parser_params_simple.xml
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/data/parser_params_simple.yaml
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/data/parser_simple.json
+-rw-r--r--   0 root         (0) root         (0)      319 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/data/parser_simple.xml
+-rw-r--r--   0 root         (0) root         (0)      152 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/data/parser_simple.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.552704 girder-slicer-cli-web-1.3.4.dev2/tests/girder_worker_plugin/
+-rw-r--r--   0 root         (0) root         (0)     2761 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/girder_worker_plugin/test_cli_progress.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/girder_worker_plugin/test_direct_docker_run.py
+-rw-r--r--   0 root         (0) root         (0)     4961 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/test_batch.py
+-rw-r--r--   0 root         (0) root         (0)      762 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     6041 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/test_docker.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/test_load.py
+-rw-r--r--   0 root         (0) root         (0)     5923 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/test_parser.py
+-rw-r--r--   0 root         (0) root         (0)    10504 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/test_rest_slicer_cli.py
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/test_web_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.556704 girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/.eslintrc
+-rw-r--r--   0 root         (0) root         (0)     2410 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/configViewSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4543 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/containerViewSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6091 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/dockerTaskSpec.js
+-rw-r--r--   0 root         (0) root         (0)     9822 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/itemSelectorWidgetSpec.js
+-rw-r--r--   0 root         (0) root         (0)     2503 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/panelGroupSpec.js
+-rw-r--r--   0 root         (0) root         (0)    27393 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/parseSpec.js
+-rw-r--r--   0 root         (0) root         (0)    43069 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/widgetSpec.js
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:20:12.556704 girder-slicer-cli-web-1.3.4.dev2/utils/
+-rw-r--r--   0 root         (0) root         (0)     3879 2023-05-02 15:19:17.000000 girder-slicer-cli-web-1.3.4.dev2/utils/xmltojson.py
```

### Comparing `girder-slicer-cli-web-1.3.3.dev6/.circleci/config.yml` & `girder-slicer-cli-web-1.3.4.dev2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/.dockerignore` & `girder-slicer-cli-web-1.3.4.dev2/.dockerignore`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/.gitignore` & `girder-slicer-cli-web-1.3.4.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/LICENSE` & `girder-slicer-cli-web-1.3.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/PKG-INFO` & `girder-slicer-cli-web-1.3.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-slicer-cli-web
-Version: 1.3.3.dev6
+Version: 1.3.4.dev2
 Summary: A girder plugin for exposing slicer CLIs over the web
 Home-page: https://github.com/girder/slicer_cli_web
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,slicer_cli_web
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `girder-slicer-cli-web-1.3.3.dev6/README.rst` & `girder-slicer-cli-web-1.3.4.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/docs/worker_management.rst` & `girder-slicer-cli-web-1.3.4.dev2/docs/worker_management.rst`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/example-average-color/.dockerignore` & `girder-slicer-cli-web-1.3.4.dev2/example-average-color/.dockerignore`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/example-average-color/README.rst` & `girder-slicer-cli-web-1.3.4.dev2/example-average-color/README.rst`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/example-average-color/average_color/average_color.py` & `girder-slicer-cli-web-1.3.4.dev2/example-average-color/average_color/average_color.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/example-average-color/average_color/average_color.xml` & `girder-slicer-cli-web-1.3.4.dev2/example-average-color/average_color/average_color.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/example-average-color/cli_list.py` & `girder-slicer-cli-web-1.3.4.dev2/example-average-color/cli_list.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/example-girder-requests/cli_list.py` & `girder-slicer-cli-web-1.3.4.dev2/example-girder-requests/cli_list.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/example-girder-requests/girder_requests/girder_requests.xml` & `girder-slicer-cli-web-1.3.4.dev2/example-girder-requests/girder_requests/girder_requests.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/girder_slicer_cli_web.egg-info/PKG-INFO` & `girder-slicer-cli-web-1.3.4.dev2/girder_slicer_cli_web.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-slicer-cli-web
-Version: 1.3.3.dev6
+Version: 1.3.4.dev2
 Summary: A girder plugin for exposing slicer CLIs over the web
 Home-page: https://github.com/girder/slicer_cli_web
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,slicer_cli_web
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `girder-slicer-cli-web-1.3.3.dev6/girder_slicer_cli_web.egg-info/SOURCES.txt` & `girder-slicer-cli-web-1.3.4.dev2/girder_slicer_cli_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/setup.py` & `girder-slicer-cli-web-1.3.4.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/__init__.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/cli_list_entrypoint.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/cli_list_entrypoint.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/cli_utils.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/cli_utils.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/config.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/config.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/ctk_cli_adjustment.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/ctk_cli_adjustment.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/docker_resource.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/docker_resource.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/girder_plugin.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/girder_plugin.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/girder_worker_plugin/__init__.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/girder_worker_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/girder_worker_plugin/cli_progress.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/girder_worker_plugin/cli_progress.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/girder_worker_plugin/direct_docker_run.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/girder_worker_plugin/direct_docker_run.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/image_job.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/image_job.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/models/docker_image.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/models/docker_image.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/models/exceptions.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/models/json_to_xml.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/models/json_to_xml.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/models/parser.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/models/parser.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/models/schema.json` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/models/schema.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/prepare_task.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/prepare_task.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/rest_slicer_cli.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/rest_slicer_cli.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/collections/WidgetCollection.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/collections/WidgetCollection.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/models/WidgetModel.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/models/WidgetModel.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/package.json` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/constraints.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/constraints.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/convert.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/convert.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/defaultValue.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/defaultValue.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/group.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/group.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/param.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/param.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/parse.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/parse.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/parser/widget.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/parser/widget.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/stylesheets/controlWidget.styl` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/stylesheets/controlWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/stylesheets/panel.styl` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/stylesheets/panel.styl`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/configView.pug` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/fileWidget.pug` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/fileWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/jobsListWidget.pug` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/jobsListWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/panelGroup.pug` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/panelGroup.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/regionWidget.pug` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/regionWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/uploadImageDialog.pug` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/uploadImageDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/templates/widget.pug` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/templates/widget.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/utils.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/utils.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/CollectionView.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/CollectionView.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/ConfigView.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/ControlWidget.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/ControlWidget.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/ControlsPanel.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/ControlsPanel.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/ItemSelectorWidget.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/ItemSelectorWidget.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/ItemView.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/JobsListWidget.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/JobsListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/JobsPanel.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/JobsPanel.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/OutputParameterDialog.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/OutputParameterDialog.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/Panel.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/Panel.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/PanelGroup.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/PanelGroup.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -91,15 +91,15 @@
         }
 
         const params = this.parameters();
         _.each(params, function(value, key) {
             if (Array.isArray(value)) {
                 params[key] = JSON.stringify(value);
             }
-            const ctlmatch = value.match(/^{#control:(.*)#}$/);
+            const ctlmatch = value ? ('' + value).match(/^{#control:(.*)#}$/) : undefined;
             if (ctlmatch) {
                 params[key] = $(ctlmatch[1]).val() || $(ctlmatch[1]).text() || $(ctlmatch[1]).prop('checked');
             }
         });
 
         // post the job to the server
         restRequest({
```

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/web_client/views/utils.js` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/web_client/views/utils.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/slicer_cli_web/worker_tools.py` & `girder-slicer-cli-web-1.3.4.dev2/slicer_cli_web/worker_tools.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/.dockerignore` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/.dockerignore`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Dockerfile` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Example1/Example1.json` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Example1/Example1.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Example1/Example1.py` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Example1/Example1.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Example1/Example1.xml` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Example1/Example1.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Example1/Example1.yaml` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Example1/Example1.yaml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Example2/Example2.json` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Example2/Example2.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Example2/Example2.py` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Example2/Example2.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Example2/Example2.xml` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Example2/Example2.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Example2/Example2.yaml` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Example2/Example2.yaml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Example3/Example3.json` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Example3/Example3.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Example3/Example3.py` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Example3/Example3.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Example3/Example3.xml` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Example3/Example3.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/Example3/Example3.yaml` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/Example3/Example3.yaml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/ExampleProgress/ExampleProgress.json` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/ExampleProgress/ExampleProgress.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/ExampleProgress/ExampleProgress.py` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/ExampleProgress/ExampleProgress.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/ExampleProgress/progress_helper.py` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/ExampleProgress/progress_helper.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/cli_list.json` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/cli_list.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/small-docker/cli_list.py` & `girder-slicer-cli-web-1.3.4.dev2/small-docker/cli_list.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/conftest.py` & `girder-slicer-cli-web-1.3.4.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/data/ExampleSpec.xml` & `girder-slicer-cli-web-1.3.4.dev2/tests/data/ExampleSpec.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/data/parser_params_advanced.json` & `girder-slicer-cli-web-1.3.4.dev2/tests/data/parser_params_advanced.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/data/parser_params_advanced.xml` & `girder-slicer-cli-web-1.3.4.dev2/tests/data/parser_params_advanced.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/data/parser_params_advanced.yaml` & `girder-slicer-cli-web-1.3.4.dev2/tests/data/parser_params_advanced.yaml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/girder_worker_plugin/test_cli_progress.py` & `girder-slicer-cli-web-1.3.4.dev2/tests/girder_worker_plugin/test_cli_progress.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/girder_worker_plugin/test_direct_docker_run.py` & `girder-slicer-cli-web-1.3.4.dev2/tests/girder_worker_plugin/test_direct_docker_run.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/test_batch.py` & `girder-slicer-cli-web-1.3.4.dev2/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/test_config.py` & `girder-slicer-cli-web-1.3.4.dev2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/test_docker.py` & `girder-slicer-cli-web-1.3.4.dev2/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/test_load.py` & `girder-slicer-cli-web-1.3.4.dev2/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/test_parser.py` & `girder-slicer-cli-web-1.3.4.dev2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/test_rest_slicer_cli.py` & `girder-slicer-cli-web-1.3.4.dev2/tests/test_rest_slicer_cli.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/test_web_client.py` & `girder-slicer-cli-web-1.3.4.dev2/tests/test_web_client.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/configViewSpec.js` & `girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/configViewSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/containerViewSpec.js` & `girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/containerViewSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/dockerTaskSpec.js` & `girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/dockerTaskSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/itemSelectorWidgetSpec.js` & `girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/itemSelectorWidgetSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/panelGroupSpec.js` & `girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/panelGroupSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/parseSpec.js` & `girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/parseSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tests/web_client_specs/widgetSpec.js` & `girder-slicer-cli-web-1.3.4.dev2/tests/web_client_specs/widgetSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/tox.ini` & `girder-slicer-cli-web-1.3.4.dev2/tox.ini`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.3.3.dev6/utils/xmltojson.py` & `girder-slicer-cli-web-1.3.4.dev2/utils/xmltojson.py`

 * *Files identical despite different names*

