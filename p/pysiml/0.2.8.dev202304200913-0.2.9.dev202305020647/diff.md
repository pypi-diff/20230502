# Comparing `tmp/pysiml-0.2.8.dev202304200913-py3-none-any.whl.zip` & `tmp/pysiml-0.2.9.dev202305020647-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 138987 bytes, number of entries: 92
--rw-r--r--  2.0 unx     1499 b- defN 80-Jan-01 00:00 pyproject.toml
+Zip file size: 151914 bytes, number of entries: 113
+-rw-r--r--  2.0 unx     1520 b- defN 80-Jan-01 00:00 pyproject.toml
 -rw-r--r--  2.0 unx      638 b- defN 80-Jan-01 00:00 siml/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 siml/__main__/__init__.py
--rw-r--r--  2.0 unx      970 b- defN 80-Jan-01 00:00 siml/__main__/convert_interim_data.py
+-rw-r--r--  2.0 unx      900 b- defN 80-Jan-01 00:00 siml/__main__/convert_interim_data.py
 -rw-r--r--  2.0 unx     1400 b- defN 80-Jan-01 00:00 siml/__main__/convert_raw_data.py
 -rw-r--r--  2.0 unx     1742 b- defN 80-Jan-01 00:00 siml/__main__/optimize.py
 -rw-r--r--  2.0 unx     8663 b- defN 80-Jan-01 00:00 siml/__main__/plot_losses.py
--rw-r--r--  2.0 unx      929 b- defN 80-Jan-01 00:00 siml/__main__/prepare_preprocess_converters.py
--rw-r--r--  2.0 unx      712 b- defN 80-Jan-01 00:00 siml/__main__/preprocess_interim_data.py
+-rw-r--r--  2.0 unx      927 b- defN 80-Jan-01 00:00 siml/__main__/prepare_preprocess_converters.py
+-rw-r--r--  2.0 unx      717 b- defN 80-Jan-01 00:00 siml/__main__/preprocess_interim_data.py
 -rw-r--r--  2.0 unx     1376 b- defN 80-Jan-01 00:00 siml/__main__/train.py
 -rw-r--r--  2.0 unx     3961 b- defN 80-Jan-01 00:00 siml/__main__/visualize_graph.py
 -rw-r--r--  2.0 unx       57 b- defN 80-Jan-01 00:00 siml/config.py
 -rw-r--r--  2.0 unx     3520 b- defN 80-Jan-01 00:00 siml/data_parallel.py
 -rw-r--r--  2.0 unx    26681 b- defN 80-Jan-01 00:00 siml/datasets.py
 -rw-r--r--  2.0 unx    27000 b- defN 80-Jan-01 00:00 siml/inferer.py
 -rw-r--r--  2.0 unx     1466 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_assignment.py
@@ -63,32 +63,53 @@
 -rw-r--r--  2.0 unx     3260 b- defN 80-Jan-01 00:00 siml/networks/tcn.py
 -rw-r--r--  2.0 unx     5969 b- defN 80-Jan-01 00:00 siml/networks/tensor_operations.py
 -rw-r--r--  2.0 unx     1415 b- defN 80-Jan-01 00:00 siml/networks/threshold.py
 -rw-r--r--  2.0 unx      782 b- defN 80-Jan-01 00:00 siml/networks/time_norm.py
 -rw-r--r--  2.0 unx     1882 b- defN 80-Jan-01 00:00 siml/networks/translator.py
 -rw-r--r--  2.0 unx     1034 b- defN 80-Jan-01 00:00 siml/networks/upper_limit.py
 -rw-r--r--  2.0 unx     6940 b- defN 80-Jan-01 00:00 siml/optimize.py
+-rw-r--r--  2.0 unx      125 b- defN 80-Jan-01 00:00 siml/path_like_objects/__init__.py
+-rw-r--r--  2.0 unx     1119 b- defN 80-Jan-01 00:00 siml/path_like_objects/siml_directory.py
+-rw-r--r--  2.0 unx     5982 b- defN 80-Jan-01 00:00 siml/path_like_objects/siml_file.py
 -rw-r--r--  2.0 unx     5523 b- defN 80-Jan-01 00:00 siml/postprocessor.py
--rw-r--r--  2.0 unx    45390 b- defN 80-Jan-01 00:00 siml/prepost.py
--rw-r--r--  2.0 unx       33 b- defN 80-Jan-01 00:00 siml/preprocessing/__init__.py
--rw-r--r--  2.0 unx    20676 b- defN 80-Jan-01 00:00 siml/preprocessing/converter.py
+-rw-r--r--  2.0 unx    25936 b- defN 80-Jan-01 00:00 siml/prepost.py
+-rw-r--r--  2.0 unx      148 b- defN 80-Jan-01 00:00 siml/preprocessing/__init__.py
+-rw-r--r--  2.0 unx    20772 b- defN 80-Jan-01 00:00 siml/preprocessing/converter.py
+-rw-r--r--  2.0 unx     9702 b- defN 80-Jan-01 00:00 siml/preprocessing/scalers_composition.py
+-rw-r--r--  2.0 unx    10594 b- defN 80-Jan-01 00:00 siml/preprocessing/scaling_converter.py
+-rw-r--r--  2.0 unx      176 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/__init__.py
+-rw-r--r--  2.0 unx     1405 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/__init__.py
+-rw-r--r--  2.0 unx      592 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/identity_scaler.py
+-rw-r--r--  2.0 unx      738 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/interface_scaler.py
+-rw-r--r--  2.0 unx     2038 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/isoam_scaler.py
+-rw-r--r--  2.0 unx     1403 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/max_abs_scaler.py
+-rw-r--r--  2.0 unx      465 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/min_max_scaler.py
+-rw-r--r--  2.0 unx     1926 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/sparse_standard_scaler.py
+-rw-r--r--  2.0 unx      570 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/standard_scaler.py
+-rw-r--r--  2.0 unx      865 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/user_defined_scaler.py
+-rw-r--r--  2.0 unx     1012 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scaler_result_save.py
+-rw-r--r--  2.0 unx     4326 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scaler_wrapper.py
 -rw-r--r--  2.0 unx    49064 b- defN 80-Jan-01 00:00 siml/setting.py
 -rw-r--r--  2.0 unx    11036 b- defN 80-Jan-01 00:00 siml/siml_manager.py
+-rw-r--r--  2.0 unx      147 b- defN 80-Jan-01 00:00 siml/siml_variables/__init__.py
+-rw-r--r--  2.0 unx      648 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/__init__.py
+-rw-r--r--  2.0 unx     1573 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/interface_wrapper.py
+-rw-r--r--  2.0 unx     1398 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/ndarray_wrapper.py
+-rw-r--r--  2.0 unx     1862 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/sparce_array_wrapper.py
+-rw-r--r--  2.0 unx     3509 b- defN 80-Jan-01 00:00 siml/siml_variables/tensor_variables/tensor_variables.py
 -rw-r--r--  2.0 unx    13021 b- defN 80-Jan-01 00:00 siml/study.py
--rw-r--r--  2.0 unx    34860 b- defN 80-Jan-01 00:00 siml/trainer.py
+-rw-r--r--  2.0 unx    34886 b- defN 80-Jan-01 00:00 siml/trainer.py
 -rw-r--r--  2.0 unx      211 b- defN 80-Jan-01 00:00 siml/update_functions/__init__.py
 -rw-r--r--  2.0 unx     1774 b- defN 80-Jan-01 00:00 siml/update_functions/element_batch_update.py
--rw-r--r--  2.0 unx     3590 b- defN 80-Jan-01 00:00 siml/update_functions/pseudo_batch_update.py
--rw-r--r--  2.0 unx     2669 b- defN 80-Jan-01 00:00 siml/update_functions/standard_update.py
+-rw-r--r--  2.0 unx     3623 b- defN 80-Jan-01 00:00 siml/update_functions/pseudo_batch_update.py
+-rw-r--r--  2.0 unx     2702 b- defN 80-Jan-01 00:00 siml/update_functions/standard_update.py
 -rw-r--r--  2.0 unx      429 b- defN 80-Jan-01 00:00 siml/update_functions/update_interface.py
--rw-r--r--  2.0 unx    37201 b- defN 80-Jan-01 00:00 siml/util.py
+-rw-r--r--  2.0 unx    23027 b- defN 80-Jan-01 00:00 siml/util.py
 -rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 siml/utils/__init__.py
 -rw-r--r--  2.0 unx     6090 b- defN 80-Jan-01 00:00 siml/utils/fem_data_utils.py
 -rw-r--r--  2.0 unx     2147 b- defN 80-Jan-01 00:00 siml/utils/path_utils.py
--rw-r--r--  2.0 unx       58 b- defN 80-Jan-01 00:00 siml/variables/__init__.py
--rw-r--r--  2.0 unx     3487 b- defN 80-Jan-01 00:00 siml/variables/siml_variables.py
-?rw-r--r--  2.0 unx      388 b- defN 16-Jan-01 00:00 pysiml-0.2.8.dev202304200913.dist-info/entry_points.txt
--rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.8.dev202304200913.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 pysiml-0.2.8.dev202304200913.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1595 b- defN 16-Jan-01 00:00 pysiml-0.2.8.dev202304200913.dist-info/METADATA
-?rw-r--r--  2.0 unx     7744 b- defN 16-Jan-01 00:00 pysiml-0.2.8.dev202304200913.dist-info/RECORD
-92 files, 534345 bytes uncompressed, 126837 bytes compressed:  76.3%
+-rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202305020647.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1638 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202305020647.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202305020647.dist-info/WHEEL
+-rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202305020647.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    10109 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202305020647.dist-info/RECORD
+113 files, 552017 bytes uncompressed, 135822 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -198,32 +198,101 @@
 
 Filename: siml/networks/upper_limit.py
 Comment: 
 
 Filename: siml/optimize.py
 Comment: 
 
+Filename: siml/path_like_objects/__init__.py
+Comment: 
+
+Filename: siml/path_like_objects/siml_directory.py
+Comment: 
+
+Filename: siml/path_like_objects/siml_file.py
+Comment: 
+
 Filename: siml/postprocessor.py
 Comment: 
 
 Filename: siml/prepost.py
 Comment: 
 
 Filename: siml/preprocessing/__init__.py
 Comment: 
 
 Filename: siml/preprocessing/converter.py
 Comment: 
 
