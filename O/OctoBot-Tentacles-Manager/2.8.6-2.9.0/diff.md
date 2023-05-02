# Comparing `tmp/OctoBot-Tentacles-Manager-2.8.6.tar.gz` & `tmp/OctoBot-Tentacles-Manager-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Tentacles-Manager-2.8.6.tar", last modified: Sat Apr 15 08:55:12 2023, max compression
+gzip compressed data, was "OctoBot-Tentacles-Manager-2.9.0.tar", last modified: Tue May  2 20:03:10 2023, max compression
```

## Comparing `OctoBot-Tentacles-Manager-2.8.6.tar` & `OctoBot-Tentacles-Manager-2.9.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/util/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/util/tentacles_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/tentacle_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/compiled_package_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Mode_config.template
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Mode_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Social_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Strategies_config.template
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Strategies_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/TA_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Util_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/description_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/tentacle_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/artifact_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/tentacle_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/tentacle_package_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/loaders/tentacle_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/profiles_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/python_modules_requirements_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/tentacle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/tentacles_init_files_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/tentacles_setup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/artifact_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/metadata_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/profile_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/tentacle_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_requirements_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/nexus_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/s3_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_fetching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/install_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/repair_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/single_install_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/tentacles_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/uninstall_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/update_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.990466 OctoBot-Tentacles-Manager-2.8.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/test_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/test_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/test_tentacle_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/test_uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/configuration/test_tentacle_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/configuration/test_tentacles_setup_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/exporters/test_tentacle_bundle_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/loaders/test_tentacle_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/managers/test_tentacles_setup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/util/test_tentacle_fetching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/workers/test_install_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/workers/test_uninstall_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/workers/test_update_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/upload_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/upload_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/upload_tests/_test_nexus_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/upload_tests/test_s3_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/util/tentacles_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/tentacle_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/compiled_package_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Mode_config.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Mode_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Social_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Strategies_config.template
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Strategies_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/TA_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Util_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/description_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/tentacle_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/artifact_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/tentacle_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/tentacle_package_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/loaders/tentacle_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/profiles_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/python_modules_requirements_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/tentacle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/tentacles_init_files_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/tentacles_setup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/artifact_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/metadata_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/profile_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/tentacle_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_requirements_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/nexus_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/s3_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/repair_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/single_install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/tentacles_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/uninstall_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/update_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.537178 OctoBot-Tentacles-Manager-2.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/test_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/test_tentacle_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/test_uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/configuration/test_tentacle_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/configuration/test_tentacles_setup_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/exporters/test_tentacle_bundle_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/loaders/test_tentacle_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/managers/test_tentacles_setup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/util/test_tentacle_fetching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/workers/test_install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/workers/test_uninstall_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/workers/test_update_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/upload_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/upload_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/upload_tests/_test_nexus_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/upload_tests/test_s3_uploader.py
```

### Comparing `OctoBot-Tentacles-Manager-2.8.6/CHANGELOG.md` & `OctoBot-Tentacles-Manager-2.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.9.0] - 2023-05-02
+### Updated
+- Supported python versions
+
 ## [2.8.6] - 2022-04-15
 ### Added
 - [API] add deactivate_all 
 
 ## [2.8.5] - 2022-03-27
 ### Added
 - [API] add get_tentacles_classes_names_for_type
```

### Comparing `OctoBot-Tentacles-Manager-2.8.6/LICENSE` & `OctoBot-Tentacles-Manager-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/PKG-INFO` & `OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: OctoBot-Tentacles-Manager
-Version: 2.8.6
+Version: 2.9.0
 Summary: OctoBot project module installer
 Home-page: https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager
 Author: Drakkar-Software
-Author-email: drakkar-software@protonmail.com
+Author-email: contact@drakkar.software
 License: LGPL-3.0
