# Comparing `tmp/funmap-0.1.8.tar.gz` & `tmp/funmap-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/funmap-0.1.8.tar", last modified: Fri Apr 28 17:44:10 2023, max compression
+gzip compressed data, was "dist/funmap-0.1.9.tar", last modified: Tue May  2 15:08:25 2023, max compression
```

## Comparing `funmap-0.1.8.tar` & `funmap-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-04-28 17:44:10.000000 funmap-0.1.8/
--rw-r--r--   0 shiz       (501) staff       (20)      154 2022-12-19 18:14:17.000000 funmap-0.1.8/AUTHORS.rst
--rw-r--r--   0 shiz       (501) staff       (20)     3506 2022-12-19 18:14:17.000000 funmap-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 shiz       (501) staff       (20)       89 2022-12-19 18:14:17.000000 funmap-0.1.8/HISTORY.rst
--rw-r--r--   0 shiz       (501) staff       (20)     1068 2022-12-19 18:14:17.000000 funmap-0.1.8/LICENSE
--rw-r--r--   0 shiz       (501) staff       (20)      324 2022-12-20 21:45:22.000000 funmap-0.1.8/MANIFEST.in
--rw-r--r--   0 shiz       (501) staff       (20)      445 2023-04-28 17:44:10.000000 funmap-0.1.8/PKG-INFO
--rw-r--r--   0 shiz       (501) staff       (20)     2242 2023-04-28 17:31:56.000000 funmap-0.1.8/README.md
-drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap/
--rw-r--r--   0 shiz       (501) staff       (20)      122 2023-04-28 17:35:30.000000 funmap-0.1.8/funmap/__init__.py
--rw-r--r--   0 shiz       (501) staff       (20)    10866 2023-03-22 21:50:52.000000 funmap-0.1.8/funmap/cli.py
--rw-r--r--   0 shiz       (501) staff       (20)      689 2023-02-20 16:05:59.000000 funmap-0.1.8/funmap/data_urls.py
--rw-r--r--   0 shiz       (501) staff       (20)    39323 2023-03-20 19:49:55.000000 funmap-0.1.8/funmap/funmap.py
--rw-r--r--   0 shiz       (501) staff       (20)    32364 2023-03-22 21:50:52.000000 funmap-0.1.8/funmap/plotting.py
--rw-r--r--   0 shiz       (501) staff       (20)     9565 2023-03-22 21:50:52.000000 funmap-0.1.8/funmap/utils.py
-drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/
--rw-r--r--   0 shiz       (501) staff       (20)      445 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/PKG-INFO
--rw-r--r--   0 shiz       (501) staff       (20)      447 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/SOURCES.txt
--rw-r--r--   0 shiz       (501) staff       (20)        1 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/dependency_links.txt
--rw-r--r--   0 shiz       (501) staff       (20)       43 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/entry_points.txt
--rw-r--r--   0 shiz       (501) staff       (20)        1 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/not-zip-safe
--rw-r--r--   0 shiz       (501) staff       (20)      136 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/requires.txt
--rw-r--r--   0 shiz       (501) staff       (20)        7 2023-04-28 17:44:10.000000 funmap-0.1.8/funmap.egg-info/top_level.txt
--rw-r--r--   0 shiz       (501) staff       (20)      378 2023-04-28 17:44:10.000000 funmap-0.1.8/setup.cfg
--rw-r--r--   0 shiz       (501) staff       (20)     1169 2023-04-28 17:43:15.000000 funmap-0.1.8/setup.py
-drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-04-28 17:44:10.000000 funmap-0.1.8/tests/
--rw-r--r--   0 shiz       (501) staff       (20)  4123534 2023-04-28 16:40:03.000000 funmap-0.1.8/tests/aml_test.tgz
--rw-r--r--   0 shiz       (501) staff       (20)      932 2023-04-28 17:01:34.000000 funmap-0.1.8/tests/test_config.yaml
+drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-05-02 15:08:25.000000 funmap-0.1.9/
+-rw-r--r--   0 shiz       (501) staff       (20)      154 2022-12-19 18:14:17.000000 funmap-0.1.9/AUTHORS.rst
+-rw-r--r--   0 shiz       (501) staff       (20)     3506 2022-12-19 18:14:17.000000 funmap-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 shiz       (501) staff       (20)       89 2022-12-19 18:14:17.000000 funmap-0.1.9/HISTORY.rst
+-rw-r--r--   0 shiz       (501) staff       (20)     1068 2022-12-19 18:14:17.000000 funmap-0.1.9/LICENSE
+-rw-r--r--   0 shiz       (501) staff       (20)      324 2022-12-20 21:45:22.000000 funmap-0.1.9/MANIFEST.in
+-rw-r--r--   0 shiz       (501) staff       (20)      445 2023-05-02 15:08:25.000000 funmap-0.1.9/PKG-INFO
+-rw-r--r--   0 shiz       (501) staff       (20)     2133 2023-05-01 19:34:03.000000 funmap-0.1.9/README.md
+drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-05-02 15:08:25.000000 funmap-0.1.9/funmap/
+-rw-r--r--   0 shiz       (501) staff       (20)      122 2023-05-02 15:07:56.000000 funmap-0.1.9/funmap/__init__.py
+-rw-r--r--   0 shiz       (501) staff       (20)    10826 2023-05-02 15:07:28.000000 funmap-0.1.9/funmap/cli.py
+-rw-r--r--   0 shiz       (501) staff       (20)      689 2023-02-20 16:05:59.000000 funmap-0.1.9/funmap/data_urls.py
+-rw-r--r--   0 shiz       (501) staff       (20)    39323 2023-03-20 19:49:55.000000 funmap-0.1.9/funmap/funmap.py
+-rw-r--r--   0 shiz       (501) staff       (20)    32364 2023-03-22 21:50:52.000000 funmap-0.1.9/funmap/plotting.py
+-rw-r--r--   0 shiz       (501) staff       (20)     9565 2023-03-22 21:50:52.000000 funmap-0.1.9/funmap/utils.py
+drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-05-02 15:08:25.000000 funmap-0.1.9/funmap.egg-info/
+-rw-r--r--   0 shiz       (501) staff       (20)      445 2023-05-02 15:08:25.000000 funmap-0.1.9/funmap.egg-info/PKG-INFO
+-rw-r--r--   0 shiz       (501) staff       (20)      447 2023-05-02 15:08:25.000000 funmap-0.1.9/funmap.egg-info/SOURCES.txt
+-rw-r--r--   0 shiz       (501) staff       (20)        1 2023-05-02 15:08:25.000000 funmap-0.1.9/funmap.egg-info/dependency_links.txt
+-rw-r--r--   0 shiz       (501) staff       (20)       43 2023-05-02 15:08:25.000000 funmap-0.1.9/funmap.egg-info/entry_points.txt
+-rw-r--r--   0 shiz       (501) staff       (20)        1 2023-05-02 15:08:25.000000 funmap-0.1.9/funmap.egg-info/not-zip-safe
+-rw-r--r--   0 shiz       (501) staff       (20)      136 2023-05-02 15:08:25.000000 funmap-0.1.9/funmap.egg-info/requires.txt
+-rw-r--r--   0 shiz       (501) staff       (20)        7 2023-05-02 15:08:25.000000 funmap-0.1.9/funmap.egg-info/top_level.txt
+-rw-r--r--   0 shiz       (501) staff       (20)      378 2023-05-02 15:08:25.000000 funmap-0.1.9/setup.cfg
+-rw-r--r--   0 shiz       (501) staff       (20)     1169 2023-05-02 15:07:56.000000 funmap-0.1.9/setup.py
+drwxr-xr-x   0 shiz       (501) staff       (20)        0 2023-05-02 15:08:25.000000 funmap-0.1.9/tests/
+-rw-r--r--   0 shiz       (501) staff       (20)  4123534 2023-05-01 19:34:03.000000 funmap-0.1.9/tests/aml_test.tgz
+-rw-r--r--   0 shiz       (501) staff       (20)      883 2023-05-02 15:07:28.000000 funmap-0.1.9/tests/test_config.yaml
```

### Comparing `funmap-0.1.8/CONTRIBUTING.rst` & `funmap-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `funmap-0.1.8/LICENSE` & `funmap-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `funmap-0.1.8/README.md` & `funmap-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # funmap
-`funmap` integrates multiple omics data types (such as proteomics and RNASeq) to predict a functional network. The predicted network can provide insights into known and novel protein complexes, as well as identifying new somatic drivers and understudied proteins.
-
+`funmap` integrates multiple omics data sets (such as proteomics and RNASeq) to construct a functional network using supervised machine learning (xgboost).
 
 ## Installation
 
 ### Dependencies
 
 `funmap` requires the following:
