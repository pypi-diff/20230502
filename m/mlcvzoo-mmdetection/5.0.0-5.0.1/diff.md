# Comparing `tmp/mlcvzoo_mmdetection-5.0.0.tar.gz` & `tmp/mlcvzoo_mmdetection-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_mmdetection-5.0.0.tar", max compression
+gzip compressed data, was "mlcvzoo_mmdetection-5.0.1.tar", max compression
```

## Comparing `mlcvzoo_mmdetection-5.0.0.tar` & `mlcvzoo_mmdetection-5.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      423 2023-02-14 09:45:07.449397 mlcvzoo_mmdetection-5.0.0/README.md
--rw-r--r--   0        0        0      177 2023-02-14 16:02:36.611874 mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/__init__.py
--rw-r--r--   0        0        0     5280 2023-02-14 16:02:36.611874 mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/configuration.py
--rw-r--r--   0        0        0     7641 2023-02-14 09:45:07.449397 mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py
--rw-r--r--   0        0        0    15883 2023-02-14 16:02:36.611874 mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/model.py
--rw-r--r--   0        0        0     6836 2023-02-14 16:02:36.611874 mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/object_detection_model.py
--rw-r--r--   0        0        0      154 2023-02-14 09:45:07.449397 mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/py.typed
--rw-r--r--   0        0        0    11398 2023-02-14 09:45:07.449397 mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/third_party/LICENSE
--rw-r--r--   0        0        0      109 2023-02-14 09:45:07.449397 mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/third_party/README.md
--rw-r--r--   0        0        0      154 2023-02-14 09:45:07.449397 mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/third_party/__init__.py
--rw-r--r--   0        0        0     2623 2023-02-14 09:45:07.449397 mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/third_party/mmdetection.py
--rw-r--r--   0        0        0     2650 2023-02-14 09:45:07.449397 mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/utils.py
--rw-r--r--   0        0        0     3856 2023-02-14 16:55:43.092144 mlcvzoo_mmdetection-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     1582 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-5.0.0/setup.py
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0      423 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/README.md
+-rw-r--r--   0        0        0      177 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/__init__.py
+-rw-r--r--   0        0        0     5279 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/configuration.py
+-rw-r--r--   0        0        0     7641 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py
+-rw-r--r--   0        0        0    15578 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/model.py
+-rw-r--r--   0        0        0     6835 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/object_detection_model.py
+-rw-r--r--   0        0        0      154 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/py.typed
+-rw-r--r--   0        0        0    11398 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/third_party/LICENSE
+-rw-r--r--   0        0        0      109 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/third_party/README.md
+-rw-r--r--   0        0        0      154 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/third_party/__init__.py
+-rw-r--r--   0        0        0     2590 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/third_party/mmdetection.py
+-rw-r--r--   0        0        0     2643 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/utils.py
+-rw-r--r--   0        0        0     3913 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1640 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-5.0.1/setup.py
+-rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-5.0.1/PKG-INFO
```

### Comparing `mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/configuration.py` & `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     cfg_options: Optional[Dict[str, Any]] = related.ChildField(
         cls=dict, default=None, required=False
     )
     # job launcher
     launcher: str = related.StringField(default="none")
 
     def check_values(self) -> bool:
-
         if self.gpus is not None:
             logger.warning(
                 "DEPRECATED: 'gpus' config attributes is deprecated "
                 "because mmdet only supports single GPU mode in non-distributed "
                 "training, use gpu_id instead"
             )
```

### Comparing `mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py` & `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/model.py` & `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,15 @@
 import sys
 import time
 from abc import ABC
 from typing import Any, Callable, Dict, Optional, Tuple, TypeVar
 
 import torch
 import torch.nn
-
-# pylint: disable=protected-access
-from config_builder import __version__ as config_builder_version
-from packaging import version
-
-if version.parse(config_builder_version) >= version.parse("7.0.0"):
-    from config_builder.replacement_map import get_current_replacement_map
-else:
-    from config_builder.replacement_map import (  # type: ignore[attr-defined,no-redef]
-        get_replacement_map_copy as get_current_replacement_map,
-    )
-
+from config_builder.replacement_map import get_current_replacement_map
 from mlcvzoo_base.api.interfaces import NetBased, Trainable
 from mlcvzoo_base.api.model import Model
 from mlcvzoo_base.configuration.class_mapping_config import ClassMappingConfig
 from mlcvzoo_base.configuration.reduction_mapping_config import ReductionMappingConfig
 from mlcvzoo_base.data_preparation.annotation_handler import AnnotationHandler
 from mmcv import Config, runner
 from mmcv.runner import get_dist_info, init_dist, load_checkpoint, set_random_seed