+Filename: siml/preprocessing/scalers_composition.py
+Comment: 
+
+Filename: siml/preprocessing/scaling_converter.py
+Comment: 
+
+Filename: siml/preprocessing/siml_scalers/__init__.py
+Comment: 
+
+Filename: siml/preprocessing/siml_scalers/scale_functions/__init__.py
+Comment: 
+
+Filename: siml/preprocessing/siml_scalers/scale_functions/identity_scaler.py
+Comment: 
+
+Filename: siml/preprocessing/siml_scalers/scale_functions/interface_scaler.py
+Comment: 
+
+Filename: siml/preprocessing/siml_scalers/scale_functions/isoam_scaler.py
+Comment: 
+
+Filename: siml/preprocessing/siml_scalers/scale_functions/max_abs_scaler.py
+Comment: 
+
+Filename: siml/preprocessing/siml_scalers/scale_functions/min_max_scaler.py
+Comment: 
+
+Filename: siml/preprocessing/siml_scalers/scale_functions/sparse_standard_scaler.py
+Comment: 
+
+Filename: siml/preprocessing/siml_scalers/scale_functions/standard_scaler.py
+Comment: 
+
+Filename: siml/preprocessing/siml_scalers/scale_functions/user_defined_scaler.py
+Comment: 
+
+Filename: siml/preprocessing/siml_scalers/scaler_result_save.py
+Comment: 
+
+Filename: siml/preprocessing/siml_scalers/scaler_wrapper.py
+Comment: 
+
 Filename: siml/setting.py
 Comment: 
 
 Filename: siml/siml_manager.py
 Comment: 
 
+Filename: siml/siml_variables/__init__.py
+Comment: 
+
+Filename: siml/siml_variables/array_variables/__init__.py
+Comment: 
+
+Filename: siml/siml_variables/array_variables/interface_wrapper.py
+Comment: 
+
+Filename: siml/siml_variables/array_variables/ndarray_wrapper.py
+Comment: 
+
+Filename: siml/siml_variables/array_variables/sparce_array_wrapper.py
+Comment: 
+
+Filename: siml/siml_variables/tensor_variables/tensor_variables.py
+Comment: 
+
 Filename: siml/study.py
 Comment: 
 
 Filename: siml/trainer.py
 Comment: 
 
 Filename: siml/update_functions/__init__.py
@@ -249,29 +318,23 @@
 
 Filename: siml/utils/fem_data_utils.py
 Comment: 
 
 Filename: siml/utils/path_utils.py
 Comment: 
 
-Filename: siml/variables/__init__.py
-Comment: 
-
-Filename: siml/variables/siml_variables.py
-Comment: 
-
-Filename: pysiml-0.2.8.dev202304200913.dist-info/entry_points.txt
+Filename: pysiml-0.2.9.dev202305020647.dist-info/LICENSE
 Comment: 
 
-Filename: pysiml-0.2.8.dev202304200913.dist-info/LICENSE
+Filename: pysiml-0.2.9.dev202305020647.dist-info/METADATA
 Comment: 
 
-Filename: pysiml-0.2.8.dev202304200913.dist-info/WHEEL
+Filename: pysiml-0.2.9.dev202305020647.dist-info/WHEEL
 Comment: 
 
-Filename: pysiml-0.2.8.dev202304200913.dist-info/METADATA
+Filename: pysiml-0.2.9.dev202305020647.dist-info/entry_points.txt
 Comment: 
 
-Filename: pysiml-0.2.8.dev202304200913.dist-info/RECORD
+Filename: pysiml-0.2.9.dev202305020647.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyproject.toml

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysiml"
-version = "0.2.8.dev202304200913"
+version = "0.2.9.dev202305020647"
 description = "SiML - a Simulation ML library"
 license = "Apache-2.0"
 authors = ["RICOS Co. Ltd."]
 readme = "README.md"
 repository = "https://github.com/ricosjp/pysiml"
 documentation = "https://ricosjp.github.io/pysiml/"
 packages = [
@@ -25,14 +25,15 @@
 pydot = "^1.4.1"
 pytorch-ignite = "^0.3"
 sqlalchemy = "==1.3.13"
 PyQt5 = {version = "^5.14.0", optional = true}
 toml = "^0.10.2"
 torch = "^1.9.0"
 metis = "^0.2a5"
+pydantic = "^1.10.7"
 
 [tool.poetry.scripts]
 convert_interim_data = "siml.__main__.convert_interim_data:main"
 optimize = "siml.__main__.optimize:main"
 plot_losses = "siml.__main__.plot_losses:main"
 prepare_preprocess_converters = "siml.__main__.prepare_preprocess_converters:main"
 preprocess_interim_data = "siml.__main__.preprocess_interim_data:main"
```

## siml/__main__/convert_interim_data.py

```diff
@@ -20,16 +20,16 @@
     parser.add_argument(
         '-g', '--group-id',
         type=int,
         default=None,
         help='Group ID to preprocess variables partially [None]')
     args = parser.parse_args()
 
-    preprocessor = siml.prepost.Preprocessor.read_settings(
-        args.settings_yaml, force_renew=args.force_renew)
-    preprocessor.merge_dict_preprocessor_setting_pkls()
-    preprocessor.convert_interim_data(group_id=args.group_id)
+    preprocessor = siml.preprocessing.ScalingConverter.read_settings(
+        args.settings_yaml, force_renew=args.force_renew
+    )
+    preprocessor.fit_transform()
     print('success')
 
 
 if __name__ == '__main__':
     main()
```

## siml/__main__/prepare_preprocess_converters.py

```diff
@@ -20,17 +20,18 @@
     parser.add_argument(
         '-g', '--group-id',
         type=int,
         default=None,
         help='Group ID to preprocess variables partially [None]')
     args = parser.parse_args()
 
-    preprocessor = siml.prepost.Preprocessor.read_settings(
-        args.settings_yaml, force_renew=args.force_renew)
-    preprocessor.prepare_preprocess_converters(group_id=args.group_id)
+    preprocessor = siml.preprocessing.ScalingConverter.read_settings(
+        args.settings_yaml, force_renew=args.force_renew
+    )
+    preprocessor.lazy_fit_all(group_id=args.group_id)
 
     print('success')
     return
 
 
 if __name__ == '__main__':
     main()
```

## siml/__main__/preprocess_interim_data.py

```diff
@@ -15,17 +15,18 @@
     parser.add_argument(
         '-f', '--force-renew',
         type=strtobool,
         default=0,
         help='If True, overwrite existing data [False]')
     args = parser.parse_args()
 
-    preprocessor = siml.prepost.Preprocessor.read_settings(
-        args.settings_yaml, force_renew=args.force_renew)
-    preprocessor.preprocess_interim_data()
+    preprocessor = siml.preprocessing.ScalingConverter.read_settings(
+        args.settings_yaml, force_renew=args.force_renew
+    )
+    preprocessor.fit_transform()
 
     print('success')
     return
 
 
 if __name__ == '__main__':
     main()
```

## siml/prepost.py

```diff
@@ -1,24 +1,22 @@
 """Module for preprocessing."""
 
 import datetime as dt
-import glob
-import io
 import itertools as it
-import multiprocessing as multi
-import pickle
-from pathlib import Path
+from typing import Union
 
 import femio
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.sparse as sp
 
-from . import setting, util
-from siml.utils import fem_data_utils, path_utils
+from siml import util
+from siml.utils import fem_data_utils
+from siml.preprocessing import ScalersComposition
+from siml.siml_variables import ArrayDataType
 
 
 def add_difference(
         fem_data, dict_data, reference_dict_data, prefix='difference'):
     if reference_dict_data is None:
         return fem_data
     intersections = set(
@@ -66,15 +64,16 @@
     )
 
     return wrapped_data.fem_data
 
 
 def concatenate_preprocessed_data(
         preprocessed_base_directories, output_directory_base, variable_names,
-        *, ratios=(.9, .05, .05), overwrite=False):
+        *, ratios=(.9, .05, .05), overwrite=False,
+        finished_file='preprocessed'):
     """Concatenate preprocessed data in the element direction.
 
     NOTE: It may lead data leakage so it is just for research use.
 
     Parameters
     ----------
     preprocessed_base_directories: pathlib.Path or list[pathlib.Path]
@@ -89,15 +88,15 @@
     overwrite: bool, optional
         If True, overwrite output data.
     """
     if np.abs(np.sum(ratios) - 1.0) > 1e-5:
         raise ValueError('The sum of ratios does not make 1.')
     preprocessed_directories = util.collect_data_directories(
         preprocessed_base_directories,
-        required_file_names=Preprocessor.FINISHED_FILE)
+        required_file_names=finished_file)
     dict_data = {
         variable_name:
         np.concatenate([
             util.load_variable(preprocessed_directory, variable_name)
             for preprocessed_directory in preprocessed_directories])
         for variable_name in variable_names}
 
@@ -127,498 +126,38 @@
         if test_length > 0:
             np.save(
                 output_directory_base / f"validation/{variable_name}.npy",
                 data[indices[train_length+validation_length:]])
     return
 
 