-Description: # OctoBot-Tentacles-Manager [2.8.6](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
-        [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
-        [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
-        [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
-        
-        A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
-        
-        - Install OctoBot-Tentacles-Manager from pip : 
-        
-        ``` {.sourceCode .bash}
-        $ python3 -m pip install OctoBot-Tentacles-Manager
-        ```
-        
-        ## Usage
-        - Install [OctoBot](https://github.com/Drakkar-Software/OctoBot)
-        
-        - Use the integrated CLI interface: 
-        
-        ``` {.sourceCode .bash}
-        $ python3 octobot_tentacles_manager/cli.py --help
-        ```
-        
-        OR 
-        
-        - Use CLI interface directly with OctoBot: 
-        
-        Python:
-        ``` {.sourceCode .bash}
-        $ python3 tentacles install all
-        ```
-        Binary:
-        ``` {.sourceCode .bash}
-        $ ./OctoBot tentacles install all
-        ```
-        
-        - Use your [OctoBot web interface at **'Tentacles'**.](https://developer.octobot.info/guides/customize-your-octobot)
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
+License-File: LICENSE
+
+# OctoBot-Tentacles-Manager [2.9.0](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+[![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
+[![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
+[![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
+
+A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
+
+- Install OctoBot-Tentacles-Manager from pip : 
+
+``` {.sourceCode .bash}
+$ python3 -m pip install OctoBot-Tentacles-Manager
+```
+
+## Usage
+- Install [OctoBot](https://github.com/Drakkar-Software/OctoBot)
+
+- Use the integrated CLI interface: 
+
+``` {.sourceCode .bash}
+$ python3 octobot_tentacles_manager/cli.py --help
+```
+
+OR 
+
+- Use CLI interface directly with OctoBot: 
+
+Python:
+``` {.sourceCode .bash}
+$ python3 tentacles install all
+```
+Binary:
+``` {.sourceCode .bash}
+$ ./OctoBot tentacles install all
+```
+
+- Use your [OctoBot web interface at **'Tentacles'**.](https://developer.octobot.info/guides/customize-your-octobot)
+
```

### Comparing `OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt` & `OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/PKG-INFO` & `OctoBot-Tentacles-Manager-2.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: OctoBot-Tentacles-Manager
-Version: 2.8.6
+Version: 2.9.0
 Summary: OctoBot project module installer
 Home-page: https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager
 Author: Drakkar-Software
-Author-email: drakkar-software@protonmail.com
+Author-email: contact@drakkar.software
 License: LGPL-3.0
-Description: # OctoBot-Tentacles-Manager [2.8.6](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
-        [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
-        [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
-        [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
-        
-        A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
-        
-        - Install OctoBot-Tentacles-Manager from pip : 
-        
-        ``` {.sourceCode .bash}
-        $ python3 -m pip install OctoBot-Tentacles-Manager
-        ```
-        
-        ## Usage
-        - Install [OctoBot](https://github.com/Drakkar-Software/OctoBot)
-        
-        - Use the integrated CLI interface: 
-        
-        ``` {.sourceCode .bash}
-        $ python3 octobot_tentacles_manager/cli.py --help
-        ```
-        
-        OR 
-        
-        - Use CLI interface directly with OctoBot: 
-        
-        Python:
-        ``` {.sourceCode .bash}
-        $ python3 tentacles install all
-        ```
-        Binary:
-        ``` {.sourceCode .bash}
-        $ ./OctoBot tentacles install all
-        ```
-        
-        - Use your [OctoBot web interface at **'Tentacles'**.](https://developer.octobot.info/guides/customize-your-octobot)
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
+License-File: LICENSE
+
+# OctoBot-Tentacles-Manager [2.9.0](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+[![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
+[![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
+[![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
+
+A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
+
+- Install OctoBot-Tentacles-Manager from pip : 
+
+``` {.sourceCode .bash}
+$ python3 -m pip install OctoBot-Tentacles-Manager
+```
+
+## Usage
+- Install [OctoBot](https://github.com/Drakkar-Software/OctoBot)
+
+- Use the integrated CLI interface: 
+
+``` {.sourceCode .bash}
+$ python3 octobot_tentacles_manager/cli.py --help
+```
+
+OR 
+
+- Use CLI interface directly with OctoBot: 
+
+Python:
+``` {.sourceCode .bash}
+$ python3 tentacles install all
+```
+Binary:
+``` {.sourceCode .bash}
+$ ./OctoBot tentacles install all
+```
+
+- Use your [OctoBot web interface at **'Tentacles'**.](https://developer.octobot.info/guides/customize-your-octobot)
+
```

### Comparing `OctoBot-Tentacles-Manager-2.8.6/README.md` & `OctoBot-Tentacles-Manager-2.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Tentacles-Manager [2.8.6](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+# OctoBot-Tentacles-Manager [2.9.0](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
 [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
 
 A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
 
 - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-VERSION = "2.8.6"
+VERSION = "2.9.0"
 PROJECT_NAME = "OctoBot-Tentacles-Manager"
```

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/configurator.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/configurator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/creator.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/inspector.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/inspector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/installer.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/installer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/loader.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/loader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/uninstaller.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/uninstaller.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/updater.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/uploader.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/util/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/util/tentacles_management.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/util/tentacles_management.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/cli.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/cli.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/config_file.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/config_file.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/tentacle_configuration.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/tentacle_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/constants.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/compiled_package_manager.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/compiled_package_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Mode_tentacle.template` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Mode_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Social_tentacle.template` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Social_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/tentacle_creator.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/tentacle_creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/enums.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/artifact_exporter.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/artifact_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,17 +166,19 @@
             util.merge_folders(folder_to_copy, self.working_folder, ignore)
 
     def zip_temporary_folder(self) -> str:
         """
         Archive creator temporary dir to a zip file
         :return: the path of the archive
         """
-        zipped_file = shutil.make_archive(os.path.join(self.artifact.output_dir, self.get_zip_file_name()),
-                                          constants.TENTACLES_PACKAGE_FORMAT,
-                                          constants.TENTACLES_PACKAGE_CREATOR_TEMP_FOLDER)
+        zipped_file = shutil.make_archive(
+            os.path.abspath(os.path.join(self.artifact.output_dir, self.get_zip_file_name())),
+            constants.TENTACLES_PACKAGE_FORMAT,
+            constants.TENTACLES_PACKAGE_CREATOR_TEMP_FOLDER
+        )
         try:
             # remove working folder
             shutil.rmtree(constants.TENTACLES_PACKAGE_CREATOR_TEMP_FOLDER)
         except Exception as e:
             self.logger.error(f"Error when cleaning up temporary folder: {e}")
         return zipped_file
```

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/tentacle_exporter.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/tentacle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/tentacle_package_exporter.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/tentacle_package_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/loaders/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/loaders/tentacle_loading.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/loaders/tentacle_loading.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/profiles_manager.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/profiles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/python_modules_requirements_manager.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/python_modules_requirements_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/tentacle_manager.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/tentacle_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/tentacles_init_files_manager.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/tentacles_init_files_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/tentacles_setup_manager.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/tentacles_setup_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/artifact.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/artifact.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/artifact_metadata.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/artifact_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/metadata_factory.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/metadata_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/profile_metadata.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/profile_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/tentacle_metadata.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/tentacle_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/profile.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/profile.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_factory.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_package.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_package.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_requirements_tree.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_requirements_tree.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_type.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_type.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/nexus_uploader.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/nexus_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/s3_uploader.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/uploader.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/file_util.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/file_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/hashing.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/hashing.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/os_util.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/os_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_cleaner.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_cleaner.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_explorer.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_explorer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_fetching.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_fetching.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_filter.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_filter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/install_worker.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/repair_worker.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/repair_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/single_install_worker.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/single_install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/tentacles_worker.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/tentacles_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/uninstall_worker.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/uninstall_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/update_worker.py` & `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/update_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/setup.py` & `OctoBot-Tentacles-Manager-2.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,39 +17,36 @@
 from setuptools import find_packages
 from setuptools import setup
 
 from octobot_tentacles_manager import PROJECT_NAME, VERSION
 
 PACKAGES = find_packages(exclude=["tests"])
 
-packages_list = []
-
 # long description from README file
 with open('README.md', encoding='utf-8') as f:
     DESCRIPTION = f.read()
 
 REQUIRED = open('requirements.txt').readlines()
 REQUIRES_PYTHON = '>=3.8'
 
 setup(
     name=PROJECT_NAME,
     version=VERSION,
     url='https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager',
     license='LGPL-3.0',
     author='Drakkar-Software',
-    author_email='drakkar-software@protonmail.com',
+    author_email='contact@drakkar.software',
     description='OctoBot project module installer',
     packages=PACKAGES,
     include_package_data=True,
     long_description=DESCRIPTION,
     tests_require=["pytest"],
     test_suite="tests",
     zip_safe=False,
     data_files=[],
-    setup_requires=REQUIRED,
     install_requires=REQUIRED,
     python_requires=REQUIRES_PYTHON,
     entry_points={
         'console_scripts': [
             PROJECT_NAME + ' = octobot_tentacles_manager.cli:main'
         ]
     },
```

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/api/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/api/test_configurator.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/api/test_configurator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/api/test_creator.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/api/test_creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/api/test_installer.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/api/test_installer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/api/test_uninstaller.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/api/test_uninstaller.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/api/test_updater.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/api/test_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/configuration/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/configuration/test_tentacle_configuration.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/configuration/test_tentacle_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/configuration/test_tentacles_setup_configuration.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/configuration/test_tentacles_setup_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/exporters/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/exporters/test_tentacle_bundle_exporter.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/exporters/test_tentacle_bundle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/loaders/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/loaders/test_tentacle_loading.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/loaders/test_tentacle_loading.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/managers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/managers/test_tentacles_setup_manager.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/managers/test_tentacles_setup_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/util/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/util/test_tentacle_fetching.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/util/test_tentacle_fetching.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/workers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/workers/test_install_worker.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/workers/test_install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/workers/test_uninstall_worker.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/workers/test_uninstall_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/tests/workers/test_update_worker.py` & `OctoBot-Tentacles-Manager-2.9.0/tests/workers/test_update_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/upload_tests/__init__.py` & `OctoBot-Tentacles-Manager-2.9.0/upload_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.6/upload_tests/_test_nexus_uploader.py` & `OctoBot-Tentacles-Manager-2.9.0/upload_tests/_test_nexus_uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     nexus_test_file_name: str = f"{time.time_ns()}"
     local_file_name: str = os.path.join(test_dir_path, f"{TEST_NEXUS_FILE_NAME}.json")
     local_zip_path: str = os.path.join(test_dir_path, f"{TEST_NEXUS_FILE_NAME}")
 
     # test upload file
     with open(local_file_name, "w") as test_file:
         test_file.write(json.dumps({'test-key': 1}))
-    shutil.make_archive(local_zip_path, constants.TENTACLES_PACKAGE_FORMAT, test_dir_path)
+    shutil.make_archive(os.path.abspath(local_zip_path), constants.TENTACLES_PACKAGE_FORMAT, test_dir_path)
     assert await uploader_api.upload_file_or_folder_to_nexus(nexus_path=TEST_NEXUS_PATH,
                                                              artifact_path=test_dir_path,
                                                              artifact_alias=nexus_test_file_name) == 0
     # test download folder files
     downloaded_file_path: str = await download_file_from_nexus(aiohttp_session,
                                                                f"{TEST_NEXUS_PATH}{nexus_test_file_name}/test.json",
                                                                "downloaded_test.json")
```

### Comparing `OctoBot-Tentacles-Manager-2.8.6/upload_tests/test_s3_uploader.py` & `OctoBot-Tentacles-Manager-2.9.0/upload_tests/test_s3_uploader.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     s3_test_file_name: str = f"{time.time_ns()}/sub_{time.time_ns()}"
     local_file_name: str = os.path.join(test_dir_path, f"{TEST_S3_FILE_NAME}.json")
     local_zip_path: str = os.path.join(test_dir_path, f"{TEST_S3_FILE_NAME}")
 
     # test upload file
     with open(local_file_name, "w") as test_file:
         test_file.write(json.dumps({'test-key': 1}))
-    shutil.make_archive(local_zip_path, constants.TENTACLES_PACKAGE_FORMAT, test_dir_path)
+    shutil.make_archive(os.path.abspath(local_zip_path), constants.TENTACLES_PACKAGE_FORMAT, test_dir_path)
     assert await uploader_api.upload_file_or_folder_to_s3(s3_path=TEST_S3_PATH,
                                                           artifact_path=test_dir_path,
                                                           artifact_alias=s3_test_file_name) == 0
     # test download folder files
     downloaded_file_path: str = await download_file_from_s3(f"{TEST_S3_PREFIX}{TEST_S3_PATH}{s3_test_file_name}/test.json",
                                                             "downloaded_test.json")
     downloaded_zip_path: str = await download_file_from_s3(f"{TEST_S3_PREFIX}{TEST_S3_PATH}{s3_test_file_name}/test.zip",
```

