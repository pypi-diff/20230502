# Comparing `tmp/fl_studio_api_stubs-28.1.0.tar.gz` & `tmp/fl_studio_api_stubs-28.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fl_studio_api_stubs-28.1.0.tar", max compression
+gzip compressed data, was "fl_studio_api_stubs-28.2.0.tar", max compression
```

## Comparing `fl_studio_api_stubs-28.1.0.tar` & `fl_studio_api_stubs-28.2.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0     7642 2023-03-30 15:13:04.516427 fl_studio_api_stubs-28.1.0/LICENSE.md
--rwxr-xr-x   0        0        0     2817 2023-03-30 15:13:04.516427 fl_studio_api_stubs-28.1.0/README.md
--rw-r--r--   0        0        0     2281 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/pyproject.toml
--rw-r--r--   0        0        0     2921 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/arrangement/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/arrangement/py.typed
--rw-r--r--   0        0        0     2391 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/channels/__init__.py
--rw-r--r--   0        0        0     1401 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/channels/__notes.py
--rw-r--r--   0        0        0    18932 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/channels/__properties.py
--rw-r--r--   0        0        0     5115 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/channels/__sequencer.py
--rw-r--r--   0        0        0     3167 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/channels/__ui.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/channels/py.typed
--rw-r--r--   0        0        0     6348 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/device/__device.py
--rw-r--r--   0        0        0     2984 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/device/__dispatch.py
--rw-r--r--   0        0        0     5049 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/device/__fl.py
--rw-r--r--   0        0        0     1510 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/device/__init__.py
--rw-r--r--   0        0        0     1804 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/device/__util.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/device/py.typed
--rw-r--r--   0        0        0      597 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/enveditor/__init__.py
--rw-r--r--   0        0        0     7538 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/enveditor/__sample.py
--rw-r--r--   0        0        0     3336 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/enveditor/__script_dialog.py
--rw-r--r--   0        0        0     1172 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/enveditor/__utils.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/enveditor/py.typed
--rw-r--r--   0        0        0       42 2023-03-30 15:13:05.004421 fl_studio_api_stubs-28.1.0/src/fl_classes/.git
--rw-r--r--   0        0        0     1366 2023-03-30 15:13:05.012421 fl_studio_api_stubs-28.1.0/src/fl_classes/.gitignore
--rw-r--r--   0        0        0     7642 2023-03-30 15:13:05.012421 fl_studio_api_stubs-28.1.0/src/fl_classes/LICENSE.md
--rw-r--r--   0        0        0      283 2023-03-30 15:13:05.012421 fl_studio_api_stubs-28.1.0/src/fl_classes/README.md
--rw-r--r--   0        0        0    20163 2023-03-30 15:13:05.012421 fl_studio_api_stubs-28.1.0/src/fl_classes/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:05.012421 fl_studio_api_stubs-28.1.0/src/fl_classes/py.typed
--rw-r--r--   0        0        0      611 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/__init__.py
--rw-r--r--   0        0        0     8350 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/channels.py
--rw-r--r--   0        0        0      444 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/configuration/__init__.py
--rw-r--r--   0        0        0      561 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/configuration/config_typings.py
--rw-r--r--   0        0        0      170 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/configuration/default.json
--rw-r--r--   0        0        0     1383 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/configuration/load_data.py
--rw-r--r--   0        0        0     1453 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/configuration/schema.json
--rw-r--r--   0        0        0      698 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/configuration/target_version.py
--rw-r--r--   0        0        0     5535 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/consts.py
--rw-r--r--   0        0        0     2930 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/decorators.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/device.py
--rw-r--r--   0        0        0     6524 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/emulation.py
--rw-r--r--   0        0        0     2683 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/exceptions.py
--rw-r--r--   0        0        0       40 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/helpers/__init__.py
--rw-r--r--   0        0        0     1114 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/helpers/file_from_here.py
--rw-r--r--   0        0        0     1331 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/models/__init__.py
--rw-r--r--   0        0        0     1746 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/models/channels.py
--rw-r--r--   0        0        0      604 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/models/device.py
--rw-r--r--   0        0        0     2406 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/models/general.py
--rw-r--r--   0        0        0     1633 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/models/mixer.py
--rw-r--r--   0        0        0     2688 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/models/pattern.py
--rw-r--r--   0        0        0      532 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/models/plugin.py
--rw-r--r--   0        0        0      618 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/models/transport.py
--rw-r--r--   0        0        0     1178 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/models/ui.py
--rw-r--r--   0        0        0     1407 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/patterns.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/py.typed
--rw-r--r--   0        0        0     1928 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/state.py
--rw-r--r--   0        0        0      337 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/fl_model/util.py
--rw-r--r--   0        0        0     3947 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/general/__fl_state.py
--rw-r--r--   0        0        0     1058 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/general/__init__.py
--rw-r--r--   0        0        0     6860 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/general/__undo.py
--rw-r--r--   0        0        0     2730 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/general/__undo_proposed.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/general/py.typed
--rw-r--r--   0        0        0     3503 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/launchMapPages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/launchMapPages/py.typed
--rw-r--r--   0        0        0      462 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/midi/__encode.py
--rw-r--r--   0        0        0    17402 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/midi/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/midi/py.typed
--rw-r--r--   0        0        0     3996 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/mixer/__events.py
--rw-r--r--   0        0        0     2796 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/mixer/__init__.py
--rw-r--r--   0        0        0     3235 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/mixer/__properties.py
--rw-r--r--   0        0        0     2041 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/mixer/__selection.py
--rw-r--r--   0        0        0    12844 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/mixer/__tracks.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/mixer/py.typed
--rw-r--r--   0        0        0     1433 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/patterns/__groups.py
--rw-r--r--   0        0        0      318 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/patterns/__helpers.py
--rw-r--r--   0        0        0     1409 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/patterns/__init__.py
--rw-r--r--   0        0        0     1095 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/patterns/__performance.py
--rw-r--r--   0        0        0     8216 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/patterns/__properties.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/patterns/py.typed
--rw-r--r--   0        0        0    15286 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/playlist/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/playlist/py.typed
--rw-r--r--   0        0        0    11615 2023-03-30 15:13:04.520427 fl_studio_api_stubs-28.1.0/src/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/plugins/py.typed
--rw-r--r--   0        0        0      919 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/transport/__init__.py
--rw-r--r--   0        0        0     3171 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/transport/__position.py
--rw-r--r--   0        0        0     9142 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/transport/__state.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/transport/py.typed
--rw-r--r--   0        0        0     3178 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/ui/__browser.py
--rw-r--r--   0        0        0     1353 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/ui/__editors.py
--rw-r--r--   0        0        0     7516 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/ui/__fl_state.py
--rw-r--r--   0        0        0     3127 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/ui/__init__.py
--rw-r--r--   0        0        0     4836 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/ui/__keyboard.py
--rw-r--r--   0        0        0     3520 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/ui/__navigation.py
--rw-r--r--   0        0        0     2403 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/ui/__overlays.py
--rw-r--r--   0        0        0     5896 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/ui/__windows.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/ui/py.typed
--rw-r--r--   0        0        0    11427 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 15:13:04.524427 fl_studio_api_stubs-28.1.0/src/utils/py.typed
--rw-r--r--   0        0        0     4220 1970-01-01 00:00:00.000000 fl_studio_api_stubs-28.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7642 2023-05-02 13:48:38.511676 fl_studio_api_stubs-28.2.0/LICENSE.md
+-rwxr-xr-x   0        0        0     2817 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/README.md
+-rw-r--r--   0        0        0     2482 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2921 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/arrangement/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/arrangement/py.typed
+-rw-r--r--   0        0        0     2391 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/channels/__init__.py
+-rw-r--r--   0        0        0     1401 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/channels/__notes.py
+-rw-r--r--   0        0        0    18932 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/channels/__properties.py
+-rw-r--r--   0        0        0     5115 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/channels/__sequencer.py
+-rw-r--r--   0        0        0     3167 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/channels/__ui.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/channels/py.typed
+-rw-r--r--   0        0        0     6348 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/device/__device.py
+-rw-r--r--   0        0        0     2984 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/device/__dispatch.py
+-rw-r--r--   0        0        0     5049 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/device/__fl.py
+-rw-r--r--   0        0        0     1510 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/device/__init__.py
+-rw-r--r--   0        0        0     1804 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/device/__util.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/device/py.typed
+-rw-r--r--   0        0        0      597 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/enveditor/__init__.py
+-rw-r--r--   0        0        0     7538 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/enveditor/__sample.py
+-rw-r--r--   0        0        0     3336 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/enveditor/__script_dialog.py
+-rw-r--r--   0        0        0     1172 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/enveditor/__utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/enveditor/py.typed
+-rw-r--r--   0        0        0       42 2023-05-02 13:48:38.891699 fl_studio_api_stubs-28.2.0/src/fl_classes/.git
+-rw-r--r--   0        0        0     1366 2023-05-02 13:48:38.899700 fl_studio_api_stubs-28.2.0/src/fl_classes/.gitignore
+-rw-r--r--   0        0        0     7642 2023-05-02 13:48:38.899700 fl_studio_api_stubs-28.2.0/src/fl_classes/LICENSE.md
+-rw-r--r--   0        0        0      283 2023-05-02 13:48:38.899700 fl_studio_api_stubs-28.2.0/src/fl_classes/README.md
+-rw-r--r--   0        0        0    20163 2023-05-02 13:48:38.899700 fl_studio_api_stubs-28.2.0/src/fl_classes/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.899700 fl_studio_api_stubs-28.2.0/src/fl_classes/py.typed
+-rw-r--r--   0        0        0      611 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/__init__.py
+-rw-r--r--   0        0        0     8350 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/channels.py
+-rw-r--r--   0        0        0      444 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/configuration/__init__.py
+-rw-r--r--   0        0        0      561 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/configuration/config_typings.py
+-rw-r--r--   0        0        0      170 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/configuration/default.json
+-rw-r--r--   0        0        0     1383 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/configuration/load_data.py
+-rw-r--r--   0        0        0     1453 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/configuration/schema.json
+-rw-r--r--   0        0        0      698 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/configuration/target_version.py
+-rw-r--r--   0        0        0     5535 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/consts.py
+-rw-r--r--   0        0        0     2930 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/decorators.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/device.py
+-rw-r--r--   0        0        0     6524 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/emulation.py
+-rw-r--r--   0        0        0     2683 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/exceptions.py
+-rw-r--r--   0        0        0       40 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/helpers/__init__.py
+-rw-r--r--   0        0        0     1114 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/helpers/file_from_here.py
+-rw-r--r--   0        0        0     1331 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/__init__.py
+-rw-r--r--   0        0        0     1746 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/channels.py
+-rw-r--r--   0        0        0      604 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/device.py
+-rw-r--r--   0        0        0     2406 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/general.py
+-rw-r--r--   0        0        0     1633 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/mixer.py
+-rw-r--r--   0        0        0     2688 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/pattern.py
+-rw-r--r--   0        0        0      532 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/plugin.py
+-rw-r--r--   0        0        0      618 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/transport.py
+-rw-r--r--   0        0        0     1178 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/models/ui.py
+-rw-r--r--   0        0        0     1407 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/patterns.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/py.typed
+-rw-r--r--   0        0        0     1928 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/state.py
+-rw-r--r--   0        0        0      337 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/fl_model/util.py
+-rw-r--r--   0        0        0     3947 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/general/__fl_state.py
+-rw-r--r--   0        0        0     1058 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/general/__init__.py
+-rw-r--r--   0        0        0     6860 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/general/__undo.py
+-rw-r--r--   0        0        0     2730 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/general/__undo_proposed.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/general/py.typed
+-rw-r--r--   0        0        0     3503 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/launchMapPages/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/launchMapPages/py.typed
+-rw-r--r--   0        0        0      462 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/midi/__encode.py
+-rw-r--r--   0        0        0    17402 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/midi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/midi/py.typed
+-rw-r--r--   0        0        0     3996 2023-05-02 13:48:38.515677 fl_studio_api_stubs-28.2.0/src/mixer/__events.py
+-rw-r--r--   0        0        0     2796 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/mixer/__init__.py
+-rw-r--r--   0        0        0     3235 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/mixer/__properties.py
+-rw-r--r--   0        0        0     2041 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/mixer/__selection.py
+-rw-r--r--   0        0        0    12844 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/mixer/__tracks.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/mixer/py.typed
+-rw-r--r--   0        0        0     1433 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/patterns/__groups.py
+-rw-r--r--   0        0        0      318 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/patterns/__helpers.py
+-rw-r--r--   0        0        0     1409 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/patterns/__init__.py
+-rw-r--r--   0        0        0     1095 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/patterns/__performance.py
+-rw-r--r--   0        0        0     8216 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/patterns/__properties.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/patterns/py.typed
+-rw-r--r--   0        0        0    15286 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/playlist/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/playlist/py.typed
+-rw-r--r--   0        0        0    14450 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/plugins/py.typed
+-rw-r--r--   0        0        0      919 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/transport/__init__.py
+-rw-r--r--   0        0        0     3171 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/transport/__position.py
+-rw-r--r--   0        0        0     9142 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/transport/__state.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/transport/py.typed
+-rw-r--r--   0        0        0     3178 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__browser.py
+-rw-r--r--   0        0        0     1353 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__editors.py
+-rw-r--r--   0        0        0     7516 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__fl_state.py
+-rw-r--r--   0        0        0     3127 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__init__.py
+-rw-r--r--   0        0        0     4836 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__keyboard.py
+-rw-r--r--   0        0        0     3520 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__navigation.py
+-rw-r--r--   0        0        0     2403 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__overlays.py
+-rw-r--r--   0        0        0     5896 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/__windows.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/ui/py.typed
+-rw-r--r--   0        0        0    11427 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:48:38.519677 fl_studio_api_stubs-28.2.0/src/utils/py.typed
+-rw-r--r--   0        0        0     4421 1970-01-01 00:00:00.000000 fl_studio_api_stubs-28.2.0/PKG-INFO
```

### Comparing `fl_studio_api_stubs-28.1.0/LICENSE.md` & `fl_studio_api_stubs-28.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/README.md` & `fl_studio_api_stubs-28.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/pyproject.toml` & `fl_studio_api_stubs-28.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fl-studio-api-stubs"
-version = "28.1.0"
+version = "28.2.0"
 
 description = "Module and function definitions and documentation for the FL Studio Python API"
 readme = "README.md"
 
 authors = ["Miguel Guthridge <hdsq@outlook.com.au>"]
 license = "LGPL-3.0-only"
 
