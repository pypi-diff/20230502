# Comparing `tmp/firefly-3.2.2.tar.gz` & `tmp/firefly-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefly-3.2.2.tar", last modified: Tue May  2 16:10:54 2023, max compression
+gzip compressed data, was "firefly-3.2.3.tar", last modified: Tue May  2 16:25:30 2023, max compression
```

## Comparing `firefly-3.2.2.tar` & `firefly-3.2.3.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.240000 firefly-3.2.2/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    35164 2022-12-20 16:39:08.000000 firefly-3.2.2/LICENSE
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)      537 2023-05-02 15:49:00.000000 firefly-3.2.2/MANIFEST.in
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2825 2023-05-02 16:10:56.000000 firefly-3.2.2/PKG-INFO
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2274 2023-05-02 15:49:00.000000 firefly-3.2.2/README.md
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)      104 2021-06-24 14:43:20.000000 firefly-3.2.2/pyproject.toml
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)       38 2023-05-02 16:10:56.000000 firefly-3.2.2/setup.cfg
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1214 2023-05-02 16:09:04.000000 firefly-3.2.2/setup.py
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.250000 firefly-3.2.2/src/
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.260000 firefly-3.2.2/src/firefly/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)       18 2021-11-04 16:05:00.000000 firefly-3.2.2/src/firefly/__init__.py
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.290000 firefly-3.2.2/src/firefly/bin/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4798 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/bin/firefly
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2023 2022-05-27 20:36:18.000000 firefly-3.2.2/src/firefly/bin/make_new_repo.sh
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.310000 firefly-3.2.2/src/firefly/data_reader/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    18456 2022-08-19 19:32:34.000000 firefly-3.2.2/src/firefly/data_reader/FIREreader.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    13875 2022-08-19 19:32:34.000000 firefly-3.2.2/src/firefly/data_reader/GAIAreader.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)      294 2022-12-20 16:39:08.000000 firefly-3.2.2/src/firefly/data_reader/__init__.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     8009 2022-08-19 19:32:34.000000 firefly-3.2.2/src/firefly/data_reader/binary_writer.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1071 2021-11-04 16:05:00.000000 firefly-3.2.2/src/firefly/data_reader/json_utils.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    45499 2023-01-16 17:03:46.000000 firefly-3.2.2/src/firefly/data_reader/octree.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    37398 2023-01-16 17:03:46.000000 firefly-3.2.2/src/firefly/data_reader/particlegroup.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    50236 2022-12-20 16:39:08.000000 firefly-3.2.2/src/firefly/data_reader/reader.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    31652 2023-05-02 15:49:00.000000 firefly-3.2.2/src/firefly/data_reader/settings.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7451 2022-08-19 19:32:34.000000 firefly-3.2.2/src/firefly/data_reader/tween.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     5957 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/index.html
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.320000 firefly-3.2.2/src/firefly/ntbks/
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.340000 firefly-3.2.2/src/firefly/ntbks/.ipynb_checkpoints/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     8174 2022-05-10 19:27:44.000000 firefly-3.2.2/src/firefly/ntbks/.ipynb_checkpoints/flask_tutorial-checkpoint.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     3415 2022-08-25 17:33:00.000000 firefly-3.2.2/src/firefly/ntbks/.ipynb_checkpoints/minimal_example-checkpoint.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2709 2023-01-23 22:55:32.000000 firefly-3.2.2/src/firefly/ntbks/.ipynb_checkpoints/passing_settings-checkpoint.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2758 2023-04-11 22:09:54.000000 firefly-3.2.2/src/firefly/ntbks/.ipynb_checkpoints/selecting_data-checkpoint.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)   224187 2022-08-19 19:32:34.000000 firefly-3.2.2/src/firefly/ntbks/GaiaDR3.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    32213 2022-08-19 19:32:34.000000 firefly-3.2.2/src/firefly/ntbks/convert_FIRE_data.ipynb
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.370000 firefly-3.2.2/src/firefly/ntbks/examples/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7689 2022-08-19 19:32:34.000000 firefly-3.2.2/src/firefly/ntbks/examples/DiskFormation.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    72201 2022-08-19 19:32:34.000000 firefly-3.2.2/src/firefly/ntbks/examples/GaiaDR3_octree.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    71574 2022-08-19 19:32:34.000000 firefly-3.2.2/src/firefly/ntbks/examples/GaiaDR3toFirefly.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    93731 2022-08-19 19:32:34.000000 firefly-3.2.2/src/firefly/ntbks/examples/SDSS_test.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     8410 2022-08-19 19:32:34.000000 firefly-3.2.2/src/firefly/ntbks/flask_tutorial.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    30391 2022-05-09 17:23:44.000000 firefly-3.2.2/src/firefly/ntbks/memoryScaling.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     3415 2022-08-25 17:33:00.000000 firefly-3.2.2/src/firefly/ntbks/minimal_example.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    27054 2022-05-09 17:39:58.000000 firefly-3.2.2/src/firefly/ntbks/multiple_datasets_tutorial.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)   292553 2022-05-09 17:23:44.000000 firefly-3.2.2/src/firefly/ntbks/octree_test.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)   299159 2022-08-19 19:32:34.000000 firefly-3.2.2/src/firefly/ntbks/performance_testing.ipynb
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.390000 firefly-3.2.2/src/firefly/ntbks/py_conversions/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     5224 2022-05-09 17:39:58.000000 firefly-3.2.2/src/firefly/ntbks/py_conversions/convert_FIRE_data.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     5477 2022-05-09 17:39:58.000000 firefly-3.2.2/src/firefly/ntbks/py_conversions/flask_tutorial.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)      959 2022-05-09 17:39:58.000000 firefly-3.2.2/src/firefly/ntbks/py_conversions/minimal_example.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4933 2022-05-09 17:39:58.000000 firefly-3.2.2/src/firefly/ntbks/py_conversions/multiple_datasets_tutorial.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7490 2022-05-09 17:39:58.000000 firefly-3.2.2/src/firefly/ntbks/py_conversions/reader_tutorial.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6969 2022-05-09 17:39:58.000000 firefly-3.2.2/src/firefly/ntbks/py_conversions/settings_tutorial.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    31864 2022-05-09 17:39:58.000000 firefly-3.2.2/src/firefly/ntbks/reader_tutorial.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    73763 2022-05-09 17:39:58.000000 firefly-3.2.2/src/firefly/ntbks/settings_tutorial.ipynb
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    15059 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/server.py
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.400000 firefly-3.2.2/src/firefly/static/
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.420000 firefly-3.2.2/src/firefly/static/css/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     9242 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/css/UIStyles.css
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7204 2021-11-04 16:05:00.000000 firefly-3.2.2/src/firefly/static/css/UIStyles2.css
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4714 2023-01-16 20:53:24.000000 firefly-3.2.2/src/firefly/static/css/mainStyles.css
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.430000 firefly-3.2.2/src/firefly/static/data/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)       29 2022-08-22 15:53:16.000000 firefly-3.2.2/src/firefly/static/data/startup.json
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.450000 firefly-3.2.2/src/firefly/static/docs/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)   299606 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/docs/FIREFLY-02_trimmed.png
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     5209 2022-05-09 17:23:44.000000 firefly-3.2.2/src/firefly/static/docs/GUIicon.png
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)      243 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/docs/README.md
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    10792 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/docs/READMEcleanPack.md
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    49203 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/docs/UI.png
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)   444248 2022-05-09 17:39:58.000000 firefly-3.2.2/src/firefly/static/docs/icon.png
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)  1220398 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/docs/jupyter_embed.png
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)  1593536 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/docs/screenGrab.png
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.480000 firefly-3.2.2/src/firefly/static/js/
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.480000 firefly-3.2.2/src/firefly/static/js/gui/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    11073 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/gui/GUIParams.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    50941 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/gui/GUIconstructors.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    14195 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/gui/GUIsocket.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    36366 2022-12-20 16:39:08.000000 firefly-3.2.2/src/firefly/static/js/gui/UI.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    13336 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/gui/colormap.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     9704 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/gui/initGUI.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    15225 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/gui/particles.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    16383 2023-01-16 17:03:46.000000 firefly-3.2.2/src/firefly/static/js/gui/sliders.js
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.510000 firefly-3.2.2/src/firefly/static/js/misc/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6078 2022-05-09 17:23:44.000000 firefly-3.2.2/src/firefly/static/js/misc/FireflyFormat1.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4902 2022-08-19 19:32:36.000000 firefly-3.2.2/src/firefly/static/js/misc/FireflyOctnodeSubstring.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1854 2022-05-09 17:23:44.000000 firefly-3.2.2/src/firefly/static/js/misc/MyArrayBuffer.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)      723 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/misc/defaultParticleSettings.json
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1179 2022-12-20 16:39:08.000000 firefly-3.2.2/src/firefly/static/js/misc/defaultSettings.json
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.530000 firefly-3.2.2/src/firefly/static/js/misc/kaitai-struct/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    26557 2022-05-09 17:23:44.000000 firefly-3.2.2/src/firefly/static/js/misc/kaitai-struct/KaitaiStream.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1027 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/misc/socketParams.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4890 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/misc/utils.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7583 2022-12-20 16:39:08.000000 firefly-3.2.2/src/firefly/static/js/misc/windowEvents.js
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.560000 firefly-3.2.2/src/firefly/static/js/octree/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6061 2022-08-19 19:32:36.000000 firefly-3.2.2/src/firefly/static/js/octree/octreeCreatePartsMesh.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7280 2022-08-19 19:32:36.000000 firefly-3.2.2/src/firefly/static/js/octree/octreeInit.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    20169 2022-12-20 16:39:54.000000 firefly-3.2.2/src/firefly/static/js/octree/octreeRenderLoop.js
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.580000 firefly-3.2.2/src/firefly/static/js/streamer/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2489 2022-08-25 16:28:22.000000 firefly-3.2.2/src/firefly/static/js/streamer/initStreamer.js
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.610000 firefly-3.2.2/src/firefly/static/js/viewer/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    23040 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/viewer/applyUISelections.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6547 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/viewer/createPartsMesh.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    58661 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/viewer/initViewer.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    27547 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/viewer/renderLoop.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4403 2022-05-09 18:36:26.000000 firefly-3.2.2/src/firefly/static/js/viewer/runTweens.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    10353 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/js/viewer/viewerParams.js
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.620000 firefly-3.2.2/src/firefly/static/lib/
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.650000 firefly-3.2.2/src/firefly/static/lib/CCapture/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    30507 2022-08-24 16:24:06.000000 firefly-3.2.2/src/firefly/static/lib/CCapture/CCapture.all.min.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     9324 2022-08-24 16:24:06.000000 firefly-3.2.2/src/firefly/static/lib/CCapture/gif.worker.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1962 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/Detector.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7032 2022-05-09 17:23:44.000000 firefly-3.2.2/src/firefly/static/lib/DeviceOrientationControls.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     3401 2022-05-09 17:23:44.000000 firefly-3.2.2/src/firefly/static/lib/KeyboardState.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    27761 2022-12-20 16:39:08.000000 firefly-3.2.2/src/firefly/static/lib/OrbitControls.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1314 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/StereoEffect.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     3222 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/THREEx.FullScreen.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1204 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/THREEx.WindowResize.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    18351 2022-12-20 16:39:08.000000 firefly-3.2.2/src/firefly/static/lib/TrackballControls.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    16253 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/Tween.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4372 2022-05-09 17:23:44.000000 firefly-3.2.2/src/firefly/static/lib/VRButton.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)   218325 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/d3.v4.10.2.min.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    86663 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/jquery-3.2.1.min.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     3555 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/nouislider.min.css
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    21186 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/nouislider.min.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    64366 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/socket.io.min.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)   161175 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/socket.io.min.js.map
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    65155 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/socket.io.min.js.org
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    15428 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/spectrum.css
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    82157 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/spectrum.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    11147 2022-05-09 17:23:44.000000 firefly-3.2.2/src/firefly/static/lib/three-fly-controls.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)   516205 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/three.min.js.old
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)   565444 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/three.min.r102.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)   619002 2022-05-09 17:23:44.000000 firefly-3.2.2/src/firefly/static/lib/three.min.r137.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    19061 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/threeoctree.min.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     9142 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/lib/wNumb.js
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.880000 firefly-3.2.2/src/firefly/static/shaders/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4586 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/shaders/fragment.glsl.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1161 2023-01-24 20:08:00.000000 firefly-3.2.2/src/firefly/static/shaders/fragment_pass2.glsl.js
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2034 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/shaders/vertex.glsl.js
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.890000 firefly-3.2.2/src/firefly/static/textures/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)      203 2022-08-19 19:32:36.000000 firefly-3.2.2/src/firefly/static/textures/bb.png
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    14790 2021-11-04 16:05:02.000000 firefly-3.2.2/src/firefly/static/textures/cmap.png
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     5058 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/textures/colormap.png
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)      414 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/textures/colormap_names.json
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)    44387 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/static/textures/createColormap.ipynb
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.910000 firefly-3.2.2/src/firefly/templates/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6587 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/templates/VR.html
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6449 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/templates/combined.html
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6381 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/templates/default.html
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     3761 2022-12-20 16:39:08.000000 firefly-3.2.2/src/firefly/templates/gui.html
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1974 2022-08-24 16:24:06.000000 firefly-3.2.2/src/firefly/templates/streamer.html
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4381 2023-05-02 15:47:56.000000 firefly-3.2.2/src/firefly/templates/viewer.html
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.940000 firefly-3.2.2/src/firefly/tests/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2022-12-20 16:39:06.000000 firefly-3.2.2/src/firefly/tests/__init__.py
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1545 2022-12-20 16:39:08.000000 firefly-3.2.2/src/firefly/tests/test_settings.py
-drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:10:46.280000 firefly-3.2.2/src/firefly.egg-info/
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2825 2023-05-02 16:10:44.000000 firefly-3.2.2/src/firefly.egg-info/PKG-INFO
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)     5293 2023-05-02 16:10:48.000000 firefly-3.2.2/src/firefly.egg-info/SOURCES.txt
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)        1 2023-05-02 16:10:44.000000 firefly-3.2.2/src/firefly.egg-info/dependency_links.txt
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)       75 2023-05-02 16:10:44.000000 firefly-3.2.2/src/firefly.egg-info/requires.txt
--rwxrwxrwx   0 ageller   (1000) ageller   (1000)        8 2023-05-02 16:10:44.000000 firefly-3.2.2/src/firefly.egg-info/top_level.txt
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.150000 firefly-3.2.3/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    35164 2022-12-20 16:39:08.000000 firefly-3.2.3/LICENSE
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)      537 2023-05-02 15:49:00.000000 firefly-3.2.3/MANIFEST.in
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2877 2023-05-02 16:25:32.000000 firefly-3.2.3/PKG-INFO
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2326 2023-05-02 16:21:40.000000 firefly-3.2.3/README.md
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)      104 2021-06-24 14:43:20.000000 firefly-3.2.3/pyproject.toml
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)       38 2023-05-02 16:25:32.000000 firefly-3.2.3/setup.cfg
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1214 2023-05-02 16:24:36.000000 firefly-3.2.3/setup.py
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.170000 firefly-3.2.3/src/
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.170000 firefly-3.2.3/src/firefly/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)       18 2021-11-04 16:05:00.000000 firefly-3.2.3/src/firefly/__init__.py
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.200000 firefly-3.2.3/src/firefly/bin/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4798 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/bin/firefly
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2023 2022-05-27 20:36:18.000000 firefly-3.2.3/src/firefly/bin/make_new_repo.sh
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.220000 firefly-3.2.3/src/firefly/data_reader/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    18456 2022-08-19 19:32:34.000000 firefly-3.2.3/src/firefly/data_reader/FIREreader.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    13875 2022-08-19 19:32:34.000000 firefly-3.2.3/src/firefly/data_reader/GAIAreader.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)      294 2022-12-20 16:39:08.000000 firefly-3.2.3/src/firefly/data_reader/__init__.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     8009 2022-08-19 19:32:34.000000 firefly-3.2.3/src/firefly/data_reader/binary_writer.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1071 2021-11-04 16:05:00.000000 firefly-3.2.3/src/firefly/data_reader/json_utils.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    45499 2023-01-16 17:03:46.000000 firefly-3.2.3/src/firefly/data_reader/octree.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    37398 2023-01-16 17:03:46.000000 firefly-3.2.3/src/firefly/data_reader/particlegroup.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    50236 2022-12-20 16:39:08.000000 firefly-3.2.3/src/firefly/data_reader/reader.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    31652 2023-05-02 15:49:00.000000 firefly-3.2.3/src/firefly/data_reader/settings.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7451 2022-08-19 19:32:34.000000 firefly-3.2.3/src/firefly/data_reader/tween.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     5957 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/index.html
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.230000 firefly-3.2.3/src/firefly/ntbks/
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.270000 firefly-3.2.3/src/firefly/ntbks/.ipynb_checkpoints/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     8174 2022-05-10 19:27:44.000000 firefly-3.2.3/src/firefly/ntbks/.ipynb_checkpoints/flask_tutorial-checkpoint.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     3415 2022-08-25 17:33:00.000000 firefly-3.2.3/src/firefly/ntbks/.ipynb_checkpoints/minimal_example-checkpoint.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2709 2023-01-23 22:55:32.000000 firefly-3.2.3/src/firefly/ntbks/.ipynb_checkpoints/passing_settings-checkpoint.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2758 2023-04-11 22:09:54.000000 firefly-3.2.3/src/firefly/ntbks/.ipynb_checkpoints/selecting_data-checkpoint.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)   224187 2022-08-19 19:32:34.000000 firefly-3.2.3/src/firefly/ntbks/GaiaDR3.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    32213 2022-08-19 19:32:34.000000 firefly-3.2.3/src/firefly/ntbks/convert_FIRE_data.ipynb
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.280000 firefly-3.2.3/src/firefly/ntbks/examples/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7689 2022-08-19 19:32:34.000000 firefly-3.2.3/src/firefly/ntbks/examples/DiskFormation.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    72201 2022-08-19 19:32:34.000000 firefly-3.2.3/src/firefly/ntbks/examples/GaiaDR3_octree.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    71574 2022-08-19 19:32:34.000000 firefly-3.2.3/src/firefly/ntbks/examples/GaiaDR3toFirefly.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    93731 2022-08-19 19:32:34.000000 firefly-3.2.3/src/firefly/ntbks/examples/SDSS_test.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     8410 2022-08-19 19:32:34.000000 firefly-3.2.3/src/firefly/ntbks/flask_tutorial.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    30391 2022-05-09 17:23:44.000000 firefly-3.2.3/src/firefly/ntbks/memoryScaling.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     3415 2022-08-25 17:33:00.000000 firefly-3.2.3/src/firefly/ntbks/minimal_example.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    27054 2022-05-09 17:39:58.000000 firefly-3.2.3/src/firefly/ntbks/multiple_datasets_tutorial.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)   292553 2022-05-09 17:23:44.000000 firefly-3.2.3/src/firefly/ntbks/octree_test.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)   299159 2022-08-19 19:32:34.000000 firefly-3.2.3/src/firefly/ntbks/performance_testing.ipynb
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.310000 firefly-3.2.3/src/firefly/ntbks/py_conversions/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     5224 2022-05-09 17:39:58.000000 firefly-3.2.3/src/firefly/ntbks/py_conversions/convert_FIRE_data.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     5477 2022-05-09 17:39:58.000000 firefly-3.2.3/src/firefly/ntbks/py_conversions/flask_tutorial.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)      959 2022-05-09 17:39:58.000000 firefly-3.2.3/src/firefly/ntbks/py_conversions/minimal_example.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4933 2022-05-09 17:39:58.000000 firefly-3.2.3/src/firefly/ntbks/py_conversions/multiple_datasets_tutorial.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7490 2022-05-09 17:39:58.000000 firefly-3.2.3/src/firefly/ntbks/py_conversions/reader_tutorial.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6969 2022-05-09 17:39:58.000000 firefly-3.2.3/src/firefly/ntbks/py_conversions/settings_tutorial.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    31864 2022-05-09 17:39:58.000000 firefly-3.2.3/src/firefly/ntbks/reader_tutorial.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    73763 2022-05-09 17:39:58.000000 firefly-3.2.3/src/firefly/ntbks/settings_tutorial.ipynb
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    15059 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/server.py
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.340000 firefly-3.2.3/src/firefly/static/
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.350000 firefly-3.2.3/src/firefly/static/css/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     9242 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/css/UIStyles.css
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7204 2021-11-04 16:05:00.000000 firefly-3.2.3/src/firefly/static/css/UIStyles2.css
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4714 2023-01-16 20:53:24.000000 firefly-3.2.3/src/firefly/static/css/mainStyles.css
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.370000 firefly-3.2.3/src/firefly/static/data/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)       29 2022-08-22 15:53:16.000000 firefly-3.2.3/src/firefly/static/data/startup.json
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.400000 firefly-3.2.3/src/firefly/static/docs/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)   299606 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/docs/FIREFLY-02_trimmed.png
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     5209 2022-05-09 17:23:44.000000 firefly-3.2.3/src/firefly/static/docs/GUIicon.png
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)      243 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/docs/README.md
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    10792 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/docs/READMEcleanPack.md
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    49203 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/docs/UI.png
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)   444248 2022-05-09 17:39:58.000000 firefly-3.2.3/src/firefly/static/docs/icon.png
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)  1220398 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/docs/jupyter_embed.png
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)  1593536 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/docs/screenGrab.png
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.420000 firefly-3.2.3/src/firefly/static/js/
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.430000 firefly-3.2.3/src/firefly/static/js/gui/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    11073 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/gui/GUIParams.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    50941 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/gui/GUIconstructors.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    14195 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/gui/GUIsocket.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    36366 2022-12-20 16:39:08.000000 firefly-3.2.3/src/firefly/static/js/gui/UI.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    13336 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/gui/colormap.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     9704 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/gui/initGUI.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    15225 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/gui/particles.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    16383 2023-01-16 17:03:46.000000 firefly-3.2.3/src/firefly/static/js/gui/sliders.js
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.450000 firefly-3.2.3/src/firefly/static/js/misc/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6078 2022-05-09 17:23:44.000000 firefly-3.2.3/src/firefly/static/js/misc/FireflyFormat1.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4902 2022-08-19 19:32:36.000000 firefly-3.2.3/src/firefly/static/js/misc/FireflyOctnodeSubstring.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1854 2022-05-09 17:23:44.000000 firefly-3.2.3/src/firefly/static/js/misc/MyArrayBuffer.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)      723 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/misc/defaultParticleSettings.json
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1179 2022-12-20 16:39:08.000000 firefly-3.2.3/src/firefly/static/js/misc/defaultSettings.json
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.480000 firefly-3.2.3/src/firefly/static/js/misc/kaitai-struct/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    26557 2022-05-09 17:23:44.000000 firefly-3.2.3/src/firefly/static/js/misc/kaitai-struct/KaitaiStream.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1027 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/misc/socketParams.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4890 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/misc/utils.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7583 2022-12-20 16:39:08.000000 firefly-3.2.3/src/firefly/static/js/misc/windowEvents.js
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.500000 firefly-3.2.3/src/firefly/static/js/octree/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6061 2022-08-19 19:32:36.000000 firefly-3.2.3/src/firefly/static/js/octree/octreeCreatePartsMesh.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7280 2022-08-19 19:32:36.000000 firefly-3.2.3/src/firefly/static/js/octree/octreeInit.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    20169 2022-12-20 16:39:54.000000 firefly-3.2.3/src/firefly/static/js/octree/octreeRenderLoop.js
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.520000 firefly-3.2.3/src/firefly/static/js/streamer/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2489 2022-08-25 16:28:22.000000 firefly-3.2.3/src/firefly/static/js/streamer/initStreamer.js
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.550000 firefly-3.2.3/src/firefly/static/js/viewer/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    23040 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/viewer/applyUISelections.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6547 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/viewer/createPartsMesh.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    58661 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/viewer/initViewer.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    27547 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/viewer/renderLoop.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4403 2022-05-09 18:36:26.000000 firefly-3.2.3/src/firefly/static/js/viewer/runTweens.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    10353 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/js/viewer/viewerParams.js
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.580000 firefly-3.2.3/src/firefly/static/lib/
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.610000 firefly-3.2.3/src/firefly/static/lib/CCapture/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    30507 2022-08-24 16:24:06.000000 firefly-3.2.3/src/firefly/static/lib/CCapture/CCapture.all.min.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     9324 2022-08-24 16:24:06.000000 firefly-3.2.3/src/firefly/static/lib/CCapture/gif.worker.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1962 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/Detector.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     7032 2022-05-09 17:23:44.000000 firefly-3.2.3/src/firefly/static/lib/DeviceOrientationControls.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     3401 2022-05-09 17:23:44.000000 firefly-3.2.3/src/firefly/static/lib/KeyboardState.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    27761 2022-12-20 16:39:08.000000 firefly-3.2.3/src/firefly/static/lib/OrbitControls.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1314 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/StereoEffect.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     3222 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/THREEx.FullScreen.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1204 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/THREEx.WindowResize.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    18351 2022-12-20 16:39:08.000000 firefly-3.2.3/src/firefly/static/lib/TrackballControls.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    16253 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/Tween.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4372 2022-05-09 17:23:44.000000 firefly-3.2.3/src/firefly/static/lib/VRButton.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)   218325 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/d3.v4.10.2.min.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    86663 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/jquery-3.2.1.min.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     3555 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/nouislider.min.css
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    21186 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/nouislider.min.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    64366 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/socket.io.min.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)   161175 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/socket.io.min.js.map
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    65155 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/socket.io.min.js.org
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    15428 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/spectrum.css
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    82157 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/spectrum.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    11147 2022-05-09 17:23:44.000000 firefly-3.2.3/src/firefly/static/lib/three-fly-controls.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)   516205 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/three.min.js.old
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)   565444 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/three.min.r102.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)   619002 2022-05-09 17:23:44.000000 firefly-3.2.3/src/firefly/static/lib/three.min.r137.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    19061 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/threeoctree.min.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     9142 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/lib/wNumb.js
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.630000 firefly-3.2.3/src/firefly/static/shaders/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4586 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/shaders/fragment.glsl.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1161 2023-01-24 20:08:00.000000 firefly-3.2.3/src/firefly/static/shaders/fragment_pass2.glsl.js
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2034 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/shaders/vertex.glsl.js
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.640000 firefly-3.2.3/src/firefly/static/textures/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)      203 2022-08-19 19:32:36.000000 firefly-3.2.3/src/firefly/static/textures/bb.png
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    14790 2021-11-04 16:05:02.000000 firefly-3.2.3/src/firefly/static/textures/cmap.png
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     5058 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/textures/colormap.png
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)      414 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/textures/colormap_names.json
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)    44387 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/static/textures/createColormap.ipynb
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.670000 firefly-3.2.3/src/firefly/templates/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6587 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/templates/VR.html
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6449 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/templates/combined.html
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     6381 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/templates/default.html
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     3761 2022-12-20 16:39:08.000000 firefly-3.2.3/src/firefly/templates/gui.html
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1974 2022-08-24 16:24:06.000000 firefly-3.2.3/src/firefly/templates/streamer.html
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     4381 2023-05-02 15:47:56.000000 firefly-3.2.3/src/firefly/templates/viewer.html
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.690000 firefly-3.2.3/src/firefly/tests/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2022-12-20 16:39:06.000000 firefly-3.2.3/src/firefly/tests/__init__.py
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     1545 2022-12-20 16:39:08.000000 firefly-3.2.3/src/firefly/tests/test_settings.py
+drwxrwxrwx   0 ageller   (1000) ageller   (1000)        0 2023-05-02 16:25:22.190000 firefly-3.2.3/src/firefly.egg-info/
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     2877 2023-05-02 16:25:20.000000 firefly-3.2.3/src/firefly.egg-info/PKG-INFO
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)     5293 2023-05-02 16:25:24.000000 firefly-3.2.3/src/firefly.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)        1 2023-05-02 16:25:20.000000 firefly-3.2.3/src/firefly.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)       75 2023-05-02 16:25:20.000000 firefly-3.2.3/src/firefly.egg-info/requires.txt
+-rwxrwxrwx   0 ageller   (1000) ageller   (1000)        8 2023-05-02 16:25:20.000000 firefly-3.2.3/src/firefly.egg-info/top_level.txt
```

### Comparing `firefly-3.2.2/LICENSE` & `firefly-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/MANIFEST.in` & `firefly-3.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/PKG-INFO` & `firefly-3.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly
-Version: 3.2.2
+Version: 3.2.3
 Summary: A browser-based particle visualization platform
 Home-page: http://www.firefly-viz.com/
 Author: Alex Gurvich, Aaron Geller
 Author-email: agurvich@u.northwestern.edu, a-geller@northwestern.edu
 Project-URL: Bug Tracker, https://github.com/ageller/Firefly/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -21,15 +21,15 @@
 
 ![logo banner](https://github.com/ageller/Firefly/blob/main/docs/source/_static/four_view_banner.png?raw=true)
 
 
 Firefly is an interactive viewer for any particle-based data. A live example is available [here](https://ageller.github.io/Firefly/)
 or if you're ready to get started creating your own interactive viewer, [click here](http://www.firefly-viz.com/docs/data_reader).
 
-If you use Firefly, please cite us using the [ADS listing](http://adsabs.harvard.edu/abs/2018ascl.soft10021G) that points to our Astrophysics Source Code Library (ASCL) entry.
+If you use Firefly, please cite our [ApJS paper](https://ui.adsabs.harvard.edu/abs/2023ApJS..265...38G/abstract) and our [entry in the Astrophysics Source Code Library (ASCL)](http://adsabs.harvard.edu/abs/2018ascl.soft10021G).
 
 ## Additional Docs
 
 Comprehensive documentation is available [here](http://www.firefly-viz.com/docs).
 
 ## Contributors 
 ### Primary Developers
```

#### html2text {}

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1 Name: firefly Version: 3.2.2 Summary: A browser-based
+Metadata-Version: 2.1 Name: firefly Version: 3.2.3 Summary: A browser-based
 particle visualization platform Home-page: http://www.firefly-viz.com/ Author:
 Alex Gurvich, Aaron Geller Author-email: agurvich@u.northwestern.edu, a-
 geller@northwestern.edu Project-URL: Bug Tracker, https://github.com/ageller/
 Firefly/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 or later
 (AGPLv3+) Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Firefly [!
 [PyPI](https://img.shields.io/pypi/v/Firefly)](https://pypi.org/project/
 Firefly) [ascl:1810.021] ![logo banner](https://github.com/ageller/Firefly/
 blob/main/docs/source/_static/four_view_banner.png?raw=true) Firefly is an
 interactive viewer for any particle-based data. A live example is available
 [here](https://ageller.github.io/Firefly/) or if you're ready to get started
 creating your own interactive viewer, [click here](http://www.firefly-viz.com/
-docs/data_reader). If you use Firefly, please cite us using the [ADS listing]
-(http://adsabs.harvard.edu/abs/2018ascl.soft10021G) that points to our
-Astrophysics Source Code Library (ASCL) entry. ## Additional Docs Comprehensive
-documentation is available [here](http://www.firefly-viz.com/docs). ##
-Contributors ### Primary Developers * Aaron Geller * Alex Gurvich ### Past
-Contributors * Mike Cronin * Zach Hafen * Alessandro Febretti ### Student
-Contributors * Mahlet Shiferaw * Luolei Zhao * Nora Linzer ### Project PI *
-Claude-AndrÃ© Faucher-GiguÃ¨re ## Acknowledgments Firefly is written in WebGL
-using the three.js library. This tool builds off of a [previous version
-developed by Alessandro Febretti](https://github.com/nuitrcs/firefly). This
-project is funded by [Northwestern's Center for Interdisciplinary Exploration
-and Research in Astrophysics (CIERA)](https://ciera.northwestern.edu/),
-[Northwestern's IT Research Computing group](https://www.it.northwestern.edu/
-research/index.html), and NSF grants AST-1412836, AST-1715216, and CAREER award
-AST-1652522 awarded to [Claude-AndrÃ© Faucher-GiguÃ¨re](https://
-www.physics.northwestern.edu/people/faculty/core-faculty/claude-andre-faucher-
-giguere.html). ## Additional Info Firefly was originally designed for [FIRE]
-(http://galaxies.northwestern.edu/fire-simulations/) data, but has since been
-extended to support any particle data. This package should not be confused with
-the serendipitously named web-based visualization software [Firefly, from
-Caltech-IPAC](https://github.com/Caltech-IPAC/firefly), a general tool for
-retrieving and viewing astronomy data.
+docs/data_reader). If you use Firefly, please cite our [ApJS paper](https://
+ui.adsabs.harvard.edu/abs/2023ApJS..265...38G/abstract) and our [entry in the
+Astrophysics Source Code Library (ASCL)](http://adsabs.harvard.edu/abs/
+2018ascl.soft10021G). ## Additional Docs Comprehensive documentation is
+available [here](http://www.firefly-viz.com/docs). ## Contributors ### Primary
+Developers * Aaron Geller * Alex Gurvich ### Past Contributors * Mike Cronin *
+Zach Hafen * Alessandro Febretti ### Student Contributors * Mahlet Shiferaw *
+Luolei Zhao * Nora Linzer ### Project PI * Claude-AndrÃ© Faucher-GiguÃ¨re ##
+Acknowledgments Firefly is written in WebGL using the three.js library. This
+tool builds off of a [previous version developed by Alessandro Febretti](https:
+//github.com/nuitrcs/firefly). This project is funded by [Northwestern's Center
+for Interdisciplinary Exploration and Research in Astrophysics (CIERA)](https:/
+/ciera.northwestern.edu/), [Northwestern's IT Research Computing group](https:/
+/www.it.northwestern.edu/research/index.html), and NSF grants AST-1412836, AST-
+1715216, and CAREER award AST-1652522 awarded to [Claude-AndrÃ© Faucher-
+GiguÃ¨re](https://www.physics.northwestern.edu/people/faculty/core-faculty/
+claude-andre-faucher-giguere.html). ## Additional Info Firefly was originally
+designed for [FIRE](http://galaxies.northwestern.edu/fire-simulations/) data,
+but has since been extended to support any particle data. This package should
+not be confused with the serendipitously named web-based visualization software
+[Firefly, from Caltech-IPAC](https://github.com/Caltech-IPAC/firefly), a
+general tool for retrieving and viewing astronomy data.
```

### Comparing `firefly-3.2.2/README.md` & `firefly-3.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ![logo banner](https://github.com/ageller/Firefly/blob/main/docs/source/_static/four_view_banner.png?raw=true)
 
 
 Firefly is an interactive viewer for any particle-based data. A live example is available [here](https://ageller.github.io/Firefly/)
 or if you're ready to get started creating your own interactive viewer, [click here](http://www.firefly-viz.com/docs/data_reader).
 
-If you use Firefly, please cite us using the [ADS listing](http://adsabs.harvard.edu/abs/2018ascl.soft10021G) that points to our Astrophysics Source Code Library (ASCL) entry.
+If you use Firefly, please cite our [ApJS paper](https://ui.adsabs.harvard.edu/abs/2023ApJS..265...38G/abstract) and our [entry in the Astrophysics Source Code Library (ASCL)](http://adsabs.harvard.edu/abs/2018ascl.soft10021G).
 
 ## Additional Docs
 
 Comprehensive documentation is available [here](http://www.firefly-viz.com/docs).
 
 ## Contributors 
 ### Primary Developers
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
  # Firefly [![PyPI](https://img.shields.io/pypi/v/Firefly)](https://pypi.org/
 project/Firefly) [ascl:1810.021] ![logo banner](https://github.com/ageller/
 Firefly/blob/main/docs/source/_static/four_view_banner.png?raw=true) Firefly is
 an interactive viewer for any particle-based data. A live example is available
 [here](https://ageller.github.io/Firefly/) or if you're ready to get started
 creating your own interactive viewer, [click here](http://www.firefly-viz.com/
-docs/data_reader). If you use Firefly, please cite us using the [ADS listing]
-(http://adsabs.harvard.edu/abs/2018ascl.soft10021G) that points to our
-Astrophysics Source Code Library (ASCL) entry. ## Additional Docs Comprehensive
-documentation is available [here](http://www.firefly-viz.com/docs). ##
-Contributors ### Primary Developers * Aaron Geller * Alex Gurvich ### Past
-Contributors * Mike Cronin * Zach Hafen * Alessandro Febretti ### Student
-Contributors * Mahlet Shiferaw * Luolei Zhao * Nora Linzer ### Project PI *
-Claude-AndrÃ© Faucher-GiguÃ¨re ## Acknowledgments Firefly is written in WebGL
-using the three.js library. This tool builds off of a [previous version
-developed by Alessandro Febretti](https://github.com/nuitrcs/firefly). This
-project is funded by [Northwestern's Center for Interdisciplinary Exploration
-and Research in Astrophysics (CIERA)](https://ciera.northwestern.edu/),
-[Northwestern's IT Research Computing group](https://www.it.northwestern.edu/
-research/index.html), and NSF grants AST-1412836, AST-1715216, and CAREER award
-AST-1652522 awarded to [Claude-AndrÃ© Faucher-GiguÃ¨re](https://
-www.physics.northwestern.edu/people/faculty/core-faculty/claude-andre-faucher-
-giguere.html). ## Additional Info Firefly was originally designed for [FIRE]
-(http://galaxies.northwestern.edu/fire-simulations/) data, but has since been
-extended to support any particle data. This package should not be confused with
-the serendipitously named web-based visualization software [Firefly, from
-Caltech-IPAC](https://github.com/Caltech-IPAC/firefly), a general tool for
-retrieving and viewing astronomy data.
+docs/data_reader). If you use Firefly, please cite our [ApJS paper](https://
+ui.adsabs.harvard.edu/abs/2023ApJS..265...38G/abstract) and our [entry in the
+Astrophysics Source Code Library (ASCL)](http://adsabs.harvard.edu/abs/
+2018ascl.soft10021G). ## Additional Docs Comprehensive documentation is
+available [here](http://www.firefly-viz.com/docs). ## Contributors ### Primary
+Developers * Aaron Geller * Alex Gurvich ### Past Contributors * Mike Cronin *
+Zach Hafen * Alessandro Febretti ### Student Contributors * Mahlet Shiferaw *
+Luolei Zhao * Nora Linzer ### Project PI * Claude-AndrÃ© Faucher-GiguÃ¨re ##
+Acknowledgments Firefly is written in WebGL using the three.js library. This
+tool builds off of a [previous version developed by Alessandro Febretti](https:
+//github.com/nuitrcs/firefly). This project is funded by [Northwestern's Center
+for Interdisciplinary Exploration and Research in Astrophysics (CIERA)](https:/
+/ciera.northwestern.edu/), [Northwestern's IT Research Computing group](https:/
+/www.it.northwestern.edu/research/index.html), and NSF grants AST-1412836, AST-
+1715216, and CAREER award AST-1652522 awarded to [Claude-AndrÃ© Faucher-
+GiguÃ¨re](https://www.physics.northwestern.edu/people/faculty/core-faculty/
+claude-andre-faucher-giguere.html). ## Additional Info Firefly was originally
+designed for [FIRE](http://galaxies.northwestern.edu/fire-simulations/) data,
+but has since been extended to support any particle data. This package should
+not be confused with the serendipitously named web-based visualization software
+[Firefly, from Caltech-IPAC](https://github.com/Caltech-IPAC/firefly), a
+general tool for retrieving and viewing astronomy data.
```

### Comparing `firefly-3.2.2/setup.py` & `firefly-3.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="firefly",
-    version="3.2.2",
+    version="3.2.3",
     author = 'Alex Gurvich, Aaron Geller',
     author_email = 'agurvich@u.northwestern.edu, a-geller@northwestern.edu',
     description="A browser-based particle visualization platform",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://www.firefly-viz.com/",
     project_urls={
```

### Comparing `firefly-3.2.2/src/firefly/bin/firefly` & `firefly-3.2.3/src/firefly/bin/firefly`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/bin/make_new_repo.sh` & `firefly-3.2.3/src/firefly/bin/make_new_repo.sh`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/data_reader/FIREreader.py` & `firefly-3.2.3/src/firefly/data_reader/FIREreader.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/data_reader/GAIAreader.py` & `firefly-3.2.3/src/firefly/data_reader/GAIAreader.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/data_reader/binary_writer.py` & `firefly-3.2.3/src/firefly/data_reader/binary_writer.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/data_reader/json_utils.py` & `firefly-3.2.3/src/firefly/data_reader/json_utils.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/data_reader/octree.py` & `firefly-3.2.3/src/firefly/data_reader/octree.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/data_reader/particlegroup.py` & `firefly-3.2.3/src/firefly/data_reader/particlegroup.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/data_reader/reader.py` & `firefly-3.2.3/src/firefly/data_reader/reader.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/data_reader/settings.py` & `firefly-3.2.3/src/firefly/data_reader/settings.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/data_reader/tween.py` & `firefly-3.2.3/src/firefly/data_reader/tween.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/index.html` & `firefly-3.2.3/src/firefly/index.html`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/.ipynb_checkpoints/flask_tutorial-checkpoint.ipynb` & `firefly-3.2.3/src/firefly/ntbks/.ipynb_checkpoints/flask_tutorial-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/.ipynb_checkpoints/minimal_example-checkpoint.ipynb` & `firefly-3.2.3/src/firefly/ntbks/.ipynb_checkpoints/minimal_example-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/.ipynb_checkpoints/passing_settings-checkpoint.ipynb` & `firefly-3.2.3/src/firefly/ntbks/.ipynb_checkpoints/passing_settings-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/.ipynb_checkpoints/selecting_data-checkpoint.ipynb` & `firefly-3.2.3/src/firefly/ntbks/.ipynb_checkpoints/selecting_data-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/GaiaDR3.ipynb` & `firefly-3.2.3/src/firefly/ntbks/GaiaDR3.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/convert_FIRE_data.ipynb` & `firefly-3.2.3/src/firefly/ntbks/convert_FIRE_data.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/examples/DiskFormation.ipynb` & `firefly-3.2.3/src/firefly/ntbks/examples/DiskFormation.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/examples/GaiaDR3_octree.ipynb` & `firefly-3.2.3/src/firefly/ntbks/examples/GaiaDR3_octree.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/examples/GaiaDR3toFirefly.ipynb` & `firefly-3.2.3/src/firefly/ntbks/examples/GaiaDR3toFirefly.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/examples/SDSS_test.ipynb` & `firefly-3.2.3/src/firefly/ntbks/examples/SDSS_test.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/flask_tutorial.ipynb` & `firefly-3.2.3/src/firefly/ntbks/flask_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/memoryScaling.ipynb` & `firefly-3.2.3/src/firefly/ntbks/memoryScaling.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/minimal_example.ipynb` & `firefly-3.2.3/src/firefly/ntbks/minimal_example.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/multiple_datasets_tutorial.ipynb` & `firefly-3.2.3/src/firefly/ntbks/multiple_datasets_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/octree_test.ipynb` & `firefly-3.2.3/src/firefly/ntbks/octree_test.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/performance_testing.ipynb` & `firefly-3.2.3/src/firefly/ntbks/performance_testing.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/py_conversions/convert_FIRE_data.py` & `firefly-3.2.3/src/firefly/ntbks/py_conversions/convert_FIRE_data.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/py_conversions/flask_tutorial.py` & `firefly-3.2.3/src/firefly/ntbks/py_conversions/flask_tutorial.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/py_conversions/minimal_example.py` & `firefly-3.2.3/src/firefly/ntbks/py_conversions/minimal_example.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/py_conversions/multiple_datasets_tutorial.py` & `firefly-3.2.3/src/firefly/ntbks/py_conversions/multiple_datasets_tutorial.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/py_conversions/reader_tutorial.py` & `firefly-3.2.3/src/firefly/ntbks/py_conversions/reader_tutorial.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/py_conversions/settings_tutorial.py` & `firefly-3.2.3/src/firefly/ntbks/py_conversions/settings_tutorial.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/reader_tutorial.ipynb` & `firefly-3.2.3/src/firefly/ntbks/reader_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/ntbks/settings_tutorial.ipynb` & `firefly-3.2.3/src/firefly/ntbks/settings_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/server.py` & `firefly-3.2.3/src/firefly/server.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/css/UIStyles.css` & `firefly-3.2.3/src/firefly/static/css/UIStyles.css`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/css/UIStyles2.css` & `firefly-3.2.3/src/firefly/static/css/UIStyles2.css`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/css/mainStyles.css` & `firefly-3.2.3/src/firefly/static/css/mainStyles.css`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/docs/FIREFLY-02_trimmed.png` & `firefly-3.2.3/src/firefly/static/docs/FIREFLY-02_trimmed.png`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/docs/GUIicon.png` & `firefly-3.2.3/src/firefly/static/docs/GUIicon.png`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/docs/READMEcleanPack.md` & `firefly-3.2.3/src/firefly/static/docs/READMEcleanPack.md`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/docs/UI.png` & `firefly-3.2.3/src/firefly/static/docs/UI.png`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/docs/icon.png` & `firefly-3.2.3/src/firefly/static/docs/icon.png`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/docs/jupyter_embed.png` & `firefly-3.2.3/src/firefly/static/docs/jupyter_embed.png`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/docs/screenGrab.png` & `firefly-3.2.3/src/firefly/static/docs/screenGrab.png`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/gui/GUIParams.js` & `firefly-3.2.3/src/firefly/static/js/gui/GUIParams.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/gui/GUIconstructors.js` & `firefly-3.2.3/src/firefly/static/js/gui/GUIconstructors.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/gui/GUIsocket.js` & `firefly-3.2.3/src/firefly/static/js/gui/GUIsocket.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/gui/UI.js` & `firefly-3.2.3/src/firefly/static/js/gui/UI.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/gui/colormap.js` & `firefly-3.2.3/src/firefly/static/js/gui/colormap.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/gui/initGUI.js` & `firefly-3.2.3/src/firefly/static/js/gui/initGUI.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/gui/particles.js` & `firefly-3.2.3/src/firefly/static/js/gui/particles.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/gui/sliders.js` & `firefly-3.2.3/src/firefly/static/js/gui/sliders.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/misc/FireflyFormat1.js` & `firefly-3.2.3/src/firefly/static/js/misc/FireflyFormat1.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/misc/FireflyOctnodeSubstring.js` & `firefly-3.2.3/src/firefly/static/js/misc/FireflyOctnodeSubstring.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/misc/MyArrayBuffer.js` & `firefly-3.2.3/src/firefly/static/js/misc/MyArrayBuffer.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/misc/defaultParticleSettings.json` & `firefly-3.2.3/src/firefly/static/js/misc/defaultParticleSettings.json`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/misc/defaultSettings.json` & `firefly-3.2.3/src/firefly/static/js/misc/defaultSettings.json`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/misc/kaitai-struct/KaitaiStream.js` & `firefly-3.2.3/src/firefly/static/js/misc/kaitai-struct/KaitaiStream.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/misc/socketParams.js` & `firefly-3.2.3/src/firefly/static/js/misc/socketParams.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/misc/utils.js` & `firefly-3.2.3/src/firefly/static/js/misc/utils.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/misc/windowEvents.js` & `firefly-3.2.3/src/firefly/static/js/misc/windowEvents.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/octree/octreeCreatePartsMesh.js` & `firefly-3.2.3/src/firefly/static/js/octree/octreeCreatePartsMesh.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/octree/octreeInit.js` & `firefly-3.2.3/src/firefly/static/js/octree/octreeInit.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/octree/octreeRenderLoop.js` & `firefly-3.2.3/src/firefly/static/js/octree/octreeRenderLoop.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/streamer/initStreamer.js` & `firefly-3.2.3/src/firefly/static/js/streamer/initStreamer.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/viewer/applyUISelections.js` & `firefly-3.2.3/src/firefly/static/js/viewer/applyUISelections.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/viewer/createPartsMesh.js` & `firefly-3.2.3/src/firefly/static/js/viewer/createPartsMesh.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/viewer/initViewer.js` & `firefly-3.2.3/src/firefly/static/js/viewer/initViewer.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/viewer/renderLoop.js` & `firefly-3.2.3/src/firefly/static/js/viewer/renderLoop.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/viewer/runTweens.js` & `firefly-3.2.3/src/firefly/static/js/viewer/runTweens.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/js/viewer/viewerParams.js` & `firefly-3.2.3/src/firefly/static/js/viewer/viewerParams.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/CCapture/CCapture.all.min.js` & `firefly-3.2.3/src/firefly/static/lib/CCapture/CCapture.all.min.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/CCapture/gif.worker.js` & `firefly-3.2.3/src/firefly/static/lib/CCapture/gif.worker.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/Detector.js` & `firefly-3.2.3/src/firefly/static/lib/Detector.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/DeviceOrientationControls.js` & `firefly-3.2.3/src/firefly/static/lib/DeviceOrientationControls.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/KeyboardState.js` & `firefly-3.2.3/src/firefly/static/lib/KeyboardState.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/OrbitControls.js` & `firefly-3.2.3/src/firefly/static/lib/OrbitControls.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/StereoEffect.js` & `firefly-3.2.3/src/firefly/static/lib/StereoEffect.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/THREEx.FullScreen.js` & `firefly-3.2.3/src/firefly/static/lib/THREEx.FullScreen.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/THREEx.WindowResize.js` & `firefly-3.2.3/src/firefly/static/lib/THREEx.WindowResize.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/TrackballControls.js` & `firefly-3.2.3/src/firefly/static/lib/TrackballControls.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/Tween.js` & `firefly-3.2.3/src/firefly/static/lib/Tween.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/VRButton.js` & `firefly-3.2.3/src/firefly/static/lib/VRButton.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/d3.v4.10.2.min.js` & `firefly-3.2.3/src/firefly/static/lib/d3.v4.10.2.min.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/jquery-3.2.1.min.js` & `firefly-3.2.3/src/firefly/static/lib/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/nouislider.min.css` & `firefly-3.2.3/src/firefly/static/lib/nouislider.min.css`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/nouislider.min.js` & `firefly-3.2.3/src/firefly/static/lib/nouislider.min.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/socket.io.min.js` & `firefly-3.2.3/src/firefly/static/lib/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/socket.io.min.js.map` & `firefly-3.2.3/src/firefly/static/lib/socket.io.min.js.map`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/socket.io.min.js.org` & `firefly-3.2.3/src/firefly/static/lib/socket.io.min.js.org`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/spectrum.css` & `firefly-3.2.3/src/firefly/static/lib/spectrum.css`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/spectrum.js` & `firefly-3.2.3/src/firefly/static/lib/spectrum.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/three-fly-controls.js` & `firefly-3.2.3/src/firefly/static/lib/three-fly-controls.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/three.min.js.old` & `firefly-3.2.3/src/firefly/static/lib/three.min.js.old`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/three.min.r102.js` & `firefly-3.2.3/src/firefly/static/lib/three.min.r102.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/three.min.r137.js` & `firefly-3.2.3/src/firefly/static/lib/three.min.r137.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/threeoctree.min.js` & `firefly-3.2.3/src/firefly/static/lib/threeoctree.min.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/lib/wNumb.js` & `firefly-3.2.3/src/firefly/static/lib/wNumb.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/shaders/fragment.glsl.js` & `firefly-3.2.3/src/firefly/static/shaders/fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/shaders/fragment_pass2.glsl.js` & `firefly-3.2.3/src/firefly/static/shaders/fragment_pass2.glsl.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/shaders/vertex.glsl.js` & `firefly-3.2.3/src/firefly/static/shaders/vertex.glsl.js`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/textures/cmap.png` & `firefly-3.2.3/src/firefly/static/textures/cmap.png`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/textures/colormap.png` & `firefly-3.2.3/src/firefly/static/textures/colormap.png`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/static/textures/createColormap.ipynb` & `firefly-3.2.3/src/firefly/static/textures/createColormap.ipynb`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/templates/VR.html` & `firefly-3.2.3/src/firefly/templates/VR.html`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/templates/combined.html` & `firefly-3.2.3/src/firefly/templates/combined.html`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/templates/default.html` & `firefly-3.2.3/src/firefly/templates/default.html`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/templates/gui.html` & `firefly-3.2.3/src/firefly/templates/gui.html`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/templates/streamer.html` & `firefly-3.2.3/src/firefly/templates/streamer.html`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/templates/viewer.html` & `firefly-3.2.3/src/firefly/templates/viewer.html`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly/tests/test_settings.py` & `firefly-3.2.3/src/firefly/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `firefly-3.2.2/src/firefly.egg-info/PKG-INFO` & `firefly-3.2.3/src/firefly.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly
-Version: 3.2.2
+Version: 3.2.3
 Summary: A browser-based particle visualization platform
 Home-page: http://www.firefly-viz.com/
 Author: Alex Gurvich, Aaron Geller
 Author-email: agurvich@u.northwestern.edu, a-geller@northwestern.edu
 Project-URL: Bug Tracker, https://github.com/ageller/Firefly/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -21,15 +21,15 @@
 
 ![logo banner](https://github.com/ageller/Firefly/blob/main/docs/source/_static/four_view_banner.png?raw=true)
 
 
 Firefly is an interactive viewer for any particle-based data. A live example is available [here](https://ageller.github.io/Firefly/)
 or if you're ready to get started creating your own interactive viewer, [click here](http://www.firefly-viz.com/docs/data_reader).
 
-If you use Firefly, please cite us using the [ADS listing](http://adsabs.harvard.edu/abs/2018ascl.soft10021G) that points to our Astrophysics Source Code Library (ASCL) entry.
+If you use Firefly, please cite our [ApJS paper](https://ui.adsabs.harvard.edu/abs/2023ApJS..265...38G/abstract) and our [entry in the Astrophysics Source Code Library (ASCL)](http://adsabs.harvard.edu/abs/2018ascl.soft10021G).
 
 ## Additional Docs
 
 Comprehensive documentation is available [here](http://www.firefly-viz.com/docs).
 
 ## Contributors 
 ### Primary Developers
```

#### html2text {}

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1 Name: firefly Version: 3.2.2 Summary: A browser-based
+Metadata-Version: 2.1 Name: firefly Version: 3.2.3 Summary: A browser-based
 particle visualization platform Home-page: http://www.firefly-viz.com/ Author:
 Alex Gurvich, Aaron Geller Author-email: agurvich@u.northwestern.edu, a-
 geller@northwestern.edu Project-URL: Bug Tracker, https://github.com/ageller/
 Firefly/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 or later
 (AGPLv3+) Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Firefly [!
 [PyPI](https://img.shields.io/pypi/v/Firefly)](https://pypi.org/project/
 Firefly) [ascl:1810.021] ![logo banner](https://github.com/ageller/Firefly/
 blob/main/docs/source/_static/four_view_banner.png?raw=true) Firefly is an
 interactive viewer for any particle-based data. A live example is available
 [here](https://ageller.github.io/Firefly/) or if you're ready to get started
 creating your own interactive viewer, [click here](http://www.firefly-viz.com/
-docs/data_reader). If you use Firefly, please cite us using the [ADS listing]
-(http://adsabs.harvard.edu/abs/2018ascl.soft10021G) that points to our
-Astrophysics Source Code Library (ASCL) entry. ## Additional Docs Comprehensive
-documentation is available [here](http://www.firefly-viz.com/docs). ##
-Contributors ### Primary Developers * Aaron Geller * Alex Gurvich ### Past
-Contributors * Mike Cronin * Zach Hafen * Alessandro Febretti ### Student
-Contributors * Mahlet Shiferaw * Luolei Zhao * Nora Linzer ### Project PI *
-Claude-AndrÃ© Faucher-GiguÃ¨re ## Acknowledgments Firefly is written in WebGL
-using the three.js library. This tool builds off of a [previous version
-developed by Alessandro Febretti](https://github.com/nuitrcs/firefly). This
-project is funded by [Northwestern's Center for Interdisciplinary Exploration
-and Research in Astrophysics (CIERA)](https://ciera.northwestern.edu/),
-[Northwestern's IT Research Computing group](https://www.it.northwestern.edu/
-research/index.html), and NSF grants AST-1412836, AST-1715216, and CAREER award
-AST-1652522 awarded to [Claude-AndrÃ© Faucher-GiguÃ¨re](https://
-www.physics.northwestern.edu/people/faculty/core-faculty/claude-andre-faucher-
-giguere.html). ## Additional Info Firefly was originally designed for [FIRE]
-(http://galaxies.northwestern.edu/fire-simulations/) data, but has since been
-extended to support any particle data. This package should not be confused with
-the serendipitously named web-based visualization software [Firefly, from
-Caltech-IPAC](https://github.com/Caltech-IPAC/firefly), a general tool for
-retrieving and viewing astronomy data.
+docs/data_reader). If you use Firefly, please cite our [ApJS paper](https://
+ui.adsabs.harvard.edu/abs/2023ApJS..265...38G/abstract) and our [entry in the
+Astrophysics Source Code Library (ASCL)](http://adsabs.harvard.edu/abs/
+2018ascl.soft10021G). ## Additional Docs Comprehensive documentation is
+available [here](http://www.firefly-viz.com/docs). ## Contributors ### Primary
+Developers * Aaron Geller * Alex Gurvich ### Past Contributors * Mike Cronin *
+Zach Hafen * Alessandro Febretti ### Student Contributors * Mahlet Shiferaw *
+Luolei Zhao * Nora Linzer ### Project PI * Claude-AndrÃ© Faucher-GiguÃ¨re ##
+Acknowledgments Firefly is written in WebGL using the three.js library. This
+tool builds off of a [previous version developed by Alessandro Febretti](https:
+//github.com/nuitrcs/firefly). This project is funded by [Northwestern's Center
+for Interdisciplinary Exploration and Research in Astrophysics (CIERA)](https:/
+/ciera.northwestern.edu/), [Northwestern's IT Research Computing group](https:/
+/www.it.northwestern.edu/research/index.html), and NSF grants AST-1412836, AST-
+1715216, and CAREER award AST-1652522 awarded to [Claude-AndrÃ© Faucher-
+GiguÃ¨re](https://www.physics.northwestern.edu/people/faculty/core-faculty/
+claude-andre-faucher-giguere.html). ## Additional Info Firefly was originally
+designed for [FIRE](http://galaxies.northwestern.edu/fire-simulations/) data,
+but has since been extended to support any particle data. This package should
+not be confused with the serendipitously named web-based visualization software
+[Firefly, from Caltech-IPAC](https://github.com/Caltech-IPAC/firefly), a
+general tool for retrieving and viewing astronomy data.
```

### Comparing `firefly-3.2.2/src/firefly.egg-info/SOURCES.txt` & `firefly-3.2.3/src/firefly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

