# Comparing `tmp/ibllib-2.9.0.tar.gz` & `tmp/ibllib-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibllib-2.9.0.tar", last modified: Mon Jan 24 09:07:18 2022, max compression
+gzip compressed data, was "ibllib-2.9.1.tar", last modified: Wed Jan 26 11:53:46 2022, max compression
```

## Comparing `ibllib-2.9.0.tar` & `ibllib-2.9.1.tar`

### file list

```diff
@@ -1,381 +1,384 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.347597 ibllib-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-01-24 09:07:07.000000 ibllib-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-01-24 09:07:07.000000 ibllib-2.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-01-24 09:07:18.347597 ibllib-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-01-24 09:07:07.000000 ibllib-2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.275593 ibllib-2.9.0/brainbox/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6644 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/atlas.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.275593 ibllib-2.9.0/brainbox/behavior/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/behavior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25176 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/behavior/dlc.py
--rw-r--r--   0 runner    (1001) docker     (121)    11425 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/behavior/pyschofit.py
--rw-r--r--   0 runner    (1001) docker     (121)    29470 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/behavior/training.py
--rw-r--r--   0 runner    (1001) docker     (121)    16300 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/behavior/wheel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4436 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    19880 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/ephys_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.275593 ibllib-2.9.0/brainbox/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    45430 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/io/one.py
--rw-r--r--   0 runner    (1001) docker     (121)     6735 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/io/spikeglx.py
--rw-r--r--   0 runner    (1001) docker     (121)     3778 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/lfp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.275593 ibllib-2.9.0/brainbox/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3644 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/metrics/electrode_drift.py
--rw-r--r--   0 runner    (1001) docker     (121)    40547 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/metrics/single_units.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.275593 ibllib-2.9.0/brainbox/modeling/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20969 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/modeling/design_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/modeling/linear.py
--rw-r--r--   0 runner    (1001) docker     (121)    11044 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/modeling/neural_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4401 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/modeling/poisson.py
--rw-r--r--   0 runner    (1001) docker     (121)     5851 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/modeling/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    34012 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    25786 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/plot_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.275593 ibllib-2.9.0/brainbox/population/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16018 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/population/cca.py
--rw-r--r--   0 runner    (1001) docker     (121)    20250 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/population/decode.py
--rw-r--r--   0 runner    (1001) docker     (121)    17926 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.275593 ibllib-2.9.0/brainbox/quality/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/quality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/quality/lfp_qc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/quality/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7431 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/singlecell.py
--rw-r--r--   0 runner    (1001) docker     (121)     4726 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/spike_features.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.275593 ibllib-2.9.0/brainbox/task/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8891 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/task/_knockoff.py
--rw-r--r--   0 runner    (1001) docker     (121)    25808 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/task/_statsmodels.py
--rw-r--r--   0 runner    (1001) docker     (121)    16854 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/task/closed_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     8701 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/task/passive.py
--rw-r--r--   0 runner    (1001) docker     (121)    14926 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/task/trials.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.279593 ibllib-2.9.0/brainbox/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.283594 ibllib-2.9.0/brainbox/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)    33480 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/fixtures/design_matrix_test.npy
--rw-r--r--   0 runner    (1001) docker     (121)     3468 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/fixtures/design_wheel_traces_test.p
--rw-r--r--   0 runner    (1001) docker     (121)  1499590 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/fixtures/ephys_test.p
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/fixtures/parquet_records.json
--rw-r--r--   0 runner    (1001) docker     (121)    39114 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/fixtures/trials_df_test.csv
--rw-r--r--   0 runner    (1001) docker     (121)   443468 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/fixtures/trials_test.pickle
--rw-r--r--   0 runner    (1001) docker     (121)  3524212 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/fixtures/wheel_test.p
--rw-r--r--   0 runner    (1001) docker     (121)    16012 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_behavior.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_cca.py
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_modeling.py
--rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_passive.py
--rw-r--r--   0 runner    (1001) docker     (121)    10816 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_plot_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7043 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_population.py
--rw-r--r--   0 runner    (1001) docker     (121)     7117 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_singlecell.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5816 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     8122 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_trials.py
--rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/tests/test_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-01-24 09:07:07.000000 ibllib-2.9.0/brainbox/video.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.287594 ibllib-2.9.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.287594 ibllib-2.9.0/examples/one/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/examples/one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3863 2022-01-24 09:07:07.000000 ibllib-2.9.0/examples/one/docs_one_queries.py
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-01-24 09:07:07.000000 ibllib-2.9.0/examples/one/one_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.287594 ibllib-2.9.0/ibllib/
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.287594 ibllib-2.9.0/ibllib/atlas/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/atlas/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   223004 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/atlas/allen_structure_tree.csv
--rw-r--r--   0 runner    (1001) docker     (121)    35228 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/atlas/atlas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/atlas/beryl.npy
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/atlas/cosmos.npy
--rw-r--r--   0 runner    (1001) docker     (121)     7078 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/atlas/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.287594 ibllib-2.9.0/ibllib/dsp/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/dsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2460 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/dsp/cadzow.py
--rw-r--r--   0 runner    (1001) docker     (121)     9648 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/dsp/fourier.py
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/dsp/savitzky_golay.py
--rw-r--r--   0 runner    (1001) docker     (121)     8712 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/dsp/smooth.py
--rw-r--r--   0 runner    (1001) docker     (121)     8703 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/dsp/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    27314 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/dsp/voltage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.291594 ibllib-2.9.0/ibllib/ephys/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28918 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/ephys/ephysqc.py
--rw-r--r--   0 runner    (1001) docker     (121)    11030 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/ephys/neuropixel.py
--rw-r--r--   0 runner    (1001) docker     (121)    20796 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/ephys/np2_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)    11634 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/ephys/spikes.py
--rw-r--r--   0 runner    (1001) docker     (121)    11843 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/ephys/sync_probes.py
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7821 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/graphic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.291594 ibllib-2.9.0/ibllib/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30231 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/certification_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.291594 ibllib-2.9.0/ibllib/io/extractors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8465 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/biased_trials.py
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/bpod_trials.py
--rw-r--r--   0 runner    (1001) docker     (121)    34516 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/camera.py
--rw-r--r--   0 runner    (1001) docker     (121)    34572 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_fpga.py
--rw-r--r--   0 runner    (1001) docker     (121)    25648 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_passive.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.303594 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/
--rw-r--r--   0 runner    (1001) docker     (121)     7776 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/passive_stim_meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_0_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    81728 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_0_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_0_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_0_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_0_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_0_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_10_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    83568 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_10_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_10_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_10_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_10_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16816 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_10_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_11_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    80288 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_11_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_11_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_11_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_11_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16160 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_11_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_1_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    80248 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_1_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_1_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_1_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_1_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16152 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_1_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_2_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    81808 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_2_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_2_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_2_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_2_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16464 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_2_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_3_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    81048 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_3_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_3_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_3_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_3_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16312 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_3_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_4_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    80488 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_4_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_4_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_4_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_4_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16200 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_4_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_5_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    80568 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_5_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_5_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_5_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_5_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16216 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_5_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_6_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    82648 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_6_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_6_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_6_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_6_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16632 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_6_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_7_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    80328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_7_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_7_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_7_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_7_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16168 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_7_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_8_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    83768 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_8_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_8_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_8_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_8_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16856 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_8_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_9_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    80608 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_9_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_9_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_9_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_9_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16224 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_9_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_mock_ephys_len_blocks.npy
--rw-r--r--   0 runner    (1001) docker     (121)    80288 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_mock_ephys_pcqs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_mock_passive_pcs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_mock_passive_stimDelays.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_mock_passive_stimIDs.npy
--rw-r--r--   0 runner    (1001) docker     (121)    16160 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_mock_stim_phase.npy
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/extractor_types.json
--rw-r--r--   0 runner    (1001) docker     (121)     6211 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/habituation_trials.py
--rw-r--r--   0 runner    (1001) docker     (121)     2623 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/opto_trials.py
--rw-r--r--   0 runner    (1001) docker     (121)     4328 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/passive_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     8264 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/signatures.py
--rw-r--r--   0 runner    (1001) docker     (121)     7175 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/training_audio.py
--rw-r--r--   0 runner    (1001) docker     (121)    26800 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/training_trials.py
--rw-r--r--   0 runner    (1001) docker     (121)    20503 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/training_wheel.py
--rw-r--r--   0 runner    (1001) docker     (121)    14814 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/extractors/video_motion.py
--rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (121)     8548 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/flags.py
--rw-r--r--   0 runner    (1001) docker     (121)     3300 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/globus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/npy_header.py
--rw-r--r--   0 runner    (1001) docker     (121)    32054 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/raw_data_loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)    32899 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/spikeglx.py
--rw-r--r--   0 runner    (1001) docker     (121)     8534 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/io/video.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.307595 ibllib-2.9.0/ibllib/misc/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/misc/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/misc/timing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/misc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.307595 ibllib-2.9.0/ibllib/oneibl/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/oneibl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2463 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/oneibl/aws.py
--rw-r--r--   0 runner    (1001) docker     (121)    16219 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/oneibl/data_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)    28897 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/oneibl/patcher.py
--rw-r--r--   0 runner    (1001) docker     (121)    20808 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/oneibl/registration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/oneibl/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.307595 ibllib-2.9.0/ibllib/pipes/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23761 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/pipes/ephys_alignment.py
--rw-r--r--   0 runner    (1001) docker     (121)    60331 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/pipes/ephys_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)    26383 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/pipes/histology.py
--rw-r--r--   0 runner    (1001) docker     (121)     8295 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/pipes/local_server.py
--rw-r--r--   0 runner    (1001) docker     (121)    26109 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/pipes/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/pipes/purge_rig_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     5100 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/pipes/remote_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     3282 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/pipes/scan_fix_passive_files.py
--rw-r--r--   0 runner    (1001) docker     (121)    25171 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/pipes/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5358 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/pipes/training_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3150 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/pipes/transfer_rig_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.307595 ibllib-2.9.0/ibllib/plots/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33495 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/plots/figures.py
--rw-r--r--   0 runner    (1001) docker     (121)     9061 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/plots/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    12744 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/plots/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.311595 ibllib-2.9.0/ibllib/qc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19164 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/alignment_qc.py
--rw-r--r--   0 runner    (1001) docker     (121)     9784 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    45669 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/camera.py
--rw-r--r--   0 runner    (1001) docker     (121)     9812 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/critical_reasons.py
--rw-r--r--   0 runner    (1001) docker     (121)    10892 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/dlc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/qcplots.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.315595 ibllib-2.9.0/ibllib/qc/reference/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/reference/frame_src.json
--rw-r--r--   0 runner    (1001) docker     (121)   655488 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/reference/frames_body.npy
--rw-r--r--   0 runner    (1001) docker     (121)  3932288 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/reference/frames_left.npy
--rw-r--r--   0 runner    (1001) docker     (121)   327808 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/reference/frames_right.npy
--rw-r--r--   0 runner    (1001) docker     (121)     9008 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/task_extractors.py
--rw-r--r--   0 runner    (1001) docker     (121)    44702 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/qc/task_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.315595 ibllib-2.9.0/ibllib/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.319595 ibllib-2.9.0/ibllib/tests/extractors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/extractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.271593 ibllib-2.9.0/ibllib/tests/extractors/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.271593 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.319595 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/
--rwxr-xr-x   0 runner    (1001) docker     (121)      909 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_ambientSensorData.raw.jsonable
--rwxr-xr-x   0 runner    (1001) docker     (121)      307 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_encoderEvents.raw.ssv
--rwxr-xr-x   0 runner    (1001) docker     (121)    14534 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv
--rwxr-xr-x   0 runner    (1001) docker     (121)      646 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_encoderTrialInfo.raw.ssv
--rwxr-xr-x   0 runner    (1001) docker     (121)    88412 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_taskData.raw.jsonable
--rwxr-xr-x   0 runner    (1001) docker     (121)     7332 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_taskSettings.raw.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.271593 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_lt5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.319595 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_encoderEvents.raw.ssv
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv
--rw-r--r--   0 runner    (1001) docker     (121)    44708 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_taskData.raw.jsonable
--rwxr-xr-x   0 runner    (1001) docker     (121)     7332 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_taskSettings.raw.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.271593 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.339597 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/
--rw-r--r--   0 runner    (1001) docker     (121)    51951 2022-01-24 09:07:07.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_encoderEvents.raw.ssv
--rw-r--r--   0 runner    (1001) docker     (121) 12148088 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_encoderPositions.raw.ssv
--rw-r--r--   0 runner    (1001) docker     (121)    15026 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_encoderTrialInfo.raw.ssv
--rw-r--r--   0 runner    (1001) docker     (121)    25677 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskCodeFiles.raw.zip
--rw-r--r--   0 runner    (1001) docker     (121)  4450594 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskData.raw.jsonable
--rw-r--r--   0 runner    (1001) docker     (121)    63782 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskDataCodeFiles.raw.zip
--rw-r--r--   0 runner    (1001) docker     (121)   130067 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskSettings.raw.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.339597 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_video_data/
--rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_video_data/_iblrig_bodyCamera.GPIO.bin
--rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_video_data/_iblrig_bodyCamera.frame_counter.bin
--rw-r--r--   0 runner    (1001) docker     (121)   274580 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_video_data/_iblrig_bodyCamera.timestamps.ssv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.271593 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.339597 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1376 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_ambientSensorData.raw.jsonable
--rwxr-xr-x   0 runner    (1001) docker     (121)      460 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_encoderEvents.raw.ssv
--rwxr-xr-x   0 runner    (1001) docker     (121)    12436 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv
--rwxr-xr-x   0 runner    (1001) docker     (121)      882 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_encoderTrialInfo.raw.ssv
--rwxr-xr-x   0 runner    (1001) docker     (121)   176885 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_taskData.raw.jsonable
--rwxr-xr-x   0 runner    (1001) docker     (121)     7684 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_taskSettings.raw.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.271593 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_lt5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.339597 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_encoderEvents.raw.ssv
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv
--rw-r--r--   0 runner    (1001) docker     (121)   778535 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_taskData.raw.jsonable
--rwxr-xr-x   0 runner    (1001) docker     (121)     7684 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_taskSettings.raw.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.271593 ibllib-2.9.0/ibllib/tests/extractors/data/wheel/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.343597 ibllib-2.9.0/ibllib/tests/extractors/data/wheel/ge5/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/wheel/ge5/_iblrig_encoderEvents.raw.ssv
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/wheel/ge5/_iblrig_encoderPositions.raw.ssv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.343597 ibllib-2.9.0/ibllib/tests/extractors/data/wheel/lt5/
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderEvents.raw.00.ssv
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderEvents.raw.CorruptMiddle.ssv
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderEvents.raw.CorruptTimestamp.ssv
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderPositions.raw.00.ssv
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderPositions.raw.01.ssv
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderPositions.raw.2firstsamples.ssv
--rw-r--r--   0 runner    (1001) docker     (121)    22012 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/test_ephys_fpga.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/test_ephys_passive.py
--rw-r--r--   0 runner    (1001) docker     (121)     7455 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/test_ephys_trials.py
--rw-r--r--   0 runner    (1001) docker     (121)    32354 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/extractors/test_extractors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.343597 ibllib-2.9.0/ibllib/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.343597 ibllib-2.9.0/ibllib/tests/fixtures/ephysalignment/
--rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/ephysalignment/alignment_data.npz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.271593 ibllib-2.9.0/ibllib/tests/fixtures/histology/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.343597 ibllib-2.9.0/ibllib/tests/fixtures/histology/tracks/
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/histology/tracks/2019-12-04_KS014_001_probe00_pts.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.271593 ibllib-2.9.0/ibllib/tests/fixtures/io/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.271593 ibllib-2.9.0/ibllib/tests/fixtures/io/data_loaders/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.271593 ibllib-2.9.0/ibllib/tests/fixtures/io/data_loaders/_iblrig_test_mouse_2020-01-01_001/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.343597 ibllib-2.9.0/ibllib/tests/fixtures/io/data_loaders/_iblrig_test_mouse_2020-01-01_001/raw_video_data/
--rw-r--r--   0 runner    (1001) docker     (121)     4320 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/io/data_loaders/_iblrig_test_mouse_2020-01-01_001/raw_video_data/_iblrig_leftCamera.frameData.bin
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.343597 ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/
--rwxr-xr-x   0 runner    (1001) docker     (121)    16660 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3A_g0_t0.imec.ap.meta
--rwxr-xr-x   0 runner    (1001) docker     (121)    12814 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3A_g0_t0.imec.lf.meta
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3A_g0_t0.imec.wiring.json
--rwxr-xr-x   0 runner    (1001) docker     (121)    16654 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3A_short_g0_t0.imec.ap.meta
--rw-r--r--   0 runner    (1001) docker     (121)    15812 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3B2_exported.imec0.ap.meta
--rw-r--r--   0 runner    (1001) docker     (121)    17648 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.imec1.ap.meta
--rw-r--r--   0 runner    (1001) docker     (121)    13840 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.imec1.lf.meta
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.nidq.meta
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.nidq.wiring.json
--rw-r--r--   0 runner    (1001) docker     (121)    15368 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sampleNP2.1_g0_t0.imec.ap.meta
--rw-r--r--   0 runner    (1001) docker     (121)    15645 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sampleNP2.4_g0_t0.imec.ap.meta
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.343597 ibllib-2.9.0/ibllib/tests/fixtures/qc/
--rw-r--r--   0 runner    (1001) docker     (121)     6487 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/qc/data_alignmentqc_existing.npz
--rw-r--r--   0 runner    (1001) docker     (121)     6761 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/qc/data_alignmentqc_manual.npz
--rw-r--r--   0 runner    (1001) docker     (121)     3328 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/qc/pupil_diameter.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1760 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/qc/wheel.npy
--rw-r--r--   0 runner    (1001) docker     (121)    11291 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.343597 ibllib-2.9.0/ibllib/tests/qc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18374 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/qc/test_alignment_qc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6022 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/qc/test_base_qc.py
--rw-r--r--   0 runner    (1001) docker     (121)    12079 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/qc/test_camera_qc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5130 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/qc/test_critical_reasons.py
--rw-r--r--   0 runner    (1001) docker     (121)     5994 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/qc/test_dlc_qc.py
--rw-r--r--   0 runner    (1001) docker     (121)    27812 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/qc/test_task_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    15873 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/test_atlas.py
--rw-r--r--   0 runner    (1001) docker     (121)    15223 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/test_dsp.py
--rw-r--r--   0 runner    (1001) docker     (121)     9730 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/test_ephys.py
--rw-r--r--   0 runner    (1001) docker     (121)     8049 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/test_histology.py
--rw-r--r--   0 runner    (1001) docker     (121)    20456 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     2219 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    13790 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/test_oneibl.py
--rw-r--r--   0 runner    (1001) docker     (121)    20432 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/test_pipes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6745 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)    22908 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/test_spikeglx.py
--rw-r--r--   0 runner    (1001) docker     (121)     9761 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     2145 2022-01-24 09:07:08.000000 ibllib-2.9.0/ibllib/time.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 09:07:18.287594 ibllib-2.9.0/ibllib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-01-24 09:07:18.000000 ibllib-2.9.0/ibllib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15143 2022-01-24 09:07:18.000000 ibllib-2.9.0/ibllib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-24 09:07:18.000000 ibllib-2.9.0/ibllib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-01-24 09:07:18.000000 ibllib-2.9.0/ibllib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-01-24 09:07:18.000000 ibllib-2.9.0/ibllib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-24 09:07:18.347597 ibllib-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-01-24 09:07:08.000000 ibllib-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.520727 ibllib-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-01-26 11:53:38.000000 ibllib-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-01-26 11:53:38.000000 ibllib-2.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-01-26 11:53:46.520727 ibllib-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-01-26 11:53:38.000000 ibllib-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.460727 ibllib-2.9.1/brainbox/
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6644 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/atlas.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.460727 ibllib-2.9.1/brainbox/behavior/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/behavior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25176 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/behavior/dlc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11425 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/behavior/pyschofit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29506 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/behavior/training.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16300 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/behavior/wheel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4436 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19880 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/ephys_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.460727 ibllib-2.9.1/brainbox/io/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47692 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/io/one.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6735 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/io/spikeglx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3778 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/lfp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.460727 ibllib-2.9.1/brainbox/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3644 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/metrics/electrode_drift.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40547 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/metrics/single_units.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.460727 ibllib-2.9.1/brainbox/modeling/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20969 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/modeling/design_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/modeling/linear.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11044 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/modeling/neural_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4401 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/modeling/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5851 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/modeling/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34012 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25786 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/plot_base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.460727 ibllib-2.9.1/brainbox/population/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16018 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/population/cca.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20250 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/population/decode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17926 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.460727 ibllib-2.9.1/brainbox/quality/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/quality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/quality/lfp_qc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/quality/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7431 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/singlecell.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4726 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/spike_features.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.460727 ibllib-2.9.1/brainbox/task/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8891 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/task/_knockoff.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25808 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/task/_statsmodels.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16854 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/task/closed_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8701 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/task/passive.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14926 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/task/trials.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.464727 ibllib-2.9.1/brainbox/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.464727 ibllib-2.9.1/brainbox/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)    33480 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/fixtures/design_matrix_test.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     3468 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/fixtures/design_wheel_traces_test.p
+-rw-r--r--   0 runner    (1001) docker     (121)  1499590 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/fixtures/ephys_test.p
+-rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/fixtures/parquet_records.json
+-rw-r--r--   0 runner    (1001) docker     (121)    39114 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/fixtures/trials_df_test.csv
+-rw-r--r--   0 runner    (1001) docker     (121)   443468 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/fixtures/trials_test.pickle
+-rw-r--r--   0 runner    (1001) docker     (121)  3524212 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/fixtures/wheel_test.p
+-rw-r--r--   0 runner    (1001) docker     (121)    16012 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_cca.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_passive.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10816 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7043 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_population.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7117 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_singlecell.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5816 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8122 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_trials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/tests/test_video.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-01-26 11:53:38.000000 ibllib-2.9.1/brainbox/video.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.468727 ibllib-2.9.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.468727 ibllib-2.9.1/examples/one/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/examples/one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3863 2022-01-26 11:53:38.000000 ibllib-2.9.1/examples/one/docs_one_queries.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-01-26 11:53:38.000000 ibllib-2.9.1/examples/one/one_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.468727 ibllib-2.9.1/ibllib/
+-rw-r--r--   0 runner    (1001) docker     (121)      878 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.472727 ibllib-2.9.1/ibllib/atlas/
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/atlas/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)   223004 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/atlas/allen_structure_tree.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    41532 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/atlas/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/atlas/beryl.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/atlas/cosmos.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    35837 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/atlas/mappings.pqt
+-rw-r--r--   0 runner    (1001) docker     (121)     5107 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/atlas/plots.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/atlas/projections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7654 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/atlas/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.472727 ibllib-2.9.1/ibllib/dsp/
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/dsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2460 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/dsp/cadzow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9648 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/dsp/fourier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/dsp/savitzky_golay.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8712 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/dsp/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8703 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/dsp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27314 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/dsp/voltage.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.472727 ibllib-2.9.1/ibllib/ephys/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28918 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/ephys/ephysqc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11030 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/ephys/neuropixel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20796 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/ephys/np2_converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11634 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/ephys/spikes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11843 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/ephys/sync_probes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7821 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/graphic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.472727 ibllib-2.9.1/ibllib/io/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30231 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/certification_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.476727 ibllib-2.9.1/ibllib/io/extractors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8465 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/biased_trials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/bpod_trials.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34516 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/camera.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34572 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_fpga.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25648 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_passive.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.484727 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/
+-rw-r--r--   0 runner    (1001) docker     (121)     7776 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/passive_stim_meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_0_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    81728 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_0_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_0_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_0_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_0_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_0_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_10_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    83568 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_10_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_10_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_10_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_10_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16816 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_10_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_11_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    80288 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_11_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_11_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_11_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_11_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16160 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_11_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_1_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    80248 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_1_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_1_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_1_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_1_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16152 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_1_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_2_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    81808 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_2_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_2_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_2_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_2_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16464 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_2_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_3_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    81048 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_3_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_3_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_3_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_3_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16312 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_3_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_4_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    80488 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_4_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_4_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_4_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_4_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16200 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_4_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_5_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    80568 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_5_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_5_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_5_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_5_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16216 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_5_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_6_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    82648 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_6_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_6_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_6_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_6_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16632 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_6_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_7_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    80328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_7_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_7_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_7_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_7_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16168 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_7_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_8_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    83768 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_8_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_8_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_8_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_8_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16856 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_8_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_9_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    80608 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_9_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_9_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_9_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_9_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16224 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_9_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_mock_ephys_len_blocks.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    80288 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_mock_ephys_pcqs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_mock_passive_pcs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_mock_passive_stimDelays.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_mock_passive_stimIDs.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    16160 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_mock_stim_phase.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/extractor_types.json
+-rw-r--r--   0 runner    (1001) docker     (121)     6211 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/habituation_trials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2623 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/opto_trials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/passive_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8264 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7175 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/training_audio.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26800 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/training_trials.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20503 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/training_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14814 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/extractors/video_motion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8548 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/flags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3300 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/globus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/npy_header.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32054 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/raw_data_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32899 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/spikeglx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8534 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/io/video.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.484727 ibllib-2.9.1/ibllib/misc/
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/misc/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/misc/timing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/misc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.484727 ibllib-2.9.1/ibllib/oneibl/
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/oneibl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2463 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/oneibl/aws.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16219 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/oneibl/data_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28897 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/oneibl/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20808 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/oneibl/registration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/oneibl/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.488727 ibllib-2.9.1/ibllib/pipes/
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23761 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/pipes/ephys_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60331 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/pipes/ephys_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26383 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/pipes/histology.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8295 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/pipes/local_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26109 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/pipes/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/pipes/purge_rig_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5100 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/pipes/remote_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3282 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/pipes/scan_fix_passive_files.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25285 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/pipes/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5358 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/pipes/training_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3150 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/pipes/transfer_rig_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.488727 ibllib-2.9.1/ibllib/plots/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34799 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/plots/figures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9061 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/plots/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12744 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/plots/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.488727 ibllib-2.9.1/ibllib/qc/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19164 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/alignment_qc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9784 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45669 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/camera.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9812 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/critical_reasons.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10892 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/dlc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/qcplots.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.492727 ibllib-2.9.1/ibllib/qc/reference/
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/reference/frame_src.json
+-rw-r--r--   0 runner    (1001) docker     (121)   655488 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/reference/frames_body.npy
+-rw-r--r--   0 runner    (1001) docker     (121)  3932288 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/reference/frames_left.npy
+-rw-r--r--   0 runner    (1001) docker     (121)   327808 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/reference/frames_right.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     9008 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/task_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44702 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/qc/task_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.496727 ibllib-2.9.1/ibllib/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.496727 ibllib-2.9.1/ibllib/tests/extractors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.456726 ibllib-2.9.1/ibllib/tests/extractors/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.456726 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.496727 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      909 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_ambientSensorData.raw.jsonable
+-rwxr-xr-x   0 runner    (1001) docker     (121)      307 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_encoderEvents.raw.ssv
+-rwxr-xr-x   0 runner    (1001) docker     (121)    14534 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv
+-rwxr-xr-x   0 runner    (1001) docker     (121)      646 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_encoderTrialInfo.raw.ssv
+-rwxr-xr-x   0 runner    (1001) docker     (121)    88412 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_taskData.raw.jsonable
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7332 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_taskSettings.raw.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.456726 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_lt5/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.496727 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_encoderEvents.raw.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)    44708 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_taskData.raw.jsonable
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7332 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_taskSettings.raw.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.456726 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.512727 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/
+-rw-r--r--   0 runner    (1001) docker     (121)    51951 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_encoderEvents.raw.ssv
+-rw-r--r--   0 runner    (1001) docker     (121) 12148088 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_encoderPositions.raw.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)    15026 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_encoderTrialInfo.raw.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)    25677 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskCodeFiles.raw.zip
+-rw-r--r--   0 runner    (1001) docker     (121)  4450594 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskData.raw.jsonable
+-rw-r--r--   0 runner    (1001) docker     (121)    63782 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskDataCodeFiles.raw.zip
+-rw-r--r--   0 runner    (1001) docker     (121)   130067 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskSettings.raw.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.512727 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_video_data/
+-rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_video_data/_iblrig_bodyCamera.GPIO.bin
+-rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_video_data/_iblrig_bodyCamera.frame_counter.bin
+-rw-r--r--   0 runner    (1001) docker     (121)   274580 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_video_data/_iblrig_bodyCamera.timestamps.ssv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.456726 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.516727 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1376 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_ambientSensorData.raw.jsonable
+-rwxr-xr-x   0 runner    (1001) docker     (121)      460 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_encoderEvents.raw.ssv
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12436 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv
+-rwxr-xr-x   0 runner    (1001) docker     (121)      882 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_encoderTrialInfo.raw.ssv
+-rwxr-xr-x   0 runner    (1001) docker     (121)   176885 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_taskData.raw.jsonable
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7684 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_taskSettings.raw.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.456726 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_lt5/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.516727 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_encoderEvents.raw.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)   778535 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_taskData.raw.jsonable
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7684 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_taskSettings.raw.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.456726 ibllib-2.9.1/ibllib/tests/extractors/data/wheel/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.516727 ibllib-2.9.1/ibllib/tests/extractors/data/wheel/ge5/
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/wheel/ge5/_iblrig_encoderEvents.raw.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/wheel/ge5/_iblrig_encoderPositions.raw.ssv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.516727 ibllib-2.9.1/ibllib/tests/extractors/data/wheel/lt5/
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderEvents.raw.00.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderEvents.raw.CorruptMiddle.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)      421 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderEvents.raw.CorruptTimestamp.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderPositions.raw.00.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderPositions.raw.01.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderPositions.raw.2firstsamples.ssv
+-rw-r--r--   0 runner    (1001) docker     (121)    22012 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/test_ephys_fpga.py
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/test_ephys_passive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7455 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/test_ephys_trials.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32354 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/extractors/test_extractors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.516727 ibllib-2.9.1/ibllib/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.516727 ibllib-2.9.1/ibllib/tests/fixtures/ephysalignment/
+-rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/ephysalignment/alignment_data.npz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.456726 ibllib-2.9.1/ibllib/tests/fixtures/histology/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.516727 ibllib-2.9.1/ibllib/tests/fixtures/histology/tracks/
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/histology/tracks/2019-12-04_KS014_001_probe00_pts.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.456726 ibllib-2.9.1/ibllib/tests/fixtures/io/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.456726 ibllib-2.9.1/ibllib/tests/fixtures/io/data_loaders/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.456726 ibllib-2.9.1/ibllib/tests/fixtures/io/data_loaders/_iblrig_test_mouse_2020-01-01_001/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.516727 ibllib-2.9.1/ibllib/tests/fixtures/io/data_loaders/_iblrig_test_mouse_2020-01-01_001/raw_video_data/
+-rw-r--r--   0 runner    (1001) docker     (121)     4320 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/io/data_loaders/_iblrig_test_mouse_2020-01-01_001/raw_video_data/_iblrig_leftCamera.frameData.bin
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.520727 ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    16660 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3A_g0_t0.imec.ap.meta
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12814 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3A_g0_t0.imec.lf.meta
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3A_g0_t0.imec.wiring.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)    16654 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3A_short_g0_t0.imec.ap.meta
+-rw-r--r--   0 runner    (1001) docker     (121)    15812 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3B2_exported.imec0.ap.meta
+-rw-r--r--   0 runner    (1001) docker     (121)    17648 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.imec1.ap.meta
+-rw-r--r--   0 runner    (1001) docker     (121)    13840 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.imec1.lf.meta
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.nidq.meta
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.nidq.wiring.json
+-rw-r--r--   0 runner    (1001) docker     (121)    15368 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sampleNP2.1_g0_t0.imec.ap.meta
+-rw-r--r--   0 runner    (1001) docker     (121)    15645 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sampleNP2.4_g0_t0.imec.ap.meta
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.520727 ibllib-2.9.1/ibllib/tests/fixtures/qc/
+-rw-r--r--   0 runner    (1001) docker     (121)     6487 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/qc/data_alignmentqc_existing.npz
+-rw-r--r--   0 runner    (1001) docker     (121)     6761 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/qc/data_alignmentqc_manual.npz
+-rw-r--r--   0 runner    (1001) docker     (121)     3328 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/qc/pupil_diameter.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     1760 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/qc/wheel.npy
+-rw-r--r--   0 runner    (1001) docker     (121)    11291 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.520727 ibllib-2.9.1/ibllib/tests/qc/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18374 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/qc/test_alignment_qc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6022 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/qc/test_base_qc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12079 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/qc/test_camera_qc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5130 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/qc/test_critical_reasons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5994 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/qc/test_dlc_qc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27812 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/qc/test_task_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15873 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/test_atlas.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15223 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/test_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9730 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/test_ephys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8049 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/test_histology.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20456 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2219 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13790 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/test_oneibl.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20432 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/test_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6745 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22908 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/test_spikeglx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9771 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2145 2022-01-26 11:53:38.000000 ibllib-2.9.1/ibllib/time.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 11:53:46.468727 ibllib-2.9.1/ibllib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-01-26 11:53:46.000000 ibllib-2.9.1/ibllib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    15219 2022-01-26 11:53:46.000000 ibllib-2.9.1/ibllib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 11:53:46.000000 ibllib-2.9.1/ibllib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-01-26 11:53:46.000000 ibllib-2.9.1/ibllib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-01-26 11:53:46.000000 ibllib-2.9.1/ibllib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-26 11:53:46.520727 ibllib-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-01-26 11:53:38.000000 ibllib-2.9.1/setup.py
```

### Comparing `ibllib-2.9.0/LICENSE` & `ibllib-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/PKG-INFO` & `ibllib-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibllib
-Version: 2.9.0
+Version: 2.9.1
 Summary: IBL libraries
 Home-page: https://www.internationalbrainlab.com/
 Author: IBL Staff
 License: MIT
 Description: # IBL Python Libraries 
         [![Coverage badge](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fibllib.hooks.internationalbrainlab.org%2Fcoverage%2Fibllib%2Fmaster)](https://ibllib.hooks.internationalbrainlab.org/coverage/master) 
         [![Tests status badge](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fibllib.hooks.internationalbrainlab.org%2Ftests%2Fibllib%2Fmaster)](https://ibllib.hooks.internationalbrainlab.org/logs/records/master)
```

### Comparing `ibllib-2.9.0/README.md` & `ibllib-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/atlas.py` & `ibllib-2.9.1/brainbox/atlas.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/behavior/dlc.py` & `ibllib-2.9.1/brainbox/behavior/dlc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/behavior/pyschofit.py` & `ibllib-2.9.1/brainbox/behavior/pyschofit.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/behavior/training.py` & `ibllib-2.9.1/brainbox/behavior/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,15 +422,15 @@
 
     if block is None:
         block_idx = np.full(trials.probabilityLeft.shape, True, dtype=bool)
     else:
         block_idx = trials.probabilityLeft == block
 
     if not np.any(block_idx):
-        return np.nan * np.zeros(2)
+        return np.nan * np.zeros(3)
 
     contrasts, n_contrasts = np.unique(signed_contrast[block_idx], return_counts=True)
     rightward = trials.choice == -1
     # Calculate the proportion rightward for each contrast type
     prob_choose_right = np.vectorize(lambda x: np.mean(rightward[(x == signed_contrast) &
                                                                  block_idx]))(contrasts)
 
@@ -580,41 +580,41 @@
     :param trials:
     :return:
     """
 
     signed_contrast = get_signed_contrast(trials)
     contrasts_fit = np.arange(-100, 100)
 
-    prob_right_50, contrasts, _ = compute_performance(trials, signed_contrast=signed_contrast, block=0.5)
+    prob_right_50, contrasts_50, _ = compute_performance(trials, signed_contrast=signed_contrast, block=0.5)
     pars_50 = compute_psychometric(trials, signed_contrast=signed_contrast, block=0.5)
     prob_right_fit_50 = psy.erf_psycho_2gammas(pars_50, contrasts_fit)
 
-    prob_right_20, contrasts, _ = compute_performance(trials, signed_contrast=signed_contrast, block=0.2)
+    prob_right_20, contrasts_20, _ = compute_performance(trials, signed_contrast=signed_contrast, block=0.2)
     pars_20 = compute_psychometric(trials, signed_contrast=signed_contrast, block=0.2)
     prob_right_fit_20 = psy.erf_psycho_2gammas(pars_20, contrasts_fit)
 
-    prob_right_80, contrasts, _ = compute_performance(trials, signed_contrast=signed_contrast, block=0.8)
+    prob_right_80, contrasts_80, _ = compute_performance(trials, signed_contrast=signed_contrast, block=0.8)
     pars_80 = compute_psychometric(trials, signed_contrast=signed_contrast, block=0.8)
     prob_right_fit_80 = psy.erf_psycho_2gammas(pars_80, contrasts_fit)
 
     cmap = sns.diverging_palette(20, 220, n=3, center="dark")
 
     if not ax:
         fig, ax = plt.subplots(**kwargs)
     else:
         fig = plt.gcf()
 
     # TODO error bars
 
     fit_50 = ax.plot(contrasts_fit, prob_right_fit_50, color=cmap[1])
-    data_50 = ax.scatter(contrasts, prob_right_50, color=cmap[1])
+    data_50 = ax.scatter(contrasts_50, prob_right_50, color=cmap[1])
     fit_20 = ax.plot(contrasts_fit, prob_right_fit_20, color=cmap[0])
-    data_20 = ax.scatter(contrasts, prob_right_20, color=cmap[0])
+    data_20 = ax.scatter(contrasts_20, prob_right_20, color=cmap[0])
     fit_80 = ax.plot(contrasts_fit, prob_right_fit_80, color=cmap[2])
-    data_80 = ax.scatter(contrasts, prob_right_80, color=cmap[2])
+    data_80 = ax.scatter(contrasts_80, prob_right_80, color=cmap[2])
     ax.legend([fit_50[0], data_50, fit_20[0], data_20, fit_80[0], data_80],
               ['p_left=0.5 fit', 'p_left=0.5 data', 'p_left=0.2 fit', 'p_left=0.2 data', 'p_left=0.8 fit', 'p_left=0.8 data'],
               loc='upper left')
     ax.set_ylim(-0.05, 1.05)
     ax.set_ylabel('Probability choosing right')
     ax.set_xlabel('Contrasts')
     if title:
@@ -627,28 +627,28 @@
     """
     Function to plot reaction time against contrast a la datajoint webpage (inversed for some reason??)
     :param trials:
     :return:
     """
 
     signed_contrast = get_signed_contrast(trials)
-    reaction_50, contrasts, _ = compute_reaction_time(trials, signed_contrast=signed_contrast, block=0.5)
-    reaction_20, contrasts, _ = compute_reaction_time(trials, signed_contrast=signed_contrast, block=0.2)
-    reaction_80, contrasts, _ = compute_reaction_time(trials, signed_contrast=signed_contrast, block=0.8)
+    reaction_50, contrasts_50, _ = compute_reaction_time(trials, signed_contrast=signed_contrast, block=0.5)
+    reaction_20, contrasts_20, _ = compute_reaction_time(trials, signed_contrast=signed_contrast, block=0.2)
+    reaction_80, contrasts_80, _ = compute_reaction_time(trials, signed_contrast=signed_contrast, block=0.8)
 
     cmap = sns.diverging_palette(20, 220, n=3, center="dark")
 
     if not ax:
         fig, ax = plt.subplots(**kwargs)
     else:
         fig = plt.gcf()
 
-    data_50 = ax.plot(contrasts, reaction_50, '-o', color=cmap[1])
-    data_20 = ax.plot(contrasts, reaction_20, '-o', color=cmap[0])
-    data_80 = ax.plot(contrasts, reaction_80, '-o', color=cmap[2])
+    data_50 = ax.plot(contrasts_50, reaction_50, '-o', color=cmap[1])
+    data_20 = ax.plot(contrasts_20, reaction_20, '-o', color=cmap[0])
+    data_80 = ax.plot(contrasts_80, reaction_80, '-o', color=cmap[2])
 
     # TODO error bars
 
     ax.legend([data_50[0], data_20[0], data_80[0]],
               ['p_left=0.5 data', 'p_left=0.2 data', 'p_left=0.8 data'],
               loc='upper left')
     ax.set_ylabel('Reaction time (s)')
```

### Comparing `ibllib-2.9.0/brainbox/behavior/wheel.py` & `ibllib-2.9.1/brainbox/behavior/wheel.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/core.py` & `ibllib-2.9.1/brainbox/core.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/ephys_plots.py` & `ibllib-2.9.1/brainbox/ephys_plots.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/io/one.py` & `ibllib-2.9.1/brainbox/io/one.py`

 * *Files 6% similar despite different names*

```diff
@@ -266,14 +266,16 @@
         return _channels_alf2bunch(channels, brain_regions=brain_regions)
     else:
         return channels
 
 
 def _load_channel_locations_traj(eid, probe=None, one=None, revision=None, aligned=False,
                                  brain_atlas=None, return_source=False):
+    if not hasattr(one, 'alyx'):
+        return {}, None
     _logger.debug(f"trying to load from traj {probe}")
     channels = Bunch()
     brain_atlas = brain_atlas or AllenAtlas
     # need to find the collection bruh
     insertion = one.alyx.rest('insertions', 'list', session=eid, name=probe)[0]
     collection = _collection_filter_from_args(probe=probe)
     collections = one.list_collections(eid, filename='channels*', collection=collection,
@@ -412,14 +414,16 @@
     :param collection: name of the spike sorting collection to load - exclusive with spike sorter name ex: "alf/probe00"
     :param return_channels: (bool) defaults to False otherwise tries and load channels from disk
     :param brain_regions: ibllib.atlas.regions.BrainRegions object - will label acronyms if provided
     :param nested: if a single probe is required, do not output a dictionary with the probe name as key
     :param return_collection: (False) if True, will return the collection used to load
     :return: spikes, clusters, channels (dict of bunch, 1 bunch per probe)
     """
+    _logger.warning('Deprecation warning: brainbox.io.one.load_spike_sorting_fast will be removed in future versions.'
+                    'Use brainbox.io.one.SpikeSortingLoader instead')
     if collection is None:
         collection = _collection_filter_from_args(probe, spike_sorter)
     _logger.debug(f"load spike sorting with collection filter {collection}")
     kwargs = dict(eid=eid, one=one, collection=collection, revision=revision, dataset_types=dataset_types,
                   brain_regions=brain_regions)
     spikes, clusters, channels = _load_spike_sorting(**kwargs, return_channels=True)
     clusters = merge_clusters_channels(clusters, channels, keys_to_add_extra=None)
@@ -451,14 +455,16 @@
     :param dataset_types: additional spikes/clusters objects to add to the standard default list
     :param spike_sorter: name of the spike sorting you want to load (None for default)
     :param return_channels: (bool) defaults to False otherwise tries and load channels from disk
     :param brain_regions: ibllib.atlas.regions.BrainRegions object - will label acronyms if provided
     :param return_collection:(bool - False) if True, returns the collection for loading the data
     :return: spikes, clusters (dict of bunch, 1 bunch per probe)
     """
+    _logger.warning('Deprecation warning: brainbox.io.one.load_spike_sorting will be removed in future versions.'
+                    'Use brainbox.io.one.SpikeSortingLoader instead')
     collection = _collection_filter_from_args(probe, spike_sorter)
     _logger.debug(f"load spike sorting with collection filter {collection}")
     spikes, clusters = _load_spike_sorting(eid=eid, one=one, collection=collection, revision=revision,
                                            return_channels=False, dataset_types=dataset_types,
                                            brain_regions=brain_regions)
     if return_collection:
         return spikes, clusters, collection
@@ -502,14 +508,16 @@
         A dict with probe labels as keys, contains bunch(es) of cluster data, with keys
         ('channels', 'depths', 'metrics')
     channels : dict of one.alf.io.AlfBunch
         A dict with probe labels as keys, contains channel locations with keys ('acronym',
         'atlas_id', 'x', 'y', 'z').  Atlas IDs non-lateralized.
     """
     # --- Get spikes and clusters data
+    _logger.warning('Deprecation warning: brainbox.io.one.load_spike_sorting will be removed in future versions.'
+                    'Use brainbox.io.one.SpikeSortingLoader instead')
     one = one or ONE()
     brain_atlas = brain_atlas or AllenAtlas()
     spikes, clusters, collection = load_spike_sorting(
         eid, one=one, probe=probe, dataset_types=dataset_types, spike_sorter=spike_sorter, return_collection=True)
     # -- Get brain regions and assign to clusters
     channels = load_channel_locations(eid, one=one, probe=probe, aligned=aligned,
                                       brain_atlas=brain_atlas)
@@ -858,31 +866,39 @@
                                         brain_atlas=ba, speedy=True)
             xyz_channels = ephysalign.get_channel_locations(feature, track)
     return xyz_channels
 
 
 @dataclass
 class SpikeSortingLoader:
-    """Class for loading spike sorting"""
-    pid: str
+    """
+    Object that will load spike sorting data for a given probe insertion.
+
+
+    """
     one: ONE
-    atlas: None
-    # the following properties are the outcome of the post init funciton
+    atlas: None = None
+    pid: str = None
     eid: str = ''
+    pname: str = ''
+    # the following properties are the outcome of the post init funciton
     session_path: Path = ''
     collections: list = None
     datasets: list = None   # list of all datasets belonging to the sesion
     # the following properties are the outcome of a reading function
     files: dict = None
     collection: str = ''
     histology: str = ''  # 'alf', 'resolved', 'aligned' or 'traced'
     spike_sorting_path: Path = None
 
     def __post_init__(self):
-        self.eid, self.pname = self.one.pid2eid(self.pid)
+        if self.pid is not None:
+            self.eid, self.pname = self.one.pid2eid(self.pid)
+        if self.atlas is None:
+            self.atlas = AllenAtlas()
         self.session_path = self.one.eid2path(self.eid)
         self.collections = self.one.list_collections(
             self.eid, filename='spikes*', collection=f"alf/{self.pname}*")
         self.datasets = self.one.list_datasets(self.eid)
         self.files = {}
 
     @staticmethod
@@ -905,40 +921,69 @@
         collection = next(filter(lambda c: c == f'alf/{self.pname}/{spike_sorter}', self.collections), None)
         # otherwise, prefers the shortest
         collection = collection or next(iter(sorted(filter(lambda c: f'alf/{self.pname}' in c, self.collections), key=len)), None)
         _logger.debug(f"selecting: {collection} to load amongst candidates: {self.collections}")
         return collection
 
     def _download_spike_sorting_object(self, obj, spike_sorter='pykilosort', dataset_types=None):
+        """
+        Downloads an ALF object
+        :param obj: object name, str between 'spikes', 'clusters' or 'channels'
+        :param spike_sorter: (defaults to 'pykilosort')
+        :param dataset_types: list of extra dataset types
+        :return:
+        """
         if len(self.collections) == 0:
             return {}, {}, {}
         self.collection = self._get_spike_sorting_collection(spike_sorter=spike_sorter)
+        _logger.debug(f"loading spike sorting from {self.collection}")
         spike_attributes, cluster_attributes = self._get_attributes(dataset_types)
         attributes = {'spikes': spike_attributes, 'clusters': cluster_attributes, 'channels': None}
         self.files[obj] = self.one.load_object(self.eid, obj=obj, attribute=attributes[obj],
                                                collection=self.collection, download_only=True)
 
     def download_spike_sorting(self, **kwargs):
-        """spike_sorter='pykilosort', dataset_types=None"""
+        """
+        Downloads spikes, clusters and channels
+        :param spike_sorter: (defaults to 'pykilosort')
+        :param dataset_types: list of extra dataset types
+        :return:
+        """
         for obj in ['spikes', 'clusters', 'channels']:
             self._download_spike_sorting_object(obj=obj, **kwargs)
         self.spike_sorting_path = self.files['spikes'][0].parent
 
     def load_spike_sorting(self, **kwargs):
-        """spike_sorter='pykilosort', dataset_types=None"""
+        """
+        Loads spikes, clusters and channels
+
+        There could be several spike sorting collections, by default the loader will get the pykilosort collection
+
+        The channel locations can come from several sources, it will load the most advanced version of the histology available,
+        regardless of the spike sorting version loaded. The steps are (from most advanced to fresh out of the imaging):
+        -   alf: the final version of channel locations, same as resolved with the difference that data is on file
+        -   resolved: channel locations alignments have been agreed upon
+        -   aligned: channel locations have been aligned, but review or other alignments are pending, potentially not accurate
+        -   traced: the histology track has been recovered from microscopy, however the depths may not match, inacurate data
+
+        :param spike_sorter: (defaults to 'pykilosort')
+        :param dataset_types: list of extra dataset types
+        :return:
+        """
         if len(self.collections) == 0:
             return {}, {}, {}
         self.download_spike_sorting(**kwargs)
         channels = alfio.load_object(self.files['channels'], wildcards=self.one.wildcards)
         clusters = alfio.load_object(self.files['clusters'], wildcards=self.one.wildcards)
         spikes = alfio.load_object(self.files['spikes'], wildcards=self.one.wildcards)
         if 'brainLocationIds_ccf_2017' not in channels:
-            channels, self.histology = _load_channel_locations_traj(
+            _channels, self.histology = _load_channel_locations_traj(
                 self.eid, probe=self.pname, one=self.one, brain_atlas=self.atlas, return_source=True)
-            channels = channels[self.pname]
+            if _channels:
+                channels = _channels[self.pname]
         else:
             channels = _channels_alf2bunch(channels, brain_regions=self.atlas.regions)
             self.histology = 'alf'
         return spikes, clusters, channels
 
     @staticmethod
     def merge_clusters(spikes, clusters, channels, cache_dir=None):
```

### Comparing `ibllib-2.9.0/brainbox/io/spikeglx.py` & `ibllib-2.9.1/brainbox/io/spikeglx.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/lfp.py` & `ibllib-2.9.1/brainbox/lfp.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/metrics/electrode_drift.py` & `ibllib-2.9.1/brainbox/metrics/electrode_drift.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/metrics/single_units.py` & `ibllib-2.9.1/brainbox/metrics/single_units.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/modeling/design_matrix.py` & `ibllib-2.9.1/brainbox/modeling/design_matrix.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/modeling/linear.py` & `ibllib-2.9.1/brainbox/modeling/linear.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/modeling/neural_model.py` & `ibllib-2.9.1/brainbox/modeling/neural_model.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/modeling/poisson.py` & `ibllib-2.9.1/brainbox/modeling/poisson.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/modeling/utils.py` & `ibllib-2.9.1/brainbox/modeling/utils.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/plot.py` & `ibllib-2.9.1/brainbox/plot.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/plot_base.py` & `ibllib-2.9.1/brainbox/plot_base.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/population/cca.py` & `ibllib-2.9.1/brainbox/population/cca.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/population/decode.py` & `ibllib-2.9.1/brainbox/population/decode.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/processing.py` & `ibllib-2.9.1/brainbox/processing.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/quality/lfp_qc.py` & `ibllib-2.9.1/brainbox/quality/lfp_qc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/quality/permutation_test.py` & `ibllib-2.9.1/brainbox/quality/permutation_test.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/singlecell.py` & `ibllib-2.9.1/brainbox/singlecell.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/spike_features.py` & `ibllib-2.9.1/brainbox/spike_features.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/task/_knockoff.py` & `ibllib-2.9.1/brainbox/task/_knockoff.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/task/_statsmodels.py` & `ibllib-2.9.1/brainbox/task/_statsmodels.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/task/closed_loop.py` & `ibllib-2.9.1/brainbox/task/closed_loop.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/task/passive.py` & `ibllib-2.9.1/brainbox/task/passive.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/task/trials.py` & `ibllib-2.9.1/brainbox/task/trials.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/fixtures/design_matrix_test.npy` & `ibllib-2.9.1/brainbox/tests/fixtures/design_matrix_test.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/fixtures/design_wheel_traces_test.p` & `ibllib-2.9.1/brainbox/tests/fixtures/design_wheel_traces_test.p`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/fixtures/ephys_test.p` & `ibllib-2.9.1/brainbox/tests/fixtures/ephys_test.p`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/fixtures/parquet_records.json` & `ibllib-2.9.1/brainbox/tests/fixtures/parquet_records.json`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/fixtures/trials_df_test.csv` & `ibllib-2.9.1/brainbox/tests/fixtures/trials_df_test.csv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/fixtures/trials_test.pickle` & `ibllib-2.9.1/brainbox/tests/fixtures/trials_test.pickle`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/fixtures/wheel_test.p` & `ibllib-2.9.1/brainbox/tests/fixtures/wheel_test.p`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_behavior.py` & `ibllib-2.9.1/brainbox/tests/test_behavior.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_cca.py` & `ibllib-2.9.1/brainbox/tests/test_cca.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_io.py` & `ibllib-2.9.1/brainbox/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_metrics.py` & `ibllib-2.9.1/brainbox/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_modeling.py` & `ibllib-2.9.1/brainbox/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_passive.py` & `ibllib-2.9.1/brainbox/tests/test_passive.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_plot_base.py` & `ibllib-2.9.1/brainbox/tests/test_plot_base.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_population.py` & `ibllib-2.9.1/brainbox/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_processing.py` & `ibllib-2.9.1/brainbox/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_singlecell.py` & `ibllib-2.9.1/brainbox/tests/test_singlecell.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_task.py` & `ibllib-2.9.1/brainbox/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_trials.py` & `ibllib-2.9.1/brainbox/tests/test_trials.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/tests/test_video.py` & `ibllib-2.9.1/brainbox/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/brainbox/video.py` & `ibllib-2.9.1/brainbox/video.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/examples/one/docs_one_queries.py` & `ibllib-2.9.1/examples/one/docs_one_queries.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/examples/one/one_queries.py` & `ibllib-2.9.1/examples/one/one_queries.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/__init__.py` & `ibllib-2.9.1/ibllib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.9.0"
+__version__ = "2.9.1"
 import warnings
 
 from ibllib.misc import logger_config
 
 warnings.filterwarnings("always", category=DeprecationWarning, module="ibllib")
 
 # if this becomes a full-blown library we should let the logging configuration to the discretion of the dev
```

### Comparing `ibllib-2.9.0/ibllib/atlas/allen_structure_tree.csv` & `ibllib-2.9.1/ibllib/atlas/allen_structure_tree.csv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/atlas/atlas.py` & `ibllib-2.9.1/ibllib/atlas/atlas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
 import logging
 import matplotlib.pyplot as plt
 from pathlib import Path, PurePosixPath
-from functools import lru_cache
 import numpy as np
 import nrrd
 
 from iblutil.numerical import ismember
 from ibllib.atlas.regions import BrainRegions
 from one.webclient import http_download_file
 import one.params
@@ -117,15 +116,15 @@
     def i2y(self, ind):
         return ind * self.dy + self.y0
 
     def i2z(self, ind):
         return ind * self.dz + self.z0
 
     def i2xyz(self, iii):
-        iii = np.array(iii)
+        iii = np.array(iii, dtype=float)
         out = np.zeros_like(iii)
         out[..., 0] = self.i2x(iii[..., 0])
         out[..., 1] = self.i2y(iii[..., 1])
         out[..., 2] = self.i2z(iii[..., 2])
         return out
 
     """Methods bounds"""
@@ -180,44 +179,71 @@
         self.image: image volume (ap, ml, dv)
         self.label: label volume (ap, ml, dv)
         self.bc: atlas.BrainCoordinate object
         self.regions: atlas.BrainRegions object
         self.top: 2d np array (ap, ml) containing the z-coordinate (m) of the surface of the brain
         self.dims2xyz and self.zyz2dims: map image axis order to xyz coordinates order
         """
+
         self.image = image
         self.label = label
         self.regions = regions
         self.dims2xyz = dims2xyz
         self.xyz2dims = xyz2dims
         assert(np.all(self.dims2xyz[self.xyz2dims] == np.array([0, 1, 2])))
         assert(np.all(self.xyz2dims[self.dims2xyz] == np.array([0, 1, 2])))
         # create the coordinate transform object that maps volume indices to real world coordinates
         nxyz = np.array(self.image.shape)[self.dims2xyz]
         bc = BrainCoordinates(nxyz=nxyz, xyz0=(0, 0, 0), dxyz=dxyz)
         self.bc = BrainCoordinates(nxyz=nxyz, xyz0=- bc.i2xyz(iorigin), dxyz=dxyz)
 
+        self.surface = None
+        self.boundary = None
+
+    def compute_surface(self):
         """
         Get the volume top, bottom, left and right surfaces, and from these the outer surface of
         the image volume. This is needed to compute probe insertions intersections
         """
-        axz = self.xyz2dims[2]  # this is the dv axis
-        _surface = (self.label == 0).astype(np.int8) * 2
-        l0 = np.diff(_surface, axis=axz, append=2)
-        _top = np.argmax(l0 == -2, axis=axz).astype(float)
-        _top[_top == 0] = np.nan
-        _bottom = self.bc.nz - np.argmax(np.flip(l0, axis=axz) == 2, axis=axz).astype(float)
-        _bottom[_bottom == self.bc.nz] = np.nan
-        self.top = self.bc.i2z(_top + 1)
-        self.bottom = self.bc.i2z(_bottom - 1)
-        self.surface = np.diff(_surface, axis=self.xyz2dims[0], append=2) + l0
-        idx_srf = np.where(self.surface != 0)
-        self.surface[idx_srf] = 1
-        self.srf_xyz = self.bc.i2xyz(np.c_[idx_srf[self.xyz2dims[0]], idx_srf[self.xyz2dims[1]],
-                                           idx_srf[self.xyz2dims[2]]].astype(float))
+        if self.surface is None:  # only compute if it hasn't already been computed
+            axz = self.xyz2dims[2]  # this is the dv axis
+            _surface = (self.label == 0).astype(np.int8) * 2
+            l0 = np.diff(_surface, axis=axz, append=2)
+            _top = np.argmax(l0 == -2, axis=axz).astype(float)
+            _top[_top == 0] = np.nan
+            _bottom = self.bc.nz - np.argmax(np.flip(l0, axis=axz) == 2, axis=axz).astype(float)
+            _bottom[_bottom == self.bc.nz] = np.nan
+            self.top = self.bc.i2z(_top + 1)
+            self.bottom = self.bc.i2z(_bottom - 1)
+            self.surface = np.diff(_surface, axis=self.xyz2dims[0], append=2) + l0
+            idx_srf = np.where(self.surface != 0)
+            self.surface[idx_srf] = 1
+            self.srf_xyz = self.bc.i2xyz(np.c_[idx_srf[self.xyz2dims[0]], idx_srf[self.xyz2dims[1]],
+                                               idx_srf[self.xyz2dims[2]]].astype(float))
+
+    def compute_boundaries(self):
+        """
+        Compute the boundaries between regions
+        """
+        if self.boundary is None:  # only compute if it hasn't already been computed
+            self.boundary = np.diff(self.label, axis=0, append=0)
+            self.boundary = self.boundary + np.diff(self.label, axis=1, append=0)
+            self.boundary = self.boundary + np.diff(self.label, axis=2, append=0)
+            self.boundary[self.boundary != 0] = 1
+
+            # Compute boundary on top view
+            self.compute_surface()
+            ix, iy = np.meshgrid(np.arange(self.bc.nx), np.arange(self.bc.ny))
+            iz = self.bc.z2i(self.top)
+            inds = self._lookup_inds(np.stack((ix, iy, iz), axis=-1))
+            vals = np.random.random(self.regions.acronym.shape[0])
+            _top_boundary = vals[self.label.flat[inds]]
+            self.top_boundary = np.diff(_top_boundary, axis=0, append=0)
+            self.top_boundary = self.top_boundary + np.diff(_top_boundary, axis=1, append=0)
+            self.top_boundary[self.top_boundary != 0] = 1
 
     def _lookup_inds(self, ixyz):
         """
         Performs a 3D lookup from volume indices ixyz to the image volume
         :param ixyz: [n, 3] array of indices in the mlapdv order
         :return: n array of flat indices
         """
@@ -370,35 +396,47 @@
         """
         :param axis: direction along which the volume is stacked:
          (2 = z for horizontal slice)
          (1 = y for coronal slice)
          (0 = x for sagittal slice)
         :return:
         """
+
         if axis == 0:
             extent = np.r_[self.bc.ylim, np.flip(self.bc.zlim)] * 1e6
         elif axis == 1:
             extent = np.r_[self.bc.xlim, np.flip(self.bc.zlim)] * 1e6
         elif axis == 2:
             extent = np.r_[self.bc.xlim, np.flip(self.bc.ylim)] * 1e6
         return extent
 
     def slice(self, coordinate, axis, volume='image', mode='raise', region_values=None,
               mapping="Allen", bc=None):
         """
-        :param coordinate: float
+        Get slice through atlas
+
+        :param coordinate: coordinate to slice in metres, float
         :param axis: xyz convention:  0 for ml, 1 for ap, 2 for dv
             - 0: sagittal slice (along ml axis)
             - 1: coronal slice (along ap axis)
             - 2: horizontal slice (along dv axis)
-        :param volume: 'image' or 'annotation'
+        :param volume:
+            - 'image' - allen image volume
+            - 'annotation' - allen annotation volume
+            - 'surface' - outer surface of mesh
+            - 'boundary' - outline of boundaries between all regions
+            - 'volume' - custom volume, must pass in volume of shape ba.image.shape as regions_value argument
+            - 'value' - custom value per allen region, must pass in array of shape ba.regions.id as regions_value argument
         :param mode: error mode for out of bounds coordinates
             -   'raise' raise an error
             -   'clip' gets the first or last index
-        :param region_values
+        :param region_values: custom values to plot
+            - if volume='volume', region_values must have shape ba.image.shape
+            - if volume='value', region_values must have shape ba.regions.id
+        :param mapping: mapping to use. Options can be found using ba.regions.mappings.keys()
         :return: 2d array or 3d RGB numpy int8 array
         """
         index = self.bc.xyz2i(np.array([coordinate] * 3))[axis]
 
         # np.take is 50 thousand times slower than straight slicing !
         def _take(vol, ind, axis):
             if mode == 'clip':
@@ -412,71 +450,146 @@
 
         def _take_remap(vol, ind, axis, mapping):
             # For the labels, remap the regions indices according to the mapping
             return self._get_mapping(mapping=mapping)[_take(vol, ind, axis)]
 
         if isinstance(volume, np.ndarray):
             return _take(volume, index, axis=self.xyz2dims[axis])
-        # add annotation_ids
-        # add annotation_indices
-        # rename annoatation_rgb ?
         elif volume in 'annotation':
             iregion = _take_remap(self.label, index, self.xyz2dims[axis], mapping)
             return self._label2rgb(iregion)
+        elif volume == 'image':
+            return _take(self.image, index, axis=self.xyz2dims[axis])
         elif volume == 'value':
             return region_values[_take_remap(self.label, index, self.xyz2dims[axis], mapping)]
         elif volume == 'image':
             return _take(self.image, index, axis=self.xyz2dims[axis])
         elif volume in ['surface', 'edges']:
+            self.compute_surface()
             return _take(self.surface, index, axis=self.xyz2dims[axis])
+        elif volume == 'boundary':
+            self.compute_boundaries()
+            return _take(self.boundary, index, axis=self.xyz2dims[axis])
         elif volume == 'volume':
             if bc is not None:
                 index = bc.xyz2i(np.array([coordinate] * 3))[axis]
             return _take(region_values, index, axis=self.xyz2dims[axis])
 
     def plot_cslice(self, ap_coordinate, volume='image', mapping='Allen', region_values=None, **kwargs):
         """
-        Imshow a coronal slice
+        Plot coronal slice through atlas at given ap_coordinate
+
         :param: ap_coordinate (m)
-        :param volume: 'image' or 'annotation'
-        :return: ax
+        :param volume:
+            - 'image' - allen image volume
+            - 'annotation' - allen annotation volume
+            - 'surface' - outer surface of mesh
+            - 'boundary' - outline of boundaries between all regions
+            - 'volume' - custom volume, must pass in volume of shape ba.image.shape as regions_value argument
+            - 'value' - custom value per allen region, must pass in array of shape ba.regions.id as regions_value argument
+        :param mapping: mapping to use. Options can be found using ba.regions.mappings.keys()
+        :param region_values: custom values to plot
+            - if volume='volume', region_values must have shape ba.image.shape
+            - if volume='value', region_values must have shape ba.regions.id
+        :param mapping: mapping to use. Options can be found using ba.regions.mappings.keys()
+        :param **kwargs: matplotlib.pyplot.imshow kwarg arguments
+        :return: matplotlib ax object
         """
+
         cslice = self.slice(ap_coordinate, axis=1, volume=volume, mapping=mapping, region_values=region_values)
         return self._plot_slice(cslice.T, extent=self.extent(axis=1), **kwargs)
 
     def plot_hslice(self, dv_coordinate, volume='image', mapping='Allen', region_values=None, **kwargs):
         """
-        Imshow a horizontal slice
+        Plot horizontal slice through atlas at given dv_coordinate
+
         :param: dv_coordinate (m)
-        :param volume: 'image' or 'annotation'
-        :return: ax
+        :param volume:
+            - 'image' - allen image volume
+            - 'annotation' - allen annotation volume
+            - 'surface' - outer surface of mesh
+            - 'boundary' - outline of boundaries between all regions
+            - 'volume' - custom volume, must pass in volume of shape ba.image.shape as regions_value argument
+            - 'value' - custom value per allen region, must pass in array of shape ba.regions.id as regions_value argument
+        :param mapping: mapping to use. Options can be found using ba.regions.mappings.keys()
+        :param region_values: custom values to plot
+            - if volume='volume', region_values must have shape ba.image.shape
+            - if volume='value', region_values must have shape ba.regions.id
+        :param mapping: mapping to use. Options can be found using ba.regions.mappings.keys()
+        :param **kwargs: matplotlib.pyplot.imshow kwarg arguments
+        :return: matplotlib ax object
         """
+
         hslice = self.slice(dv_coordinate, axis=2, volume=volume, mapping=mapping, region_values=region_values)
         return self._plot_slice(hslice, extent=self.extent(axis=2), **kwargs)
 
     def plot_sslice(self, ml_coordinate, volume='image', mapping='Allen', region_values=None, **kwargs):
         """
-        Imshow a sagittal slice
+        Plot sagittal slice through atlas at given ml_coordinate
+
         :param: ml_coordinate (m)
-        :param volume: 'image' or 'annotation'
-        :return: ax
+        :param volume:
+            - 'image' - allen image volume
+            - 'annotation' - allen annotation volume
+            - 'surface' - outer surface of mesh
+            - 'boundary' - outline of boundaries between all regions
+            - 'volume' - custom volume, must pass in volume of shape ba.image.shape as regions_value argument
+            - 'value' - custom value per allen region, must pass in array of shape ba.regions.id as regions_value argument
+        :param mapping: mapping to use. Options can be found using ba.regions.mappings.keys()
+        :param region_values: custom values to plot
+            - if volume='volume', region_values must have shape ba.image.shape
+            - if volume='value', region_values must have shape ba.regions.id
+        :param mapping: mapping to use. Options can be found using ba.regions.mappings.keys()
+        :param **kwargs: matplotlib.pyplot.imshow kwarg arguments
+        :return: matplotlib ax object
         """
+
         sslice = self.slice(ml_coordinate, axis=0, volume=volume, mapping=mapping, region_values=region_values)
         return self._plot_slice(np.swapaxes(sslice, 0, 1), extent=self.extent(axis=0), **kwargs)
 
-    def plot_top(self, ax=None):
+    def plot_top(self, volume='annotation', mapping='Allen', region_values=None, ax=None, **kwargs):
+        """
+        Plot top view of atlas
+        :param volume:
+            - 'image' - allen image volume
+            - 'annotation' - allen annotation volume
+            - 'boundary' - outline of boundaries between all regions
+            - 'volume' - custom volume, must pass in volume of shape ba.image.shape as regions_value argument
+            - 'value' - custom value per allen region, must pass in array of shape ba.regions.id as regions_value argument
+
+        :param mapping: mapping to use. Options can be found using ba.regions.mappings.keys()
+        :param region_values:
+        :param ax:
+        :param kwargs:
+        :return:
+        """
+
+        self.compute_surface()
         ix, iy = np.meshgrid(np.arange(self.bc.nx), np.arange(self.bc.ny))
         iz = self.bc.z2i(self.top)
         inds = self._lookup_inds(np.stack((ix, iy, iz), axis=-1))
-        if not ax:
-            ax = plt.gca()
-            ax.axis('equal')
-        ax.imshow(self._label2rgb(self.label.flat[inds]),
-                  extent=self.extent(axis=2), origin='upper')
-        return ax
+
+        regions = self._get_mapping(mapping=mapping)[self.label.flat[inds]]
+
+        if volume == 'annotation':
+            im = self._label2rgb(regions)
+        elif volume == 'image':
+            im = self.top
+        elif volume == 'value':
+            im = region_values[regions]
+        elif volume == 'volume':
+            im = np.zeros((iz.shape))
+            for x in range(im.shape[0]):
+                for y in range(im.shape[1]):
+                    im[x, y] = region_values[x, y, iz[x, y]]
+        elif volume == 'boundary':
+            self.compute_boundaries()
+            im = self.top_boundary
+
+        return self._plot_slice(im, self.extent(axis=2), ax=ax, **kwargs)
 
 
 @dataclass
 class Trajectory:
     """
     3D Trajectory (usually for a linear probe). Minimally defined by a vector and a point.
     instantiate from a best fit from a n by 3 array containing xyz coordinates:
@@ -661,14 +774,16 @@
     @property
     def tip(self):
         return sph2cart(- self.depth, self.theta, self.phi) + np.array((self.x, self.y, self.z))
 
     @staticmethod
     def _get_surface_intersection(traj, brain_atlas, surface='top'):
 
+        brain_atlas.compute_surface()
+
         distance = traj.mindist(brain_atlas.srf_xyz)
         dist_sort = np.argsort(distance)
         # In some cases the nearest two intersection points are not the top and bottom of brain
         # So we find all intersection points that fall within one voxel and take the one with
         # highest dV to be entry and lowest dV to be exit
         idx_lim = np.sum(distance[dist_sort] * 1e6 < brain_atlas.res_um)
         dist_lim = dist_sort[0:idx_lim]
@@ -706,29 +821,29 @@
         :param brain_atlas:
         :return: 3 element array x,y,z
         """
         # Find point where trajectory intersects with top of brain
         return Insertion._get_surface_intersection(traj, brain_atlas, surface='top')
 
 
-@lru_cache(maxsize=1)
 class AllenAtlas(BrainAtlas):
     """
     Instantiates an atlas.BrainAtlas corresponding to the Allen CCF at the given resolution
     using the IBL Bregma and coordinate system
     """
 
     def __init__(self, res_um=25, scaling=np.array([1, 1, 1]), mock=False, hist_path=None):
         """
         :param res_um: 10, 25 or 50 um
         :param scaling: scale factor along ml, ap, dv for squeeze and stretch ([1, 1, 1])
         :param mock: for testing purpose
         :param hist_path
         :return: atlas.BrainAtlas
         """
+
         par = one.params.get(silent=True)
         FLAT_IRON_ATLAS_REL_PATH = PurePosixPath('histology', 'ATLAS', 'Needles', 'Allen')
         LUT_VERSION = "v01"  # version 01 is the lateralized version
         regions = BrainRegions()
         xyz2dims = np.array([1, 0, 2])  # this is the c-contiguous ordering
         dims2xyz = np.array([1, 0, 2])
         # we use Bregma as the origin
@@ -761,14 +876,15 @@
                 _, im = ismember(label, regions.id)
                 label = np.reshape(im.astype(np.uint16), label.shape)
                 _logger.info(f"saving {file_label_remap} ...")
                 np.savez_compressed(file_label_remap, label)
             # loads the files
             label = self._read_volume(file_label_remap)
             image = self._read_volume(file_image)
+
         super().__init__(image, label, dxyz, regions, ibregma,
                          dims2xyz=dims2xyz, xyz2dims=xyz2dims)
 
     @staticmethod
     def _read_volume(file_volume):
         if file_volume.suffix == '.nrrd':
             volume, _ = nrrd.read(file_volume, index_order='C')  # ml, dv, ap
@@ -796,15 +912,15 @@
         """
         Converts coordinates from the CCF coordinates, which is assumed to be the cube indices
         times the spacing.
         :param ccf coordinates in CCF space in um, origin is the front left top corner of the data
         volume
         :param ccf_order: order of ccf coordinates given 'mlapdv' (ibl) or 'apdvml'
         (Allen mcc vertices)
-        :return: xyz: mlapdv coordinates in um, origin Bregma
+        :return: xyz: mlapdv coordinates in m, origin Bregma
         """
         ordre = self._ccf_order(ccf_order, reverse=True)
         return self.bc.i2xyz((ccf[..., ordre] / float(self.res_um)))
 
     @staticmethod
     def _ccf_order(ccf_order, reverse=False):
         """
```

### Comparing `ibllib-2.9.0/ibllib/atlas/beryl.npy` & `ibllib-2.9.1/ibllib/atlas/beryl.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/atlas/regions.py` & `ibllib-2.9.1/ibllib/atlas/regions.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from iblutil.util import Bunch
 from iblutil.numerical import ismember
 
 _logger = logging.getLogger('ibllib')
 # 'Beryl' is the name given to an atlas containing a subset of the most relevant allen annotations
 FILE_BERYL = str(Path(__file__).parent.joinpath('beryl.npy'))
 FILE_COSMOS = str(Path(__file__).parent.joinpath('cosmos.npy'))
+FILE_MAPPINGS = str(Path(__file__).parent.joinpath('mappings.pqt'))
 FILE_REGIONS = str(Path(__file__).parent.joinpath('allen_structure_tree.csv'))
 
 
 @dataclass
 class _BrainRegions:
     id: np.ndarray
     name: object
@@ -29,16 +30,14 @@
     ibllib.atlas.regions.BrainRegions(brainmap='Allen')
     The Allen atlas ids are kept intact but lateralized as follows: labels are duplicated
      and ids multiplied by -1, with the understanding that left hemisphere regions have negative
      ids.
     """
     def __init__(self):
         df_regions = pd.read_csv(FILE_REGIONS)
-        beryl = np.load(FILE_BERYL)
-        cosmos = np.load(FILE_COSMOS)
         # lateralize
         df_regions_left = df_regions.iloc[np.array(df_regions.id > 0), :].copy()
         df_regions_left['id'] = - df_regions_left['id']
         df_regions_left['parent_structure_id'] = - df_regions_left['parent_structure_id']
         df_regions_left['name'] = df_regions_left['name'].apply(lambda x: x + ' (left)')
         df_regions = pd.concat((df_regions, df_regions_left), axis=0)
         # converts colors to RGB uint8 array
@@ -50,22 +49,35 @@
         super().__init__(id=df_regions.id.to_numpy(),
                          name=df_regions.name.to_numpy(),
                          acronym=df_regions.acronym.to_numpy(),
                          rgb=c,
                          level=df_regions.depth.to_numpy(),
                          parent=df_regions.parent_structure_id.to_numpy())
         # mappings are indices not ids: they range from 0 to n regions -1
+        mappings = pd.read_parquet(FILE_MAPPINGS)
+        self.mappings = {k: mappings[k].to_numpy() for k in mappings}
+
+    def _compute_mappings(self):
+        """
+        Recomputes the mapping indices for all mappings
+        This is left mainly as a reference for adding future mappings as this take a few seconds
+        to execute. In production,we use the MAPPING_FILES npz to avoid recompuing at each \
+        instantiation
+        """
+        beryl = np.load(FILE_BERYL)
+        cosmos = np.load(FILE_COSMOS)
         self.mappings = {
             'Allen': self._mapping_from_regions_list(np.unique(np.abs(self.id)), lateralize=False),
             'Allen-lr': np.arange(self.id.size),
             'Beryl': self._mapping_from_regions_list(beryl, lateralize=False),
             'Beryl-lr': self._mapping_from_regions_list(beryl, lateralize=True),
             'Cosmos': self._mapping_from_regions_list(cosmos, lateralize=False),
             'Cosmos-lr': self._mapping_from_regions_list(cosmos, lateralize=True),
         }
+        pd.DataFrame(self.mappings).to_parquet(FILE_MAPPINGS)
 
     def get(self, ids) -> Bunch:
         """
         Get a bunch of the name/id
         """
         uid, uind = np.unique(ids, return_inverse=True)
         a, iself, _ = np.intersect1d(self.id, uid, assume_unique=False, return_indices=True)
```

### Comparing `ibllib-2.9.0/ibllib/dsp/cadzow.py` & `ibllib-2.9.1/ibllib/dsp/cadzow.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/dsp/fourier.py` & `ibllib-2.9.1/ibllib/dsp/fourier.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/dsp/savitzky_golay.py` & `ibllib-2.9.1/ibllib/dsp/savitzky_golay.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/dsp/smooth.py` & `ibllib-2.9.1/ibllib/dsp/smooth.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/dsp/utils.py` & `ibllib-2.9.1/ibllib/dsp/utils.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/dsp/voltage.py` & `ibllib-2.9.1/ibllib/dsp/voltage.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/ephys/ephysqc.py` & `ibllib-2.9.1/ibllib/ephys/ephysqc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/ephys/neuropixel.py` & `ibllib-2.9.1/ibllib/ephys/neuropixel.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/ephys/np2_converter.py` & `ibllib-2.9.1/ibllib/ephys/np2_converter.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/ephys/spikes.py` & `ibllib-2.9.1/ibllib/ephys/spikes.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/ephys/sync_probes.py` & `ibllib-2.9.1/ibllib/ephys/sync_probes.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/exceptions.py` & `ibllib-2.9.1/ibllib/exceptions.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/graphic.py` & `ibllib-2.9.1/ibllib/graphic.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/certification_protocol.py` & `ibllib-2.9.1/ibllib/io/certification_protocol.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/base.py` & `ibllib-2.9.1/ibllib/io/extractors/base.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/biased_trials.py` & `ibllib-2.9.1/ibllib/io/extractors/biased_trials.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/bpod_trials.py` & `ibllib-2.9.1/ibllib/io/extractors/bpod_trials.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/camera.py` & `ibllib-2.9.1/ibllib/io/extractors/camera.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_fpga.py` & `ibllib-2.9.1/ibllib/io/extractors/ephys_fpga.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_passive.py` & `ibllib-2.9.1/ibllib/io/extractors/ephys_passive.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/passive_stim_meta.json` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/passive_stim_meta.json`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_0_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_0_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_0_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_0_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_0_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_0_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_0_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_0_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_0_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_0_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_10_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_10_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_10_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_10_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_10_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_10_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_10_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_10_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_10_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_10_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_11_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_11_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_11_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_11_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_11_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_11_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_11_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_11_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_11_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_11_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_1_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_1_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_1_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_1_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_1_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_1_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_1_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_1_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_1_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_1_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_2_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_2_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_2_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_2_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_2_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_2_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_2_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_2_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_2_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_2_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_3_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_3_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_3_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_3_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_3_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_3_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_3_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_3_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_3_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_3_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_4_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_4_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_4_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_4_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_4_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_4_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_4_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_4_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_4_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_4_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_5_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_5_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_5_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_5_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_5_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_5_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_5_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_5_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_5_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_5_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_6_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_6_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_6_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_6_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_6_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_6_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_6_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_6_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_6_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_6_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_7_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_7_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_7_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_7_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_7_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_7_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_7_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_7_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_7_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_7_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_8_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_8_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_8_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_8_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_8_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_8_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_8_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_8_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_8_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_8_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_9_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_9_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_9_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_9_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_9_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_9_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_9_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_9_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_9_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_9_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_mock_ephys_pcqs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_mock_ephys_pcqs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_mock_passive_pcs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_mock_passive_pcs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_mock_passive_stimDelays.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_mock_passive_stimDelays.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_mock_passive_stimIDs.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_mock_passive_stimIDs.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/ephys_sessions/session_mock_stim_phase.npy` & `ibllib-2.9.1/ibllib/io/extractors/ephys_sessions/session_mock_stim_phase.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/extractor_types.json` & `ibllib-2.9.1/ibllib/io/extractors/extractor_types.json`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/habituation_trials.py` & `ibllib-2.9.1/ibllib/io/extractors/habituation_trials.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/opto_trials.py` & `ibllib-2.9.1/ibllib/io/extractors/opto_trials.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/passive_plotting.py` & `ibllib-2.9.1/ibllib/io/extractors/passive_plotting.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/signatures.py` & `ibllib-2.9.1/ibllib/io/extractors/signatures.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/training_audio.py` & `ibllib-2.9.1/ibllib/io/extractors/training_audio.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/training_trials.py` & `ibllib-2.9.1/ibllib/io/extractors/training_trials.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/training_wheel.py` & `ibllib-2.9.1/ibllib/io/extractors/training_wheel.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/extractors/video_motion.py` & `ibllib-2.9.1/ibllib/io/extractors/video_motion.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/ffmpeg.py` & `ibllib-2.9.1/ibllib/io/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/flags.py` & `ibllib-2.9.1/ibllib/io/flags.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/globus.py` & `ibllib-2.9.1/ibllib/io/globus.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/misc.py` & `ibllib-2.9.1/ibllib/io/misc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/npy_header.py` & `ibllib-2.9.1/ibllib/io/npy_header.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/raw_data_loaders.py` & `ibllib-2.9.1/ibllib/io/raw_data_loaders.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/spikeglx.py` & `ibllib-2.9.1/ibllib/io/spikeglx.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/io/video.py` & `ibllib-2.9.1/ibllib/io/video.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/misc/misc.py` & `ibllib-2.9.1/ibllib/misc/misc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/misc/timing.py` & `ibllib-2.9.1/ibllib/misc/timing.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/misc/version.py` & `ibllib-2.9.1/ibllib/misc/version.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/oneibl/aws.py` & `ibllib-2.9.1/ibllib/oneibl/aws.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/oneibl/data_handlers.py` & `ibllib-2.9.1/ibllib/oneibl/data_handlers.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/oneibl/patcher.py` & `ibllib-2.9.1/ibllib/oneibl/patcher.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/oneibl/registration.py` & `ibllib-2.9.1/ibllib/oneibl/registration.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/oneibl/stream.py` & `ibllib-2.9.1/ibllib/oneibl/stream.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/pipes/ephys_alignment.py` & `ibllib-2.9.1/ibllib/pipes/ephys_alignment.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/pipes/ephys_preprocessing.py` & `ibllib-2.9.1/ibllib/pipes/ephys_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/pipes/histology.py` & `ibllib-2.9.1/ibllib/pipes/histology.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/pipes/local_server.py` & `ibllib-2.9.1/ibllib/pipes/local_server.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/pipes/misc.py` & `ibllib-2.9.1/ibllib/pipes/misc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/pipes/purge_rig_data.py` & `ibllib-2.9.1/ibllib/pipes/purge_rig_data.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/pipes/remote_server.py` & `ibllib-2.9.1/ibllib/pipes/remote_server.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/pipes/scan_fix_passive_files.py` & `ibllib-2.9.1/ibllib/pipes/scan_fix_passive_files.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/pipes/tasks.py` & `ibllib-2.9.1/ibllib/pipes/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,19 +83,21 @@
         if use_alyx:
             tdict = self.one.alyx.rest('tasks', 'partial_update', id=self.taskid,
                                        data={'status': 'Started'})
             self.log = ('' if not tdict['log'] else tdict['log'] +
                         '\n\n=============================RERUN=============================\n')
 
         # Setup the console handler with a StringIO object
+        logger_level = _logger.level
         log_capture_string = io.StringIO()
         ch = logging.StreamHandler(log_capture_string)
         str_format = '%(asctime)s,%(msecs)d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s'
         ch.setFormatter(logging.Formatter(str_format))
         _logger.addHandler(ch)
+        _logger.setLevel(logging.INFO)
         _logger.info(f"Starting job {self.__class__}")
         if self.machine:
             _logger.info(f"Running on machine: {self.machine}")
         _logger.info(f"running ibllib version {version.ibllib()}")
         # setup
         start_time = time.time()
         try:
@@ -121,15 +123,14 @@
                 _logger.info(f"Job {self.__class__} complete")
         except Exception:
             _logger.error(traceback.format_exc())
             _logger.info(f"Job {self.__class__} errored")
             self.status = -1
 
         self.time_elapsed_secs = time.time() - start_time
-
         # log the outputs
         if isinstance(self.outputs, list):
             nout = len(self.outputs)
         elif self.outputs is None:
             nout = 0
         else:
             nout = 1
@@ -137,14 +138,15 @@
         _logger.info(f"N outputs: {nout}")
         _logger.info(f"--- {self.time_elapsed_secs} seconds run-time ---")
         # after the run, capture the log output, amend to any existing logs if not overwrite
         new_log = log_capture_string.getvalue()
         self.log = new_log if self.clobber else self.log + new_log
         log_capture_string.close()
         _logger.removeHandler(ch)
+        _logger.setLevel(logger_level)
         # tear down
         self.tearDown()
         return self.status
 
     def register_datasets(self, one=None, **kwargs):
         """
         Register output datasets form the task to Alyx
```

### Comparing `ibllib-2.9.0/ibllib/pipes/training_preprocessing.py` & `ibllib-2.9.1/ibllib/pipes/training_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/pipes/transfer_rig_data.py` & `ibllib-2.9.1/ibllib/pipes/transfer_rig_data.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/plots/figures.py` & `ibllib-2.9.1/ibllib/plots/figures.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from ibllib.io.video import get_video_frame, url_from_eid
 from brainbox.plot import driftmap
 from brainbox.behavior.dlc import SAMPLING, plot_trace_on_frame, plot_wheel_position, plot_lick_hist, \
     plot_lick_raster, plot_motion_energy_hist, plot_speed_hist, plot_pupil_diameter_hist
 from brainbox.ephys_plots import image_lfp_spectrum_plot, image_rms_plot, plot_brain_regions
 from brainbox.io.one import load_spike_sorting_fast
 from brainbox.behavior import training
+from iblutil.numerical import ismember
 
 
 logger = logging.getLogger('ibllib')
 
 
 def set_axis_label_size(ax, labels=14, ticklabels=12, title=14, cmap=False):
     """
@@ -65,15 +66,21 @@
 
 
 class BehaviourPlots(ReportSnapshot):
     """
     Behavioural plots
     """
 
-    signature = {'input_files': [('*trials*', 'alf', True)],
+    signature = {'input_files': [('*trials.contrastLeft.npy', 'alf', True),
+                                 ('*trials.contrastRight.npy', 'alf', True),
+                                 ('*trials.feedbackType.npy', 'alf', True),
+                                 ('*trials.probabilityLeft.npy', 'alf', True),
+                                 ('*trials.choice.npy', 'alf', True),
+                                 ('*trials.response_times.npy', 'alf', True),
+                                 ('*trials.stimOn_times.npy', 'alf', True)],
                  'output_files': [('psychometric_curve.png', 'snapshot/behaviour', True),
                                   ('chronometric_curve.png', 'snapshot/behaviour', True),
                                   ('reaction_time_with_trials.png', 'snapshot/behaviour', True)]
                  }
 
     def __init__(self, eid, session_path=None, one=None, **kwargs):
         self.one = one or ONE()
@@ -122,15 +129,15 @@
 
     def _run(self):
 
         assert self.pid
         assert self.brain_atlas
 
         output_files = []
-
+        self.histology_status = self.get_histology_status()
         electrodes = self.get_channels('electrodeSites', f'alf/{self.pname}')
 
         if self.hist_lookup[self.histology_status] > 0:
             fig = plt.figure(figsize=(12, 9))
             gs = fig.add_gridspec(2, 2, width_ratios=[.95, .05])
             ax1 = fig.add_subplot(gs[0, 0])
             self.brain_atlas.plot_tilted_slice(electrodes['mlapdv'], 1, ax=ax1)
@@ -386,33 +393,48 @@
                             ('raw_ephys_bad_channels_difference.png', f'snapshot/{pname}', True),
                             ]
         self.signature = {'input_files': input_signature, 'output_files': output_signature}
 
     def _run(self):
         """runs for initiated PID, streams data, destripe and check bad channels"""
         assert self.pid
+        self.eqcs = []
+        if self.location != 'server':
+            self.histology_status = self.get_histology_status()
+            electrodes = self.get_channels('electrodeSites', f'alf/{self.pname}')
+
+            if 'atlas_id' in electrodes.keys():
+                electrodes['ibr'] = ismember(electrodes['atlas_id'], self.brain_regions.id)[1]
+                electrodes['acronym'] = self.brain_regions.acronym[electrodes['ibr']]
+                electrodes['name'] = self.brain_regions.name[electrodes['ibr']]
+            else:
+                electrodes = None
+        else:
+            electrodes = None
+
         SNAPSHOT_LABEL = "raw_ephys_bad_channels"
         eid, pname = self.one.pid2eid(self.pid)
         output_files = list(self.output_directory.glob(f'{SNAPSHOT_LABEL}*'))
         if len(output_files) == 4:
             return output_files
         self.output_directory.mkdir(exist_ok=True, parents=True)
         from brainbox.io.spikeglx import stream
         T0 = 60 * 30
         sr, t0 = stream(self.pid, T0, nsecs=1, one=self.one)
         raw = sr[:, :-sr.nsync].T
         channel_labels, channel_features = voltage.detect_bad_channels(raw, sr.fs)
-        _, _, output_files = ephys_bad_channels(
-            raw=raw, fs=sr.fs, channel_labels=channel_labels, channel_features=channel_features,
-            title=SNAPSHOT_LABEL, destripe=True, save_dir=self.output_directory)
+        _, eqcs, output_files = ephys_bad_channels(
+            raw=raw, fs=sr.fs, channel_labels=channel_labels, channel_features=channel_features, channels=electrodes,
+            title=SNAPSHOT_LABEL, destripe=True, save_dir=self.output_directory, br=self.brain_regions)
+        self.eqcs = eqcs
         return output_files
 
 
-def ephys_bad_channels(raw, fs, channel_labels, channel_features, title="ephys_bad_channels", save_dir=None,
-                       destripe=False, eqcs=None):
+def ephys_bad_channels(raw, fs, channel_labels, channel_features, channels=None, title="ephys_bad_channels", save_dir=None,
+                       destripe=False, eqcs=None, br=None):
     nc, ns = raw.shape
     rl = ns / fs
     if fs >= 2600:  # AP band
         ylim_rms = [0, 100]
         ylim_psd_hf = [0, 0.1]
         eqc_xrange = [450, 500]
         butter_kwargs = {'N': 3, 'Wn': 300 / fs * 2, 'btype': 'highpass'}
@@ -424,26 +446,27 @@
         eqc_xrange = [450, 950]
         butter_kwargs = {'N': 3, 'Wn': np.array([2, 125]) / fs * 2, 'btype': 'bandpass'}
         eqc_gain = - 78
 
     inoisy = np.where(channel_labels == 2)[0]
     idead = np.where(channel_labels == 1)[0]
     ioutside = np.where(channel_labels == 3)[0]
-    from easyqc.gui import viewseis
+    from viewspikes.gui import viewephys
 
     # display voltage traces
     eqcs = [] if eqcs is None else eqcs
     # butterworth, for display only
     sos = scipy.signal.butter(**butter_kwargs, output='sos')
     butt = scipy.signal.sosfiltfilt(sos, raw)
-    eqcs.append(viewseis(butt.T, si=1 / fs * 1e3, title='highpass', taxis=0))
+    eqcs.append(viewephys(butt, fs=fs, channels=channels, title='highpass', br=br))
     if destripe:
         dest = voltage.destripe(raw, fs=fs, channel_labels=channel_labels)
-        eqcs.append(viewseis(dest.T, si=1 / fs * 1e3, title='destripe', taxis=0))
-        eqcs.append(viewseis((butt - dest).T, si=1 / fs * 1e3, title='difference', taxis=0))
+        eqcs.append(viewephys(dest, fs=fs, channels=channels, title='destripe', br=br))
+        eqcs.append(viewephys((butt - dest), fs=fs, channels=channels, title='difference', br=br))
+
     for eqc in eqcs:
         y, x = np.meshgrid(ioutside, np.linspace(0, rl * 1e3, 500))
         eqc.ctrl.add_scatter(x.flatten(), y.flatten(), rgb=(164, 142, 35), label='outside')
         y, x = np.meshgrid(inoisy, np.linspace(0, rl * 1e3, 500))
         eqc.ctrl.add_scatter(x.flatten(), y.flatten(), rgb=(255, 0, 0), label='noisy')
         y, x = np.meshgrid(idead, np.linspace(0, rl * 1e3, 500))
         eqc.ctrl.add_scatter(x.flatten(), y.flatten(), rgb=(0, 0, 255), label='dead')
```

### Comparing `ibllib-2.9.0/ibllib/plots/misc.py` & `ibllib-2.9.1/ibllib/plots/misc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/plots/snapshot.py` & `ibllib-2.9.1/ibllib/plots/snapshot.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/qc/alignment_qc.py` & `ibllib-2.9.1/ibllib/qc/alignment_qc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/qc/base.py` & `ibllib-2.9.1/ibllib/qc/base.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/qc/camera.py` & `ibllib-2.9.1/ibllib/qc/camera.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/qc/critical_reasons.py` & `ibllib-2.9.1/ibllib/qc/critical_reasons.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/qc/dlc.py` & `ibllib-2.9.1/ibllib/qc/dlc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/qc/qcplots.py` & `ibllib-2.9.1/ibllib/qc/qcplots.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/qc/reference/frames_body.npy` & `ibllib-2.9.1/ibllib/qc/reference/frames_body.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/qc/reference/frames_left.npy` & `ibllib-2.9.1/ibllib/qc/reference/frames_left.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/qc/reference/frames_right.npy` & `ibllib-2.9.1/ibllib/qc/reference/frames_right.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/qc/task_extractors.py` & `ibllib-2.9.1/ibllib/qc/task_extractors.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/qc/task_metrics.py` & `ibllib-2.9.1/ibllib/qc/task_metrics.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_ambientSensorData.raw.jsonable` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_ambientSensorData.raw.jsonable`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_encoderTrialInfo.raw.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_encoderTrialInfo.raw.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_taskData.raw.jsonable` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_taskData.raw.jsonable`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_taskSettings.raw.json` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_ge5/raw_behavior_data/_iblrig_taskSettings.raw.json`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_encoderEvents.raw.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_encoderEvents.raw.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_taskData.raw.jsonable` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_taskData.raw.jsonable`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_taskSettings.raw.json` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_biased_lt5/raw_behavior_data/_iblrig_taskSettings.raw.json`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_encoderEvents.raw.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_encoderEvents.raw.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_encoderPositions.raw.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_encoderPositions.raw.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_encoderTrialInfo.raw.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_encoderTrialInfo.raw.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskCodeFiles.raw.zip` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskCodeFiles.raw.zip`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskData.raw.jsonable` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskData.raw.jsonable`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskDataCodeFiles.raw.zip` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskDataCodeFiles.raw.zip`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskSettings.raw.json` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_behavior_data/_iblrig_taskSettings.raw.json`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_video_data/_iblrig_bodyCamera.frame_counter.bin` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_video_data/_iblrig_bodyCamera.frame_counter.bin`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_ephys/raw_video_data/_iblrig_bodyCamera.timestamps.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_ephys/raw_video_data/_iblrig_bodyCamera.timestamps.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_ambientSensorData.raw.jsonable` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_ambientSensorData.raw.jsonable`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_encoderTrialInfo.raw.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_encoderTrialInfo.raw.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_taskData.raw.jsonable` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_taskData.raw.jsonable`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_taskSettings.raw.json` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_training_ge5/raw_behavior_data/_iblrig_taskSettings.raw.json`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_encoderEvents.raw.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_encoderEvents.raw.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_encoderPositions.raw.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_taskData.raw.jsonable` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_taskData.raw.jsonable`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_taskSettings.raw.json` & `ibllib-2.9.1/ibllib/tests/extractors/data/session_training_lt5/raw_behavior_data/_iblrig_taskSettings.raw.json`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderEvents.raw.00.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderEvents.raw.00.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderEvents.raw.CorruptMiddle.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderEvents.raw.CorruptMiddle.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderPositions.raw.00.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderPositions.raw.00.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderPositions.raw.01.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderPositions.raw.01.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderPositions.raw.2firstsamples.ssv` & `ibllib-2.9.1/ibllib/tests/extractors/data/wheel/lt5/_iblrig_encoderPositions.raw.2firstsamples.ssv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/test_ephys_fpga.py` & `ibllib-2.9.1/ibllib/tests/extractors/test_ephys_fpga.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/test_ephys_passive.py` & `ibllib-2.9.1/ibllib/tests/extractors/test_ephys_passive.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/test_ephys_trials.py` & `ibllib-2.9.1/ibllib/tests/extractors/test_ephys_trials.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/extractors/test_extractors.py` & `ibllib-2.9.1/ibllib/tests/extractors/test_extractors.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/ephysalignment/alignment_data.npz` & `ibllib-2.9.1/ibllib/tests/fixtures/ephysalignment/alignment_data.npz`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/histology/tracks/2019-12-04_KS014_001_probe00_pts.csv` & `ibllib-2.9.1/ibllib/tests/fixtures/histology/tracks/2019-12-04_KS014_001_probe00_pts.csv`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/io/data_loaders/_iblrig_test_mouse_2020-01-01_001/raw_video_data/_iblrig_leftCamera.frameData.bin` & `ibllib-2.9.1/ibllib/tests/fixtures/io/data_loaders/_iblrig_test_mouse_2020-01-01_001/raw_video_data/_iblrig_leftCamera.frameData.bin`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3A_g0_t0.imec.ap.meta` & `ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3A_g0_t0.imec.ap.meta`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3A_g0_t0.imec.lf.meta` & `ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3A_g0_t0.imec.lf.meta`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3A_short_g0_t0.imec.ap.meta` & `ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3A_short_g0_t0.imec.ap.meta`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3B2_exported.imec0.ap.meta` & `ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3B2_exported.imec0.ap.meta`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.imec1.ap.meta` & `ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.imec1.ap.meta`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.imec1.lf.meta` & `ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.imec1.lf.meta`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.nidq.meta` & `ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sample3B_g0_t0.nidq.meta`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sampleNP2.1_g0_t0.imec.ap.meta` & `ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sampleNP2.1_g0_t0.imec.ap.meta`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/io/spikeglx/sampleNP2.4_g0_t0.imec.ap.meta` & `ibllib-2.9.1/ibllib/tests/fixtures/io/spikeglx/sampleNP2.4_g0_t0.imec.ap.meta`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/qc/data_alignmentqc_existing.npz` & `ibllib-2.9.1/ibllib/tests/fixtures/qc/data_alignmentqc_existing.npz`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/qc/data_alignmentqc_manual.npz` & `ibllib-2.9.1/ibllib/tests/fixtures/qc/data_alignmentqc_manual.npz`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/qc/pupil_diameter.npy` & `ibllib-2.9.1/ibllib/tests/fixtures/qc/pupil_diameter.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/qc/wheel.npy` & `ibllib-2.9.1/ibllib/tests/fixtures/qc/wheel.npy`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/fixtures/utils.py` & `ibllib-2.9.1/ibllib/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/qc/test_alignment_qc.py` & `ibllib-2.9.1/ibllib/tests/qc/test_alignment_qc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/qc/test_base_qc.py` & `ibllib-2.9.1/ibllib/tests/qc/test_base_qc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/qc/test_camera_qc.py` & `ibllib-2.9.1/ibllib/tests/qc/test_camera_qc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/qc/test_critical_reasons.py` & `ibllib-2.9.1/ibllib/tests/qc/test_critical_reasons.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/qc/test_dlc_qc.py` & `ibllib-2.9.1/ibllib/tests/qc/test_dlc_qc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/qc/test_task_metrics.py` & `ibllib-2.9.1/ibllib/tests/qc/test_task_metrics.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/test_atlas.py` & `ibllib-2.9.1/ibllib/tests/test_atlas.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/test_dsp.py` & `ibllib-2.9.1/ibllib/tests/test_dsp.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/test_ephys.py` & `ibllib-2.9.1/ibllib/tests/test_ephys.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/test_histology.py` & `ibllib-2.9.1/ibllib/tests/test_histology.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/test_io.py` & `ibllib-2.9.1/ibllib/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/test_misc.py` & `ibllib-2.9.1/ibllib/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/test_oneibl.py` & `ibllib-2.9.1/ibllib/tests/test_oneibl.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/test_pipes.py` & `ibllib-2.9.1/ibllib/tests/test_pipes.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/test_plots.py` & `ibllib-2.9.1/ibllib/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/test_spikeglx.py` & `ibllib-2.9.1/ibllib/tests/test_spikeglx.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/tests/test_tasks.py` & `ibllib-2.9.1/ibllib/tests/test_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,22 +138,20 @@
         self.tasks = tasks
 
 
 class TestPipelineAlyx(unittest.TestCase):
 
     def setUp(self) -> None:
         self.td = tempfile.TemporaryDirectory()
-
-        ses = one.alyx.rest('sessions', 'list', subject=ses_dict['subject'],
-                            date_range=[ses_dict['start_time'][:10]] * 2,
-                            number=ses_dict['number'],
-                            no_cache=True)
-        if len(ses):
-            one.alyx.rest('sessions', 'delete', ses[0]['url'][-36:])
-
+        # ses = one.alyx.rest('sessions', 'list', subject=ses_dict['subject'],
+        #                     date_range=[ses_dict['start_time'][:10]] * 2,
+        #                     number=ses_dict['number'],
+        #                     no_cache=True)
+        # if len(ses):
+        #     one.alyx.rest('sessions', 'delete', ses[0]['url'][-36:])
         ses = one.alyx.rest('sessions', 'create', data=ses_dict)
         session_path = Path(self.td.name).joinpath(
             ses['subject'], ses['start_time'][:10], str(ses['number']).zfill(3))
         session_path.joinpath('alf').mkdir(exist_ok=True, parents=True)
         self.session_path = session_path
         self.eid = ses['url'][-36:]
```

### Comparing `ibllib-2.9.0/ibllib/tests/test_time.py` & `ibllib-2.9.1/ibllib/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib/time.py` & `ibllib-2.9.1/ibllib/time.py`

 * *Files identical despite different names*

### Comparing `ibllib-2.9.0/ibllib.egg-info/PKG-INFO` & `ibllib-2.9.1/ibllib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibllib
-Version: 2.9.0
+Version: 2.9.1
 Summary: IBL libraries
 Home-page: https://www.internationalbrainlab.com/
 Author: IBL Staff
 License: MIT
 Description: # IBL Python Libraries 
         [![Coverage badge](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fibllib.hooks.internationalbrainlab.org%2Fcoverage%2Fibllib%2Fmaster)](https://ibllib.hooks.internationalbrainlab.org/coverage/master) 
         [![Tests status badge](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fibllib.hooks.internationalbrainlab.org%2Ftests%2Fibllib%2Fmaster)](https://ibllib.hooks.internationalbrainlab.org/logs/records/master)
```

### Comparing `ibllib-2.9.0/ibllib.egg-info/SOURCES.txt` & `ibllib-2.9.1/ibllib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,17 @@
 ibllib.egg-info/requires.txt
 ibllib.egg-info/top_level.txt
 ibllib/atlas/__init__.py
 ibllib/atlas/allen_structure_tree.csv
 ibllib/atlas/atlas.py
 ibllib/atlas/beryl.npy
 ibllib/atlas/cosmos.npy
+ibllib/atlas/mappings.pqt
+ibllib/atlas/plots.py
+ibllib/atlas/projections.py
 ibllib/atlas/regions.py
 ibllib/dsp/__init__.py
 ibllib/dsp/cadzow.py
 ibllib/dsp/fourier.py
 ibllib/dsp/savitzky_golay.py
 ibllib/dsp/smooth.py
 ibllib/dsp/utils.py
```

### Comparing `ibllib-2.9.0/setup.py` & `ibllib-2.9.1/setup.py`

 * *Files identical despite different names*