@@ -25,14 +25,18 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
     "Environment :: Other Environment",
+    "Topic :: Software Development :: Documentation",
+    "Topic :: Software Development :: Libraries :: Application Frameworks",
+    "Typing :: Typed",
+    "Typing :: Stubs Only",
 ]
 include = ["py.typed"]
 
 packages = [
     { include = "arrangement", from = "src" },
     { include = "channels", from = "src" },
     { include = "device", from = "src" },
@@ -69,11 +73,12 @@
 types-jsonschema = "^4.17.0"
 mkdocs = "^1.4.2"
 mkdocs-gen-files = "^0.4.0"
 mkdocs-autorefs = "^0.4.1"
 mkdocs-material = "^8.5.11"
 mkdocs-material-extensions = "^1.1.1"
 mkdocstrings-python = "^0.8.3"
+autopep8 = "^2.0.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fl_studio_api_stubs-28.1.0/src/arrangement/__init__.py` & `fl_studio_api_stubs-28.2.0/src/arrangement/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/channels/__init__.py` & `fl_studio_api_stubs-28.2.0/src/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/channels/__notes.py` & `fl_studio_api_stubs-28.2.0/src/channels/__notes.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/channels/__properties.py` & `fl_studio_api_stubs-28.2.0/src/channels/__properties.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/channels/__sequencer.py` & `fl_studio_api_stubs-28.2.0/src/channels/__sequencer.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/channels/__ui.py` & `fl_studio_api_stubs-28.2.0/src/channels/__ui.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/device/__device.py` & `fl_studio_api_stubs-28.2.0/src/device/__device.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/device/__dispatch.py` & `fl_studio_api_stubs-28.2.0/src/device/__dispatch.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/device/__fl.py` & `fl_studio_api_stubs-28.2.0/src/device/__fl.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/device/__init__.py` & `fl_studio_api_stubs-28.2.0/src/device/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/device/__util.py` & `fl_studio_api_stubs-28.2.0/src/device/__util.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/enveditor/__init__.py` & `fl_studio_api_stubs-28.2.0/src/enveditor/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/enveditor/__sample.py` & `fl_studio_api_stubs-28.2.0/src/enveditor/__sample.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/enveditor/__script_dialog.py` & `fl_studio_api_stubs-28.2.0/src/enveditor/__script_dialog.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/enveditor/__utils.py` & `fl_studio_api_stubs-28.2.0/src/enveditor/__utils.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_classes/.gitignore` & `fl_studio_api_stubs-28.2.0/src/fl_classes/.gitignore`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_classes/LICENSE.md` & `fl_studio_api_stubs-28.2.0/src/fl_classes/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_classes/__init__.py` & `fl_studio_api_stubs-28.2.0/src/fl_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/__init__.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/channels.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/channels.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/configuration/config_typings.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/configuration/config_typings.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/configuration/load_data.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/configuration/load_data.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/configuration/schema.json` & `fl_studio_api_stubs-28.2.0/src/fl_model/configuration/schema.json`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/configuration/target_version.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/configuration/target_version.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/consts.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/consts.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/decorators.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/decorators.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/emulation.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/emulation.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/exceptions.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/exceptions.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/helpers/file_from_here.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/helpers/file_from_here.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/models/__init__.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/models/channels.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/models/channels.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/models/device.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/models/device.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/models/general.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/models/general.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/models/mixer.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/models/mixer.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/models/pattern.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/models/pattern.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/models/plugin.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/models/plugin.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/models/transport.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/models/transport.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/models/ui.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/models/ui.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/patterns.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/patterns.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/fl_model/state.py` & `fl_studio_api_stubs-28.2.0/src/fl_model/state.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/general/__fl_state.py` & `fl_studio_api_stubs-28.2.0/src/general/__fl_state.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/general/__init__.py` & `fl_studio_api_stubs-28.2.0/src/general/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/general/__undo.py` & `fl_studio_api_stubs-28.2.0/src/general/__undo.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/general/__undo_proposed.py` & `fl_studio_api_stubs-28.2.0/src/general/__undo_proposed.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/launchMapPages/__init__.py` & `fl_studio_api_stubs-28.2.0/src/launchMapPages/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/midi/__init__.py` & `fl_studio_api_stubs-28.2.0/src/midi/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/mixer/__events.py` & `fl_studio_api_stubs-28.2.0/src/mixer/__events.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/mixer/__init__.py` & `fl_studio_api_stubs-28.2.0/src/mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/mixer/__properties.py` & `fl_studio_api_stubs-28.2.0/src/mixer/__properties.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/mixer/__selection.py` & `fl_studio_api_stubs-28.2.0/src/mixer/__selection.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/mixer/__tracks.py` & `fl_studio_api_stubs-28.2.0/src/mixer/__tracks.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/patterns/__groups.py` & `fl_studio_api_stubs-28.2.0/src/patterns/__groups.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/patterns/__init__.py` & `fl_studio_api_stubs-28.2.0/src/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/patterns/__performance.py` & `fl_studio_api_stubs-28.2.0/src/patterns/__performance.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/patterns/__properties.py` & `fl_studio_api_stubs-28.2.0/src/patterns/__properties.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/playlist/__init__.py` & `fl_studio_api_stubs-28.2.0/src/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/plugins/__init__.py` & `fl_studio_api_stubs-28.2.0/src/plugins/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 # If you use the unary `*` operator, the tuple is unpacked to take up multiple
 # arguments. Both of these function calls work correctly.
 plugins.isValid(*index1)
 plugins.isValid(*index2)
 ```
 
+Note that this may be unreliable if you are also specifying `useGlobalIndex`
+
 ## Interacting with VST plugins
 
 VST plugins can behave somewhat unintuitively as a result of the system that FL
 Studio uses for parameter mapping. In the VST specification, all VSTs have 4096
 parameters available to use, but aren't required to use all of them. Unused
 parameters are hidden in FL Studio's UI, but they are accessible through the
 API - their returned names will be an empty string. However, there are actually
@@ -45,103 +47,142 @@
 Module added in API version 8.
 """
 from fl_model.decorators import since
 import midi
 
 
 @since(8)
-def isValid(index: int, slotIndex: int = -1) -> bool:
+def isValid(
+    index: int,
+    slotIndex: int = -1,
+    useGlobalIndex: bool = False,
+) -> bool:
     """Returns whether there is a valid plugin at `index`/`slotIndex`.
 
     ## Notes
     * Audio samples are not considered to be plugins in FL Studio.
 
     ## Args:
-     * `index` (`int`): index on channel rack or mixer
+    * `index` (`int`): index on channel rack or mixer
+
+    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
 
-     * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to -1.
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
 
     ## Returns:
      * `bool`: whether there is a valid plugin at `index`.
 
     Included since API version 8
     """
     return False
 
 
 @since(12)
-def getPluginName(index: int, slotIndex: int = -1, userName: int = 0) -> str:
+def getPluginName(
+    index: int,
+    slotIndex: int = -1,
+    userName: bool = False,
+    useGlobalIndex: bool = False,
+) -> str:
     """Returns the name of the plugin at `index`/slotIndex`. This returns the
     original plugin name if `userName` is `False`, otherwise the name of the
     plugin as set by the user.
 
     ## Args:
-     * `index` (`int`): index on channel rack or mixer
+    * `index` (`int`): index on channel rack or mixer
 
-     * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to -1.
+    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
+
+    * `userName` (`bool`, optional): whether to return the user's name for the
+      plugin (`True`), or the default name for the plugin (`False`). Defaults
+      to `False`.
+
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
 
     ## Returns:
      * `str`: plugin name
 
     Included since API version 8, with `userName` parameter added in API version
     12
     """
     return ""
 
 
 @since(8)
-def getParamCount(index: int, slotIndex: int = -1) -> int:
+def getParamCount(
+    index: int,
+    slotIndex: int = -1,
+    useGlobalIndex: bool = False,
+) -> int:
     """Returns the number of parameters that the plugin at `index`/`slotIndex`
     has.
 
     ## NOTE:
     * VST plugins are listed as having `4240` parameters, but not all of
       these are necessarily used by the plugin. The first `4096` are for
       parameters, then the next `128` are used for MIDI CC sends `0` to `127`.
       The final `16` are used for after-touch on each MIDI channel.
 
     ## Args:
     * `index` (`int`): index on channel rack or mixer
 
-    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to -1.
+    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
+
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
 
     ## Returns:
     * `int`: number of parameters
 
     Included since API version 8
     """
     return 0
 
 
 @since(8)
-def getParamName(paramIndex: int, index: int, slotIndex: int = -1) -> str:
+def getParamName(
+    paramIndex: int,
+    index: int,
+    slotIndex: int = -1,
+    useGlobalIndex: bool = False,
+) -> str:
     """Returns the name of the parameter at `paramIndex` for the plugin at
     `index`/`slotIndex`.
 
     ## WARNING:
     * In API versions < v20, FL Studio's Python environment will crash if an
       invalid paramIndex is provided to this function.
 
     ## Args:
     * `paramIndex` (`int`): index of parameter
 
     * `index` (`int`): index of plugin on channel rack or mixer
 
-    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to -1.
+    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
+
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
 
     ## Returns:
     * `str`: name of parameter
 
     Included since API version 8
     """
     return ""
 
 
 @since(8)
-def getParamValue(paramIndex: int, index: int, slotIndex: int = -1) -> float:
+def getParamValue(
+    paramIndex: int,
+    index: int,
+    slotIndex: int = -1,
+    useGlobalIndex: bool = False,
+) -> float:
     """Returns the value of the parameter at `paramIndex` for the plugin at
     `index`/`slotIndex`.
 
     ## Warnings:
     * In API versions < v20, the return values of this function for VST plugins
       seem to be very broken, often being incorrect by orders of magnitude.
 
@@ -149,57 +190,65 @@
       functions that interact with plugins.
 
     ## Args:
     * `paramIndex` (`int`): index of parameter
 
     * `index` (`int`): index of plugin on channel rack or mixer
 
-    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to -1.
+    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
+
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
 
     ## Returns:
     * `float`: parameter value, between `0.0` and `1.0`
 
     Included since API version 8
     """
     return 0.0
 
 
 @since(8)
 def setParamValue(
     value: float,
     paramIndex: int,
     index: int,
-    slotIndex: int = -1
+    slotIndex: int = -1,
+    useGlobalIndex: bool = False,
 ) -> None:
     """Sets the value of the parameter at `paramIndex` for the plugin at
     `index`/`slotIndex`.
 
     ## Warnings:
-    * This appears to have poor performance, being 40x slower than many other
-      functions that interact with plugins.
+    * This appears to have poor performance before FL Studio 21, being 40x
+      slower than many other functions that interact with plugins.
 
     ## Args:
     * `value` (`float`): new value of parameter (between `0.0` and `1.0`)
 
     * `paramIndex` (`int`): index of parameter
 
     * `index` (`int`): index of plugin on channel rack or mixer
 
-    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to -1.
+    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
+
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
 
     Included since API version 8
     """
 
 
 @since(8)
 def getParamValueString(
     paramIndex: int,
     index: int,
     slotIndex: int = -1,
     pickupMode: int = midi.PIM_None,
+    useGlobalIndex: bool = False,
 ) -> str:
     """
     Returns a string value of the parameter at `paramIndex` for the plugin at
     `index`/`slotIndex`. This function is only supported by some FL Studio
     plugins.
 
     TODO: Find plugins
@@ -209,71 +258,79 @@
       invalid paramIndex is provided to this function.
 
     ## Args:
     * `paramIndex` (`int`): index of parameter
 
     * `index` (`int`): index of plugin on channel rack or mixer
 
-    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to -1.
+    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
+
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
 
     ## Returns:
      * `str`: string parameter value
 
     Included since API version 8
     """
     return ""
 
 
 @since(12)
 def getColor(
     index: int,
     slotIndex: int = -1,
-    flag: int = midi.GC_BackgroundColor
+    flag: int = midi.GC_BackgroundColor,
+    useGlobalIndex: bool = False,
 ) -> int:
     """Returns various plugin color parameter values for the plugin at
     `index`/`slotIndex`.
 
     ## Args:
     * `index` (`int`): index of plugin on channel rack or mixer
 
-    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to -1.
+    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
 
     * `flag` (`int`, optional): color type to return:
-         * `GC_BackgroundColor` (`0`, default): The darkest background color
-         of the plugin.
+          * `GC_BackgroundColor` (`0`, default): The darkest background color
+          of the plugin.
+
+          * `GC_Semitone` (`1`): Retrieves semitone color (in FPC, returns
+            color of drum pads).
 
-         * `GC_Semitone` (`1`): Retrieves semitone color (in FPC, returns
-           color of drum pads).
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
 
     ## Returns:
     * `int`: color (`0x--BBGGRR`)
 
     Included since API version 12
     """
     return 0
 
 
 @since(13)
 def getName(
     index: int,
     slotIndex: int = -1,
     flag: int = midi.FPN_Param,
-    paramIndex: int = 0
+    paramIndex: int = 0,
+    useGlobalIndex: bool = False,
 ) -> str:
     """Returns various names for parts of plugins for the plugin at
     `index`/`slotIndex`.
 
     ## HELP WANTED:
     * Explanation of `flag` values from `3` onwards, excluding `6`.
     * Fixing the markdown formatting here: I can't get it to behave in VS Code.
 
     ## Args:
     * `index` (`int`): index of plugin on channel rack or mixer
 
-    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to -1.
+    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
 
     * `flag` (`int`, optional): name type to return. Names marked with a *
       require the `paramIndex` parameter in order to work correctly.
           * `FPN_Param` (`0`, default) * : Name of plugin parameter.
               * Eg: `"Expression"`
 
           * `FPN_ParamValue` (`1`) * : Text value of plugin parameter.
@@ -302,95 +359,124 @@
 
           * `FPN_VoiceColor` (`9`): For plugins that output voices, the name of output voice
               * `paramIndex` as voice number?
 
     * `paramIndex` (`int`, optional): index required by requested flag (if
       necessary)
 
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
+
     ## Returns:
      * `str`: name of requested parameter
 
     Included since API version 13
     """
     return ""
 
 
 @since(19)
 def getPadInfo(
     chanIndex: int,
     slotIndex: int = -1,
     paramOption: int = 0,
-    paramIndex: int = -1
+    paramIndex: int = -1,
+    useGlobalIndex: bool = False,
 ) -> int:
     """
     Returns info about drum pads
 
     Currently only supported by FPC
 
     ## Notes:
     * The official documentation lists this as returning a string, but it
       actually returns an int.
 
     ## Args:
     * `chanIndex` (`int`): channel of plugin to check
 
-    * `slotIndex` (`int`, optional): slot of mixer track plugin. Defaults to -1.
+    * `slotIndex` (`int`, optional): slot of mixer track plugin. Defaults to `-1`.
 
     * `paramOption` (`int`, optional): type of query:
           * `0`: number of pads (note: given number is one greater than there
             actually are, ie. FPC has 32 pads but 33 is returned)
 
           * `1`: semitone number of pad (use `paramIndex`)
 
           * `2`: color of pad as 0xBBGGRR (use `paramIndex`)
 
     * `paramIndex` (`int`, optional): drum pad number (0-indexed)
 
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
+
     ## Returns:
     * `int`: number of parameters, or
 
     * `int`: note number of pad, or
 
     * `int`: color of pad
 
     Included since API Version 19
     """
     return 0
 
 
 @since(15)
-def getPresetCount(index: int, slotIndex: int = -1) -> int:
+def getPresetCount(
+    index: int,
+    slotIndex: int = -1,
+    useGlobalIndex: bool = False,
+) -> int:
     """Returns the number of presets available for the selected plugin.
 
     ## Args:
-     * `index` (`int`): index of plugin on channel rack or mixer.
+    * `index` (`int`): index of plugin on channel rack or mixer.
+
+    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
 
-     * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to -1.
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
 
     Included since API version 15
     """
     return 0
 
 
 @since(10)
-def nextPreset(index: int, slotIndex: int = -1) -> None:
+def nextPreset(
+    index: int,
+    slotIndex: int = -1,
+    useGlobalIndex: bool = False,
+) -> None:
     """Navigate to the next preset for plugin at `index`/`slotIndex`.
 
     ## Args:
-     * `index` (`int`): index of plugin on channel rack or mixer
-     * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to -1.
+    * `index` (`int`): index of plugin on channel rack or mixer
+
+    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
+
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
 
     Included since API version 10
     """
 
 
 @since(10)
-def prevPreset(index: int, slotIndex: int = -1) -> None:
+def prevPreset(
+    index: int,
+    slotIndex: int = -1,
+    useGlobalIndex: bool = False,
+) -> None:
     """Navigate to the previous preset for plugin at `index`/`slotIndex`.
 
     ## Args:
-     * `index` (`int`): index of plugin on channel rack or mixer
+    * `index` (`int`): index of plugin on channel rack or mixer
+
+    * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to `-1`.
 
-     * `slotIndex` (`int`, optional): mixer slot if on mixer. Defaults to -1.
+    * `useGlobalIndex` (`bool`, optional): whether to use global channel
+      indexes when modifying plugins on the channel rack. Defaults to `False`.
 
     Included since API version 10
     """
```

### Comparing `fl_studio_api_stubs-28.1.0/src/transport/__init__.py` & `fl_studio_api_stubs-28.2.0/src/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/transport/__position.py` & `fl_studio_api_stubs-28.2.0/src/transport/__position.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/transport/__state.py` & `fl_studio_api_stubs-28.2.0/src/transport/__state.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/ui/__browser.py` & `fl_studio_api_stubs-28.2.0/src/ui/__browser.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/ui/__editors.py` & `fl_studio_api_stubs-28.2.0/src/ui/__editors.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/ui/__fl_state.py` & `fl_studio_api_stubs-28.2.0/src/ui/__fl_state.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/ui/__init__.py` & `fl_studio_api_stubs-28.2.0/src/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/ui/__keyboard.py` & `fl_studio_api_stubs-28.2.0/src/ui/__keyboard.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/ui/__navigation.py` & `fl_studio_api_stubs-28.2.0/src/ui/__navigation.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/ui/__overlays.py` & `fl_studio_api_stubs-28.2.0/src/ui/__overlays.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/ui/__windows.py` & `fl_studio_api_stubs-28.2.0/src/ui/__windows.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/src/utils/__init__.py` & `fl_studio_api_stubs-28.2.0/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fl_studio_api_stubs-28.1.0/PKG-INFO` & `fl_studio_api_stubs-28.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fl-studio-api-stubs
-Version: 28.1.0
+Version: 28.2.0
 Summary: Module and function definitions and documentation for the FL Studio Python API
 Home-page: https://github.com/MiguelGuthridge/FL-Studio-Api-Stubs
 License: LGPL-3.0-only
 Keywords: fl-studio,midi,api,documentation,stubs,fl,studio,daw,controller
 Author: Miguel Guthridge
 Author-email: hdsq@outlook.com.au
 Requires-Python: >=3.9.1,<4.0.0
@@ -14,14 +14,18 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Typing :: Stubs Only
+Classifier: Typing :: Typed
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/MiguelGuthridge/FL-Studio-Api-Stubs/issues
 Project-URL: Documentation, https://miguelguthridge.github.io/FL-Studio-API-Stubs/
 Project-URL: Online Documentation, https://miguelguthridge.github.io/FL-Studio-API-Stubs/
 Project-URL: Repository, https://github.com/MiguelGuthridge/FL-Studio-Api-Stubs
 Description-Content-Type: text/markdown
```