@@ -105,22 +94,24 @@
     def get_checkpoint_filename_suffix(self) -> str:
         return ".pth"
 
     def get_training_output_dir(self) -> str:
         return self.configuration.train_config.argparse_config.work_dir
 
     @staticmethod
-    def _get_framework_imports() -> Tuple[  # type: ignore[type-arg]
-        Callable,
-        Callable,
-        Callable,
-        Callable,
-        Callable,
-        Callable,
-    ]:
+    def _get_framework_imports() -> (
+        Tuple[  # type: ignore[type-arg]
+            Callable,
+            Callable,
+            Callable,
+            Callable,
+            Callable,
+            Callable,
+        ]
+    ):
         from mmdet.apis import init_detector, init_random_seed, train_detector
         from mmdet.datasets import build_dataset
         from mmdet.models import build_detector
         from mmdet.utils import collect_env
 
         return (
             init_detector,
@@ -138,15 +129,14 @@
     @staticmethod
     def _get_framework_version() -> Any:
         from mmdet import __version__ as framework_version
 
         return framework_version
 
     def _build_val_dataset(self, cfg: Config) -> Any:
-
         (
             _,
             _,
             _,
             build_dataset,
             _,
             _,
@@ -156,15 +146,14 @@
         val_dataset.pipeline = cfg.data.train.pipeline
         return build_dataset(val_dataset)
 
     def get_net(self) -> Optional[torch.nn.Module]:
         return self.net
 
     def _init_inference_model(self) -> None:
-
         (
             init_detector,
             _,
             _,
             _,
             _,
             _,
@@ -194,15 +183,14 @@
                 checkpoint_path=self.configuration.inference_config.checkpoint_path
             )
 
     def store(self, checkpoint_path: str) -> None:
         pass
 
     def restore(self, checkpoint_path: str) -> None:
-
         if self.net is None:
             raise ValueError(
                 "In order to restore a checkpoint, the net attribute has"
                 "to be initialized!"
             )
 
         logger.info(
@@ -267,15 +255,14 @@
         logger.info(
             "Saved checkpoint from '%s' in a reduced version to '%s'.",
             input_checkpoint_path,
             output_checkpoint_path,
         )
 
     def train(self) -> None:
-
         if self.configuration.train_config.argparse_config.launcher == "none":
             self._train(
                 argparse_config=self.configuration.train_config.argparse_config,
                 string_replacement_map=self.configuration.string_replacement_map,
                 class_mapping_config=self.configuration.class_mapping,
                 reduction_mapping_config=self.configuration.inference_config.reduction_class_mapping,
             )
@@ -312,37 +299,36 @@
         """
         Run mmdet multi-gpu/distributed training.
 
         Returns:
             None
         """
 
-        cuda_visible_devices = multi_gpu_config.cuda_visible_devices
-        gpus = argparse_config.gpus
-        port = multi_gpu_config.multi_gpu_sync_port
+        if argparse_config.gpu_ids is None:
+            raise ValueError("argparse_config.gpus_ids is None")
 
         env = os.environ.copy()
         env[
             "PYTHONPATH"
         ] = f"{os.environ.get('PYTHONPATH') if os.environ.get('PYTHONPATH') is not None else ''}"
 
-        env["cuda_visible_devices"] = cuda_visible_devices
+        env["cuda_visible_devices"] = multi_gpu_config.cuda_visible_devices
 
         for key, value in get_current_replacement_map().items():
             env[key] = value
 
         _, new_config_path = init_mmdetection_config(
             config_path=argparse_config.config,
             string_replacement_map=string_replacement_map,
         )
 
         command = (
             f"-m torch.distributed.run "
-            f"--nproc_per_node={gpus} "
-            f"--master_port={port} "
+            f"--nproc_per_node={len(argparse_config.gpu_ids)} "
+            f"--master_port={multi_gpu_config.multi_gpu_sync_port} "
             f"{__file__} "
             f"{new_config_path} "
         )
 
         logger.debug("Run command: %s", command)
 
         command_split = [sys.executable]
```

### Comparing `mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/object_detection_model.py` & `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/object_detection_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         self,
         from_yaml: Optional[str] = None,
         configuration: Optional[MMDetectionConfig] = None,
         string_replacement_map: Optional[Dict[str, str]] = None,
         init_for_inference: bool = False,
         is_multi_gpu_instance: bool = False,
     ) -> None:
-
         MMDetectionModel.__init__(
             self,
             from_yaml=from_yaml,
             configuration=configuration,
             string_replacement_map=string_replacement_map,
             init_for_inference=init_for_inference,
             is_multi_gpu_instance=is_multi_gpu_instance,
```

### Comparing `mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/third_party/LICENSE` & `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/third_party/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/third_party/mmdetection.py` & `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/third_party/mmdetection.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     init_random_seed: Callable,  # type: ignore[type-arg]
     set_random_seed: Callable,  # type: ignore[type-arg]
 ) -> Config:
     # set random seeds
     seed = init_random_seed(argparse_config.seed, device=cfg.device)
 
     if argparse_config.diff_seed:
-        seed = seed + dist.get_rank()  # type: ignore[no-untyped-call]
+        seed = seed + dist.get_rank()
     logger.info(
         f"Set random seed to {seed}, " f"deterministic: {argparse_config.deterministic}"
     )
     set_random_seed(
         seed,
         deterministic=argparse_config.deterministic,
     )
```

### Comparing `mlcvzoo_mmdetection-5.0.0/mlcvzoo_mmdetection/utils.py` & `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,39 +18,35 @@
 logger = logging.getLogger(__name__)
 
 
 # TODO: do we really need this method, or is it enough to have "modify_config"
 def init_mmdetection_config(
     config_path: str, string_replacement_map: Dict[str, str]
 ) -> Tuple[Config, str]:
-
     new_config_path = modify_config(
         config_path=config_path, string_replacement_map=string_replacement_map
     )
 
     # Build config provided by mmdetection framework
     logger.info("Load mmdetection config from: %s", new_config_path)
 
     cfg = Config.fromfile(new_config_path)
 
     return cfg, new_config_path
 
 
 def modify_config(config_path: str, string_replacement_map: Dict[str, str]) -> str:
-
     with open(file=config_path, mode="r", encoding="'utf-8") as config_file:
         config_file_content = config_file.readlines()
 
     new_config_file_content = list()
     for config_content in config_file_content:
-
         new_config_content = config_content
 
         for replacement_key, replacement_value in string_replacement_map.items():
-
             if replacement_key in config_content:
                 new_config_content = new_config_content.replace(
                     replacement_key, replacement_value
                 )
 
                 logger.info(
                     "Replace '%s' in config-line '%s' with '%s'",
@@ -67,19 +63,16 @@
 
     return new_config_path
 
 
 def run_str_string_replacement(
     input_string: str, string_replacement_map: Dict[str, str]
 ) -> str:
-
     for replacement_key, replacement_value in string_replacement_map.items():
-
         if replacement_key in input_string:
-
             input_string = input_string.replace(replacement_key, replacement_value)
 
             logger.info(
                 "Replace '%s' in string %s with '%s'",
                 replacement_key,
                 input_string,
                 replacement_value,
```

### Comparing `mlcvzoo_mmdetection-5.0.0/pyproject.toml` & `mlcvzoo_mmdetection-5.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlcvzoo_mmdetection"
-version = "5.0.0"
+version = "5.0.1"
 license = "Open Logistics License Version 1.0"
 description = "MLCVZoo MMDetection Package"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc"
 classifiers = [
@@ -29,38 +29,39 @@
     { include = "mlcvzoo_mmdetection" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 yaml-config-builder = { version = "^8" }
-related-mltoolbox = { version = "^1.0" }
-mlcvzoo_base = { version = "^5.0" }
+related-mltoolbox = { version = "^1" }
+mlcvzoo_base = { version = "^5" }
 
 attrs = { version = ">=20" }
+# 4.6.0.66 leads to errors when building mmcv-full
+opencv-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66" }
+opencv-contrib-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66" }
 mmdet = { version="^2.14.0" }
 mmcv-full = { version="^1.3,!=1.3.18" }
-pycocotools = { version="^2.0.2", markers = "platform_machine == 'x86_64'" }
+pycocotools = { version=">=2.0.2", markers = "platform_machine == 'x86_64'" }
 # 1.19.2 is oldest available on aarch64 but 1.19.5 leads to unbuildable pytorch there, all is well on amd64
 numpy = { version = ">=1.19.2,!=1.19.5" }
-nptyping = { version = "^2.0" }
-torch = { version = "^1.9" }
-torchvision = { version = "^0.10" }
-# TODO: remove when fixed by tensorboard: https://github.com/tensorflow/tensorboard/issues/5703
-protobuf =  {version="<=3.20"}
+nptyping = { version = ">=2.0" }
+torch = { version = ">=1.9" }
+torchvision = { version = ">=0.10" }
 
 [tool.poetry.dev-dependencies]
-mock = { version = "^4.0" }
-pytest = { version = "^7.0" }
-pytest-cov = { version = "^3.0.0" }
-black = { version = "^22" }
+mock = { version = ">=4.0" }
+pytest = { version = ">=7.0" }
+pytest-cov = { version = ">=3.0.0" }
+black = { version = ">=22" }
 mypy = { version = ">=0.961" }
-pylint = { version = "^2.9.6" }
-isort = { version = "^5.9" }
-pytest-mock = "^3.7"
+pylint = { version = ">=2.9.6" }
+isort = { version = ">=5.9" }
+pytest-mock = ">=3.7"
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
 requires = ["setuptools", "poetry_core>=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `mlcvzoo_mmdetection-5.0.0/setup.py` & `mlcvzoo_mmdetection-5.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,31 +5,32 @@
 ['mlcvzoo_mmdetection', 'mlcvzoo_mmdetection.third_party']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['attrs>=20',
- 'mlcvzoo_base>=5.0,<6.0',
+ 'mlcvzoo_base>=5,<6',
  'mmcv-full>=1.3,<2.0,!=1.3.18',
  'mmdet>=2.14.0,<3.0.0',
- 'nptyping>=2.0,<3.0',
+ 'nptyping>=2.0',
  'numpy>=1.19.2,!=1.19.5',
- 'protobuf<=3.20',
- 'related-mltoolbox>=1.0,<2.0',
- 'torch>=1.9,<2.0',
- 'torchvision>=0.10,<0.11',
+ 'opencv-contrib-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66',
+ 'opencv-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66',
+ 'related-mltoolbox>=1,<2',
+ 'torch>=1.9',
+ 'torchvision>=0.10',
  'yaml-config-builder>=8,<9']
 
 extras_require = \
-{':platform_machine == "x86_64"': ['pycocotools>=2.0.2,<3.0.0']}
+{':platform_machine == "x86_64"': ['pycocotools>=2.0.2']}
 
 setup_kwargs = {
     'name': 'mlcvzoo-mmdetection',
-    'version': '5.0.0',
+    'version': '5.0.1',
     'description': 'MLCVZoo MMDetection Package',
     'long_description': '# MLCVZoo MMDetection\n\nThe MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)\ncomputer vision algorithms. The package **mlcvzoo_mmdetection** is the wrapper module for\nthe [mmdetection framework](https://github.com/open-mmlab/mmdetection).\n\nFurther information about the MLCVZoo can be found [here](../README.md).\n\n## Install\n`\npip install mlcvzoo-mmdetection\n`\n\n## Technology stack\n\n- Python\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo',
```

### Comparing `mlcvzoo_mmdetection-5.0.0/PKG-INFO` & `mlcvzoo_mmdetection-5.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-mmdetection
-Version: 5.0.0
+Version: 5.0.1
 Summary: MLCVZoo MMDetection Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 License: Open Logistics License Version 1.0
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,24 +13,25 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=20)
-Requires-Dist: mlcvzoo_base (>=5.0,<6.0)
+Requires-Dist: mlcvzoo_base (>=5,<6)
 Requires-Dist: mmcv-full (>=1.3,<2.0,!=1.3.18)
 Requires-Dist: mmdet (>=2.14.0,<3.0.0)
-Requires-Dist: nptyping (>=2.0,<3.0)
+Requires-Dist: nptyping (>=2.0)
 Requires-Dist: numpy (>=1.19.2,!=1.19.5)
-Requires-Dist: protobuf (<=3.20)
-Requires-Dist: pycocotools (>=2.0.2,<3.0.0) ; platform_machine == "x86_64"
-Requires-Dist: related-mltoolbox (>=1.0,<2.0)
-Requires-Dist: torch (>=1.9,<2.0)
-Requires-Dist: torchvision (>=0.10,<0.11)
+Requires-Dist: opencv-contrib-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66)
+Requires-Dist: opencv-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66)
+Requires-Dist: pycocotools (>=2.0.2) ; platform_machine == "x86_64"
+Requires-Dist: related-mltoolbox (>=1,<2)
+Requires-Dist: torch (>=1.9)
+Requires-Dist: torchvision (>=0.10)
 Requires-Dist: yaml-config-builder (>=8,<9)
 Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc
 Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 Description-Content-Type: text/markdown
 
 # MLCVZoo MMDetection
```