```

### Comparing `funmap-0.1.8/funmap/cli.py` & `funmap-0.1.9/funmap/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 from funmap.utils import dict_hash
 from funmap.data_urls import misc_urls as urls
 from funmap import __version__
 
 # add option for user to specify results directory
 def arg_parse():
     parser = argparse.ArgumentParser(description='command line arguments.')
+    parser.add_argument('--qc-only', required=False, type=Path,
+                        help='if true, plot the data qc plots and quit, default: False')
     parser.add_argument('-c', '--config-file', required=True, type=Path,
                         help='path to experiment configuration yaml file')
     parser.add_argument('-d', '--data-file', required=True, type=Path,
                         help='path to tar gzipped data file')
     parser.add_argument('-o', '--output-dir', required=False, type=str,
-                        help='path to output directory')
+                        help='path to output directory, default: ./results')
     parser.add_argument('--version', action='version', version=f'{__version__}')
 
     args = parser.parse_args()
 
     return args
 
 
@@ -68,15 +70,15 @@
     # check if all files in data_files are in tar_files
     if not all(file['path'] in tar_files for file in data_files):
         print(f'Files listed under data_files are not in the tar.gz file!')
         raise ValueError('Files listed under data_files are not in the tar.gz file!')
 
     # separte cfg into two parts.
     model_cfg['seed'] = cfg_dict['seed'] if 'seed' in cfg_dict else 42