-class Preprocessor:
-
-    REQUIRED_FILE_NAMES = ['converted']
-    FINISHED_FILE = 'preprocessed'
-    PREPROCESSORS_PKL_NAME = 'preprocessors.pkl'
-
-    @classmethod
-    def read_settings(cls, settings_yaml, **args):
-        main_setting = setting.MainSetting.read_settings_yaml(
-            settings_yaml, replace_preprocessed=False)
-        return cls(main_setting, **args)
-
-    def __init__(
-            self, main_setting, force_renew=False, save_func=None,
-            recursive=True,
-            str_replace='interim', max_process=None, allow_missing=False):
-        """Initialize preprocessor of interim data with preprocessing
-        e.g. standardization and then save them.
-
-        Parameters
-        ----------
-        force_renew: bool, optional
-            If True, renew npy files even if they are alerady exist.
-        recursive: bool, optional
-            If True, search data recursively.
-        save_func: callable, optional
-            Callback function to customize save data. It should accept
-            output_directory, variable_name, and transformed_data.
-        str_replace: str, optional
-            String to replace data directory in order to convert from interim
-            data to preprocessed data.
-        max_process: int, optional
-            The maximum number of processes.
-        allow_missing: bool, optional
-            If True, continue even if some of variables are missing.
-        """
-        self.setting = main_setting
-        self.recursive = recursive
-        self.force_renew = force_renew
-        self.save_func = save_func
-        if self.recursive:
-            self.interim_directories = util.collect_data_directories(
-                self.setting.data.interim,
-                required_file_names=self.REQUIRED_FILE_NAMES)
-        else:
-            self.interim_directories = self.setting.data.interim
-        self.str_replace = str_replace
-        self.max_process = util.determine_max_process(max_process)
-        self.allow_missing = allow_missing
-        if len(self.interim_directories) == 0:
-            raise ValueError(
-                'No converted data found. Perform conversion first.')
-        return
-
-    def preprocess_interim_data(self):
-        """Preprocess interim data.
-
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        dict_preprocessor_setting: dict
-            dict describing settings and parameters for preprocessors.
-        """
-        self.prepare_preprocess_converters()
-        dict_preprocessor_settings = \
-            self.merge_dict_preprocessor_setting_pkls()
-        self.convert_interim_data()
-        return dict_preprocessor_settings
-
-    def prepare_preprocess_converters(self, *, group_id=None):
-        """Prepare preprocess converters by reading data files lazily to
-        determine preprocessing parameters (like std and mean for
-        StandardScaler, min and max for MinMaxScaler.
-
-        Parameters
-        ----------
-        group_id: int, optional
-            group_id to specify chunk of preprocessing group. Useful when
-            MemoryError occurs with all variables preprocessed in one node.
-            If not specified, process all variables.
-
-        Returns
-        -------
-        dict_preprocessor_setting: dict
-            dict describing settings and parameters for preprocessors.
-        """
-        preprocessor_inputs = [
-            (variable_name, preprocess_setting)
-            for variable_name, preprocess_setting
-            in self.setting.preprocess.items()
-            if group_id is None or preprocess_setting['group_id'] == group_id]
-
-        with multi.Pool(self.max_process) as pool:
-            list_dict_preprocessor_setting = pool.starmap(
-                self.prepare_preprocess_converter, preprocessor_inputs,
-                chunksize=1)
-
-        dict_preprocessor_settings = {}
-        for dict_preprocessor_setting in list_dict_preprocessor_setting:
-            if dict_preprocessor_setting is not None:
-                dict_preprocessor_settings.update(dict_preprocessor_setting)
-        return dict_preprocessor_settings
-
-    def merge_dict_preprocessor_setting_pkls(self, data_directory=None):
-        """Merge variable-wise preprocessor settings pkl files into one file.
-
-        Parameters
-        ----------
-        data_directory: pathlib.Path, optional
-            Directory path contains variable-wise preprocessor settings pkl
-            files. If not fed, looking at self.setting.data.preprocessed_root .
-
-        Returns
-        -------
-        dict_preprocessor_setting: dict
-            dict describing settings and parameters for preprocessors after
-            merger.
-        """
-        if data_directory is None:
-            data_directory = self.setting.data.preprocessed_root
-        preprocessors_pkl_path = data_directory / self.PREPROCESSORS_PKL_NAME
-
-        if self.force_renew or not preprocessors_pkl_path.is_file():
-            pkl_files = glob.glob(
-                str(data_directory / f"*_{self.PREPROCESSORS_PKL_NAME}"))
-
-            dict_before_replacement = {}
-            for pkl_file in pkl_files:
-                with open(pkl_file, 'rb') as f:
-                    dict_before_replacement.update(pickle.load(f))
-
-            dict_preprocessor_settings = {
-                variable_name: self._collect_reference_dict_setting(
-                    variable_name, dict_before_replacement)
-                for variable_name in dict_before_replacement.keys()}
-
-            self.dump_preprocessors(
-                dict_preprocessor_settings, preprocessors_pkl_path)
-
-        else:
-            print(f"{preprocessors_pkl_path} already exists. Skip merger.")
-            with open(preprocessors_pkl_path, 'rb') as f:
-                dict_preprocessor_settings = pickle.load(f)
-
-        return dict_preprocessor_settings
-
-    def convert_interim_data(
-            self, preprocessor_pkl=None, *, group_id=None):
-        """Convert interim data with the determined preprocessor_settings.
-
-        Parameters
-        ----------
-        preprocessor_pkl: dict or pathlib.Path, optional
-            dict or pickle file path describing settings and parameters for
-            preprocessors. If not fed, data will be loaded from
-            self.setting.data.preprocessed_root.
-        group_id: int, optional
-            group_id to specify chunk of preprocessing group. Useful when
-            MemoryError occurs with all variables preprocessed in one node.
-            If not specified, process all variables.
-
-        Returns
-        -------
-        None
-        """
-
-        if preprocessor_pkl is None:
-            preprocessor_pkl = self.setting.data.preprocessed_root \
-                / self.PREPROCESSORS_PKL_NAME
-            if not preprocessor_pkl.is_file():
-                raise ValueError(f"{preprocessor_pkl} not found.")
-
-        if isinstance(preprocessor_pkl, Path):
-            with open(preprocessor_pkl, 'rb') as f:
-                dict_preprocessor_settings = pickle.load(f)
-        else:
-            dict_preprocessor_settings = preprocessor_pkl
-
-        preprocess_converter_inputs = \
-            self._generate_preprocess_converter_inputs(
-                dict_preprocessor_settings, group_id)
-        with multi.Pool(self.max_process) as pool:
-            pool.starmap(
-                self.transform_single_variable, preprocess_converter_inputs,
-                chunksize=1)
-
-        # Touch finished files
-        for data_directory in self.interim_directories:
-            output_directory = path_utils.determine_output_directory(
-                data_directory, self.setting.data.preprocessed_root,
-                self.str_replace)
-            (output_directory / self.FINISHED_FILE).touch()
-
-        yaml_file = self.setting.data.preprocessed_root / 'settings.yml'
-        if not yaml_file.exists():
-            setting.write_yaml(self.setting, yaml_file)
-
-        return
-
-    def _generate_preprocess_converter_inputs(
-            self, dict_preprocessor_settings, group_id):
-
-        preprocess_converter_inputs = [
-            (
-                variable_name,
-                self._collect_preprocess_converter_input(
-                    variable_name, dict_preprocessor_settings))
-            for variable_name, setting in self.setting.preprocess.items()
-            if group_id is None or setting['group_id'] == group_id]
-        return preprocess_converter_inputs
-
-    def _collect_preprocess_converter_input(
-            self, variable_name, dict_preprocessor_settings):
-
-        reference_dict = self._collect_reference_dict_setting(
-            variable_name, dict_preprocessor_settings)
-
-        preprocess_converter = util.PreprocessConverter(
-            reference_dict['preprocess_converter'],
-            method=reference_dict['method'],
-            componentwise=reference_dict['componentwise'],
-            power=reference_dict.get('power', 1.),
-            other_components=reference_dict['other_components'])
-        if preprocess_converter is None:
-            raise ValueError(f"Reference of {variable_name} is None")
-
-        return preprocess_converter
-
-    def _collect_reference_dict_setting(
-            self, variable_name, dict_preprocessor_settings):
-        if dict_preprocessor_settings[variable_name]['preprocess_converter'] \
-                is None:
-            value = dict_preprocessor_settings[variable_name]
-            reference_name = self.setting.preprocess[variable_name]['same_as']
-            if reference_name is None:
-                raise ValueError(
-                    f"Invalid setting for {variable_name}: {value}")
-            reference_dict = dict_preprocessor_settings[reference_name]
-
-        else:
-            reference_dict = dict_preprocessor_settings[
-                variable_name]
-
-        return reference_dict
-
-    def prepare_preprocess_converter(self, variable_name, preprocess_setting):
-        """Prepare preprocess converter for single variable.
-
-        Parameters
-        ----------
-        variable_name: str
-            The name of the variable.
-        preprocess_setting: dict
-            Dictionary of preprocess setting contains 'method' and
-            'componentwise' keywords.
-
-        Returns
-        -------
-        dict_preprocessor_setting: dict
-            Dict of preprocessor setting for the variable.
-        """
-        print(variable_name, preprocess_setting)
-
-        # Check if data already exists
-        pkl_file = self.setting.data.preprocessed_root \
-            / self.PREPROCESSORS_PKL_NAME
-        variable_pkl_file = self.setting.data.preprocessed_root \
-            / f"{variable_name}_{self.PREPROCESSORS_PKL_NAME}"
-        if not self.force_renew and (
-                pkl_file.exists() or variable_pkl_file.exists()):
-            print(
-                'Data already exists in '
-                f"{self.setting.data.preprocessed_root} for {variable_name}. "
-                'Skipped.')
-            return
-
-        # Prepare preprocessor
-        if (self.interim_directories[0] / (variable_name + '.npy')).exists():
-            ext = '.npy'
-        elif (
-                self.interim_directories[0]
-                / (variable_name + '.npy.enc')).exists():
-            ext = '.npy.enc'
-        elif (self.interim_directories[0] / (variable_name + '.npz')).exists():
-            ext = '.npz'
-        elif (
-                self.interim_directories[0]
-                / (variable_name + '.npz.enc')).exists():
-            ext = '.npz.enc'
-        else:
-            raise ValueError(
-                f"Unknown extension or file not found for {variable_name}")
-
-        if preprocess_setting['same_as'] is None:
-            if preprocess_setting['method'] == 'identity':
-                preprocess_converter = util.PreprocessConverter(
-                    'identity',
-                    componentwise=preprocess_setting['componentwise'],
-                    other_components=[],
-                    power=1., key=self.setting.data.encrypt_key)
-            else:
-                data_files = [
-                    data_directory / (variable_name + ext)
-                    for data_directory in self.interim_directories]
-                for other_component in preprocess_setting['other_components']:
-                    data_files += [
-                        data_directory / (other_component + ext)
-                        for data_directory in self.interim_directories]
-                preprocess_converter = util.PreprocessConverter(
-                    preprocess_setting['method'], data_files=data_files,
-                    componentwise=preprocess_setting['componentwise'],
-                    power=preprocess_setting['power'],
-                    other_components=preprocess_setting['other_components'],
-                    key=self.setting.data.encrypt_key)
-        else:
-            # same_as is set so no need to prepare preprocessor
-            preprocess_converter = None
-
-        dict_preprocessor_setting = {
-            variable_name: {
-                'method': preprocess_setting['method'],
-                'componentwise': preprocess_setting['componentwise'],
-                'preprocess_converter': preprocess_converter,
-                'power': preprocess_setting['power'],
-                'other_components': preprocess_setting['other_components'],
-            }}
-        if not self.setting.data.preprocessed_root.exists():
-            self.setting.data.preprocessed_root.mkdir(
-                parents=True, exist_ok=True)
-        partial_pkl_name = self.setting.data.preprocessed_root \
-            / f"{variable_name}_{self.PREPROCESSORS_PKL_NAME}"
-        self.dump_preprocessors(dict_preprocessor_setting, partial_pkl_name)
-
-        return dict_preprocessor_setting
-
-    def dump_preprocessors(self, dict_preprocessor_setting, file_path):
-        dict_to_dump = {}
-        for key, value in dict_preprocessor_setting.items():
-            dict_to_dump[key] = {}
-            for k, v in value.items():
-                if k == 'preprocess_converter' and v is not None:
-                    if isinstance(v, dict):
-                        dict_to_dump[key].update({k: v})
-                    else:
-                        dict_to_dump[key].update({k: vars(v.converter)})
-                else:
-                    dict_to_dump[key].update({k: v})
-        with open(file_path, 'wb') as f:
-            pickle.dump(dict_to_dump, f)
-
-        return
-
-    def _file_exists(self, output_directory, variable_name):
-        npy_file = output_directory / (variable_name + '.npy')
-        npy_enc_file = output_directory / (
-            variable_name + '.npy.enc')
-        npz_file = output_directory / (variable_name + '.npz')
-        npz_enc_file = output_directory / (
-            variable_name + '.npz.enc')
-        if npy_file.is_file():
-            return True
-        if npy_enc_file.is_file():
-            return True
-        if npz_file.is_file():
-            return True
-        if npz_enc_file.is_file():
-            return True
-        return False
-
-    def transform_single_variable(self, variable_name, preprocess_converter):
-        """Transform single variable with the created preprocess_converter.
-
-        Parameters
-        ----------
-        variable_name: str
-            The name of the variable.
-        preprocess_converter: siml.util.PreprocessConverter
-            The PreprocessConverter object to transform.
-
-        Returns
-        -------
-        None
-        """
-        if isinstance(preprocess_converter.converter, util.Identity):
-            # Shortcut preprocessing
-
-            for data_directory in self.interim_directories:
-                output_directory = path_utils.determine_output_directory(
-                    data_directory, self.setting.data.preprocessed_root,
-                    self.str_replace)
-                if not self.force_renew \
-                        and self._file_exists(output_directory, variable_name):
-                    print(
-                        f"{output_directory} / {variable_name} "
-                        'already exists. Skipped.')
-                    continue
-
-                util.copy_variable_file(
-                    data_directory, variable_name, output_directory,
-                    allow_missing=self.allow_missing)
-            return
-
-        for data_directory in self.interim_directories:
-            output_directory = path_utils.determine_output_directory(
-                data_directory, self.setting.data.preprocessed_root,
-                self.str_replace)
-            if not self.force_renew \
-                    and self._file_exists(output_directory, variable_name):
-                print(
-                    f"{output_directory} / {variable_name} "
-                    'already exists. Skipped.')
-                continue
-
-            loaded_data = util.load_variable(
-                data_directory, variable_name,
-                allow_missing=self.allow_missing,
-                decrypt_key=self.setting.data.encrypt_key)
-            if loaded_data is None:
-                continue
-            else:
-                transformed_data = preprocess_converter.transform(loaded_data)
-
-            if self.save_func is None:
-                util.save_variable(
-                    output_directory, variable_name, transformed_data,
-                    encrypt_key=self.setting.data.encrypt_key)
-            else:
-                self.save_func(
-                    output_directory, variable_name, transformed_data)
-
-        return
-
-
 class Converter:
 
     def __init__(self, converter_parameters_pkl, key=None):
-        self.converters = self._generate_converters(
-            converter_parameters_pkl, key=key)
-        return
-
-    def _generate_converters(self, converter_parameters_pkl, key=None):
-        if key is not None and converter_parameters_pkl.suffix == '.enc':
-            return self._generate_converters(
-                util.decrypt_file(key, converter_parameters_pkl))
-
-        if isinstance(converter_parameters_pkl, io.BufferedIOBase):
-            converter_parameters = pickle.load(converter_parameters_pkl)
-        elif isinstance(converter_parameters_pkl, Path):
-            with open(converter_parameters_pkl, 'rb') as f:
-                converter_parameters = pickle.load(f)
-        else:
-            raise ValueError(
-                f"Input type {converter_parameters_pkl.__class__} not "
-                'understood')
-        preprocess_setting = setting.PreprocessSetting(
-            preprocess=converter_parameters)
-
-        converters = {
-            variable_name:
-            util.PreprocessConverter(
-                value['preprocess_converter'],
-                method=value['method'],
-                componentwise=value['componentwise'],
-                other_components=value['other_components'])
-            for variable_name, value in preprocess_setting.preprocess.items()}
-        return converters
-
-    def preprocess(self, dict_data_x):
-        converted_dict_data_x = {
-            variable_name:
-            self.converters[variable_name].transform(data)
-            for variable_name, data in dict_data_x.items()
-            if variable_name in self.converters.keys()}
+        self.converters = ScalersComposition.create_from_file(
+            converter_parameters_pkl=converter_parameters_pkl,
+            key=key
+        )
+
+    def preprocess(self, dict_data_x: dict):
+        input_dict = {
+            name: v for name, v in dict_data_x.items()
+            if name in self.converters.get_variable_names()
+        }
+
+        converted_dict_data_x = self.converters.transform_dict(input_dict)
         if len(converted_dict_data_x) == 0:
             raise ValueError(
                 'No converted data found. '
                 'Check the preprocessed directory set correctly.')
         return converted_dict_data_x
 
     def postprocess(
-            self, dict_data_x, dict_data_y, output_directory=None, *,
+            self, dict_data_x: dict, dict_data_y: dict, output_directory=None,
+            *,
             dict_data_y_answer=None,
             overwrite=False, save_x=False, write_simulation=False,
             write_npy=True, write_simulation_stem=None,
             write_simulation_base=None, read_simulation_type='fistr',
             save_function=None,
             write_simulation_type='fistr', skip_femio=False,
             load_function=None, convert_to_order1=False,
@@ -673,78 +212,32 @@
             inversed_dict_data_y: dict
                 Inversed output data.
             inversed_dict_answer: dict
                 Inversed answer data. None when the answer not available.
             fem_data: femio.FEMData
                 FEMData object with input and output data.
         """
-        if perform_inverse:
-            dict_post_function = {
-                k: v.inverse for k, v in self.converters.items()}
-        else:
-            dict_post_function = {
-                k: lambda x: x for k, v in self.converters.items()}
-
-        if isinstance(list(dict_data_x.values())[0], dict):
-            return_dict_data_x = {
-                variable_name:
-                dict_post_function[variable_name](data)
-                for value in dict_data_x.values()
-                for variable_name, data in value.items()
-                if variable_name in dict_post_function.keys()}
-        else:
-            return_dict_data_x = {
-                variable_name:
-                dict_post_function[variable_name](data)
-                for variable_name, data in dict_data_x.items()
-                if variable_name in dict_post_function.keys()}
-
-        if dict_data_y_answer is not None and len(dict_data_y_answer) > 0:
-            if isinstance(list(dict_data_y_answer.values())[0], dict):
-                return_dict_data_y_answer = {
-                    variable_name:
-                    dict_post_function[variable_name](data)
-                    for value in dict_data_y_answer.values()
-                    for variable_name, data in value.items()
-                    if variable_name in dict_post_function.keys()}
-            else:
-                return_dict_data_y_answer = {
-                    variable_name:
-                    dict_post_function[variable_name](data)
-                    for variable_name, data in dict_data_y_answer.items()
-                    if variable_name in dict_post_function.keys()}
-        else:
-            return_dict_data_y_answer = None
+        _dict_data_x = self._format_dict_shape(dict_data_x)
+        _dict_data_y = self._format_dict_shape(dict_data_y)
+        _dict_data_y_answer = self._format_dict_shape(dict_data_y_answer)
 
-        if len(dict_data_y) > 0:
-            if isinstance(list(dict_data_y.values())[0], dict):
-                return_dict_data_y = {
-                    variable_name:
-                    dict_post_function[variable_name](data)
-                    for value in dict_data_y.values()
-                    for variable_name, data in value.items()
-                    if variable_name in dict_post_function.keys()}
-            else:
-                return_dict_data_y = {
-                    variable_name:
-                    dict_post_function[variable_name](data)
-                    for variable_name, data in dict_data_y.items()
-                    if variable_name in dict_post_function.keys()}
-        else:
-            return_dict_data_y = {}
+        if perform_inverse:
+            _dict_data_x = self._inverse_process(_dict_data_x)
+            _dict_data_y = self._inverse_process(_dict_data_y)
+            _dict_data_y_answer = self._inverse_process(_dict_data_y_answer)
 
         # Save data
         if skip_fem_data_creation or write_simulation_base is None \
                 or not write_simulation_base.exists():
             fem_data = None
         else:
             try:
                 fem_data = self._create_fem_data(
-                    return_dict_data_x, return_dict_data_y,
-                    dict_data_answer=return_dict_data_y_answer,
+                    _dict_data_x, _dict_data_y,
+                    dict_data_answer=_dict_data_y_answer,
                     write_simulation_base=write_simulation_base,
                     write_simulation_stem=write_simulation_stem,
                     read_simulation_type=read_simulation_type,
                     data_addition_function=data_addition_function,
                     skip_femio=skip_femio, load_function=load_function,
                     convert_to_order1=convert_to_order1,
                     required_file_names=required_file_names)
@@ -758,30 +251,67 @@
                 )
                 fem_data = None
                 write_simulation_base = None
                 write_simulation = False
         if output_directory is not None:
             if write_npy:
                 if save_x:
-                    self.save(return_dict_data_x, output_directory)
-                self.save(return_dict_data_y, output_directory)
+                    self.save(_dict_data_x, output_directory)
+                self.save(_dict_data_y, output_directory)
             if write_simulation:
                 if write_simulation_base is None:
                     raise ValueError('No write_simulation_base fed.')
                 self._write_simulation(
                     output_directory, fem_data, overwrite=overwrite,
                     write_simulation_type=write_simulation_type,
                     less_output=less_output)
             if save_function is not None:
                 save_function(
                     output_directory, fem_data, overwrite=overwrite,
                     write_simulation_type=write_simulation_type)
 
-        return return_dict_data_x, return_dict_data_y, \
-            return_dict_data_y_answer, fem_data
+        return _dict_data_x, _dict_data_y, \
+            _dict_data_y_answer, fem_data
+
+    def _inverse_process(
+        self,
+        dict_data: Union[dict[str, ArrayDataType], None]
+    ) -> dict[str, ArrayDataType]:
+        if dict_data is None:
+            return {}
+
+        dict_data_answer = self.converters.inverse_transform_dict(dict_data)
+        return dict_data_answer
+
+    def _format_dict_shape(
+        self,
+        dict_data: Union[dict, None]
+    ) -> Union[dict[str, ArrayDataType], None]:
+        # This function should be deprecated
+        # It is not appropriate to overwrite value for variable name
+        if dict_data is None:
+            return None
+
+        if len(dict_data) == 0:
+            return None
+
+        if isinstance(list(dict_data.values())[0], dict):
+            return_dict_data = {
+                variable_name: data
+                for value in dict_data.values()
+                for variable_name, data in value.items()
+                if variable_name in self.converters.get_variable_names()
+            }
+        else:
+            return_dict_data = {
+                variable_name: data
+                for variable_name, data in dict_data.items()
+                if variable_name in self.converters.get_variable_names()
+            }
+        return return_dict_data
 
     def _create_fem_data(
             self, dict_data_x, dict_data_y, write_simulation_base, *,
             dict_data_answer=None,
             write_simulation_stem=None,
             read_simulation_type='fistr', data_addition_function=None,
             skip_femio=False, load_function=None,
```

## siml/preprocessing/__init__.py

```diff
@@ -1,2 +1,3 @@
-
 from . import converter  # NOQA
+from .scaling_converter import ScalingConverter  # NOQA
+from .scalers_composition import ScalersComposition  # NOQA
```

## siml/preprocessing/converter.py

```diff
@@ -9,43 +9,47 @@
 import numpy as np
 
 from siml import setting, util
 from siml.utils import fem_data_utils, path_utils
 
 
 class IConvertFunction(metaclass=abc.ABCMeta):
+    @abc.abstractmethod
     def __call__(
         self,
         fem_data: femio.FEMData,
         data_directory: pathlib.Path
     ) -> dict[str, np.ndarray]:
         raise NotImplementedError()
 
 
 class ILoadFunction(metaclass=abc.ABCMeta):
+    @abc.abstractmethod
     def __call__(
         self,
         data_files: list[pathlib.Path],
         raw_path: pathlib.Path
     ) -> tuple[Dict, femio.FEMData]:
         raise NotImplementedError()
 
 
 class ISaveFunction(metaclass=abc.ABCMeta):
+    @abc.abstractmethod
     def __call__(
         self,
         fem_data: femio.FEMData,
         dict_data: dict[str, np.ndarray],
         output_directory: pathlib.Path,
         force_renew: bool
     ) -> None:
         raise NotImplementedError()
 
 
 class IFilterFunction(metaclass=abc.ABCMeta):
+    @abc.abstractmethod
     def __call__(
         self,
         fem_data: femio.FEMData,
         raw_path: pathlib.Path,
         dict_data: dict[str, np.ndarray]
     ) -> bool:
         raise NotImplementedError()
```

## siml/trainer.py

```diff
@@ -18,15 +18,15 @@
 from . import datasets
 from . import networks
 from . import setting
 from . import siml_manager
 from . import util
 
 from . import update_functions
-from .variables import siml_variables
+from .siml_variables import siml_tensor_variables
 
 
 class Trainer(siml_manager.SimlManager):
 
     def __init__(self,
                  settings,
                  *,
@@ -673,15 +673,15 @@
                     non_blocking=self.setting.trainer.non_blocking)
                 split_xs, split_ys = self._split_data_if_needed(
                     x, y,
                     self.setting.trainer.time_series_split_evaluation)
 
                 y_pred = []
                 for split_x in split_xs:
-                    siml_x = siml_variables(split_x['x'])
+                    siml_x = siml_tensor_variables(split_x['x'])
                     split_x['x'] = siml_x.send(self.device).get_values()
                     y_pred.append(self.model(split_x))
 
                 if self.setting.trainer.time_series_split_evaluation is None:
                     original_shapes = x['original_shapes']
                 else:
                     cat_x = util.cat_time_series(
@@ -692,15 +692,15 @@
                 y_pred = util.cat_time_series(
                     y_pred, time_series_keys=self.output_time_series_keys)
 
                 ans_y = util.cat_time_series(
                     split_ys,
                     time_series_keys=self.output_time_series_keys
                 )
-                ans_siml_y = siml_variables(ans_y)
+                ans_siml_y = siml_tensor_variables(ans_y)
                 y = ans_siml_y.send(self.output_device).get_values()
                 return y_pred, y, {
                     'original_shapes': original_shapes,
                     'model': self.model}
 
         evaluator_engine = ignite.engine.Engine(_inference)
```

## siml/update_functions/pseudo_batch_update.py

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typing import Any, Callable
 import numpy as np
 import torch
 
 from siml.networks.network import Network
-from siml.variables import siml_variables
+from siml.siml_variables import siml_tensor_variables
 
 from .update_interface import IStepUpdateFunction
 
 
 class Counter():
     def __init__(self, base_value: int):
         assert base_value > 0
@@ -78,23 +78,23 @@
         )
 
         loss_value = np.nan
         for split_x, split_y in zip(split_xs, split_ys):
             if self._allow_zero_grad():
                 optimizer.zero_grad()
 
-            siml_x = siml_variables(split_x['x']).send(self.device)
-            siml_y = siml_variables(split_y).send(self.output_device)
+            siml_x = siml_tensor_variables(split_x['x']).send(self.device)
+            siml_y = siml_tensor_variables(split_y).send(self.output_device)
 
             split_x['x'] = siml_x.get_values()
             split_y = siml_y.get_values()
 
             split_y_pred = model(split_x)
 
-            siml_y_pred = siml_variables(split_y_pred)
+            siml_y_pred = siml_tensor_variables(split_y_pred)
 
             _loss = self._loss_func(
                 siml_y_pred.slice(self.loss_slice).get_values(),
                 siml_y.slice(self.loss_slice).get_values(),
                 split_x['original_shapes']
             )
             _other_loss = self._other_loss_func(
```

## siml/update_functions/standard_update.py

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typing import Any, Callable
 import numpy as np
 import torch
 
 from siml.networks.network import Network
-from siml.variables import siml_variables
+from siml.siml_variables import siml_tensor_variables
 from .update_interface import IStepUpdateFunction
 
 
 class StandardUpdate(IStepUpdateFunction):
     def __init__(
         self,
         loss_func: Callable,
@@ -45,24 +45,24 @@
         split_xs, split_ys = self._split_data_func(
             x, y, self.time_series_split
         )
 
         loss_value = np.nan
         for split_x, split_y in zip(split_xs, split_ys):
             optimizer.zero_grad()
-            siml_x = siml_variables(split_x['x']).send(self.device)
-            siml_y = siml_variables(split_y).send(self.output_device)
+            siml_x = siml_tensor_variables(split_x['x']).send(self.device)
+            siml_y = siml_tensor_variables(split_y).send(self.output_device)
 
             split_x['x'] = \
                 siml_x.get_values()
             split_y = \
                 siml_y.get_values()
 
             split_y_pred = model(split_x)
-            siml_y_pred = siml_variables(split_y_pred)
+            siml_y_pred = siml_tensor_variables(split_y_pred)
 
             loss = self._loss_func(
                 siml_y_pred.slice(self.loss_slice).get_values(),
                 siml_y.slice(self.loss_slice).get_values(),
                 split_x['original_shapes']
             )
             other_loss = self._other_loss_func(
```

## siml/util.py

```diff
@@ -1,25 +1,21 @@
 import datetime as dt
-import gc
 from glob import glob, iglob
 import io
 import os
 from pathlib import Path
 import re
 import shutil
 import subprocess
-import pickle
 from typing import List
 
 from Cryptodome.Cipher import AES
 
 import numpy as np
 import scipy.sparse as sp
-from sklearn.base import BaseEstimator, TransformerMixin
-from sklearn import preprocessing
 import torch
 import yaml
 
 
 INFERENCE_FLAG_FILE = 'inference'
 
 
@@ -413,427 +409,14 @@
         file_names = [file_names]
     a = np.all([
         len(list(directory.glob(file_name))) > 0
         for file_name in file_names])
     return a
 
 
-class PreprocessConverter():
-
-    MAX_RETRY = 3
-
-    def __init__(
-            self, setting_data, *,
-            data_files=None, componentwise=True, power=1., method=None,
-            other_components=[], key=None):
-        self.is_erroneous = None
-        self.setting_data = setting_data
-        self.power = power
-        self.other_components = other_components
-        self.key = key
-        self.use_diagonal = False
-        self.method = method
-
-        self._init_converter()
-
-        self.componentwise = componentwise
-        self.retry_count = 0
-
-        if not isinstance(
-                self.converter, (SparseStandardScaler, MaxAbsScaler)):
-            if abs(self.power - 1) > 1e-5:
-                raise ValueError(
-                    f"power option is not supported for {self.converter}")
-
-        if data_files is not None:
-            self.lazy_read_files(data_files)
-        return
-
-    def _init_converter(self):
-        if isinstance(self.setting_data, dict):
-            self._init_with_dict(self.setting_data)
-        elif isinstance(self.setting_data, str):
-            self._init_with_str(self.setting_data)
-        elif isinstance(self.setting_data, BaseEstimator):
-            self._init_with_converter(self.setting_data)
-        elif isinstance(self.setting_data, PreprocessConverter):
-            self._init_with_converter(self.setting_data.converter)
-        else:
-            raise ValueError(f"Unsupported setting_data: {self.setting_data}")
-
-    def _init_with_dict(self, setting_dict):
-        if 'method' in setting_dict:
-            preprocess_method = setting_dict['method']
-            self._init_with_str(preprocess_method)
-        else:
-            if self.method is None:
-                raise ValueError('Feed ''method'' when initialize with pkl')
-            self._init_with_str(self.method)
-            for key, value in setting_dict.items():
-                setattr(self.converter, key, value)
-        return
-
-    def _init_with_str(self, preprocess_method: str):
-        if preprocess_method == 'identity':
-            self.converter = Identity()
-        elif preprocess_method == 'standardize':
-            self.converter = preprocessing.StandardScaler()
-            self.is_erroneous = self.is_standard_scaler_var_nan
-        elif preprocess_method == 'std_scale':
-            self.converter = preprocessing.StandardScaler(with_mean=False)
-            self.is_erroneous = self.is_standard_scaler_var_nan
-        elif preprocess_method == 'sparse_std':
-            self.converter = SparseStandardScaler(
-                power=self.power, other_components=self.other_components)
-            self.is_erroneous = self.is_standard_scaler_var_nan
-        elif preprocess_method == 'isoam_scale':
-            self.converter = IsoAMScaler(
-                other_components=self.other_components)
-            self.is_erroneous = self.is_standard_scaler_var_nan
-            self.use_diagonal = True
-        elif preprocess_method == 'min_max':
-            self.converter = preprocessing.MinMaxScaler()
-        elif preprocess_method == 'max_abs':
-            self.converter = MaxAbsScaler(power=self.power)
-        elif preprocess_method.startswith('user_defined'):
-            pkl_path = preprocess_method.split("?Path=")[1]
-            self.converter = UserDefinedScalar(pkl_path)
-        else:
-            raise ValueError(
-                f"Unknown preprocessing method: {preprocess_method}")
-        return
-
-    def _init_with_converter(self, converter):
-        self.converter = converter
-        return
-
-    def apply_data_with_rehspe_if_needed(
-            self, data, function, return_applied=True, use_diagonal=False,
-            skip_nan=False):
-        if isinstance(data, np.ndarray):
-            if use_diagonal:
-                raise ValueError('Cannot set use_diagonal=True for dense data')
-            result = self.apply_numpy_data_with_reshape_if_needed(
-                data, function, return_applied=return_applied,
-                skip_nan=skip_nan)
-        elif isinstance(data, (sp.coo_matrix, sp.csr_matrix, sp.csc_matrix)):
-            result = self.apply_sparse_data_with_reshape_if_needed(
-                data, function, return_applied=return_applied,
-                use_diagonal=use_diagonal)
-        else:
-            raise ValueError(f"Unsupported data type: {data.__class__}")
-
-        return result
-
-    def is_standard_scaler_var_nan(self):
-        return np.any(np.isnan(self.converter.var_))
-
-    def apply_sparse_data_with_reshape_if_needed(
-            self, data, function, return_applied=True, use_diagonal=False):
-        if self.componentwise:
-            applied = function(data)
-            if return_applied:
-                return applied.tocoo()
-            else:
-                return
-
-        elif use_diagonal:
-            print('Start diagonal')
-            print(dt.datetime.now())
-            reshaped = data.diagonal()
-            print('Start apply')
-            print(dt.datetime.now())
-            applied_reshaped = function(reshaped)
-            if return_applied:
-                raise ValueError(
-                    'Cannot set return_applied=True when use_diagonal=True')
-            else:
-                return
-
-        else:
-            shape = data.shape
-            print('Start reshape')
-            print(dt.datetime.now())
-            reshaped = data.reshape((shape[0] * shape[1], 1))
-            print('Start apply')
-            print(dt.datetime.now())
-            applied_reshaped = function(reshaped)
-            if return_applied:
-                return applied_reshaped.reshape(shape).tocoo()
-            else:
-                return
-
-    def apply_numpy_data_with_reshape_if_needed(
-            self, data, function, return_applied=True, skip_nan=False):
-        if skip_nan:
-            if return_applied:
-                raise ValueError(
-                    'Cannot set return_applied=True when skip_nan=True')
-        shape = data.shape
-
-        if self.componentwise:
-            reshaped = np.reshape(data, (np.prod(shape[:-1]), shape[-1]))
-            if skip_nan:
-                isnan = np.isnan(np.prod(reshaped, axis=-1))
-                reshaped_wo_nan = reshaped[~isnan]
-                if reshaped_wo_nan.size == 0:
-                    return
-                applied_reshaped = function(reshaped_wo_nan)
-                return
-            else:
-                applied_reshaped = function(reshaped)
-            if return_applied:
-                applied = np.reshape(applied_reshaped, shape)
-                return applied
-            else:
-                return
-
-        else:
-            reshaped = np.reshape(data, (-1, 1))
-            if skip_nan:
-                reshaped_wo_nan = reshaped[~np.isnan(reshaped)][:, None]
-                if reshaped_wo_nan.size == 0:
-                    return
-                applied_reshaped = function(reshaped_wo_nan)
-                return
-
-            else:
-                applied_reshaped = function(reshaped)
-
-                if return_applied:
-                    applied = np.reshape(applied_reshaped, shape)
-                    return applied
-                else:
-                    return
-
-    def lazy_read_files(self, data_files):
-        for data_file in data_files:
-            print(f"Start load data: {data_file}")
-            print(dt.datetime.now())
-            data = self.load_file(data_file)
-            print(f"Start partial_fit: {data_file}")
-            print(dt.datetime.now())
-            self.apply_data_with_rehspe_if_needed(
-                data, self.converter.partial_fit, return_applied=False,
-                use_diagonal=self.use_diagonal, skip_nan=True)
-            print(f"Start del: {data_file}")
-            print(dt.datetime.now())
-            del data
-            print(f"Start GC: {data_file}")
-            print(dt.datetime.now())
-            gc.collect()
-            print(f"Finish one iter: {data_file}")
-            print(dt.datetime.now())
-
-        return
-
-    def load_file(self, data_file):
-        str_data_file = str(data_file)
-        if str_data_file.endswith('.npy'):
-            data = np.load(data_file)
-        elif str_data_file.endswith('.npy.enc'):
-            data = np.load(decrypt_file(self.key, data_file))
-        elif str_data_file.endswith('.npz'):
-            data = sp.load_npz(data_file)
-            if not sp.issparse(data):
-                raise ValueError(f"Data type not understood for: {data_file}")
-        elif str_data_file.endswith('.npz.enc'):
-            data = sp.load_npz(decrypt_file(self.key, data_file))
-            if not sp.issparse(data):
-                raise ValueError(f"Data type not understood for: {data_file}")
-        else:
-            raise ValueError(f"Data type not understood for: {data_file}")
-        return data
-
-    def transform(self, data):
-        return self.apply_data_with_rehspe_if_needed(
-            data, self.converter.transform)
-
-    def inverse(self, data):
-        return self.apply_data_with_rehspe_if_needed(
-            data, self.converter.inverse_transform)
-
-
-class MaxAbsScaler(TransformerMixin, BaseEstimator):
-
-    def __init__(self, power=1.):
-        self.max_ = 0.
-        self.power = power
-        return
-
-    def partial_fit(self, data):
-        if sp.issparse(data):
-            self.max_ = np.maximum(
-                np.ravel(np.max(np.abs(data), axis=0).toarray()), self.max_)
-        else:
-            self.max_ = np.maximum(
-                np.max(np.abs(data), axis=0), self.max_)
-        return self
-
-    def transform(self, data):
-        if np.max(self.max_) == 0.:
-            scale = 0.
-        else:
-            scale = (1 / self.max_)**self.power
-
-        if sp.issparse(data):
-            if len(scale) != 1:
-                raise ValueError('Should be componentwise: false')
-            scale = scale[0]
-        return data * scale
-
-    def inverse_transform(self, data):
-        inverse_scale = self.max_
-        if sp.issparse(data):
-            if len(inverse_scale) != 1:
-                raise ValueError('Should be componentwise: false')
-            inverse_scale = inverse_scale[0]**(self.power)
-        return data * inverse_scale
-
-
-class SparseStandardScaler(TransformerMixin, BaseEstimator):
-    """Class to perform standardization for sparse data."""
-
-    def __init__(self, power=1., other_components=[]):
-        self.var_ = 0.
-        self.std_ = 0.
-        self.mean_square_ = 0.
-        self.n_ = 0
-        self.power = power
-        self.component_dim = len(other_components) + 1
-        return
-
-    def partial_fit(self, data):
-        self._raise_if_not_sparse(data)
-        self._update(data)
-        return self
-
-    def _update(self, sparse_dats):
-        m = np.prod(sparse_dats.shape)
-        mean_square = (
-            self.mean_square_ * self.n_ + np.sum(sparse_dats.data**2)) / (
-                self.n_ + m)
-
-        self.mean_square_ = mean_square
-        self.n_ += m
-
-        # To use mean_i [x_i^2 + y_i^2 + z_i^2], multiply by the dim
-        self.var_ = self.mean_square_ * self.component_dim
-        self.std_ = np.sqrt(self.var_)
-        return
-
-    def _raise_if_not_sparse(self, data):
-        if not sp.issparse(data):
-            raise ValueError('Data is not sparse')
-        return
-
-    def transform(self, data):
-        self._raise_if_not_sparse(data)
-        if self.std_ == 0.:
-            scale = 0.
-        else:
-            scale = (1 / self.std_)**self.power
-        return data * scale
-
-    def inverse_transform(self, data):
-        self._raise_if_not_sparse(data)
-        inverse_scale = self.std_**(self.power)
-        return data * inverse_scale
-
-
-class IsoAMScaler(TransformerMixin, BaseEstimator):
-    """Class to perform scaling for IsoAM based on
-    https://arxiv.org/abs/2005.06316.
-    """
-
-    def __init__(self, other_components=[]):
-        self.var_ = 0.
-        self.std_ = 0.
-        self.mean_square_ = 0.
-        self.n_ = 0
-        self.component_dim = len(other_components) + 1
-        if self.component_dim == 1:
-            raise ValueError(
-                'To use IsoAMScaler, feed other_components: '
-                f"{other_components}")
-        return
-
-    def partial_fit(self, data):
-        self._update(data)
-        return self
-
-    def _update(self, diagonal_data):
-        if len(diagonal_data.shape) != 1:
-            raise ValueError(f"Input data should be 1D: {diagonal_data}")
-        m = len(diagonal_data)
-        mean_square = (
-            self.mean_square_ * self.n_ + np.sum(diagonal_data**2)) / (
-                self.n_ + m)
-
-        self.mean_square_ = mean_square
-        self.n_ += m
-
-        # To use mean_i [x_i^2 + y_i^2 + z_i^2], multiply by the dim
-        self.var_ = self.mean_square_ * self.component_dim
-        self.std_ = np.sqrt(self.var_)
-        return
-
-    def _raise_if_not_sparse(self, data):
-        if not sp.issparse(data):
-            raise ValueError('Data is not sparse')
-        return
-
-    def transform(self, data):
-        if self.std_ == 0.:
-            scale = 0.
-        else:
-            scale = (1 / self.std_)
-        return data * scale
-
-    def inverse_transform(self, data):
-        inverse_scale = self.std_
-        return data * inverse_scale
-
-
-class Identity(TransformerMixin, BaseEstimator):
-    """Class to perform identity conversion (do nothing)."""
-
-    def partial_fit(self, data):
-        return
-
-    def transform(self, data):
-        return data
-
-    def inverse_transform(self, data):
-        return data
-
-
-class UserDefinedScalar(TransformerMixin, BaseEstimator):
-
-    def __init__(self, pkl_path: Path):
-        self.scalar = self._load_pkl(pkl_path)
-        return
-
-    def _load_pkl(self, pkl_path: Path):
-        with open(pkl_path, 'rb') as fr:
-            scalar = pickle.load(fr)
-        return scalar
-
-    def partial_fit(self, data):
-        return
-
-    def transform(self, data):
-        out = self.scalar.transform(data)
-        return out
-
-    def inverse_transform(self, data):
-        inverse_out = self.scalar.inverse_transform(data)
-        return inverse_out
-
-
 def get_top_directory():
     completed_process = subprocess.run(
         ['git', 'rev-parse', '--show-toplevel'],
         capture_output=True, text=True)
     path = Path(completed_process.stdout.rstrip('\n'))
     return path
```

## Comparing `siml/variables/siml_variables.py` & `siml/siml_variables/tensor_variables/tensor_variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
+
 from typing import TypeVar
-import torch
 
+import torch
 
 BuiltInVars = TypeVar(
     'BuiltInVars',
     torch.Tensor, dict, list
 )
 
 
@@ -19,15 +20,15 @@
     def slice(self, loss_slice: slice) -> ISimlVariables:
         raise NotImplementedError()
 
     def send(self, device: str) -> ISimlVariables:
         raise NotImplementedError()
 
 
-def siml_variables(values: BuiltInVars) -> ISimlVariables:
+def siml_tensor_variables(values: BuiltInVars) -> ISimlVariables:
     if isinstance(values, torch.Tensor):
         return TensorSimlVariables(values)
     if isinstance(values, dict):
         return DictSimlVariables(values)
     if isinstance(values, list):
         return ListSimlVaraiables(values)
 
@@ -65,15 +66,15 @@
     def send(self, device: str) -> TensorSimlVariables:
         tmp = self._x.to(device)
         return TensorSimlVariables(tmp)
 
 
 class DictSimlVariables(ISimlVariables):
     def __init__(self, value: dict):
-        self._x = {k: siml_variables(v) for k, v in value.items()}
+        self._x = {k: siml_tensor_variables(v) for k, v in value.items()}
 
     def __str__(self) -> str:
         txt = ""
         for k, v in self._x.items():
             txt += f"{k}: {v}, "
         return f"{self.__class__.__name__}" + '{' + txt + '}'
 
@@ -88,15 +89,15 @@
     def send(self, device: str) -> TensorSimlVariables:
         tmp = {k: v.send(device) for k, v in self._x.items()}
         return DictSimlVariables(tmp)
 
 
 class ListSimlVaraiables(ISimlVariables):
     def __init__(self, value: list[torch.Tensor]):
-        self._x = [siml_variables(v) for v in value]
+        self._x = [siml_tensor_variables(v) for v in value]
 
     def __str__(self) -> str:
         values = [str(v) for v in self._x]
         txt = ", ".join(values)
         return f"{self.__class__.__name__}" + '[' + txt + ']'
 
     def get_values(self) -> list[torch.Tensor]:
```

## Comparing `pysiml-0.2.8.dev202304200913.dist-info/LICENSE` & `pysiml-0.2.9.dev202305020647.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pysiml-0.2.8.dev202304200913.dist-info/METADATA` & `pysiml-0.2.9.dev202305020647.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pysiml
-Version: 0.2.8.dev202304200913
+Version: 0.2.9.dev202305020647
 Summary: SiML - a Simulation ML library
 Home-page: https://github.com/ricosjp/pysiml
 License: Apache-2.0
 Author: RICOS Co. Ltd.
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: PyQt5
 Provides-Extra: cupy
-Requires-Dist: PyQt5 (>=5.14.0,<6.0.0); extra == "PyQt5"
+Provides-Extra: pyqt5
+Requires-Dist: PyQt5 (>=5.14.0,<6.0.0) ; extra == "pyqt5"
 Requires-Dist: PyYAML (>=5.2,<6.0)
 Requires-Dist: einops (>=0.2,<0.3)
 Requires-Dist: femio (>=0.3.1)
 Requires-Dist: joblib (>=0.14.1,<0.15.0)
 Requires-Dist: metis (>=0.2a5,<0.3)
 Requires-Dist: optuna (>=1.3,<2.0)
 Requires-Dist: pandas (>=1.0,<2.0)
 Requires-Dist: pycryptodomex (>=3.9.0,<4.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pydot (>=1.4.1,<2.0.0)
 Requires-Dist: pytorch-ignite (>=0.3,<0.4)
 Requires-Dist: sqlalchemy (==1.3.13)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: torch (>=1.9.0,<2.0.0)
 Project-URL: Documentation, https://ricosjp.github.io/pysiml/
 Project-URL: Repository, https://github.com/ricosjp/pysiml
```

## Comparing `pysiml-0.2.8.dev202304200913.dist-info/RECORD` & `pysiml-0.2.9.dev202305020647.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-pyproject.toml,sha256=BGTtWpF5gkubVixtujxhQeYX9rQeNyK01kF8g5RUC4w,1499
+pyproject.toml,sha256=9S007qq5glhjvU2ldx4ExNVtIR8kSeB9YnlrEgULwJw,1520
 siml/__init__.py,sha256=mC61oSLHO5F6zXHhOrzH51R-vkH0mL4MShhSBiRRe6s,638
 siml/__main__/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-siml/__main__/convert_interim_data.py,sha256=63owXqB0-VG0fZn0f-1LE6FbxHirCHJ1d0twZlDRjRs,970
+siml/__main__/convert_interim_data.py,sha256=jA6GD7BlnsEjARcln3UBwXlFj64BeFALAmgD1ohBkqo,900
 siml/__main__/convert_raw_data.py,sha256=VNVOyx9lChopF2Q-9OXtN_-MtfBsyjS_JvFwCjdkv0c,1400
 siml/__main__/optimize.py,sha256=6HALn60Mxh4GUiPbSXjvrdpkoQ4NgYSzCHCBRbli4W0,1742
 siml/__main__/plot_losses.py,sha256=0uMsoPN-xR0JhPg0WzSQL5GbD80ovuFO12eVpc0x6Xc,8663
-siml/__main__/prepare_preprocess_converters.py,sha256=wdr7jA690BMyuTYxZYmLnBZV10_0rKvqt98p7l6wU94,929
-siml/__main__/preprocess_interim_data.py,sha256=D74mGTZcAk-4kQQtq5BN2dc7rAIxwx49oYBFtpJfupc,712
+siml/__main__/prepare_preprocess_converters.py,sha256=w_rzic--RUyISagQOJw_5-oEkOFEKXUN7G1TkTOxd8g,927
+siml/__main__/preprocess_interim_data.py,sha256=M5_di_6ORZ3yJL_oUb0kkkelh5ybJelke-vvLz3Xg5w,717
 siml/__main__/train.py,sha256=7cLknw6yx4Ehm_K9UkUGIbg3QPAXJpr_HpNWP60MvPs,1376
 siml/__main__/visualize_graph.py,sha256=xyPqVZHA0p3xnB41w4PsKCfy7feicBRMXZveQdo_lpM,3961
 siml/config.py,sha256=_Cc2w65g05Y5QDuh8b8UIY_XFZbwKmXx_Z40ATxVw_I,57
 siml/data_parallel.py,sha256=b4DU0QCVVbFWB02QdvtMLuLuTIz57npYSlbmKfJVjVo,3520
 siml/datasets.py,sha256=8nYbgADi86eqzy95pXUlNHs9iBxMDbk1oyIuL7DPOqg,26681
 siml/inferer.py,sha256=SfoblDVNBF3V1U5j7nKUI5sZRLJDvUuacMAwsFzFNFw,27000
 siml/loss_operations/loss_assignment.py,sha256=LuGyNfM_y0agzwSTfdMqSGwB25HmgziqXz1araAmEbE,1466
@@ -62,31 +62,52 @@
 siml/networks/tcn.py,sha256=k3T3yLfcWHhi-ibEqZtmVLIOKkbFOVToEez8LHfxhGo,3260
 siml/networks/tensor_operations.py,sha256=bzzxvWswGKj5zx9xOPmpQuY-r2KORtodKbvRB-fsJfM,5969
 siml/networks/threshold.py,sha256=oy-7D58Z68uZBn8SZ5XJHzo7GXbUiiBkW5MZL0qq5EE,1415
 siml/networks/time_norm.py,sha256=fM0A7WF6CjmAcvvBlbziinSQEjQlAIHRkQEQ0Y8tLr0,782
 siml/networks/translator.py,sha256=-X4wO4QmdtF6byUcHdNRmCCds-c2F-UUvprgW6msCCE,1882
 siml/networks/upper_limit.py,sha256=OUi7vXtqf0r83ZebSX98Jlo0N6C_v2KpdcF1pccIfGw,1034
 siml/optimize.py,sha256=KJAkJSvb4s4XF2y86fAt5MZafYrbW9SGXPPsJFqkqkA,6940
+siml/path_like_objects/__init__.py,sha256=E7R0q4U21egIs-B4NS5pei0g5AOjx_sO1ozu1PeE6uw,125
+siml/path_like_objects/siml_directory.py,sha256=sNIHgtItIqoSFCidPL6pypbnS-PudlUB9ZNbdx1VWk8,1119
+siml/path_like_objects/siml_file.py,sha256=-nmvNX4vK_S-Bg1AnQEqMJ13aNJNk8tQ1a7C9r7FwE8,5982
 siml/postprocessor.py,sha256=5DXPxY3Xdutc5WSLkJ6FAo8lZXMPyG29XsSHn_mB3kI,5523
-siml/prepost.py,sha256=QTMoM4JJUKYFqYQg9_bfGRoS-n1sgbbKyEM4vXx4--0,45390
-siml/preprocessing/__init__.py,sha256=uGj2n-EecOO5XxBoVCmp96skKw-mM43QHMEKC179GE4,33
-siml/preprocessing/converter.py,sha256=AYzhEaB1wc_usbqENhQMsQSn9HMHVqhqKfHBfNfwxUM,20676
+siml/prepost.py,sha256=pzVvFwmAgat79SJuR4dS4U3UT5dSOXLvZKBX52wBLh0,25936
+siml/preprocessing/__init__.py,sha256=74VUugOzkJIGD6ppx8v3nVEZBT5Gi4oRXtJVwr-9xBw,148
+siml/preprocessing/converter.py,sha256=FLunn6_jY_sGD8uJSMbLuEtTjt2DXVEjbYw_DXWIdeM,20772
+siml/preprocessing/scalers_composition.py,sha256=jm0Fk-v4odx4SvgzB3CxlGnmItMtC2NR8p6i2rmYAs4,9702
+siml/preprocessing/scaling_converter.py,sha256=d0LRO0fcpHOeXil5flvIXi61vQwoKtqM7rZ77FtoBc0,10594
+siml/preprocessing/siml_scalers/__init__.py,sha256=s1f6V4Z56KY1klO29hFYszuQLNiyTTMx36jsLRtb9PA,176
+siml/preprocessing/siml_scalers/scale_functions/__init__.py,sha256=U0OYAqKY6HRAVhztbmQgDEc7u7sqULBYYnCaYxRhZjQ,1405
+siml/preprocessing/siml_scalers/scale_functions/identity_scaler.py,sha256=W3GyGt6BzJrg6jV_SDc59cDkXuNyAxgdSEqm0JpXvlg,592
+siml/preprocessing/siml_scalers/scale_functions/interface_scaler.py,sha256=Om7j_rA9pI0eeHK15IFQInHd-edIL2jIJEOur-xbI6o,738
+siml/preprocessing/siml_scalers/scale_functions/isoam_scaler.py,sha256=KlPbXA0Ysotk5uYW6DHGvaedAZlOkU8QzUE4h5F0OQ0,2038
+siml/preprocessing/siml_scalers/scale_functions/max_abs_scaler.py,sha256=ws97VhwtXV-KoU4lHefXIxmLDAdxoKIPh19wDvezSFI,1403
+siml/preprocessing/siml_scalers/scale_functions/min_max_scaler.py,sha256=A4gg2J8tCYCmDOivgVkIRmfZnhLk-2mQJXY0KQvZc6U,465
+siml/preprocessing/siml_scalers/scale_functions/sparse_standard_scaler.py,sha256=wdk1e2Cil-OyIo5SiG1PYKY5K60zHUEIPEYPmND4hQA,1926
+siml/preprocessing/siml_scalers/scale_functions/standard_scaler.py,sha256=qvyUGXXw4j60xGw0RwXUaHaYlnVZHR9XB_DFkayySBg,570
+siml/preprocessing/siml_scalers/scale_functions/user_defined_scaler.py,sha256=GFwX9UyJ6z9iTy8XiiJgvlv65W6dBRZ8bDLV2sECdTs,865
+siml/preprocessing/siml_scalers/scaler_result_save.py,sha256=9ZD7dibMlteAZvpePfsK5sEAhf4VMadAMclKJpypz54,1012
+siml/preprocessing/siml_scalers/scaler_wrapper.py,sha256=y6A0quhyYilNc9CeWJ8ISHXyKubMXG1rA9L8XN9N7vs,4326
 siml/setting.py,sha256=ntrNdSYLh_QOowJVZT0fMzfQKxz4hTbPFTwB73-Rk6g,49064
 siml/siml_manager.py,sha256=K6Umxl8JFMLWhkSyrHk9dJ7r0luNw-FWXpw6Ue__hIA,11036
+siml/siml_variables/__init__.py,sha256=s5y2hQSp6pQ7Je1sPnnKFQal9-ziX-72RS5HfGH1M_M,147
+siml/siml_variables/array_variables/__init__.py,sha256=Cw7kWo0eEgcqNMUM_6unbgZCyGF4iomSTyCVAgstEog,648
+siml/siml_variables/array_variables/interface_wrapper.py,sha256=Wi0GcuEexwx6sqTqVcBCtWo2K7kw_LQN6LOdoXnNFYw,1573
+siml/siml_variables/array_variables/ndarray_wrapper.py,sha256=oNOfbQu_5twQZq9AM_NEWcbswnCzASAEGzCPpUXcujM,1398
+siml/siml_variables/array_variables/sparce_array_wrapper.py,sha256=oMefInkZwZP8NdClKRcE4m0GoTei7EIw6CEsX7t-cD0,1862
+siml/siml_variables/tensor_variables/tensor_variables.py,sha256=PlsOpq4aMXW8KiBWYOCEIQHHo7KkY4ZqXfoC-j2GqZ4,3509
 siml/study.py,sha256=VsiEuAiwcC0a1voORjic9RcZcnPVJiBowV-mobS6tAQ,13021
-siml/trainer.py,sha256=StgBFmZaJHdMeCdulluL_qRJzD7K_0Sl3uWccfjJSBY,34860
+siml/trainer.py,sha256=4I5a72crf3PGsmnwD8mhDzVcTal8Ag7-OwqFsruTyng,34886
 siml/update_functions/__init__.py,sha256=fQY19xMEhZv7k6flZPBmhIgLl3uHuBWkay-YCFfaY64,211
 siml/update_functions/element_batch_update.py,sha256=93_L9jl4D9lFQXmEX1Lo8l4n3rDf1wdZljPJIQd9rUs,1774
-siml/update_functions/pseudo_batch_update.py,sha256=rmkCSATfWm-0JGaPGNbdBbmizZ7IoXXxr4pVczLwTPo,3590
-siml/update_functions/standard_update.py,sha256=8FRbEEkpI4qwRuRLLqNtbtesSkB5xzx1820zqH2qBhQ,2669
+siml/update_functions/pseudo_batch_update.py,sha256=7PS6SEXOMB57uaJQhZ8VrtEiIkDF59JE1c6yyrKL3YY,3623
+siml/update_functions/standard_update.py,sha256=jIgeQ_c9R1dgcxDQWzx-w5TkJ7naDKmNi_WUFFchxc4,2702
 siml/update_functions/update_interface.py,sha256=O1fGrE21iXckz7NTOTDNlyQ4rll1SQDehdc_Kk5we0Q,429
-siml/util.py,sha256=OI3ve02GZ1iy-H53vI74WGRVXgSYYp7Ibap7BWw6DrU,37201
+siml/util.py,sha256=AzvnYN1svE28ioHGPgMjkpiK35hCA5m5qwFEDb3agHA,23027
 siml/utils/__init__.py,sha256=tVmXHjjriMvU91mYn_MF20FEevUs7QvzHtuiOYttIxY,71
 siml/utils/fem_data_utils.py,sha256=u3mCaTHP2BSvBGBQojmF1TYtwH5XWoefeivgP-iAdcg,6090
 siml/utils/path_utils.py,sha256=nBR68zANQQDUANjvl7noE6aZBMXg7HxErTh3bDJQJko,2147
-siml/variables/__init__.py,sha256=827EnWPECNl5CepRa19l_p7KvR1rx1xk2xgoJFfltVg,58
-siml/variables/siml_variables.py,sha256=sr2ZyrNJuZy-0SQrz173a0qBPcFMNEymQlUXaUscMVo,3487
-pysiml-0.2.8.dev202304200913.dist-info/entry_points.txt,sha256=zXU0Gd56XeUfgaeG-CGXcYaTpORSU6kVeQ_vVvjIFPs,388
-pysiml-0.2.8.dev202304200913.dist-info/LICENSE,sha256=Ok4O8jxCIpLhGZjTNzgBW8V8xITF_SUVEp1juLijZpA,11431
-pysiml-0.2.8.dev202304200913.dist-info/WHEEL,sha256=y3eDiaFVSNTPbgzfNn0nYn5tEn1cX6WrdetDlQM4xWw,83
-pysiml-0.2.8.dev202304200913.dist-info/METADATA,sha256=W5i6LgQOF7u5D1ZDAAuFNLTYJksZHcW0r4KgWISoL9I,1595
-pysiml-0.2.8.dev202304200913.dist-info/RECORD,,
+pysiml-0.2.9.dev202305020647.dist-info/LICENSE,sha256=Ok4O8jxCIpLhGZjTNzgBW8V8xITF_SUVEp1juLijZpA,11431
+pysiml-0.2.9.dev202305020647.dist-info/METADATA,sha256=owgQfXny74uh6H6lgH6WIpgy3P0WalLuxvsYps36ge0,1638
+pysiml-0.2.9.dev202305020647.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+pysiml-0.2.9.dev202305020647.dist-info/entry_points.txt,sha256=zXU0Gd56XeUfgaeG-CGXcYaTpORSU6kVeQ_vVvjIFPs,388
+pysiml-0.2.9.dev202305020647.dist-info/RECORD,,
```