-    model_cfg['cor_type'] = 'spearman'
+    model_cfg['cor_type'] = 'pearson'
     model_cfg['split_by'] = 'edge'
     model_cfg['test_size'] = 0.5
     model_cfg['ml_type'] = 'xgboost'
     model_cfg['filter_before_prediction'] = True
     model_cfg['min_feature_count'] = 1
     model_cfg['min_sample_count'] = cfg_dict['min_sample_count'] \
                                     if 'min_sample_count' in cfg_dict else 20
@@ -121,28 +123,28 @@
     filter_blacklist = run_cfg['filter_blacklist']
     n_jobs = run_cfg['n_jobs']
     n_chunks = run_cfg['n_chunks']
     max_num_edges = run_cfg['max_num_edges']
     step_size = run_cfg['step_size']
 
     all_cfg = {**model_cfg, **data_cfg, **run_cfg}
-    # results will only be affected by model_cfg and data_cfg
-    res_cfg = {**model_cfg, **data_cfg}
-    if args.output_dir is None:
-        results_dir = Path('results')
-        hash_str = dict_hash(res_cfg)
-        results_dir = results_dir / f'results-{hash_str}'
-    else: # user specified output directory
-        results_dir = Path(args.output_dir)
+    results_dir = Path('results')
     data_dir = results_dir / 'saved_data'
     model_dir = results_dir / model_dir
     prediction_dir = results_dir / prediction_dir
     figure_dir = results_dir / 'figures'
     network_dir = results_dir / 'networks'
 
+    all_fig_names = []
+    fig_names = explore_data(data_cfg, args.data_file, min_sample_count, figure_dir)
+    all_fig_names.extend(fig_names)
+    if args.qc_only:
+        merge_and_delete(figure_dir, all_fig_names, 'all_figures.pdf')
+        return 0
+
     print(f'Output directory: {results_dir}')
     results_dir.mkdir(parents=True, exist_ok=True)
     data_dir.mkdir(parents=True, exist_ok=True)
     model_dir.mkdir(parents=True, exist_ok=True)
     prediction_dir.mkdir(parents=True, exist_ok=True)
     figure_dir.mkdir(parents=True, exist_ok=True)
     network_dir.mkdir(parents=True, exist_ok=True)
@@ -157,17 +159,14 @@
 
     llr_res_files = {feature: results_dir / f'llr_results_{feature}_{max_num_edges}.tsv'
                         for feature in feature_mapping }
     edge_list_paths = {feature: network_dir/ f'network_{feature}_{max_num_edges}.tsv'
                         for feature in feature_mapping }
     # llr obtained with each invividual dataset
     llr_dataset_file = results_dir / 'llr_dataset.tsv'
-    all_fig_names = []
-    fig_names = explore_data(data_cfg, args.data_file, min_sample_count, figure_dir)
-    all_fig_names.extend(fig_names)
     all_feature_df = None
     gs_train = gs_test_pos = gs_test_neg = None
 
     feature_args = {
         'data_dir': data_dir,
         'data_config': data_cfg,
         'data_file': args.data_file,
```

### Comparing `funmap-0.1.8/funmap/data_urls.py` & `funmap-0.1.9/funmap/data_urls.py`

 * *Files identical despite different names*

### Comparing `funmap-0.1.8/funmap/funmap.py` & `funmap-0.1.9/funmap/funmap.py`

 * *Files identical despite different names*

### Comparing `funmap-0.1.8/funmap/plotting.py` & `funmap-0.1.9/funmap/plotting.py`

 * *Files identical despite different names*

### Comparing `funmap-0.1.8/funmap/utils.py` & `funmap-0.1.9/funmap/utils.py`

 * *Files identical despite different names*

### Comparing `funmap-0.1.8/setup.py` & `funmap-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords=['funmap', 'bioinformatics', 'biological-network'],
     name='funmap',
     packages=find_packages(include=['funmap', 'funmap.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/bzhanglab/funmap',
-    version='0.1.8',
+    version='0.1.9',
     zip_safe=False,
 )
```

### Comparing `funmap-0.1.8/tests/aml_test.tgz` & `funmap-0.1.9/tests/aml_test.tgz`

 * *Files identical despite different names*

### Comparing `funmap-0.1.8/tests/test_config.yaml` & `funmap-0.1.9/tests/test_config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 seed: 42
-results_dir: results
 n_jobs: 8
 n_chunk: 4
 # minimum number of valid data point when computing correlation
 min_sample_count: 15
 # whether to output the edge list or not
 output_edgelist: True
 max_num_edges: 25000
 step_size: 1
 lr_cutoff: 10
 dataset_name: aml
 # path to the root directory of the data files
-data_root: 'tests/aml_test'
 data_files:
   - name: 'BeatAMl-T'
     type: 'rna'
     path: 'BeatAMl-T.tsv'
   - name: 'Blood2022-P-T'
     type: 'rna'
     path: 'Blood2022-P-T.tsv'
```

