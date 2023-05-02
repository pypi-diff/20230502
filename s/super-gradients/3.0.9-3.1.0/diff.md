# Comparing `tmp/super_gradients-3.0.9-py3-none-any.whl.zip` & `tmp/super_gradients-3.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,531 +1,560 @@
-Zip file size: 938547 bytes, number of entries: 529
--rw-r--r--  2.0 unx      932 b- defN 23-Apr-19 13:58 super_gradients/__init__.py
--rwxr-xr-x  2.0 unx       44 b- defN 23-Apr-19 13:59 super_gradients/requirements.pro.txt
--rwxr-xr-x  2.0 unx      729 b- defN 23-Apr-19 13:59 super_gradients/requirements.txt
--rw-r--r--  2.0 unx      654 b- defN 23-Apr-19 13:58 super_gradients/train_from_recipe.py
--rw-r--r--  2.0 unx     1098 b- defN 23-Apr-19 13:58 super_gradients/common/__init__.py
--rw-r--r--  2.0 unx    15140 b- defN 23-Apr-19 13:58 super_gradients/common/object_names.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/common/abstractions/__init__.py
--rw-r--r--  2.0 unx      879 b- defN 23-Apr-19 13:58 super_gradients/common/abstractions/abstract_logger.py
--rw-r--r--  2.0 unx     3129 b- defN 23-Apr-19 13:58 super_gradients/common/abstractions/mute_processes.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/common/auto_logging/__init__.py
--rw-r--r--  2.0 unx     4687 b- defN 23-Apr-19 13:58 super_gradients/common/auto_logging/auto_logger.py
--rw-r--r--  2.0 unx     6625 b- defN 23-Apr-19 13:58 super_gradients/common/auto_logging/console_logging.py
--rw-r--r--  2.0 unx      142 b- defN 23-Apr-19 13:58 super_gradients/common/aws_connection/__init__.py
--rw-r--r--  2.0 unx     4182 b- defN 23-Apr-19 13:58 super_gradients/common/aws_connection/aws_connector.py
--rw-r--r--  2.0 unx     7198 b- defN 23-Apr-19 13:58 super_gradients/common/aws_connection/aws_secrets_manager_connector.py
--rw-r--r--  2.0 unx      119 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/__init__.py
--rw-r--r--  2.0 unx      669 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/crash_handler.py
--rw-r--r--  2.0 unx    11775 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/crash_tips.py
--rw-r--r--  2.0 unx      886 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/crash_tips_setup.py
--rw-r--r--  2.0 unx     1740 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/exception.py
--rw-r--r--  2.0 unx     2357 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/exception_monitoring_setup.py
--rw-r--r--  2.0 unx      789 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/utils.py
--rw-r--r--  2.0 unx      140 b- defN 23-Apr-19 13:58 super_gradients/common/data_connection/__init__.py
--rw-r--r--  2.0 unx    17959 b- defN 23-Apr-19 13:58 super_gradients/common/data_connection/s3_connector.py
--rw-r--r--  2.0 unx      325 b- defN 23-Apr-19 13:58 super_gradients/common/data_interface/__init__.py
--rw-r--r--  2.0 unx     9699 b- defN 23-Apr-19 13:58 super_gradients/common/data_interface/adnn_model_repository_data_interface.py
--rw-r--r--  2.0 unx     2050 b- defN 23-Apr-19 13:58 super_gradients/common/data_interface/dataset_data_interface.py
--rw-r--r--  2.0 unx      220 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/__init__.py
--rw-r--r--  2.0 unx      597 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/__init__.py
--rw-r--r--  2.0 unx      309 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/deep_learning_task.py
--rw-r--r--  2.0 unx      108 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/downsample_mode.py
--rw-r--r--  2.0 unx      317 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/evaluation_type.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/multi_gpu_mode.py
--rw-r--r--  2.0 unx     1200 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/strict_load.py
--rw-r--r--  2.0 unx      160 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/upsample_mode.py
--rw-r--r--  2.0 unx      257 b- defN 23-Apr-19 13:58 super_gradients/common/decorators/__init__.py
--rw-r--r--  2.0 unx     1567 b- defN 23-Apr-19 13:58 super_gradients/common/decorators/code_save_decorator.py
--rw-r--r--  2.0 unx     3663 b- defN 23-Apr-19 13:58 super_gradients/common/decorators/deci_logger.py
--rw-r--r--  2.0 unx     2921 b- defN 23-Apr-19 13:58 super_gradients/common/decorators/explicit_params_validator.py
--rw-r--r--  2.0 unx     1315 b- defN 23-Apr-19 13:58 super_gradients/common/decorators/factory_decorator.py
--rw-r--r--  2.0 unx     1132 b- defN 23-Apr-19 13:58 super_gradients/common/decorators/singleton.py
--rw-r--r--  2.0 unx      202 b- defN 23-Apr-19 13:58 super_gradients/common/environment/__init__.py
--rw-r--r--  2.0 unx      993 b- defN 23-Apr-19 13:58 super_gradients/common/environment/argparse_utils.py
--rw-r--r--  2.0 unx     9170 b- defN 23-Apr-19 13:58 super_gradients/common/environment/cfg_utils.py
--rw-r--r--  2.0 unx     4218 b- defN 23-Apr-19 13:58 super_gradients/common/environment/checkpoints_dir_utils.py
--rw-r--r--  2.0 unx     2682 b- defN 23-Apr-19 13:58 super_gradients/common/environment/ddp_utils.py
--rw-r--r--  2.0 unx      752 b- defN 23-Apr-19 13:58 super_gradients/common/environment/device_utils.py
--rw-r--r--  2.0 unx     1147 b- defN 23-Apr-19 13:58 super_gradients/common/environment/env_variables.py
--rw-r--r--  2.0 unx     1768 b- defN 23-Apr-19 13:58 super_gradients/common/environment/omegaconf_utils.py
--rw-r--r--  2.0 unx      459 b- defN 23-Apr-19 13:58 super_gradients/common/environment/path_utils.py
--rw-r--r--  2.0 unx      112 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/__init__.py
--rw-r--r--  2.0 unx      153 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/cpu.py
--rw-r--r--  2.0 unx     2517 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/data_models.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/disk.py
--rw-r--r--  2.0 unx     5427 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/monitoring.py
--rw-r--r--  2.0 unx      948 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/network.py
--rw-r--r--  2.0 unx      629 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/utils.py
--rw-r--r--  2.0 unx      145 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/virtual_memory.py
--rw-r--r--  2.0 unx      681 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/gpu/__init__.py
--rw-r--r--  2.0 unx     2270 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/gpu/gpu.py
--rw-r--r--  2.0 unx   121647 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/gpu/pynvml.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/common/exceptions/__init__.py
--rw-r--r--  2.0 unx      926 b- defN 23-Apr-19 13:58 super_gradients/common/exceptions/factory_exceptions.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/common/factories/__init__.py
--rw-r--r--  2.0 unx     1715 b- defN 23-Apr-19 13:58 super_gradients/common/factories/activations_type_factory.py
--rw-r--r--  2.0 unx     2881 b- defN 23-Apr-19 13:58 super_gradients/common/factories/base_factory.py
--rw-r--r--  2.0 unx      258 b- defN 23-Apr-19 13:58 super_gradients/common/factories/bbox_format_factory.py
--rw-r--r--  2.0 unx      232 b- defN 23-Apr-19 13:58 super_gradients/common/factories/callbacks_factory.py
--rw-r--r--  2.0 unx      263 b- defN 23-Apr-19 13:58 super_gradients/common/factories/collate_functions_factory.py
--rw-r--r--  2.0 unx      292 b- defN 23-Apr-19 13:58 super_gradients/common/factories/context_modules_factory.py
--rw-r--r--  2.0 unx      321 b- defN 23-Apr-19 13:58 super_gradients/common/factories/data_formats_factory.py
--rw-r--r--  2.0 unx      237 b- defN 23-Apr-19 13:58 super_gradients/common/factories/datasets_factory.py
--rw-r--r--  2.0 unx     1014 b- defN 23-Apr-19 13:58 super_gradients/common/factories/detection_modules_factory.py
--rw-r--r--  2.0 unx      572 b- defN 23-Apr-19 13:58 super_gradients/common/factories/list_factory.py
--rw-r--r--  2.0 unx      223 b- defN 23-Apr-19 13:58 super_gradients/common/factories/losses_factory.py
--rw-r--r--  2.0 unx      226 b- defN 23-Apr-19 13:58 super_gradients/common/factories/metrics_factory.py
--rw-r--r--  2.0 unx      467 b- defN 23-Apr-19 13:58 super_gradients/common/factories/optimizers_type_factory.py
--rw-r--r--  2.0 unx      271 b- defN 23-Apr-19 13:58 super_gradients/common/factories/pre_launch_callbacks_factory.py
--rw-r--r--  2.0 unx      623 b- defN 23-Apr-19 13:58 super_gradients/common/factories/processing_factory.py
--rw-r--r--  2.0 unx      229 b- defN 23-Apr-19 13:58 super_gradients/common/factories/samplers_factory.py
--rw-r--r--  2.0 unx      263 b- defN 23-Apr-19 13:58 super_gradients/common/factories/target_generator_factory.py
--rw-r--r--  2.0 unx     1873 b- defN 23-Apr-19 13:58 super_gradients/common/factories/transforms_factory.py
--rw-r--r--  2.0 unx     2377 b- defN 23-Apr-19 13:58 super_gradients/common/factories/type_factory.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/common/plugins/__init__.py
--rw-r--r--  2.0 unx    10974 b- defN 23-Apr-19 13:58 super_gradients/common/plugins/deci_client.py
--rw-r--r--  2.0 unx      271 b- defN 23-Apr-19 13:58 super_gradients/common/registry/__init__.py
--rw-r--r--  2.0 unx     1231 b- defN 23-Apr-19 13:58 super_gradients/common/registry/albumentation.py
--rw-r--r--  2.0 unx     6006 b- defN 23-Apr-19 13:58 super_gradients/common/registry/registry.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/common/registry/registry_utils.py
--rw-r--r--  2.0 unx      409 b- defN 23-Apr-19 13:58 super_gradients/common/sg_loggers/__init__.py
--rw-r--r--  2.0 unx     7355 b- defN 23-Apr-19 13:58 super_gradients/common/sg_loggers/abstract_sg_logger.py
--rw-r--r--  2.0 unx    14980 b- defN 23-Apr-19 13:58 super_gradients/common/sg_loggers/base_sg_logger.py
--rw-r--r--  2.0 unx    10055 b- defN 23-Apr-19 13:58 super_gradients/common/sg_loggers/clearml_sg_logger.py
--rw-r--r--  2.0 unx     6618 b- defN 23-Apr-19 13:58 super_gradients/common/sg_loggers/deci_platform_sg_logger.py
--rw-r--r--  2.0 unx    13073 b- defN 23-Apr-19 13:58 super_gradients/common/sg_loggers/wandb_sg_logger.py
--rw-r--r--  2.0 unx    85509 b- defN 23-Apr-19 13:58 super_gradients/examples/SG_Walkthrough.ipynb
--rw-r--r--  2.0 unx    69618 b- defN 23-Apr-19 13:58 super_gradients/examples/SG_quickstart_classification.ipynb
--rw-r--r--  2.0 unx    54966 b- defN 23-Apr-19 13:58 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb
--rw-r--r--  2.0 unx    65090 b- defN 23-Apr-19 13:58 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/cifar10_training_torch_objects/__init__.py
--rw-r--r--  2.0 unx     2526 b- defN 23-Apr-19 13:58 super_gradients/examples/cifar10_training_torch_objects/cifar10_training_torch_objects_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/convert_recipe_example/__init__.py
--rw-r--r--  2.0 unx      870 b- defN 23-Apr-19 13:58 super_gradients/examples/convert_recipe_example/convert_recipe_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/ddrnet_imagenet/__init__.py
--rw-r--r--  2.0 unx     3114 b- defN 23-Apr-19 13:58 super_gradients/examples/ddrnet_imagenet/ddrnet_classification_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/deci_lab_export_example/__init__.py
--rw-r--r--  2.0 unx     3562 b- defN 23-Apr-19 13:58 super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/early_stop/__init__.py
--rw-r--r--  2.0 unx     1596 b- defN 23-Apr-19 13:58 super_gradients/examples/early_stop/early_stop_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/evaluate_checkpoint_example/__init__.py
--rw-r--r--  2.0 unx     1683 b- defN 23-Apr-19 13:58 super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/evaluate_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx     1779 b- defN 23-Apr-19 13:58 super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/loggers_examples/__init__.py
--rw-r--r--  2.0 unx     1206 b- defN 23-Apr-19 13:58 super_gradients/examples/loggers_examples/clearml_logger_example.py
--rw-r--r--  2.0 unx     1088 b- defN 23-Apr-19 13:58 super_gradients/examples/loggers_examples/deci_platform_logger_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/qat_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      700 b- defN 23-Apr-19 13:58 super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/__init__.py
--rw-r--r--  2.0 unx     1104 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/non_default_calibrators_example.py
--rw-r--r--  2.0 unx     2310 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/ptq_e2e_example.py
--rw-r--r--  2.0 unx     1850 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/register_quantization_mapping_with_decorator_example.py
--rw-r--r--  2.0 unx     4923 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/resnet_qat_example.py
--rw-r--r--  2.0 unx     1163 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/skipping_quantization_example.py
--rw-r--r--  2.0 unx      832 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/vanilla_quantize_all_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/regseg_transfer_learning_example/__init__.py
--rw-r--r--  2.0 unx     2379 b- defN 23-Apr-19 13:58 super_gradients/examples/regseg_transfer_learning_example/regseg_transfer_learning_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/resume_experiment_example/__init__.py
--rw-r--r--  2.0 unx      534 b- defN 23-Apr-19 13:58 super_gradients/examples/resume_experiment_example/resume_experiment.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_kd_recipe_example/__init__.py
--rw-r--r--  2.0 unx      655 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      627 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_example/train_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_with_dataset_registry/__init__.py
--rw-r--r--  2.0 unx     1334 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_with_dataset_registry/train.py
--rw-r--r--  2.0 unx     1643 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_with_dataset_registry/user_dataset.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_with_user_objects/__init__.py
--rw-r--r--  2.0 unx     1326 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_with_user_objects/train.py
--rw-r--r--  2.0 unx     2548 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py
--rw-r--r--  2.0 unx      118 b- defN 23-Apr-19 13:58 super_gradients/module_interfaces/__init__.py
--rw-r--r--  2.0 unx      958 b- defN 23-Apr-19 13:58 super_gradients/module_interfaces/module_interfaces.py
--rw-r--r--  2.0 unx     2589 b- defN 23-Apr-19 13:58 super_gradients/modules/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/modules/all_detection_modules.py
--rw-r--r--  2.0 unx      617 b- defN 23-Apr-19 13:58 super_gradients/modules/anti_alias.py
--rw-r--r--  2.0 unx     2073 b- defN 23-Apr-19 13:58 super_gradients/modules/conv_bn_act_block.py
--rw-r--r--  2.0 unx     1976 b- defN 23-Apr-19 13:58 super_gradients/modules/conv_bn_relu_block.py
--rw-r--r--  2.0 unx    15129 b- defN 23-Apr-19 13:58 super_gradients/modules/detection_modules.py
--rw-r--r--  2.0 unx     4362 b- defN 23-Apr-19 13:58 super_gradients/modules/multi_output_modules.py
--rw-r--r--  2.0 unx     3958 b- defN 23-Apr-19 13:58 super_gradients/modules/pose_estimation_modules.py
--rw-r--r--  2.0 unx    11642 b- defN 23-Apr-19 13:58 super_gradients/modules/qarepvgg_block.py
--rw-r--r--  2.0 unx     8544 b- defN 23-Apr-19 13:58 super_gradients/modules/repvgg_block.py
--rw-r--r--  2.0 unx     1887 b- defN 23-Apr-19 13:58 super_gradients/modules/sampling.py
--rw-r--r--  2.0 unx     1459 b- defN 23-Apr-19 13:58 super_gradients/modules/se_blocks.py
--rw-r--r--  2.0 unx     1403 b- defN 23-Apr-19 13:58 super_gradients/modules/skip_connections.py
--rw-r--r--  2.0 unx     2565 b- defN 23-Apr-19 13:58 super_gradients/modules/utils.py
--rw-r--r--  2.0 unx      716 b- defN 23-Apr-19 13:58 super_gradients/modules/quantization/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 23-Apr-19 13:58 super_gradients/modules/quantization/quantized_skip_connections.py
--rw-r--r--  2.0 unx     4604 b- defN 23-Apr-19 13:58 super_gradients/modules/quantization/quantized_stdc_blocks.py
--rw-r--r--  2.0 unx     1281 b- defN 23-Apr-19 13:58 super_gradients/modules/quantization/resnet_bottleneck.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/recipes/__init__.py
--rw-r--r--  2.0 unx     1516 b- defN 23-Apr-19 13:58 super_gradients/recipes/cifar10_resnet.yaml
--rw-r--r--  2.0 unx     3856 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_ddrnet.yaml
--rw-r--r--  2.0 unx     4072 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_kd_base.yaml
--rw-r--r--  2.0 unx     3615 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_pplite_seg50.yaml
--rw-r--r--  2.0 unx     3514 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_pplite_seg75.yaml
--rw-r--r--  2.0 unx     2771 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_regseg48.yaml
--rw-r--r--  2.0 unx     4293 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_segformer.yaml
--rw-r--r--  2.0 unx      852 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_stdc_base.yaml
--rw-r--r--  2.0 unx     3175 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_stdc_seg50.yaml
--rw-r--r--  2.0 unx     3369 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_stdc_seg75.yaml
--rw-r--r--  2.0 unx     2063 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_pose_ddrnet39.yaml
--rw-r--r--  2.0 unx     3821 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml
--rw-r--r--  2.0 unx     2231 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_pose_pppose_l.yaml
--rw-r--r--  2.0 unx     2388 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_ppyoloe_l.yaml
--rw-r--r--  2.0 unx     2388 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_ppyoloe_m.yaml
--rw-r--r--  2.0 unx     2274 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_ppyoloe_s.yaml
--rw-r--r--  2.0 unx     2367 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_ppyoloe_x.yaml
--rw-r--r--  2.0 unx     2202 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml
--rw-r--r--  2.0 unx     3053 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_yolox.yaml
--rw-r--r--  2.0 unx     1649 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml
--rw-r--r--  2.0 unx     1418 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_efficientnet.yaml
--rw-r--r--  2.0 unx     1402 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_mobilenetv2.yaml
--rw-r--r--  2.0 unx      741 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_mobilenetv3_base.yaml
--rw-r--r--  2.0 unx      992 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_mobilenetv3_large.yaml
--rw-r--r--  2.0 unx      992 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_mobilenetv3_small.yaml
--rw-r--r--  2.0 unx     2387 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_regnetY.yaml
--rw-r--r--  2.0 unx     1519 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_repvgg.yaml
--rw-r--r--  2.0 unx     1442 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_resnet50.yaml
--rw-r--r--  2.0 unx     2998 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_resnet50_kd.yaml
--rw-r--r--  2.0 unx     1409 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_vit_base.yaml
--rw-r--r--  2.0 unx     1283 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_vit_large.yaml
--rw-r--r--  2.0 unx     2226 b- defN 23-Apr-19 13:58 super_gradients/recipes/roboflow_ppyoloe.yaml
--rw-r--r--  2.0 unx     2134 b- defN 23-Apr-19 13:58 super_gradients/recipes/roboflow_yolox.yaml
--rw-r--r--  2.0 unx     1520 b- defN 23-Apr-19 13:58 super_gradients/recipes/supervisely_unet.yaml
--rw-r--r--  2.0 unx     1906 b- defN 23-Apr-19 13:58 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
--rw-r--r--  2.0 unx     2367 b- defN 23-Apr-19 13:58 super_gradients/recipes/user_recipe_mnist_example.yaml
--rw-r--r--  2.0 unx     2222 b- defN 23-Apr-19 13:58 super_gradients/recipes/anchors/ssd_anchors.yaml
--rw-r--r--  2.0 unx      563 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml
--rw-r--r--  2.0 unx      104 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b1_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b2_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b3_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b4_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b5_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b6_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b7_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b8_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_l2_arch_params.yaml
--rw-r--r--  2.0 unx      194 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/mobilenet_v2_arch_params.yaml
--rw-r--r--  2.0 unx      156 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/mobilenet_v3_arch_params.yaml
--rw-r--r--  2.0 unx      409 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml
--rw-r--r--  2.0 unx      356 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml
--rw-r--r--  2.0 unx      281 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/pose_ddrnet39_arch_params.yaml
--rw-r--r--  2.0 unx     1245 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml
--rw-r--r--  2.0 unx      985 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml
--rw-r--r--  2.0 unx     1112 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ppyoloe_arch_params.yaml
--rw-r--r--  2.0 unx      196 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ppyoloe_l_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ppyoloe_m_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ppyoloe_s_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ppyoloe_x_arch_params.yaml
--rw-r--r--  2.0 unx      204 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/regnetY_arch_params.yaml
--rw-r--r--  2.0 unx      352 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvgg_arch_params.yaml
--rw-r--r--  2.0 unx       98 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvgga0_arch_params.yaml
--rw-r--r--  2.0 unx       89 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvgga1_arch_params.yaml
--rw-r--r--  2.0 unx       95 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvgga2_arch_params.yaml
--rw-r--r--  2.0 unx       88 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvggb0_arch_params.yaml
--rw-r--r--  2.0 unx       86 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvggb1_arch_params.yaml
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvggb2_arch_params.yaml
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/resnet18_cifar_arch_params.yaml
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/resnet50_arch_params.yaml
--rw-r--r--  2.0 unx       32 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/shelfnet34_lw_arch_params.yaml
--rw-r--r--  2.0 unx      655 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ssd_lite_mobilenetv2_arch_params.yaml
--rw-r--r--  2.0 unx      605 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ssd_mobilenetv1_arch_params.yaml
--rw-r--r--  2.0 unx     1369 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/unet_arch_params.yaml
--rw-r--r--  2.0 unx     3014 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/unet_default_arch_params.yaml
--rw-r--r--  2.0 unx       63 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/vit_base_arch_params.yaml
--rw-r--r--  2.0 unx     2393 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolo_arch_params.yaml
--rw-r--r--  2.0 unx      235 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolox_s_arch_params.yaml
--rw-r--r--  2.0 unx      229 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml
--rw-r--r--  2.0 unx      228 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml
--rw-r--r--  2.0 unx      611 b- defN 23-Apr-19 13:58 super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml
--rw-r--r--  2.0 unx       72 b- defN 23-Apr-19 13:58 super_gradients/recipes/checkpoint_params/vit_base_imagenet_checkpoint_params.yaml
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/recipes/conversion_params/__init__.py
--rw-r--r--  2.0 unx     1807 b- defN 23-Apr-19 13:58 super_gradients/recipes/conversion_params/cifar10_conversion_params.yaml
--rw-r--r--  2.0 unx     2040 b- defN 23-Apr-19 13:58 super_gradients/recipes/conversion_params/default_conversion_params.yaml
--rw-r--r--  2.0 unx      869 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cifar100_dataset_params.yaml
--rw-r--r--  2.0 unx     1530 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml
--rw-r--r--  2.0 unx     1056 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml
--rw-r--r--  2.0 unx      615 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml
--rw-r--r--  2.0 unx      525 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml
--rw-r--r--  2.0 unx      706 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml
--rw-r--r--  2.0 unx      644 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml
--rw-r--r--  2.0 unx      721 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml
--rw-r--r--  2.0 unx      709 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml
--rw-r--r--  2.0 unx      708 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml
--rw-r--r--  2.0 unx     3946 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml
--rw-r--r--  2.0 unx     3661 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_detection_deci_yolo_dataset_params.yaml
--rw-r--r--  2.0 unx     4202 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml
--rw-r--r--  2.0 unx     3590 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml
--rw-r--r--  2.0 unx     2461 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml
--rw-r--r--  2.0 unx      405 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml
--rw-r--r--  2.0 unx     1466 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx      931 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml
--rw-r--r--  2.0 unx      732 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml
--rw-r--r--  2.0 unx      794 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml
--rw-r--r--  2.0 unx      142 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml
--rw-r--r--  2.0 unx      734 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_regnetY_dataset_params.yaml
--rw-r--r--  2.0 unx     1059 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml
--rw-r--r--  2.0 unx     1093 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml
--rw-r--r--  2.0 unx      845 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml
--rw-r--r--  2.0 unx     1762 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml
--rw-r--r--  2.0 unx      149 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx     1571 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml
--rw-r--r--  2.0 unx     1414 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx     3398 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml
--rw-r--r--  2.0 unx      961 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml
--rw-r--r--  2.0 unx      559 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml
--rw-r--r--  2.0 unx     1155 b- defN 23-Apr-19 13:58 super_gradients/recipes/quantization_params/default_quantization_params.yaml
--rw-r--r--  2.0 unx      591 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml
--rw-r--r--  2.0 unx      700 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml
--rw-r--r--  2.0 unx      877 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml
--rw-r--r--  2.0 unx     1302 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml
--rw-r--r--  2.0 unx      723 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml
--rw-r--r--  2.0 unx      956 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml
--rw-r--r--  2.0 unx      461 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml
--rw-r--r--  2.0 unx     5459 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/default_train_params.yaml
--rw-r--r--  2.0 unx      794 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml
--rw-r--r--  2.0 unx      742 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml
--rw-r--r--  2.0 unx      549 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml
--rw-r--r--  2.0 unx      795 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml
--rw-r--r--  2.0 unx      476 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_repvgg_train_params.yaml
--rw-r--r--  2.0 unx      484 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_resnet50_kd_train_params.yaml
--rw-r--r--  2.0 unx      522 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml
--rw-r--r--  2.0 unx      602 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml
--rw-r--r--  2.0 unx      519 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml
--rw-r--r--  2.0 unx      107 b- defN 23-Apr-19 13:58 super_gradients/sanity_check/__init__.py
--rw-r--r--  2.0 unx     5262 b- defN 23-Apr-19 13:58 super_gradients/sanity_check/env_sanity_check.py
--rw-r--r--  2.0 unx      666 b- defN 23-Apr-19 13:58 super_gradients/training/__init__.py
--rw-r--r--  2.0 unx     4155 b- defN 23-Apr-19 13:58 super_gradients/training/params.py
--rw-r--r--  2.0 unx     5696 b- defN 23-Apr-19 13:58 super_gradients/training/pretrained_models.py
--rw-r--r--  2.0 unx     3228 b- defN 23-Apr-19 13:58 super_gradients/training/dataloaders/__init__.py
--rw-r--r--  2.0 unx    31443 b- defN 23-Apr-19 13:58 super_gradients/training/dataloaders/dataloaders.py
--rw-r--r--  2.0 unx     1811 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/__init__.py
--rw-r--r--  2.0 unx    14162 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/auto_augment.py
--rw-r--r--  2.0 unx     3705 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_augmentation.py
--rw-r--r--  2.0 unx     3484 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/datasets_conf.py
--rw-r--r--  2.0 unx    30279 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/datasets_utils.py
--rw-r--r--  2.0 unx    14663 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/mixup.py
--rw-r--r--  2.0 unx    11746 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/sg_dataset.py
--rw-r--r--  2.0 unx      252 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/classification_datasets/__init__.py
--rw-r--r--  2.0 unx     3096 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/classification_datasets/cifar.py
--rw-r--r--  2.0 unx     1706 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py
--rw-r--r--  2.0 unx      862 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/__init__.py
--rw-r--r--  2.0 unx     3927 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/default_formats.py
--rw-r--r--  2.0 unx     3071 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/format_converter.py
--rw-r--r--  2.0 unx     7928 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/formats.py
--rw-r--r--  2.0 unx     1044 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/__init__.py
--rw-r--r--  2.0 unx     2674 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/bbox_format.py
--rw-r--r--  2.0 unx     5094 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py
--rw-r--r--  2.0 unx     2089 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/normalized_cxcywh.py
--rw-r--r--  2.0 unx     2043 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xywh.py
--rw-r--r--  2.0 unx     5043 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xyxy.py
--rw-r--r--  2.0 unx     2948 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py
--rw-r--r--  2.0 unx      575 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py
--rw-r--r--  2.0 unx     1792 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/output_adapters/__init__.py
--rw-r--r--  2.0 unx     8373 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py
--rw-r--r--  2.0 unx      683 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/__init__.py
--rw-r--r--  2.0 unx     2505 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/coco_detection.py
--rw-r--r--  2.0 unx     9258 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/coco_format_detection.py
--rw-r--r--  2.0 unx    25694 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/detection_dataset.py
--rw-r--r--  2.0 unx    11353 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py
--rw-r--r--  2.0 unx    10390 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/yolo_format_detection.py
--rw-r--r--  2.0 unx      328 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/roboflow/__init__.py
--rw-r--r--  2.0 unx    18882 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/roboflow/metadata.py
--rw-r--r--  2.0 unx     3504 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py
--rw-r--r--  2.0 unx     1997 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/roboflow/utils.py
--rw-r--r--  2.0 unx      502 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/pose_estimation_datasets/__init__.py
--rw-r--r--  2.0 unx     4910 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py
--rw-r--r--  2.0 unx     9066 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py
--rw-r--r--  2.0 unx     5929 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py
--rw-r--r--  2.0 unx    10167 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py
--rw-r--r--  2.0 unx      385 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/samplers/__init__.py
--rw-r--r--  2.0 unx     2516 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/samplers/infinite_sampler.py
--rw-r--r--  2.0 unx     4809 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py
--rw-r--r--  2.0 unx     1037 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/__init__.py
--rw-r--r--  2.0 unx     6714 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py
--rw-r--r--  2.0 unx     7717 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py
--rw-r--r--  2.0 unx     5518 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py
--rw-r--r--  2.0 unx    11146 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py
--rw-r--r--  2.0 unx     8470 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py
--rw-r--r--  2.0 unx     3062 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/exceptions/__init__.py
--rw-r--r--  2.0 unx     1761 b- defN 23-Apr-19 13:58 super_gradients/training/exceptions/dataset_exceptions.py
--rw-r--r--  2.0 unx     2826 b- defN 23-Apr-19 13:58 super_gradients/training/exceptions/kd_trainer_exceptions.py
--rw-r--r--  2.0 unx      946 b- defN 23-Apr-19 13:58 super_gradients/training/exceptions/loss_exceptions.py
--rw-r--r--  2.0 unx     1268 b- defN 23-Apr-19 13:58 super_gradients/training/exceptions/sg_trainer_exceptions.py
--rw-r--r--  2.0 unx      132 b- defN 23-Apr-19 13:58 super_gradients/training/kd_trainer/__init__.py
--rw-r--r--  2.0 unx    16582 b- defN 23-Apr-19 13:58 super_gradients/training/kd_trainer/kd_trainer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/legacy/__init__.py
--rw-r--r--  2.0 unx     4198 b- defN 23-Apr-19 13:58 super_gradients/training/legacy/utils.py
--rw-r--r--  2.0 unx     1476 b- defN 23-Apr-19 13:58 super_gradients/training/losses/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/losses/all_losses.py
--rw-r--r--  2.0 unx     1219 b- defN 23-Apr-19 13:58 super_gradients/training/losses/bce_dice_loss.py
--rw-r--r--  2.0 unx      419 b- defN 23-Apr-19 13:58 super_gradients/training/losses/bce_loss.py
--rw-r--r--  2.0 unx     2374 b- defN 23-Apr-19 13:58 super_gradients/training/losses/cwd_loss.py
--rw-r--r--  2.0 unx     2525 b- defN 23-Apr-19 13:58 super_gradients/training/losses/ddrnet_loss.py
--rw-r--r--  2.0 unx     3377 b- defN 23-Apr-19 13:58 super_gradients/training/losses/dekr_loss.py
--rw-r--r--  2.0 unx     5618 b- defN 23-Apr-19 13:58 super_gradients/training/losses/dice_ce_edge_loss.py
--rw-r--r--  2.0 unx     5208 b- defN 23-Apr-19 13:58 super_gradients/training/losses/dice_loss.py
--rw-r--r--  2.0 unx     1214 b- defN 23-Apr-19 13:58 super_gradients/training/losses/focal_loss.py
--rw-r--r--  2.0 unx     5051 b- defN 23-Apr-19 13:58 super_gradients/training/losses/iou_loss.py
--rw-r--r--  2.0 unx     2176 b- defN 23-Apr-19 13:58 super_gradients/training/losses/kd_losses.py
--rw-r--r--  2.0 unx     4177 b- defN 23-Apr-19 13:58 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py
--rw-r--r--  2.0 unx      550 b- defN 23-Apr-19 13:58 super_gradients/training/losses/loss_utils.py
--rw-r--r--  2.0 unx     3854 b- defN 23-Apr-19 13:58 super_gradients/training/losses/mask_loss.py
--rw-r--r--  2.0 unx     4129 b- defN 23-Apr-19 13:58 super_gradients/training/losses/ohem_ce_loss.py
--rw-r--r--  2.0 unx    41319 b- defN 23-Apr-19 13:58 super_gradients/training/losses/ppyolo_loss.py
--rw-r--r--  2.0 unx     1010 b- defN 23-Apr-19 13:58 super_gradients/training/losses/r_squared_loss.py
--rw-r--r--  2.0 unx     3453 b- defN 23-Apr-19 13:58 super_gradients/training/losses/seg_kd_loss.py
--rw-r--r--  2.0 unx     1650 b- defN 23-Apr-19 13:58 super_gradients/training/losses/shelfnet_ohem_loss.py
--rw-r--r--  2.0 unx     1949 b- defN 23-Apr-19 13:58 super_gradients/training/losses/shelfnet_semantic_encoding_loss.py
--rw-r--r--  2.0 unx     8794 b- defN 23-Apr-19 13:58 super_gradients/training/losses/ssd_loss.py
--rw-r--r--  2.0 unx     9721 b- defN 23-Apr-19 13:58 super_gradients/training/losses/stdc_loss.py
--rw-r--r--  2.0 unx     5771 b- defN 23-Apr-19 13:58 super_gradients/training/losses/structure_loss.py
--rw-r--r--  2.0 unx    50149 b- defN 23-Apr-19 13:58 super_gradients/training/losses/yolox_loss.py
--rw-r--r--  2.0 unx     1052 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/all_metrics.py
--rw-r--r--  2.0 unx     3262 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/classification_metrics.py
--rw-r--r--  2.0 unx    10741 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/detection_metrics.py
--rw-r--r--  2.0 unx     3973 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/metric_utils.py
--rw-r--r--  2.0 unx    15346 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/pose_estimation_metrics.py
--rw-r--r--  2.0 unx    11454 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/pose_estimation_utils.py
--rw-r--r--  2.0 unx    11935 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/segmentation_metrics.py
--rw-r--r--  2.0 unx     8368 b- defN 23-Apr-19 13:58 super_gradients/training/models/__init__.py
--rw-r--r--  2.0 unx     1226 b- defN 23-Apr-19 13:58 super_gradients/training/models/arch_params_factory.py
--rw-r--r--  2.0 unx     7060 b- defN 23-Apr-19 13:58 super_gradients/training/models/conversion.py
--rw-r--r--  2.0 unx    11875 b- defN 23-Apr-19 13:58 super_gradients/training/models/model_factory.py
--rw-r--r--  2.0 unx    10850 b- defN 23-Apr-19 13:58 super_gradients/training/models/prediction_results.py
--rw-r--r--  2.0 unx     2054 b- defN 23-Apr-19 13:58 super_gradients/training/models/predictions.py
--rw-r--r--  2.0 unx     2998 b- defN 23-Apr-19 13:58 super_gradients/training/models/sg_module.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/__init__.py
--rw-r--r--  2.0 unx    20025 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/beit.py
--rw-r--r--  2.0 unx     7472 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/densenet.py
--rw-r--r--  2.0 unx     3707 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/dpn.py
--rw-r--r--  2.0 unx    36745 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/efficientnet.py
--rw-r--r--  2.0 unx     8862 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/googlenet.py
--rw-r--r--  2.0 unx      798 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/lenet.py
--rw-r--r--  2.0 unx     2407 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/mobilenet.py
--rw-r--r--  2.0 unx     9472 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/mobilenetv2.py
--rw-r--r--  2.0 unx     8696 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/mobilenetv3.py
--rw-r--r--  2.0 unx     4339 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/pnasnet.py
--rw-r--r--  2.0 unx     4209 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/preact_resnet.py
--rw-r--r--  2.0 unx    13599 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/regnet.py
--rw-r--r--  2.0 unx     7924 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/repvgg.py
--rw-r--r--  2.0 unx    15042 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/resnet.py
--rw-r--r--  2.0 unx     6294 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/resnext.py
--rw-r--r--  2.0 unx     4134 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/senet.py
--rw-r--r--  2.0 unx     3660 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/shufflenet.py
--rw-r--r--  2.0 unx     9768 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/shufflenetv2.py
--rw-r--r--  2.0 unx     1538 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/vgg.py
--rw-r--r--  2.0 unx     9210 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/vit.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/__init__.py
--rw-r--r--  2.0 unx     9502 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/csp_darknet53.py
--rw-r--r--  2.0 unx     9814 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/csp_resnet.py
--rw-r--r--  2.0 unx     8784 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/customizable_detector.py
--rw-r--r--  2.0 unx     4746 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/darknet53.py
--rw-r--r--  2.0 unx     2315 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/ssd.py
--rw-r--r--  2.0 unx    29459 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/yolo_base.py
--rw-r--r--  2.0 unx     2459 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/yolox.py
--rw-r--r--  2.0 unx      155 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py
--rw-r--r--  2.0 unx     6984 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/pp_yolo_e/pan.py
--rw-r--r--  2.0 unx     3487 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py
--rw-r--r--  2.0 unx     8240 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py
--rw-r--r--  2.0 unx    12334 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/models/kd_modules/__init__.py
--rw-r--r--  2.0 unx     3553 b- defN 23-Apr-19 13:58 super_gradients/training/models/kd_modules/kd_module.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/models/pose_estimation_models/__init__.py
--rw-r--r--  2.0 unx    21231 b- defN 23-Apr-19 13:58 super_gradients/training/models/pose_estimation_models/dekr_hrnet.py
--rw-r--r--  2.0 unx     1294 b- defN 23-Apr-19 13:58 super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py
--rw-r--r--  2.0 unx     1335 b- defN 23-Apr-19 13:58 super_gradients/training/models/pose_estimation_models/pose_ppyolo.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/__init__.py
--rw-r--r--  2.0 unx      964 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/common.py
--rw-r--r--  2.0 unx     5139 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/context_modules.py
--rw-r--r--  2.0 unx    27896 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/ddrnet.py
--rw-r--r--  2.0 unx     2439 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/ddrnet_backbones.py
--rw-r--r--  2.0 unx    21760 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/laddernet.py
--rw-r--r--  2.0 unx    15648 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/ppliteseg.py
--rw-r--r--  2.0 unx    14424 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/regseg.py
--rw-r--r--  2.0 unx    20334 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/segformer.py
--rw-r--r--  2.0 unx     2256 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/segmentation_module.py
--rw-r--r--  2.0 unx    24833 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/shelfnet.py
--rw-r--r--  2.0 unx    29005 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/stdc.py
--rw-r--r--  2.0 unx      260 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/unet/__init__.py
--rw-r--r--  2.0 unx    12324 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/unet/unet.py
--rw-r--r--  2.0 unx     8305 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/unet/unet_decoder.py
--rw-r--r--  2.0 unx    13292 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/unet/unet_encoder.py
--rw-r--r--  2.0 unx      119 b- defN 23-Apr-19 13:58 super_gradients/training/models/user_models/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/pipelines/__init__.py
--rw-r--r--  2.0 unx    14399 b- defN 23-Apr-19 13:58 super_gradients/training/pipelines/pipelines.py
--rw-r--r--  2.0 unx      393 b- defN 23-Apr-19 13:58 super_gradients/training/pre_launch_callbacks/__init__.py
--rw-r--r--  2.0 unx    13955 b- defN 23-Apr-19 13:58 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py
--rw-r--r--  2.0 unx      517 b- defN 23-Apr-19 13:58 super_gradients/training/processing/__init__.py
--rw-r--r--  2.0 unx    13178 b- defN 23-Apr-19 13:58 super_gradients/training/processing/processing.py
--rw-r--r--  2.0 unx       98 b- defN 23-Apr-19 13:58 super_gradients/training/qat_trainer/__init__.py
--rw-r--r--  2.0 unx     9896 b- defN 23-Apr-19 13:58 super_gradients/training/qat_trainer/qat_trainer.py
--rw-r--r--  2.0 unx      184 b- defN 23-Apr-19 13:58 super_gradients/training/sg_trainer/__init__.py
--rw-r--r--  2.0 unx    97370 b- defN 23-Apr-19 13:58 super_gradients/training/sg_trainer/sg_trainer.py
--rw-r--r--  2.0 unx     1685 b- defN 23-Apr-19 13:58 super_gradients/training/training_hyperparams/__init__.py
--rw-r--r--  2.0 unx     3774 b- defN 23-Apr-19 13:58 super_gradients/training/training_hyperparams/training_hyperparams.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Apr-19 13:58 super_gradients/training/transforms/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/transforms/all_transforms.py
--rw-r--r--  2.0 unx    16193 b- defN 23-Apr-19 13:58 super_gradients/training/transforms/keypoint_transforms.py
--rw-r--r--  2.0 unx     1134 b- defN 23-Apr-19 13:58 super_gradients/training/transforms/pipeline_adaptors.py
--rw-r--r--  2.0 unx    55085 b- defN 23-Apr-19 13:58 super_gradients/training/transforms/transforms.py
--rw-r--r--  2.0 unx     6048 b- defN 23-Apr-19 13:58 super_gradients/training/transforms/utils.py
--rw-r--r--  2.0 unx     1104 b- defN 23-Apr-19 13:58 super_gradients/training/utils/__init__.py
--rw-r--r--  2.0 unx     1673 b- defN 23-Apr-19 13:58 super_gradients/training/utils/activations_utils.py
--rw-r--r--  2.0 unx     1111 b- defN 23-Apr-19 13:58 super_gradients/training/utils/bbox_utils.py
--rw-r--r--  2.0 unx    14834 b- defN 23-Apr-19 13:58 super_gradients/training/utils/checkpoint_utils.py
--rw-r--r--  2.0 unx     9794 b- defN 23-Apr-19 13:58 super_gradients/training/utils/config_utils.py
--rw-r--r--  2.0 unx     1132 b- defN 23-Apr-19 13:58 super_gradients/training/utils/deprecated_utils.py
--rw-r--r--  2.0 unx    53611 b- defN 23-Apr-19 13:58 super_gradients/training/utils/detection_utils.py
--rw-r--r--  2.0 unx    16195 b- defN 23-Apr-19 13:58 super_gradients/training/utils/distributed_training_utils.py
--rw-r--r--  2.0 unx     6352 b- defN 23-Apr-19 13:58 super_gradients/training/utils/early_stopping.py
--rw-r--r--  2.0 unx     9322 b- defN 23-Apr-19 13:58 super_gradients/training/utils/ema.py
--rw-r--r--  2.0 unx     2610 b- defN 23-Apr-19 13:58 super_gradients/training/utils/ema_decay_schedules.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Apr-19 13:58 super_gradients/training/utils/export_utils.py
--rw-r--r--  2.0 unx     7508 b- defN 23-Apr-19 13:58 super_gradients/training/utils/get_model_stats.py
--rw-r--r--  2.0 unx      771 b- defN 23-Apr-19 13:58 super_gradients/training/utils/kd_trainer_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/utils/load_image.py
--rw-r--r--  2.0 unx     5827 b- defN 23-Apr-19 13:58 super_gradients/training/utils/optimizer_utils.py
--rw-r--r--  2.0 unx      839 b- defN 23-Apr-19 13:58 super_gradients/training/utils/regularization_utils.py
--rw-r--r--  2.0 unx    10388 b- defN 23-Apr-19 13:58 super_gradients/training/utils/segmentation_utils.py
--rw-r--r--  2.0 unx    19625 b- defN 23-Apr-19 13:58 super_gradients/training/utils/sg_trainer_utils.py
--rw-r--r--  2.0 unx     6272 b- defN 23-Apr-19 13:58 super_gradients/training/utils/ssd_utils.py
--rw-r--r--  2.0 unx    18273 b- defN 23-Apr-19 13:58 super_gradients/training/utils/utils.py
--rw-r--r--  2.0 unx      303 b- defN 23-Apr-19 13:58 super_gradients/training/utils/version_utils.py
--rw-r--r--  2.0 unx     6209 b- defN 23-Apr-19 13:58 super_gradients/training/utils/weight_averaging_utils.py
--rw-r--r--  2.0 unx     2030 b- defN 23-Apr-19 13:58 super_gradients/training/utils/callbacks/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/utils/callbacks/all_callbacks.py
--rw-r--r--  2.0 unx    20126 b- defN 23-Apr-19 13:58 super_gradients/training/utils/callbacks/base_callbacks.py
--rw-r--r--  2.0 unx    32630 b- defN 23-Apr-19 13:58 super_gradients/training/utils/callbacks/callbacks.py
--rw-r--r--  2.0 unx     1169 b- defN 23-Apr-19 13:58 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/utils/media/__init__.py
--rw-r--r--  2.0 unx     5775 b- defN 23-Apr-19 13:58 super_gradients/training/utils/media/image.py
--rw-r--r--  2.0 unx     4046 b- defN 23-Apr-19 13:58 super_gradients/training/utils/media/stream.py
--rw-r--r--  2.0 unx     5360 b- defN 23-Apr-19 13:58 super_gradients/training/utils/media/video.py
--rw-r--r--  2.0 unx      396 b- defN 23-Apr-19 13:58 super_gradients/training/utils/optimizers/__init__.py
--rw-r--r--  2.0 unx     9760 b- defN 23-Apr-19 13:58 super_gradients/training/utils/optimizers/lamb.py
--rw-r--r--  2.0 unx     3008 b- defN 23-Apr-19 13:58 super_gradients/training/utils/optimizers/lion.py
--rw-r--r--  2.0 unx     6834 b- defN 23-Apr-19 13:58 super_gradients/training/utils/optimizers/rmsprop_tf.py
--rw-r--r--  2.0 unx      213 b- defN 23-Apr-19 13:58 super_gradients/training/utils/pose_estimation/__init__.py
--rw-r--r--  2.0 unx    11167 b- defN 23-Apr-19 13:58 super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py
--rw-r--r--  2.0 unx     7140 b- defN 23-Apr-19 13:58 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py
--rw-r--r--  2.0 unx      387 b- defN 23-Apr-19 13:58 super_gradients/training/utils/quantization/__init__.py
--rw-r--r--  2.0 unx     6271 b- defN 23-Apr-19 13:58 super_gradients/training/utils/quantization/calibrator.py
--rw-r--r--  2.0 unx     8417 b- defN 23-Apr-19 13:58 super_gradients/training/utils/quantization/core.py
--rw-r--r--  2.0 unx     2196 b- defN 23-Apr-19 13:58 super_gradients/training/utils/quantization/export.py
--rw-r--r--  2.0 unx    17062 b- defN 23-Apr-19 13:58 super_gradients/training/utils/quantization/selective_quantization_utils.py
--rw-r--r--  2.0 unx    11341 b- defN 23-Apr-19 13:59 super_gradients-3.0.9.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    34221 b- defN 23-Apr-19 13:59 super_gradients-3.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 13:59 super_gradients-3.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-19 13:59 super_gradients-3.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    61129 b- defN 23-Apr-19 13:59 super_gradients-3.0.9.dist-info/RECORD
-529 files, 2735180 bytes uncompressed, 835793 bytes compressed:  69.4%
+Zip file size: 965424 bytes, number of entries: 558
+-rw-r--r--  2.0 unx      711 b- defN 23-May-02 15:39 super_gradients/__init__.py
+-rw-r--r--  2.0 unx     1657 b- defN 23-May-02 15:39 super_gradients/evaluate_checkpoint.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-May-02 15:39 super_gradients/evaluate_from_recipe.py
+-rw-r--r--  2.0 unx      702 b- defN 23-May-02 15:39 super_gradients/qat_from_recipe.py
+-rwxr-xr-x  2.0 unx       44 b- defN 23-May-02 15:39 super_gradients/requirements.pro.txt
+-rwxr-xr-x  2.0 unx      729 b- defN 23-May-02 15:39 super_gradients/requirements.txt
+-rw-r--r--  2.0 unx      537 b- defN 23-May-02 15:39 super_gradients/resume_experiment.py
+-rw-r--r--  2.0 unx      693 b- defN 23-May-02 15:39 super_gradients/train_from_kd_recipe.py
+-rw-r--r--  2.0 unx      650 b- defN 23-May-02 15:39 super_gradients/train_from_recipe.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-May-02 15:39 super_gradients/common/__init__.py
+-rw-r--r--  2.0 unx    15372 b- defN 23-May-02 15:39 super_gradients/common/object_names.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/common/abstractions/__init__.py
+-rw-r--r--  2.0 unx      879 b- defN 23-May-02 15:39 super_gradients/common/abstractions/abstract_logger.py
+-rw-r--r--  2.0 unx     3129 b- defN 23-May-02 15:39 super_gradients/common/abstractions/mute_processes.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/common/auto_logging/__init__.py
+-rw-r--r--  2.0 unx     4687 b- defN 23-May-02 15:39 super_gradients/common/auto_logging/auto_logger.py
+-rw-r--r--  2.0 unx     6625 b- defN 23-May-02 15:39 super_gradients/common/auto_logging/console_logging.py
+-rw-r--r--  2.0 unx      142 b- defN 23-May-02 15:39 super_gradients/common/aws_connection/__init__.py
+-rw-r--r--  2.0 unx     4182 b- defN 23-May-02 15:39 super_gradients/common/aws_connection/aws_connector.py
+-rw-r--r--  2.0 unx     7198 b- defN 23-May-02 15:39 super_gradients/common/aws_connection/aws_secrets_manager_connector.py
+-rw-r--r--  2.0 unx      119 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/__init__.py
+-rw-r--r--  2.0 unx      669 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/crash_handler.py
+-rw-r--r--  2.0 unx    11775 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/crash_tips.py
+-rw-r--r--  2.0 unx      886 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/crash_tips_setup.py
+-rw-r--r--  2.0 unx     1740 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/exception.py
+-rw-r--r--  2.0 unx     2357 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/exception_monitoring_setup.py
+-rw-r--r--  2.0 unx      789 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/utils.py
+-rw-r--r--  2.0 unx      140 b- defN 23-May-02 15:39 super_gradients/common/data_connection/__init__.py
+-rw-r--r--  2.0 unx    17959 b- defN 23-May-02 15:39 super_gradients/common/data_connection/s3_connector.py
+-rw-r--r--  2.0 unx      325 b- defN 23-May-02 15:39 super_gradients/common/data_interface/__init__.py
+-rw-r--r--  2.0 unx     9699 b- defN 23-May-02 15:39 super_gradients/common/data_interface/adnn_model_repository_data_interface.py
+-rw-r--r--  2.0 unx     2050 b- defN 23-May-02 15:39 super_gradients/common/data_interface/dataset_data_interface.py
+-rw-r--r--  2.0 unx      220 b- defN 23-May-02 15:39 super_gradients/common/data_types/__init__.py
+-rw-r--r--  2.0 unx      597 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/__init__.py
+-rw-r--r--  2.0 unx      309 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/deep_learning_task.py
+-rw-r--r--  2.0 unx      108 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/downsample_mode.py
+-rw-r--r--  2.0 unx      317 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/evaluation_type.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/multi_gpu_mode.py
+-rw-r--r--  2.0 unx     1200 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/strict_load.py
+-rw-r--r--  2.0 unx      202 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/upsample_mode.py
+-rw-r--r--  2.0 unx      257 b- defN 23-May-02 15:39 super_gradients/common/decorators/__init__.py
+-rw-r--r--  2.0 unx     1567 b- defN 23-May-02 15:39 super_gradients/common/decorators/code_save_decorator.py
+-rw-r--r--  2.0 unx     3663 b- defN 23-May-02 15:39 super_gradients/common/decorators/deci_logger.py
+-rw-r--r--  2.0 unx     2921 b- defN 23-May-02 15:39 super_gradients/common/decorators/explicit_params_validator.py
+-rw-r--r--  2.0 unx     1315 b- defN 23-May-02 15:39 super_gradients/common/decorators/factory_decorator.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-May-02 15:39 super_gradients/common/decorators/singleton.py
+-rw-r--r--  2.0 unx      202 b- defN 23-May-02 15:39 super_gradients/common/environment/__init__.py
+-rw-r--r--  2.0 unx      993 b- defN 23-May-02 15:39 super_gradients/common/environment/argparse_utils.py
+-rw-r--r--  2.0 unx     9170 b- defN 23-May-02 15:39 super_gradients/common/environment/cfg_utils.py
+-rw-r--r--  2.0 unx     4218 b- defN 23-May-02 15:39 super_gradients/common/environment/checkpoints_dir_utils.py
+-rw-r--r--  2.0 unx     2682 b- defN 23-May-02 15:39 super_gradients/common/environment/ddp_utils.py
+-rw-r--r--  2.0 unx      752 b- defN 23-May-02 15:39 super_gradients/common/environment/device_utils.py
+-rw-r--r--  2.0 unx     1147 b- defN 23-May-02 15:39 super_gradients/common/environment/env_variables.py
+-rw-r--r--  2.0 unx     4047 b- defN 23-May-02 15:39 super_gradients/common/environment/omegaconf_utils.py
+-rw-r--r--  2.0 unx      459 b- defN 23-May-02 15:39 super_gradients/common/environment/path_utils.py
+-rw-r--r--  2.0 unx      112 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/__init__.py
+-rw-r--r--  2.0 unx      153 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/cpu.py
+-rw-r--r--  2.0 unx     2517 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/data_models.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/disk.py
+-rw-r--r--  2.0 unx     5427 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/monitoring.py
+-rw-r--r--  2.0 unx      948 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/network.py
+-rw-r--r--  2.0 unx      629 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/utils.py
+-rw-r--r--  2.0 unx      145 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/virtual_memory.py
+-rw-r--r--  2.0 unx      681 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/gpu/__init__.py
+-rw-r--r--  2.0 unx     2270 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/gpu/gpu.py
+-rw-r--r--  2.0 unx   121647 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/gpu/pynvml.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/common/exceptions/__init__.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-02 15:39 super_gradients/common/exceptions/factory_exceptions.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/common/factories/__init__.py
+-rw-r--r--  2.0 unx     1715 b- defN 23-May-02 15:39 super_gradients/common/factories/activations_type_factory.py
+-rw-r--r--  2.0 unx     2881 b- defN 23-May-02 15:39 super_gradients/common/factories/base_factory.py
+-rw-r--r--  2.0 unx      258 b- defN 23-May-02 15:39 super_gradients/common/factories/bbox_format_factory.py
+-rw-r--r--  2.0 unx      232 b- defN 23-May-02 15:39 super_gradients/common/factories/callbacks_factory.py
+-rw-r--r--  2.0 unx      263 b- defN 23-May-02 15:39 super_gradients/common/factories/collate_functions_factory.py
+-rw-r--r--  2.0 unx      292 b- defN 23-May-02 15:39 super_gradients/common/factories/context_modules_factory.py
+-rw-r--r--  2.0 unx      321 b- defN 23-May-02 15:39 super_gradients/common/factories/data_formats_factory.py
+-rw-r--r--  2.0 unx      237 b- defN 23-May-02 15:39 super_gradients/common/factories/datasets_factory.py
+-rw-r--r--  2.0 unx     1014 b- defN 23-May-02 15:39 super_gradients/common/factories/detection_modules_factory.py
+-rw-r--r--  2.0 unx      572 b- defN 23-May-02 15:39 super_gradients/common/factories/list_factory.py
+-rw-r--r--  2.0 unx      223 b- defN 23-May-02 15:39 super_gradients/common/factories/losses_factory.py
+-rw-r--r--  2.0 unx      226 b- defN 23-May-02 15:39 super_gradients/common/factories/metrics_factory.py
+-rw-r--r--  2.0 unx      467 b- defN 23-May-02 15:39 super_gradients/common/factories/optimizers_type_factory.py
+-rw-r--r--  2.0 unx      271 b- defN 23-May-02 15:39 super_gradients/common/factories/pre_launch_callbacks_factory.py
+-rw-r--r--  2.0 unx      623 b- defN 23-May-02 15:39 super_gradients/common/factories/processing_factory.py
+-rw-r--r--  2.0 unx      229 b- defN 23-May-02 15:39 super_gradients/common/factories/samplers_factory.py
+-rw-r--r--  2.0 unx      263 b- defN 23-May-02 15:39 super_gradients/common/factories/target_generator_factory.py
+-rw-r--r--  2.0 unx     1873 b- defN 23-May-02 15:39 super_gradients/common/factories/transforms_factory.py
+-rw-r--r--  2.0 unx     2377 b- defN 23-May-02 15:39 super_gradients/common/factories/type_factory.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/common/plugins/__init__.py
+-rw-r--r--  2.0 unx    10974 b- defN 23-May-02 15:39 super_gradients/common/plugins/deci_client.py
+-rw-r--r--  2.0 unx      271 b- defN 23-May-02 15:39 super_gradients/common/registry/__init__.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-May-02 15:39 super_gradients/common/registry/albumentation.py
+-rw-r--r--  2.0 unx     6006 b- defN 23-May-02 15:39 super_gradients/common/registry/registry.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/common/registry/registry_utils.py
+-rw-r--r--  2.0 unx      508 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/__init__.py
+-rw-r--r--  2.0 unx     7355 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/abstract_sg_logger.py
+-rw-r--r--  2.0 unx    14980 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/base_sg_logger.py
+-rw-r--r--  2.0 unx    10055 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/clearml_sg_logger.py
+-rw-r--r--  2.0 unx    10103 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/dagshub_sg_logger.py
+-rw-r--r--  2.0 unx     6618 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/deci_platform_sg_logger.py
+-rw-r--r--  2.0 unx    13073 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/wandb_sg_logger.py
+-rw-r--r--  2.0 unx    85509 b- defN 23-May-02 15:39 super_gradients/examples/SG_Walkthrough.ipynb
+-rw-r--r--  2.0 unx    69618 b- defN 23-May-02 15:39 super_gradients/examples/SG_quickstart_classification.ipynb
+-rw-r--r--  2.0 unx    54966 b- defN 23-May-02 15:39 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb
+-rw-r--r--  2.0 unx    65090 b- defN 23-May-02 15:39 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/cifar10_training_torch_objects/__init__.py
+-rw-r--r--  2.0 unx     2526 b- defN 23-May-02 15:39 super_gradients/examples/cifar10_training_torch_objects/cifar10_training_torch_objects_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/convert_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      870 b- defN 23-May-02 15:39 super_gradients/examples/convert_recipe_example/convert_recipe_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/ddrnet_imagenet/__init__.py
+-rw-r--r--  2.0 unx     3114 b- defN 23-May-02 15:39 super_gradients/examples/ddrnet_imagenet/ddrnet_classification_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/deci_lab_export_example/__init__.py
+-rw-r--r--  2.0 unx     3562 b- defN 23-May-02 15:39 super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/early_stop/__init__.py
+-rw-r--r--  2.0 unx     1596 b- defN 23-May-02 15:39 super_gradients/examples/early_stop/early_stop_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/evaluate_checkpoint_example/__init__.py
+-rw-r--r--  2.0 unx      289 b- defN 23-May-02 15:39 super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/evaluate_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      292 b- defN 23-May-02 15:39 super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/loggers_examples/__init__.py
+-rw-r--r--  2.0 unx     1206 b- defN 23-May-02 15:39 super_gradients/examples/loggers_examples/clearml_logger_example.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-02 15:39 super_gradients/examples/loggers_examples/deci_platform_logger_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/qat_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      277 b- defN 23-May-02 15:39 super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/quantization/__init__.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-May-02 15:39 super_gradients/examples/quantization/non_default_calibrators_example.py
+-rw-r--r--  2.0 unx     2310 b- defN 23-May-02 15:39 super_gradients/examples/quantization/ptq_e2e_example.py
+-rw-r--r--  2.0 unx     1850 b- defN 23-May-02 15:39 super_gradients/examples/quantization/register_quantization_mapping_with_decorator_example.py
+-rw-r--r--  2.0 unx     4732 b- defN 23-May-02 15:39 super_gradients/examples/quantization/resnet_qat_example.py
+-rw-r--r--  2.0 unx     1163 b- defN 23-May-02 15:39 super_gradients/examples/quantization/skipping_quantization_example.py
+-rw-r--r--  2.0 unx      832 b- defN 23-May-02 15:39 super_gradients/examples/quantization/vanilla_quantize_all_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/regseg_transfer_learning_example/__init__.py
+-rw-r--r--  2.0 unx     2379 b- defN 23-May-02 15:39 super_gradients/examples/regseg_transfer_learning_example/regseg_transfer_learning_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/resume_experiment_example/__init__.py
+-rw-r--r--  2.0 unx      283 b- defN 23-May-02 15:39 super_gradients/examples/resume_experiment_example/resume_experiment.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/train_from_kd_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      292 b- defN 23-May-02 15:39 super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      283 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_example/train_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_with_dataset_registry/__init__.py
+-rw-r--r--  2.0 unx     1334 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_with_dataset_registry/train.py
+-rw-r--r--  2.0 unx     1643 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_with_dataset_registry/user_dataset.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_with_user_objects/__init__.py
+-rw-r--r--  2.0 unx     1326 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_with_user_objects/train.py
+-rw-r--r--  2.0 unx     2548 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py
+-rw-r--r--  2.0 unx      174 b- defN 23-May-02 15:39 super_gradients/module_interfaces/__init__.py
+-rw-r--r--  2.0 unx     2043 b- defN 23-May-02 15:39 super_gradients/module_interfaces/module_interfaces.py
+-rw-r--r--  2.0 unx     3366 b- defN 23-May-02 15:39 super_gradients/modules/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/modules/all_detection_modules.py
+-rw-r--r--  2.0 unx      617 b- defN 23-May-02 15:39 super_gradients/modules/anti_alias.py
+-rw-r--r--  2.0 unx      776 b- defN 23-May-02 15:39 super_gradients/modules/base_modules.py
+-rw-r--r--  2.0 unx     3054 b- defN 23-May-02 15:39 super_gradients/modules/conv_bn_act_block.py
+-rw-r--r--  2.0 unx     1976 b- defN 23-May-02 15:39 super_gradients/modules/conv_bn_relu_block.py
+-rw-r--r--  2.0 unx    14805 b- defN 23-May-02 15:39 super_gradients/modules/detection_modules.py
+-rw-r--r--  2.0 unx     2143 b- defN 23-May-02 15:39 super_gradients/modules/head_replacement_utils.py
+-rw-r--r--  2.0 unx     4362 b- defN 23-May-02 15:39 super_gradients/modules/multi_output_modules.py
+-rw-r--r--  2.0 unx      860 b- defN 23-May-02 15:39 super_gradients/modules/pixel_shuffle.py
+-rw-r--r--  2.0 unx     3953 b- defN 23-May-02 15:39 super_gradients/modules/pose_estimation_modules.py
+-rw-r--r--  2.0 unx    11642 b- defN 23-May-02 15:39 super_gradients/modules/qarepvgg_block.py
+-rw-r--r--  2.0 unx     8544 b- defN 23-May-02 15:39 super_gradients/modules/repvgg_block.py
+-rw-r--r--  2.0 unx     2138 b- defN 23-May-02 15:39 super_gradients/modules/sampling.py
+-rw-r--r--  2.0 unx     1459 b- defN 23-May-02 15:39 super_gradients/modules/se_blocks.py
+-rw-r--r--  2.0 unx     1403 b- defN 23-May-02 15:39 super_gradients/modules/skip_connections.py
+-rw-r--r--  2.0 unx     2968 b- defN 23-May-02 15:39 super_gradients/modules/utils.py
+-rw-r--r--  2.0 unx      716 b- defN 23-May-02 15:39 super_gradients/modules/quantization/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 23-May-02 15:39 super_gradients/modules/quantization/quantized_skip_connections.py
+-rw-r--r--  2.0 unx     4604 b- defN 23-May-02 15:39 super_gradients/modules/quantization/quantized_stdc_blocks.py
+-rw-r--r--  2.0 unx     1281 b- defN 23-May-02 15:39 super_gradients/modules/quantization/resnet_bottleneck.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/recipes/__init__.py
+-rw-r--r--  2.0 unx     1136 b- defN 23-May-02 15:39 super_gradients/recipes/cifar10_resnet.yaml
+-rw-r--r--  2.0 unx     3502 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_ddrnet.yaml
+-rw-r--r--  2.0 unx     3754 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_kd_base.yaml
+-rw-r--r--  2.0 unx     3354 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_pplite_seg50.yaml
+-rw-r--r--  2.0 unx     3253 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_pplite_seg75.yaml
+-rw-r--r--  2.0 unx     2498 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_regseg48.yaml
+-rw-r--r--  2.0 unx     4020 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_segformer.yaml
+-rw-r--r--  2.0 unx      618 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_stdc_base.yaml
+-rw-r--r--  2.0 unx     2862 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_stdc_seg50.yaml
+-rw-r--r--  2.0 unx     3055 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_stdc_seg75.yaml
+-rw-r--r--  2.0 unx     1830 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_pose_ddrnet39.yaml
+-rw-r--r--  2.0 unx     3549 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml
+-rw-r--r--  2.0 unx     1998 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_pose_pppose_l.yaml
+-rw-r--r--  2.0 unx     1996 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_ppyoloe_l.yaml
+-rw-r--r--  2.0 unx     1996 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_ppyoloe_m.yaml
+-rw-r--r--  2.0 unx     1882 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_ppyoloe_s.yaml
+-rw-r--r--  2.0 unx     1975 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_ppyoloe_x.yaml
+-rw-r--r--  2.0 unx     1889 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml
+-rw-r--r--  2.0 unx     1385 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_yolo_nas_s.yaml
+-rw-r--r--  2.0 unx     2583 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_yolox.yaml
+-rw-r--r--  2.0 unx     1376 b- defN 23-May-02 15:39 super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml
+-rw-r--r--  2.0 unx     1145 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_efficientnet.yaml
+-rw-r--r--  2.0 unx     1129 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_mobilenetv2.yaml
+-rw-r--r--  2.0 unx      507 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_mobilenetv3_base.yaml
+-rw-r--r--  2.0 unx      719 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_mobilenetv3_large.yaml
+-rw-r--r--  2.0 unx      719 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_mobilenetv3_small.yaml
+-rw-r--r--  2.0 unx     1997 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_regnetY.yaml
+-rw-r--r--  2.0 unx     1246 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_repvgg.yaml
+-rw-r--r--  2.0 unx     1169 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_resnet50.yaml
+-rw-r--r--  2.0 unx     2722 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_resnet50_kd.yaml
+-rw-r--r--  2.0 unx     1136 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_vit_base.yaml
+-rw-r--r--  2.0 unx     1010 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_vit_large.yaml
+-rw-r--r--  2.0 unx     2007 b- defN 23-May-02 15:39 super_gradients/recipes/roboflow_ppyoloe.yaml
+-rw-r--r--  2.0 unx     2347 b- defN 23-May-02 15:39 super_gradients/recipes/roboflow_yolo_nas_m.yaml
+-rw-r--r--  2.0 unx     2347 b- defN 23-May-02 15:39 super_gradients/recipes/roboflow_yolo_nas_s.yaml
+-rw-r--r--  2.0 unx      473 b- defN 23-May-02 15:39 super_gradients/recipes/roboflow_yolo_nas_s_qat.yaml
+-rw-r--r--  2.0 unx     1915 b- defN 23-May-02 15:39 super_gradients/recipes/roboflow_yolox.yaml
+-rw-r--r--  2.0 unx     1246 b- defN 23-May-02 15:39 super_gradients/recipes/supervisely_unet.yaml
+-rw-r--r--  2.0 unx     1672 b- defN 23-May-02 15:39 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
+-rw-r--r--  2.0 unx     2133 b- defN 23-May-02 15:39 super_gradients/recipes/user_recipe_mnist_example.yaml
+-rw-r--r--  2.0 unx     2000 b- defN 23-May-02 15:39 super_gradients/recipes/variable_setup.yaml
+-rw-r--r--  2.0 unx     2222 b- defN 23-May-02 15:39 super_gradients/recipes/anchors/ssd_anchors.yaml
+-rw-r--r--  2.0 unx      563 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml
+-rw-r--r--  2.0 unx      104 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b1_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b2_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b3_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b4_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b5_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b6_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b7_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b8_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_l2_arch_params.yaml
+-rw-r--r--  2.0 unx      194 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/mobilenet_v2_arch_params.yaml
+-rw-r--r--  2.0 unx      156 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/mobilenet_v3_arch_params.yaml
+-rw-r--r--  2.0 unx      409 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml
+-rw-r--r--  2.0 unx      356 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml
+-rw-r--r--  2.0 unx      281 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/pose_ddrnet39_arch_params.yaml
+-rw-r--r--  2.0 unx     1245 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml
+-rw-r--r--  2.0 unx      985 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml
+-rw-r--r--  2.0 unx     1112 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ppyoloe_arch_params.yaml
+-rw-r--r--  2.0 unx      196 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ppyoloe_l_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ppyoloe_m_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ppyoloe_s_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ppyoloe_x_arch_params.yaml
+-rw-r--r--  2.0 unx      204 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/regnetY_arch_params.yaml
+-rw-r--r--  2.0 unx      352 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvgg_arch_params.yaml
+-rw-r--r--  2.0 unx       98 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvgga0_arch_params.yaml
+-rw-r--r--  2.0 unx       89 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvgga1_arch_params.yaml
+-rw-r--r--  2.0 unx       95 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvgga2_arch_params.yaml
+-rw-r--r--  2.0 unx       88 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvggb0_arch_params.yaml
+-rw-r--r--  2.0 unx       86 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvggb1_arch_params.yaml
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvggb2_arch_params.yaml
+-rw-r--r--  2.0 unx       15 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/resnet18_cifar_arch_params.yaml
+-rw-r--r--  2.0 unx       17 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/resnet50_arch_params.yaml
+-rw-r--r--  2.0 unx       32 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/shelfnet34_lw_arch_params.yaml
+-rw-r--r--  2.0 unx      655 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ssd_lite_mobilenetv2_arch_params.yaml
+-rw-r--r--  2.0 unx      605 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ssd_mobilenetv1_arch_params.yaml
+-rw-r--r--  2.0 unx     1369 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/unet_arch_params.yaml
+-rw-r--r--  2.0 unx     3031 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/unet_default_arch_params.yaml
+-rw-r--r--  2.0 unx       63 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/vit_base_arch_params.yaml
+-rw-r--r--  2.0 unx     2393 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolo_arch_params.yaml
+-rw-r--r--  2.0 unx     2337 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolo_nas_l_arch_params.yaml
+-rw-r--r--  2.0 unx     2346 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolo_nas_m_arch_params.yaml
+-rw-r--r--  2.0 unx     2341 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolo_nas_s_arch_params.yaml
+-rw-r--r--  2.0 unx      235 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolox_s_arch_params.yaml
+-rw-r--r--  2.0 unx      229 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml
+-rw-r--r--  2.0 unx      228 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml
+-rw-r--r--  2.0 unx      611 b- defN 23-May-02 15:39 super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml
+-rw-r--r--  2.0 unx       72 b- defN 23-May-02 15:39 super_gradients/recipes/checkpoint_params/vit_base_imagenet_checkpoint_params.yaml
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/recipes/conversion_params/__init__.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-May-02 15:39 super_gradients/recipes/conversion_params/cifar10_conversion_params.yaml
+-rw-r--r--  2.0 unx     2040 b- defN 23-May-02 15:39 super_gradients/recipes/conversion_params/default_conversion_params.yaml
+-rw-r--r--  2.0 unx      869 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cifar100_dataset_params.yaml
+-rw-r--r--  2.0 unx     1530 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml
+-rw-r--r--  2.0 unx     1056 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml
+-rw-r--r--  2.0 unx      615 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml
+-rw-r--r--  2.0 unx      525 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml
+-rw-r--r--  2.0 unx      706 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml
+-rw-r--r--  2.0 unx      644 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml
+-rw-r--r--  2.0 unx      721 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml
+-rw-r--r--  2.0 unx      709 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml
+-rw-r--r--  2.0 unx      708 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml
+-rw-r--r--  2.0 unx     3946 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx     4202 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml
+-rw-r--r--  2.0 unx     3590 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml
+-rw-r--r--  2.0 unx     5568 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml
+-rw-r--r--  2.0 unx     3646 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml
+-rw-r--r--  2.0 unx     2461 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml
+-rw-r--r--  2.0 unx      405 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml
+-rw-r--r--  2.0 unx     1466 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx      931 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml
+-rw-r--r--  2.0 unx      732 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml
+-rw-r--r--  2.0 unx      794 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml
+-rw-r--r--  2.0 unx      142 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml
+-rw-r--r--  2.0 unx      734 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_regnetY_dataset_params.yaml
+-rw-r--r--  2.0 unx     1059 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml
+-rw-r--r--  2.0 unx     1093 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml
+-rw-r--r--  2.0 unx      845 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml
+-rw-r--r--  2.0 unx     1762 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml
+-rw-r--r--  2.0 unx      149 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx     1571 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx     1414 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx     4112 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx      961 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml
+-rw-r--r--  2.0 unx      559 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml
+-rw-r--r--  2.0 unx     1155 b- defN 23-May-02 15:39 super_gradients/recipes/quantization_params/default_quantization_params.yaml
+-rw-r--r--  2.0 unx      591 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml
+-rw-r--r--  2.0 unx      700 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml
+-rw-r--r--  2.0 unx      877 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml
+-rw-r--r--  2.0 unx     1302 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml
+-rw-r--r--  2.0 unx      723 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml
+-rw-r--r--  2.0 unx     1121 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/coco2017_yolo_nas_train_params.yaml
+-rw-r--r--  2.0 unx      956 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml
+-rw-r--r--  2.0 unx      461 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml
+-rw-r--r--  2.0 unx     5459 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/default_train_params.yaml
+-rw-r--r--  2.0 unx      794 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml
+-rw-r--r--  2.0 unx      742 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml
+-rw-r--r--  2.0 unx      549 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml
+-rw-r--r--  2.0 unx      795 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml
+-rw-r--r--  2.0 unx      476 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_repvgg_train_params.yaml
+-rw-r--r--  2.0 unx      484 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_resnet50_kd_train_params.yaml
+-rw-r--r--  2.0 unx      522 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml
+-rw-r--r--  2.0 unx      602 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml
+-rw-r--r--  2.0 unx      519 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml
+-rw-r--r--  2.0 unx      107 b- defN 23-May-02 15:39 super_gradients/sanity_check/__init__.py
+-rw-r--r--  2.0 unx     5262 b- defN 23-May-02 15:39 super_gradients/sanity_check/env_sanity_check.py
+-rw-r--r--  2.0 unx      666 b- defN 23-May-02 15:39 super_gradients/training/__init__.py
+-rw-r--r--  2.0 unx     4155 b- defN 23-May-02 15:39 super_gradients/training/params.py
+-rw-r--r--  2.0 unx     4301 b- defN 23-May-02 15:39 super_gradients/training/pretrained_models.py
+-rw-r--r--  2.0 unx     3224 b- defN 23-May-02 15:39 super_gradients/training/dataloaders/__init__.py
+-rw-r--r--  2.0 unx    32361 b- defN 23-May-02 15:39 super_gradients/training/dataloaders/dataloaders.py
+-rw-r--r--  2.0 unx     1811 b- defN 23-May-02 15:39 super_gradients/training/datasets/__init__.py
+-rw-r--r--  2.0 unx    14162 b- defN 23-May-02 15:39 super_gradients/training/datasets/auto_augment.py
+-rw-r--r--  2.0 unx     3705 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_augmentation.py
+-rw-r--r--  2.0 unx     3484 b- defN 23-May-02 15:39 super_gradients/training/datasets/datasets_conf.py
+-rw-r--r--  2.0 unx    30279 b- defN 23-May-02 15:39 super_gradients/training/datasets/datasets_utils.py
+-rw-r--r--  2.0 unx    14663 b- defN 23-May-02 15:39 super_gradients/training/datasets/mixup.py
+-rw-r--r--  2.0 unx    11746 b- defN 23-May-02 15:39 super_gradients/training/datasets/sg_dataset.py
+-rw-r--r--  2.0 unx      252 b- defN 23-May-02 15:39 super_gradients/training/datasets/classification_datasets/__init__.py
+-rw-r--r--  2.0 unx     3096 b- defN 23-May-02 15:39 super_gradients/training/datasets/classification_datasets/cifar.py
+-rw-r--r--  2.0 unx     1706 b- defN 23-May-02 15:39 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py
+-rw-r--r--  2.0 unx      862 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/__init__.py
+-rw-r--r--  2.0 unx     3927 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/default_formats.py
+-rw-r--r--  2.0 unx     3071 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/format_converter.py
+-rw-r--r--  2.0 unx     7928 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/formats.py
+-rw-r--r--  2.0 unx     1044 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/__init__.py
+-rw-r--r--  2.0 unx     2674 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/bbox_format.py
+-rw-r--r--  2.0 unx     5094 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py
+-rw-r--r--  2.0 unx     2089 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/normalized_cxcywh.py
+-rw-r--r--  2.0 unx     2043 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xywh.py
+-rw-r--r--  2.0 unx     5043 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xyxy.py
+-rw-r--r--  2.0 unx     2948 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py
+-rw-r--r--  2.0 unx      575 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py
+-rw-r--r--  2.0 unx     1792 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/output_adapters/__init__.py
+-rw-r--r--  2.0 unx     8373 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py
+-rw-r--r--  2.0 unx      683 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/__init__.py
+-rw-r--r--  2.0 unx     2505 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/coco_detection.py
+-rw-r--r--  2.0 unx     9258 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/coco_format_detection.py
+-rw-r--r--  2.0 unx    26159 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/detection_dataset.py
+-rw-r--r--  2.0 unx    11353 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py
+-rw-r--r--  2.0 unx    11120 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/yolo_format_detection.py
+-rw-r--r--  2.0 unx      328 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/roboflow/__init__.py
+-rw-r--r--  2.0 unx    18882 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/roboflow/metadata.py
+-rw-r--r--  2.0 unx     3504 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py
+-rw-r--r--  2.0 unx     1997 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/roboflow/utils.py
+-rw-r--r--  2.0 unx      502 b- defN 23-May-02 15:39 super_gradients/training/datasets/pose_estimation_datasets/__init__.py
+-rw-r--r--  2.0 unx     4910 b- defN 23-May-02 15:39 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py
+-rw-r--r--  2.0 unx     9066 b- defN 23-May-02 15:39 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py
+-rw-r--r--  2.0 unx     5929 b- defN 23-May-02 15:39 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py
+-rw-r--r--  2.0 unx    10167 b- defN 23-May-02 15:39 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py
+-rw-r--r--  2.0 unx      385 b- defN 23-May-02 15:39 super_gradients/training/datasets/samplers/__init__.py
+-rw-r--r--  2.0 unx     2516 b- defN 23-May-02 15:39 super_gradients/training/datasets/samplers/infinite_sampler.py
+-rw-r--r--  2.0 unx     4809 b- defN 23-May-02 15:39 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py
+-rw-r--r--  2.0 unx     1037 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/__init__.py
+-rw-r--r--  2.0 unx     6714 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py
+-rw-r--r--  2.0 unx     7717 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py
+-rw-r--r--  2.0 unx     5518 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py
+-rw-r--r--  2.0 unx    11146 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py
+-rw-r--r--  2.0 unx     8470 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py
+-rw-r--r--  2.0 unx     3062 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/exceptions/__init__.py
+-rw-r--r--  2.0 unx     1761 b- defN 23-May-02 15:39 super_gradients/training/exceptions/dataset_exceptions.py
+-rw-r--r--  2.0 unx     2826 b- defN 23-May-02 15:39 super_gradients/training/exceptions/kd_trainer_exceptions.py
+-rw-r--r--  2.0 unx      946 b- defN 23-May-02 15:39 super_gradients/training/exceptions/loss_exceptions.py
+-rw-r--r--  2.0 unx     1268 b- defN 23-May-02 15:39 super_gradients/training/exceptions/sg_trainer_exceptions.py
+-rw-r--r--  2.0 unx      132 b- defN 23-May-02 15:39 super_gradients/training/kd_trainer/__init__.py
+-rw-r--r--  2.0 unx    16582 b- defN 23-May-02 15:39 super_gradients/training/kd_trainer/kd_trainer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/legacy/__init__.py
+-rw-r--r--  2.0 unx     4198 b- defN 23-May-02 15:39 super_gradients/training/legacy/utils.py
+-rw-r--r--  2.0 unx     1476 b- defN 23-May-02 15:39 super_gradients/training/losses/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/losses/all_losses.py
+-rw-r--r--  2.0 unx     1219 b- defN 23-May-02 15:39 super_gradients/training/losses/bce_dice_loss.py
+-rw-r--r--  2.0 unx      419 b- defN 23-May-02 15:39 super_gradients/training/losses/bce_loss.py
+-rw-r--r--  2.0 unx     2374 b- defN 23-May-02 15:39 super_gradients/training/losses/cwd_loss.py
+-rw-r--r--  2.0 unx     2525 b- defN 23-May-02 15:39 super_gradients/training/losses/ddrnet_loss.py
+-rw-r--r--  2.0 unx     3377 b- defN 23-May-02 15:39 super_gradients/training/losses/dekr_loss.py
+-rw-r--r--  2.0 unx     5618 b- defN 23-May-02 15:39 super_gradients/training/losses/dice_ce_edge_loss.py
+-rw-r--r--  2.0 unx     5208 b- defN 23-May-02 15:39 super_gradients/training/losses/dice_loss.py
+-rw-r--r--  2.0 unx     1214 b- defN 23-May-02 15:39 super_gradients/training/losses/focal_loss.py
+-rw-r--r--  2.0 unx     5051 b- defN 23-May-02 15:39 super_gradients/training/losses/iou_loss.py
+-rw-r--r--  2.0 unx     2176 b- defN 23-May-02 15:39 super_gradients/training/losses/kd_losses.py
+-rw-r--r--  2.0 unx     4177 b- defN 23-May-02 15:39 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py
+-rw-r--r--  2.0 unx      550 b- defN 23-May-02 15:39 super_gradients/training/losses/loss_utils.py
+-rw-r--r--  2.0 unx     3854 b- defN 23-May-02 15:39 super_gradients/training/losses/mask_loss.py
+-rw-r--r--  2.0 unx     4129 b- defN 23-May-02 15:39 super_gradients/training/losses/ohem_ce_loss.py
+-rw-r--r--  2.0 unx    41319 b- defN 23-May-02 15:39 super_gradients/training/losses/ppyolo_loss.py
+-rw-r--r--  2.0 unx     1010 b- defN 23-May-02 15:39 super_gradients/training/losses/r_squared_loss.py
+-rw-r--r--  2.0 unx     3453 b- defN 23-May-02 15:39 super_gradients/training/losses/seg_kd_loss.py
+-rw-r--r--  2.0 unx     1650 b- defN 23-May-02 15:39 super_gradients/training/losses/shelfnet_ohem_loss.py
+-rw-r--r--  2.0 unx     1949 b- defN 23-May-02 15:39 super_gradients/training/losses/shelfnet_semantic_encoding_loss.py
+-rw-r--r--  2.0 unx     8794 b- defN 23-May-02 15:39 super_gradients/training/losses/ssd_loss.py
+-rw-r--r--  2.0 unx     9721 b- defN 23-May-02 15:39 super_gradients/training/losses/stdc_loss.py
+-rw-r--r--  2.0 unx     5771 b- defN 23-May-02 15:39 super_gradients/training/losses/structure_loss.py
+-rw-r--r--  2.0 unx    50149 b- defN 23-May-02 15:39 super_gradients/training/losses/yolox_loss.py
+-rw-r--r--  2.0 unx     1052 b- defN 23-May-02 15:39 super_gradients/training/metrics/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/metrics/all_metrics.py
+-rw-r--r--  2.0 unx     3262 b- defN 23-May-02 15:39 super_gradients/training/metrics/classification_metrics.py
+-rw-r--r--  2.0 unx    10741 b- defN 23-May-02 15:39 super_gradients/training/metrics/detection_metrics.py
+-rw-r--r--  2.0 unx     3973 b- defN 23-May-02 15:39 super_gradients/training/metrics/metric_utils.py
+-rw-r--r--  2.0 unx    15346 b- defN 23-May-02 15:39 super_gradients/training/metrics/pose_estimation_metrics.py
+-rw-r--r--  2.0 unx    11454 b- defN 23-May-02 15:39 super_gradients/training/metrics/pose_estimation_utils.py
+-rw-r--r--  2.0 unx    11935 b- defN 23-May-02 15:39 super_gradients/training/metrics/segmentation_metrics.py
+-rw-r--r--  2.0 unx     8617 b- defN 23-May-02 15:39 super_gradients/training/models/__init__.py
+-rw-r--r--  2.0 unx     1226 b- defN 23-May-02 15:39 super_gradients/training/models/arch_params_factory.py
+-rw-r--r--  2.0 unx     7060 b- defN 23-May-02 15:39 super_gradients/training/models/conversion.py
+-rw-r--r--  2.0 unx    11875 b- defN 23-May-02 15:39 super_gradients/training/models/model_factory.py
+-rw-r--r--  2.0 unx    10986 b- defN 23-May-02 15:39 super_gradients/training/models/prediction_results.py
+-rw-r--r--  2.0 unx     2054 b- defN 23-May-02 15:39 super_gradients/training/models/predictions.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/models/results.py
+-rw-r--r--  2.0 unx     2998 b- defN 23-May-02 15:39 super_gradients/training/models/sg_module.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/__init__.py
+-rw-r--r--  2.0 unx    20025 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/beit.py
+-rw-r--r--  2.0 unx     7472 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/densenet.py
+-rw-r--r--  2.0 unx     3707 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/dpn.py
+-rw-r--r--  2.0 unx    36745 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/efficientnet.py
+-rw-r--r--  2.0 unx     8862 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/googlenet.py
+-rw-r--r--  2.0 unx      798 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/lenet.py
+-rw-r--r--  2.0 unx     2407 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/mobilenet.py
+-rw-r--r--  2.0 unx     9472 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/mobilenetv2.py
+-rw-r--r--  2.0 unx     8696 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/mobilenetv3.py
+-rw-r--r--  2.0 unx     4339 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/pnasnet.py
+-rw-r--r--  2.0 unx     4209 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/preact_resnet.py
+-rw-r--r--  2.0 unx    13599 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/regnet.py
+-rw-r--r--  2.0 unx     7924 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/repvgg.py
+-rw-r--r--  2.0 unx    15025 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/resnet.py
+-rw-r--r--  2.0 unx     6294 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/resnext.py
+-rw-r--r--  2.0 unx     4134 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/senet.py
+-rw-r--r--  2.0 unx     3660 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/shufflenet.py
+-rw-r--r--  2.0 unx     9768 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/shufflenetv2.py
+-rw-r--r--  2.0 unx     1538 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/vgg.py
+-rw-r--r--  2.0 unx     9210 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/vit.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/__init__.py
+-rw-r--r--  2.0 unx     9130 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/csp_darknet53.py
+-rw-r--r--  2.0 unx     9814 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/csp_resnet.py
+-rw-r--r--  2.0 unx     9120 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/customizable_detector.py
+-rw-r--r--  2.0 unx     4746 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/darknet53.py
+-rw-r--r--  2.0 unx     2315 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/ssd.py
+-rw-r--r--  2.0 unx    29459 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolo_base.py
+-rw-r--r--  2.0 unx     2459 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolox.py
+-rw-r--r--  2.0 unx      251 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py
+-rw-r--r--  2.0 unx     7000 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/pp_yolo_e/pan.py
+-rw-r--r--  2.0 unx     3487 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py
+-rw-r--r--  2.0 unx     8243 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py
+-rw-r--r--  2.0 unx    12397 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py
+-rw-r--r--  2.0 unx      756 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolo_nas/__init__.py
+-rw-r--r--  2.0 unx    12084 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py
+-rw-r--r--  2.0 unx     2646 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolo_nas/panneck.py
+-rw-r--r--  2.0 unx     4124 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py
+-rw-r--r--  2.0 unx    13329 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/models/kd_modules/__init__.py
+-rw-r--r--  2.0 unx     3553 b- defN 23-May-02 15:39 super_gradients/training/models/kd_modules/kd_module.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/models/pose_estimation_models/__init__.py
+-rw-r--r--  2.0 unx    21231 b- defN 23-May-02 15:39 super_gradients/training/models/pose_estimation_models/dekr_hrnet.py
+-rw-r--r--  2.0 unx     1294 b- defN 23-May-02 15:39 super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py
+-rw-r--r--  2.0 unx     1335 b- defN 23-May-02 15:39 super_gradients/training/models/pose_estimation_models/pose_ppyolo.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/__init__.py
+-rw-r--r--  2.0 unx      964 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/common.py
+-rw-r--r--  2.0 unx     5139 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/context_modules.py
+-rw-r--r--  2.0 unx    27896 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/ddrnet.py
+-rw-r--r--  2.0 unx     2439 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/ddrnet_backbones.py
+-rw-r--r--  2.0 unx    21760 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/laddernet.py
+-rw-r--r--  2.0 unx    15648 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/ppliteseg.py
+-rw-r--r--  2.0 unx    14424 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/regseg.py
+-rw-r--r--  2.0 unx    20334 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/segformer.py
+-rw-r--r--  2.0 unx     2256 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/segmentation_module.py
+-rw-r--r--  2.0 unx    24833 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/shelfnet.py
+-rw-r--r--  2.0 unx    29005 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/stdc.py
+-rw-r--r--  2.0 unx      260 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/unet/__init__.py
+-rw-r--r--  2.0 unx    12324 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/unet/unet.py
+-rw-r--r--  2.0 unx    10718 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/unet/unet_decoder.py
+-rw-r--r--  2.0 unx    13292 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/unet/unet_encoder.py
+-rw-r--r--  2.0 unx      119 b- defN 23-May-02 15:39 super_gradients/training/models/user_models/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/pipelines/__init__.py
+-rw-r--r--  2.0 unx    14562 b- defN 23-May-02 15:39 super_gradients/training/pipelines/pipelines.py
+-rw-r--r--  2.0 unx      393 b- defN 23-May-02 15:39 super_gradients/training/pre_launch_callbacks/__init__.py
+-rw-r--r--  2.0 unx    13955 b- defN 23-May-02 15:39 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py
+-rw-r--r--  2.0 unx      517 b- defN 23-May-02 15:39 super_gradients/training/processing/__init__.py
+-rw-r--r--  2.0 unx    13177 b- defN 23-May-02 15:39 super_gradients/training/processing/processing.py
+-rw-r--r--  2.0 unx       98 b- defN 23-May-02 15:39 super_gradients/training/qat_trainer/__init__.py
+-rw-r--r--  2.0 unx     9701 b- defN 23-May-02 15:39 super_gradients/training/qat_trainer/qat_trainer.py
+-rw-r--r--  2.0 unx      184 b- defN 23-May-02 15:39 super_gradients/training/sg_trainer/__init__.py
+-rw-r--r--  2.0 unx    97356 b- defN 23-May-02 15:39 super_gradients/training/sg_trainer/sg_trainer.py
+-rw-r--r--  2.0 unx     1685 b- defN 23-May-02 15:39 super_gradients/training/training_hyperparams/__init__.py
+-rw-r--r--  2.0 unx     3774 b- defN 23-May-02 15:39 super_gradients/training/training_hyperparams/training_hyperparams.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-02 15:39 super_gradients/training/transforms/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/transforms/all_transforms.py
+-rw-r--r--  2.0 unx    16193 b- defN 23-May-02 15:39 super_gradients/training/transforms/keypoint_transforms.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-May-02 15:39 super_gradients/training/transforms/pipeline_adaptors.py
+-rw-r--r--  2.0 unx    55089 b- defN 23-May-02 15:39 super_gradients/training/transforms/transforms.py
+-rw-r--r--  2.0 unx     6048 b- defN 23-May-02 15:39 super_gradients/training/transforms/utils.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-May-02 15:39 super_gradients/training/utils/__init__.py
+-rw-r--r--  2.0 unx     1673 b- defN 23-May-02 15:39 super_gradients/training/utils/activations_utils.py
+-rw-r--r--  2.0 unx     1111 b- defN 23-May-02 15:39 super_gradients/training/utils/bbox_utils.py
+-rw-r--r--  2.0 unx    15315 b- defN 23-May-02 15:39 super_gradients/training/utils/checkpoint_utils.py
+-rw-r--r--  2.0 unx     9794 b- defN 23-May-02 15:39 super_gradients/training/utils/config_utils.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-May-02 15:39 super_gradients/training/utils/deprecated_utils.py
+-rw-r--r--  2.0 unx    53278 b- defN 23-May-02 15:39 super_gradients/training/utils/detection_utils.py
+-rw-r--r--  2.0 unx    16195 b- defN 23-May-02 15:39 super_gradients/training/utils/distributed_training_utils.py
+-rw-r--r--  2.0 unx     6352 b- defN 23-May-02 15:39 super_gradients/training/utils/early_stopping.py
+-rw-r--r--  2.0 unx     9322 b- defN 23-May-02 15:39 super_gradients/training/utils/ema.py
+-rw-r--r--  2.0 unx     2610 b- defN 23-May-02 15:39 super_gradients/training/utils/ema_decay_schedules.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-May-02 15:39 super_gradients/training/utils/export_utils.py
+-rw-r--r--  2.0 unx     7508 b- defN 23-May-02 15:39 super_gradients/training/utils/get_model_stats.py
+-rw-r--r--  2.0 unx      771 b- defN 23-May-02 15:39 super_gradients/training/utils/kd_trainer_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/utils/load_image.py
+-rw-r--r--  2.0 unx     5827 b- defN 23-May-02 15:39 super_gradients/training/utils/optimizer_utils.py
+-rw-r--r--  2.0 unx      839 b- defN 23-May-02 15:39 super_gradients/training/utils/regularization_utils.py
+-rw-r--r--  2.0 unx    10388 b- defN 23-May-02 15:39 super_gradients/training/utils/segmentation_utils.py
+-rw-r--r--  2.0 unx    19625 b- defN 23-May-02 15:39 super_gradients/training/utils/sg_trainer_utils.py
+-rw-r--r--  2.0 unx     6272 b- defN 23-May-02 15:39 super_gradients/training/utils/ssd_utils.py
+-rw-r--r--  2.0 unx    18273 b- defN 23-May-02 15:39 super_gradients/training/utils/utils.py
+-rw-r--r--  2.0 unx      303 b- defN 23-May-02 15:39 super_gradients/training/utils/version_utils.py
+-rw-r--r--  2.0 unx     6209 b- defN 23-May-02 15:39 super_gradients/training/utils/weight_averaging_utils.py
+-rw-r--r--  2.0 unx     2030 b- defN 23-May-02 15:39 super_gradients/training/utils/callbacks/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/utils/callbacks/all_callbacks.py
+-rw-r--r--  2.0 unx    20126 b- defN 23-May-02 15:39 super_gradients/training/utils/callbacks/base_callbacks.py
+-rw-r--r--  2.0 unx    32630 b- defN 23-May-02 15:39 super_gradients/training/utils/callbacks/callbacks.py
+-rw-r--r--  2.0 unx     1169 b- defN 23-May-02 15:39 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/utils/media/__init__.py
+-rw-r--r--  2.0 unx     5880 b- defN 23-May-02 15:39 super_gradients/training/utils/media/image.py
+-rw-r--r--  2.0 unx     4046 b- defN 23-May-02 15:39 super_gradients/training/utils/media/stream.py
+-rw-r--r--  2.0 unx     6926 b- defN 23-May-02 15:39 super_gradients/training/utils/media/video.py
+-rw-r--r--  2.0 unx      396 b- defN 23-May-02 15:39 super_gradients/training/utils/optimizers/__init__.py
+-rw-r--r--  2.0 unx     9760 b- defN 23-May-02 15:39 super_gradients/training/utils/optimizers/lamb.py
+-rw-r--r--  2.0 unx     3008 b- defN 23-May-02 15:39 super_gradients/training/utils/optimizers/lion.py
+-rw-r--r--  2.0 unx     6834 b- defN 23-May-02 15:39 super_gradients/training/utils/optimizers/rmsprop_tf.py
+-rw-r--r--  2.0 unx      213 b- defN 23-May-02 15:39 super_gradients/training/utils/pose_estimation/__init__.py
+-rw-r--r--  2.0 unx    11167 b- defN 23-May-02 15:39 super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py
+-rw-r--r--  2.0 unx     7140 b- defN 23-May-02 15:39 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py
+-rw-r--r--  2.0 unx      387 b- defN 23-May-02 15:39 super_gradients/training/utils/quantization/__init__.py
+-rw-r--r--  2.0 unx     6271 b- defN 23-May-02 15:39 super_gradients/training/utils/quantization/calibrator.py
+-rw-r--r--  2.0 unx     8417 b- defN 23-May-02 15:39 super_gradients/training/utils/quantization/core.py
+-rw-r--r--  2.0 unx     2196 b- defN 23-May-02 15:39 super_gradients/training/utils/quantization/export.py
+-rw-r--r--  2.0 unx    17062 b- defN 23-May-02 15:39 super_gradients/training/utils/quantization/selective_quantization_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/utils/visualization/__init__.py
+-rw-r--r--  2.0 unx     1698 b- defN 23-May-02 15:39 super_gradients/training/utils/visualization/detection.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-May-02 15:39 super_gradients/training/utils/visualization/utils.py
+-rw-r--r--  2.0 unx     2218 b- defN 23-May-02 15:40 super_gradients-3.1.0.dist-info/LICENSE.YOLONAS.md
+-rw-r--r--  2.0 unx    11341 b- defN 23-May-02 15:40 super_gradients-3.1.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    36159 b- defN 23-May-02 15:40 super_gradients-3.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 15:40 super_gradients-3.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-02 15:40 super_gradients-3.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    64352 b- defN 23-May-02 15:40 super_gradients-3.1.0.dist-info/RECORD
+558 files, 2818306 bytes uncompressed, 857306 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -1,16 +1,31 @@
 Filename: super_gradients/__init__.py
 Comment: 
 
+Filename: super_gradients/evaluate_checkpoint.py
+Comment: 
+
+Filename: super_gradients/evaluate_from_recipe.py
+Comment: 
+
+Filename: super_gradients/qat_from_recipe.py
+Comment: 
+
 Filename: super_gradients/requirements.pro.txt
 Comment: 
 
 Filename: super_gradients/requirements.txt
 Comment: 
 
+Filename: super_gradients/resume_experiment.py
+Comment: 
+
+Filename: super_gradients/train_from_kd_recipe.py
+Comment: 
+
 Filename: super_gradients/train_from_recipe.py
 Comment: 
 
 Filename: super_gradients/common/__init__.py
 Comment: 
 
 Filename: super_gradients/common/object_names.py
@@ -273,14 +288,17 @@
 
 Filename: super_gradients/common/sg_loggers/base_sg_logger.py
 Comment: 
 
 Filename: super_gradients/common/sg_loggers/clearml_sg_logger.py
 Comment: 
 
+Filename: super_gradients/common/sg_loggers/dagshub_sg_logger.py
+Comment: 
+
 Filename: super_gradients/common/sg_loggers/deci_platform_sg_logger.py
 Comment: 
 
 Filename: super_gradients/common/sg_loggers/wandb_sg_logger.py
 Comment: 
 
 Filename: super_gradients/examples/SG_Walkthrough.ipynb
@@ -429,26 +447,35 @@
 
 Filename: super_gradients/modules/all_detection_modules.py
 Comment: 
 
 Filename: super_gradients/modules/anti_alias.py
 Comment: 
 
+Filename: super_gradients/modules/base_modules.py
+Comment: 
+
 Filename: super_gradients/modules/conv_bn_act_block.py
 Comment: 
 
 Filename: super_gradients/modules/conv_bn_relu_block.py
 Comment: 
 
 Filename: super_gradients/modules/detection_modules.py
 Comment: 
 
+Filename: super_gradients/modules/head_replacement_utils.py
+Comment: 
+
 Filename: super_gradients/modules/multi_output_modules.py
 Comment: 
 
+Filename: super_gradients/modules/pixel_shuffle.py
+Comment: 
+
 Filename: super_gradients/modules/pose_estimation_modules.py
 Comment: 
 
 Filename: super_gradients/modules/qarepvgg_block.py
 Comment: 
 
 Filename: super_gradients/modules/repvgg_block.py
@@ -531,14 +558,17 @@
 
 Filename: super_gradients/recipes/coco2017_ppyoloe_x.yaml
 Comment: 
 
 Filename: super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml
 Comment: 
 
+Filename: super_gradients/recipes/coco2017_yolo_nas_s.yaml
+Comment: 
+
 Filename: super_gradients/recipes/coco2017_yolox.yaml
 Comment: 
 
 Filename: super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml
 Comment: 
 
 Filename: super_gradients/recipes/imagenet_efficientnet.yaml
@@ -573,26 +603,38 @@
 
 Filename: super_gradients/recipes/imagenet_vit_large.yaml
 Comment: 
 
 Filename: super_gradients/recipes/roboflow_ppyoloe.yaml
 Comment: 
 
+Filename: super_gradients/recipes/roboflow_yolo_nas_m.yaml
+Comment: 
+
+Filename: super_gradients/recipes/roboflow_yolo_nas_s.yaml
+Comment: 
+
+Filename: super_gradients/recipes/roboflow_yolo_nas_s_qat.yaml
+Comment: 
+
 Filename: super_gradients/recipes/roboflow_yolox.yaml
 Comment: 
 
 Filename: super_gradients/recipes/supervisely_unet.yaml
 Comment: 
 
 Filename: super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
 Comment: 
 
 Filename: super_gradients/recipes/user_recipe_mnist_example.yaml
 Comment: 
 
+Filename: super_gradients/recipes/variable_setup.yaml
+Comment: 
+
 Filename: super_gradients/recipes/anchors/ssd_anchors.yaml
 Comment: 
 
 Filename: super_gradients/recipes/arch_params/efficientnet_arch_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml
@@ -708,14 +750,23 @@
 
 Filename: super_gradients/recipes/arch_params/vit_base_arch_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/arch_params/yolo_arch_params.yaml
 Comment: 
 
+Filename: super_gradients/recipes/arch_params/yolo_nas_l_arch_params.yaml
+Comment: 
+
+Filename: super_gradients/recipes/arch_params/yolo_nas_m_arch_params.yaml
+Comment: 
+
+Filename: super_gradients/recipes/arch_params/yolo_nas_s_arch_params.yaml
+Comment: 
+
 Filename: super_gradients/recipes/arch_params/yolox_l_arch_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/arch_params/yolox_m_arch_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml
@@ -774,23 +825,26 @@
 
 Filename: super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml
 Comment: 
 
-Filename: super_gradients/recipes/dataset_params/coco_detection_deci_yolo_dataset_params.yaml
-Comment: 
-
 Filename: super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml
 Comment: 
 
+Filename: super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml
+Comment: 
+
+Filename: super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml
+Comment: 
+
 Filename: super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml
@@ -855,14 +909,17 @@
 
 Filename: super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml
 Comment: 
 
+Filename: super_gradients/recipes/training_hyperparams/coco2017_yolo_nas_train_params.yaml
+Comment: 
+
 Filename: super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/training_hyperparams/default_train_params.yaml
@@ -1206,14 +1263,17 @@
 
 Filename: super_gradients/training/models/prediction_results.py
 Comment: 
 
 Filename: super_gradients/training/models/predictions.py
 Comment: 
 
+Filename: super_gradients/training/models/results.py
+Comment: 
+
 Filename: super_gradients/training/models/sg_module.py
 Comment: 
 
 Filename: super_gradients/training/models/classification_models/__init__.py
 Comment: 
 
 Filename: super_gradients/training/models/classification_models/beit.py
@@ -1311,14 +1371,29 @@
 
 Filename: super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py
 Comment: 
 
 Filename: super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py
 Comment: 
 
+Filename: super_gradients/training/models/detection_models/yolo_nas/__init__.py
+Comment: 
+
+Filename: super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py
+Comment: 
+
+Filename: super_gradients/training/models/detection_models/yolo_nas/panneck.py
+Comment: 
+
+Filename: super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py
+Comment: 
+
+Filename: super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py
+Comment: 
+
 Filename: super_gradients/training/models/kd_modules/__init__.py
 Comment: 
 
 Filename: super_gradients/training/models/kd_modules/kd_module.py
 Comment: 
 
 Filename: super_gradients/training/models/pose_estimation_models/__init__.py
@@ -1566,23 +1641,35 @@
 
 Filename: super_gradients/training/utils/quantization/export.py
 Comment: 
 
 Filename: super_gradients/training/utils/quantization/selective_quantization_utils.py
 Comment: 
 
-Filename: super_gradients-3.0.9.dist-info/LICENSE.md
+Filename: super_gradients/training/utils/visualization/__init__.py
+Comment: 
+
+Filename: super_gradients/training/utils/visualization/detection.py
+Comment: 
+
+Filename: super_gradients/training/utils/visualization/utils.py
+Comment: 
+
+Filename: super_gradients-3.1.0.dist-info/LICENSE.YOLONAS.md
+Comment: 
+
+Filename: super_gradients-3.1.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: super_gradients-3.0.9.dist-info/METADATA
+Filename: super_gradients-3.1.0.dist-info/METADATA
 Comment: 
 
-Filename: super_gradients-3.0.9.dist-info/WHEEL
+Filename: super_gradients-3.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: super_gradients-3.0.9.dist-info/top_level.txt
+Filename: super_gradients-3.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: super_gradients-3.0.9.dist-info/RECORD
+Filename: super_gradients-3.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## super_gradients/__init__.py

```diff
@@ -1,12 +1,10 @@
 from super_gradients.common import init_trainer, is_distributed, object_names
 from super_gradients.training import losses, utils, datasets_utils, DataAugmentation, Trainer, KDTrainer, QATTrainer
 from super_gradients.common.registry.registry import ARCHITECTURES
-from super_gradients.examples.train_from_recipe_example import train_from_recipe
-from super_gradients.examples.train_from_kd_recipe_example import train_from_kd_recipe
 from super_gradients.sanity_check import env_sanity_check
 from super_gradients.training.utils.distributed_training_utils import setup_device
 
 __all__ = [
     "ARCHITECTURES",
     "losses",
     "utils",
@@ -14,16 +12,14 @@
     "DataAugmentation",
     "Trainer",
     "KDTrainer",
     "QATTrainer",
     "object_names",
     "init_trainer",
     "is_distributed",
-    "train_from_recipe",
-    "train_from_kd_recipe",
     "env_sanity_check",
     "setup_device",
 ]
 
-__version__ = "3.0.9"
+__version__ = "3.1.0"
 
 env_sanity_check()
```

## super_gradients/train_from_recipe.py

```diff
@@ -3,24 +3,23 @@
 
 General use: python -m super_gradients.train_from_recipe --config-name="DESIRED_RECIPE".
 For recipe's specific instructions and details refer to the recipe's configuration file in the recipes directory.
 """
 
 from omegaconf import DictConfig
 import hydra
-import pkg_resources
 
 from super_gradients import Trainer, init_trainer
 
 
-@hydra.main(config_path=pkg_resources.resource_filename("super_gradients.recipes", ""), version_base="1.2")
-def main(cfg: DictConfig) -> None:
+@hydra.main(config_path="recipes", version_base="1.2")
+def _main(cfg: DictConfig) -> None:
     Trainer.train_from_config(cfg)
 
 
-def run():
-    init_trainer()
-    main()
+def main() -> None:
+    init_trainer()  # `init_trainer` needs to be called before `@hydra.main`
+    _main()
 
 
 if __name__ == "__main__":
-    run()
+    main()
```

## super_gradients/common/object_names.py

```diff
@@ -300,14 +300,17 @@
     SEGFORMER_B4 = "segformer_b4"
     SEGFORMER_B5 = "segformer_b5"
 
     DEKR_CUSTOM = "dekr_custom"
     DEKR_W32_NO_DC = "dekr_w32_no_dc"
     POSE_PP_YOLO_L = "pose_ppyolo_l"
     POSE_DDRNET_39 = "pose_ddrnet39"
+    YOLO_NAS_S = "yolo_nas_s"
+    YOLO_NAS_M = "yolo_nas_m"
+    YOLO_NAS_L = "yolo_nas_l"
 
 
 class ConcatenatedTensorFormats:
     XYXY_LABEL = "XYXY_LABEL"
     XYWH_LABEL = "XYWH_LABEL"
     CXCYWH_LABEL = "CXCYWH_LABEL"
     LABEL_XYXY = "LABEL_XYXY"
@@ -322,22 +325,24 @@
 
 
 class Dataloaders:
     COCO2017_TRAIN = "coco2017_train"
     COCO2017_VAL = "coco2017_val"
     COCO2017_TRAIN_YOLOX = "coco2017_train_yolox"
     COCO2017_VAL_YOLOX = "coco2017_val_yolox"
-    COCO2017_TRAIN_DECIYOLO = "coco2017_train_deci_yolo"
-    COCO2017_VAL_DECIYOLO = "coco2017_val_deci_yolo"
+    COCO2017_TRAIN_YOLO_NAS = "coco2017_train_yolo_nas"
+    COCO2017_VAL_YOLO_NAS = "coco2017_val_yolo_nas"
     COCO2017_TRAIN_PPYOLOE = "coco2017_train_ppyoloe"
     COCO2017_VAL_PPYOLOE = "coco2017_val_ppyoloe"
     COCO2017_TRAIN_SSD_LITE_MOBILENET_V2 = "coco2017_train_ssd_lite_mobilenet_v2"
     COCO2017_VAL_SSD_LITE_MOBILENET_V2 = "coco2017_val_ssd_lite_mobilenet_v2"
     COCO2017_POSE_TRAIN = "coco2017_pose_train"
     COCO2017_POSE_VAL = "coco2017_pose_val"
+    COCO_DETECTION_YOLO_FORMAT_TRAIN = "coco_detection_yolo_format_train"
+    COCO_DETECTION_YOLO_FORMAT_VAL = "coco_detection_yolo_format_val"
     IMAGENET_TRAIN = "imagenet_train"
     IMAGENET_VAL = "imagenet_val"
     IMAGENET_EFFICIENTNET_TRAIN = "imagenet_efficientnet_train"
     IMAGENET_EFFICIENTNET_VAL = "imagenet_efficientnet_val"
     IMAGENET_MOBILENETV2_TRAIN = "imagenet_mobilenetv2_train"
     IMAGENET_MOBILENETV2_VAL = "imagenet_mobilenetv2_val"
     IMAGENET_MOBILENETV3_TRAIN = "imagenet_mobilenetv3_train"
```

## super_gradients/common/data_types/enum/upsample_mode.py

```diff
@@ -1,8 +1,9 @@
 from enum import Enum
 
 
 class UpsampleMode(Enum):
     NEAREST = "nearest"
     BILINEAR = "bilinear"
     BICUBIC = "bicubic"
-    SNPE_BILINEAR = "snpe_bilinear"
+    NN_PIXEL_SHUFFLE = "nn_pixel_shuffle"
+    PIXEL_SHUFFLE = "pixel_shuffle"
```

## super_gradients/common/environment/omegaconf_utils.py

```diff
@@ -1,13 +1,66 @@
 import importlib
 import sys
+from typing import Any
 
-from omegaconf import OmegaConf
+from omegaconf import OmegaConf, DictConfig
 
 from super_gradients.common.environment.checkpoints_dir_utils import get_checkpoints_dir_path
+from hydra.experimental.callback import Callback
+
+
+class RecipeShortcutsCallback(Callback):
+    """
+    Interpolates the shortcuts defined in variable_set.yaml:
+            lr
+            batch_size
+            val_batch_size
+            ema
+            epochs
+            resume: False
+            num_workers
+
+    When any of the above are not set, they will be populated with the original values (for example
+        config.lr will be set with config.training_hyperparams.initial_lr) for clarity in logs.
+
+    """
+
+    def on_run_start(self, config: DictConfig, **kwargs: Any) -> None:
+        config.lr, config.training_hyperparams.initial_lr = self._override_with_shortcut(config.lr, config.training_hyperparams.initial_lr)
+
+        config.batch_size, config.dataset_params.train_dataloader_params.batch_size = self._override_with_shortcut(
+            config.batch_size, config.dataset_params.train_dataloader_params.batch_size
+        )
+
+        config.val_batch_size, config.dataset_params.val_dataloader_params.batch_size = self._override_with_shortcut(
+            config.val_batch_size, config.dataset_params.val_dataloader_params.batch_size
+        )
+
+        config.resume, config.training_hyperparams.resume = self._override_with_shortcut(config.resume, config.training_hyperparams.resume)
+
+        config.epochs, config.training_hyperparams.max_epochs = self._override_with_shortcut(config.epochs, config.training_hyperparams.max_epochs)
+
+        config.ema, config.training_hyperparams.ema = self._override_with_shortcut(config.ema, config.training_hyperparams.ema)
+
+        config.num_workers, config.dataset_params.train_dataloader_params.num_workers = self._override_with_shortcut(
+            config.num_workers, config.dataset_params.train_dataloader_params.num_workers
+        )
+
+        config.num_workers, config.dataset_params.val_dataloader_params.num_workers = self._override_with_shortcut(
+            config.num_workers, config.dataset_params.val_dataloader_params.num_workers
+        )
+
+    @staticmethod
+    def _override_with_shortcut(shortcut_value, main_value):
+        if shortcut_value is not None:
+            value = shortcut_value
+        else:
+            value = main_value
+
+        return value, value
 
 
 def get_cls(cls_path: str):
     """
     A resolver for Hydra/OmegaConf to allow getting a class instead on an instance.
     usage:
     class_of_optimizer: ${class:torch.optim.Adam}
```

## super_gradients/common/sg_loggers/__init__.py

```diff
@@ -1,6 +1,7 @@
 from super_gradients.common.sg_loggers.base_sg_logger import BaseSGLogger
 from super_gradients.common.sg_loggers.clearml_sg_logger import ClearMLSGLogger
 from super_gradients.common.sg_loggers.deci_platform_sg_logger import DeciPlatformSGLogger
 from super_gradients.common.sg_loggers.wandb_sg_logger import WandBSGLogger
+from super_gradients.common.sg_loggers.dagshub_sg_logger import DagsHubSGLogger
 
-__all__ = ["BaseSGLogger", "ClearMLSGLogger", "DeciPlatformSGLogger", "WandBSGLogger"]
+__all__ = ["BaseSGLogger", "ClearMLSGLogger", "DeciPlatformSGLogger", "WandBSGLogger", "DagsHubSGLogger"]
```

## super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py

```diff
@@ -1,40 +1,8 @@
-"""
-Evaluate a checkpoint resulting from an experiment that you ran previously.
+import warnings
 
-Use this script if:
-    - You want to evaluate a checkpoint resulting from one of your previous experiment,
-        using the same parameters (dataset, valid_metrics,...) as used during the training of the experiment.
-
-Don't use this script if:
-    - You want to train and evaluate a model (use examples/train_from_recipe_example)
-    - You want to evaluate a pretrained model from model zoo (use examples/evaluate_from_recipe_example)
-    - You want to evaluate a checkpoint from one of your previous experiment, but with different validation parameters
-        such as dataset params or metrics for instance (use examples/evaluate_from_recipe_example)
-
-Note:
-    The parameters will be unchanged even if the recipe used for that experiment was changed since then.
-    This is to ensure that validation of the experiment will remain exactly the same as during training.
-
-Example: python evaluate_checkpoint.py --experiment_name=my_experiment_name --ckpt_name=average_model.pth
--> Evaluate the checkpoint average_model from experiment my_experiment_name.
-
-"""
-from super_gradients import Trainer, init_trainer
-from super_gradients.common.environment.argparse_utils import pop_arg
-
-
-def main() -> None:
-    init_trainer()
-    experiment_name = pop_arg("experiment_name")
-    ckpt_name = pop_arg("ckpt_name", default_value="ckpt_latest.pth")
-    ckpt_root_dir = pop_arg("ckpt_root_dir", default_value=None)
-    Trainer.evaluate_checkpoint(experiment_name=experiment_name, ckpt_name=ckpt_name, ckpt_root_dir=ckpt_root_dir)
-
-
-def run():
-    init_trainer()
-    main()
+if __name__ == "__main__":
 
+    warnings.warn("This script is deprecated and will be removed in the future. Please use `super_gradients.evaluate_checkpoint` instead.", DeprecationWarning)
+    from super_gradients import evaluate_checkpoint
 
-if __name__ == "__main__":
-    run()
+    evaluate_checkpoint.main()
```

## super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py

```diff
@@ -1,45 +1,8 @@
-"""
-Evaluate a SuperGradient's recipes.
+import warnings
 
-Use this script if:
-    - You want to evaluate a pretrained model from model zoo
-    - You want to evaluate a checkpoint from one of your previous experiment, but with different validation parameters
-        such as dataset params or metrics for instance
-
-Don't use this script if:
-    - You want to train and evaluate a model (use examples/train_from_recipe_example)
-    - You want to evaluate a checkpoint from one of your previous experiment, using the same parameters as used during the
-        training of the experiment (use examples/evaluate_checkpoint_example)
-
-Note:
-    This script does NOT run TRAINING, so make sure in the recipe that you load a PRETRAINED MODEL
-    either from one of your checkpoint or from a pretrained model.
-
-General use: python evaluate_from_recipe.py --config-name="DESIRED_RECIPE".
--> Evaluate the latest checkpoint according to parameters set in "DESIRED_RECIPE"
-
-You can specify which checkpoint you want to evaluate by overriding training_hyperparams.ckpt_name as in the following example:
-python evaluate_from_recipe.py --config-name="DESIRED_RECIPE" training_hyperparams.ckpt_name=average_model.pth
--> Evaluate the checkpoint 'average_model.pth' according to parameters set in "DESIRED_RECIPE"
-
-For recipe's specific instructions and details refer to the recipe's configuration file in the recipes directory.
-"""
-from omegaconf import DictConfig
-import hydra
-import pkg_resources
-
-from super_gradients import Trainer, init_trainer
-
-
-@hydra.main(config_path=pkg_resources.resource_filename("super_gradients.recipes", ""), version_base="1.2")
-def main(cfg: DictConfig) -> None:
-    Trainer.evaluate_from_recipe(cfg)
-
-
-def run():
-    init_trainer()
-    main()
+if __name__ == "__main__":
 
+    warnings.warn("This script is deprecated and will be removed in the future. Please use `super_gradients.evaluate_from_recipe` instead.", DeprecationWarning)
+    from super_gradients import evaluate_from_recipe
 
-if __name__ == "__main__":
-    run()
+    evaluate_from_recipe.main()
```

## super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py

```diff
@@ -1,27 +1,8 @@
-"""
-Example code for running QAT on SuperGradient's recipes.
+import warnings
 
-General use: python train_from_recipe.py --config-name="DESIRED_RECIPE".
-For recipe's specific instructions and details refer to the recipe's configuration file in the recipes directory.
-"""
-
-import hydra
-import pkg_resources
-from omegaconf import DictConfig
-
-from super_gradients import init_trainer
-from super_gradients.training.qat_trainer.qat_trainer import QATTrainer
-
-
-@hydra.main(config_path=pkg_resources.resource_filename("super_gradients.recipes", ""), version_base="1.2")
-def main(cfg: DictConfig) -> None:
-    QATTrainer.train_from_config(cfg)
-
-
-def run():
-    init_trainer()
-    main()
+if __name__ == "__main__":
 
+    warnings.warn("This script is deprecated and will be removed in the future. Please use `super_gradients.qat_from_recipe` instead.", DeprecationWarning)
+    from super_gradients import qat_from_recipe
 
-if __name__ == "__main__":
-    run()
+    qat_from_recipe.main()
```

## super_gradients/examples/quantization/resnet_qat_example.py

```diff
@@ -6,15 +6,14 @@
 from super_gradients import Trainer
 from super_gradients.common.object_names import Models
 from super_gradients.modules.quantization.resnet_bottleneck import QuantBottleneck as sg_QuantizedBottleneck
 from super_gradients.training import MultiGPUMode
 from super_gradients.training import models as sg_models
 from super_gradients.training.dataloaders import imagenet_train, imagenet_val
 from super_gradients.training.metrics import Accuracy, Top5
-from super_gradients.training.metrics.metric_utils import get_metrics_dict
 from super_gradients.training.models.classification_models.resnet import Bottleneck
 from super_gradients.training.models.classification_models.resnet import Bottleneck as sg_Bottleneck
 from super_gradients.training.utils.quantization.calibrator import QuantizationCalibrator
 from super_gradients.training.utils.quantization.core import QuantizedMetadata
 from super_gradients.training.utils.quantization.export import export_quantized_module_to_onnx
 from super_gradients.training.utils.quantization.selective_quantization_utils import SelectiveQuantizer
 
@@ -108,13 +107,12 @@
 
     if args.calibrate:
         calibrator = QuantizationCalibrator(verbose=True)
         calibrator.calibrate_model(model, method="percentile", calib_data_loader=train_dataloader, num_calib_batches=1024 // args.batch or 1)
 
     trainer.train(model=model, training_params=train_params, train_loader=train_dataloader, valid_loader=val_dataloader)
 
-    val_results_tuple = trainer.test(model=model, test_loader=val_dataloader, test_metrics_list=[Accuracy()], metrics_progress_verbose=True)
-    valid_metrics_dict = get_metrics_dict(val_results_tuple, trainer.test_metrics, trainer.loss_logging_items_names)
+    valid_metrics_dict = trainer.test(model=model, test_loader=val_dataloader, test_metrics_list=[Accuracy()], metrics_progress_verbose=True)
 
     export_quantized_module_to_onnx(model=model, onnx_filename=f"{args.model_name}.onnx", input_shape=(args.batch, 3, 224, 224))
 
     print(f"FINAL ACCURACY: {valid_metrics_dict['Accuracy'].cpu().item()}")
```

## super_gradients/examples/resume_experiment_example/resume_experiment.py

```diff
@@ -1,18 +1,8 @@
-"""
-Example code for resuming SuperGradient's recipes.
+import warnings
 
-General use: python resume_experiment.py --experiment_name=<PREVIOUSLY-RUN-EXPERIMENT>
-"""
-from super_gradients import Trainer, init_trainer
-from super_gradients.common.environment.argparse_utils import pop_arg
-
-
-def main() -> None:
-    init_trainer()
-    experiment_name = pop_arg("experiment_name")
-    ckpt_root_dir = pop_arg("ckpt_root_dir")
-    Trainer.resume_experiment(experiment_name=experiment_name, ckpt_root_dir=ckpt_root_dir)
+if __name__ == "__main__":
 
+    warnings.warn("This script is deprecated and will be removed in the future. Please use `super_gradients.resume_experiment` instead.", DeprecationWarning)
+    from super_gradients import resume_experiment
 
-if __name__ == "__main__":
-    main()
+    resume_experiment.main()
```

## super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py

```diff
@@ -1,22 +1,8 @@
-"""
-Example code for running SuperGradient's recipes.
+import warnings
 
-General use: python train_from_kd_recipe.py --config-name="DESIRED_RECIPE".
-For recipe's specific instructions and details refer to the recipe's configuration file in the recipes directory.
-"""
-
-import super_gradients
-from omegaconf import DictConfig
-import hydra
-import pkg_resources
-from super_gradients.training.kd_trainer import KDTrainer
-
-
-@hydra.main(config_path=pkg_resources.resource_filename("super_gradients.recipes", ""), version_base="1.2")
-def main(cfg: DictConfig) -> None:
-    KDTrainer.train_from_config(cfg)
+if __name__ == "__main__":
 
+    warnings.warn("This script is deprecated and will be removed in the future. Please use `super_gradients.train_from_kd_recipe` instead.", DeprecationWarning)
+    from super_gradients import train_from_kd_recipe
 
-if __name__ == "__main__":
-    super_gradients.init_trainer()
-    main()
+    train_from_kd_recipe.main()
```

## super_gradients/examples/train_from_recipe_example/train_from_recipe.py

```diff
@@ -1,26 +1,8 @@
-"""
-Example code for running SuperGradient's recipes.
+import warnings
 
-General use: python train_from_recipe.py --config-name="DESIRED_RECIPE".
-For recipe's specific instructions and details refer to the recipe's configuration file in the recipes directory.
-"""
-
-from omegaconf import DictConfig
-import hydra
-import pkg_resources
-
-from super_gradients import Trainer, init_trainer
-
-
-@hydra.main(config_path=pkg_resources.resource_filename("super_gradients.recipes", ""), version_base="1.2")
-def main(cfg: DictConfig) -> None:
-    Trainer.train_from_config(cfg)
-
-
-def run():
-    init_trainer()
-    main()
+if __name__ == "__main__":
 
+    warnings.warn("This script is deprecated and will be removed in the future. Please use `super_gradients.train_from_recipe` instead.", DeprecationWarning)
+    from super_gradients import train_from_recipe
 
-if __name__ == "__main__":
-    run()
+    train_from_recipe.main()
```

## super_gradients/module_interfaces/__init__.py

```diff
@@ -1,3 +1,3 @@
-from .module_interfaces import HasPredict, HasPreprocessingParams
+from .module_interfaces import HasPredict, HasPreprocessingParams, SupportsReplaceNumClasses
 
-__all__ = ["HasPredict", "HasPreprocessingParams"]
+__all__ = ["HasPredict", "HasPreprocessingParams", "SupportsReplaceNumClasses"]
```

## super_gradients/module_interfaces/module_interfaces.py

```diff
@@ -1,7 +1,10 @@
+from typing import Callable
+
+from torch import nn
 from typing_extensions import Protocol, runtime_checkable
 
 
 @runtime_checkable
 class HasPreprocessingParams(Protocol):
     """
     Protocol interface for torch datasets that support getting preprocessing params, later to be passed to a model
@@ -27,7 +30,32 @@
         ...
 
     def predict(self, images, *args, **kwargs):
         ...
 
     def predict_webcam(self, *args, **kwargs):
         ...
+
+
+@runtime_checkable
+class SupportsReplaceNumClasses(Protocol):
+    """
+    Protocol interface for modules that support replacing the number of classes.
+    Derived classes should implement the `replace_num_classes` method.
+
+    This interface class serves a purpose of explicitly indicating whether a class supports optimized head replacement:
+
+    >>> class PredictionHead(nn.Module, SupportsReplaceNumClasses):
+    >>>    def replace_num_classes(self, num_classes: int, compute_new_weights_fn: Callable[[nn.Module, int], nn.Module] = None):
+    >>>       ...
+    """
+
+    def replace_num_classes(self, num_classes: int, compute_new_weights_fn: Callable[[nn.Module, int], nn.Module]):
+        """
+        Replace the number of classes in the module.
+
+        :param num_classes: New number of classes.
+        :param compute_new_weights_fn: (callable) An optional function that computes the new weights for the new classes.
+            It takes existing nn.Module and returns a new one.
+        :return: None
+        """
+        ...
```

## super_gradients/modules/__init__.py

```diff
@@ -1,39 +1,69 @@
 from super_gradients.modules.anti_alias import AntiAliasDownsample
+from super_gradients.modules.pixel_shuffle import PixelShuffle
 from super_gradients.modules.pose_estimation_modules import LightweightDEKRHead
-from super_gradients.modules.conv_bn_act_block import ConvBNAct
+from super_gradients.modules.conv_bn_act_block import ConvBNAct, Conv
 from super_gradients.modules.conv_bn_relu_block import ConvBNReLU
 from super_gradients.modules.repvgg_block import RepVGGBlock
 from super_gradients.modules.qarepvgg_block import QARepVGGBlock
 from super_gradients.modules.se_blocks import SEBlock, EffectiveSEBlock
 from super_gradients.modules.skip_connections import (
     Residual,
     SkipConnection,
     CrossModelSkipConnection,
     BackboneInternalSkipConnection,
     HeadInternalSkipConnection,
 )
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.registry.registry import ALL_DETECTION_MODULES
 
+from super_gradients.modules.base_modules import BaseDetectionModule
+from super_gradients.modules.detection_modules import (
+    PANNeck,
+    NHeads,
+    MultiOutputBackbone,
+    NStageBackbone,
+    MobileNetV1Backbone,
+    MobileNetV2Backbone,
+    SSDNeck,
+    SSDInvertedResidualNeck,
+    SSDBottleneckNeck,
+    SSDHead,
+)
+from super_gradients.module_interfaces import SupportsReplaceNumClasses
+
 __all__ = [
+    "BaseDetectionModule",
     "ALL_DETECTION_MODULES",
+    "PixelShuffle",
     "AntiAliasDownsample",
+    "Conv",
     "ConvBNAct",
     "ConvBNReLU",
     "RepVGGBlock",
     "QARepVGGBlock",
     "SEBlock",
     "EffectiveSEBlock",
     "Residual",
     "SkipConnection",
     "CrossModelSkipConnection",
     "BackboneInternalSkipConnection",
     "HeadInternalSkipConnection",
     "LightweightDEKRHead",
+    "PANNeck",
+    "NHeads",
+    "MultiOutputBackbone",
+    "NStageBackbone",
+    "MobileNetV1Backbone",
+    "MobileNetV2Backbone",
+    "SSDNeck",
+    "SSDInvertedResidualNeck",
+    "SSDBottleneckNeck",
+    "SSDHead",
+    "SupportsReplaceNumClasses",
 ]
 
 logger = get_logger(__name__)
 try:
     # flake8 respects only the first occurence of __all__ defined in the module's root
     from .quantization import QuantBottleneck  # noqa: F401
```

## super_gradients/modules/conv_bn_act_block.py

```diff
@@ -1,11 +1,13 @@
 from typing import Union, Tuple, Type
 
 from torch import nn
 
+from super_gradients.modules.utils import autopad
+
 
 class ConvBNAct(nn.Module):
     """
     Class for Convolution2d-Batchnorm2d-Activation layer.
         Default behaviour is Conv-BN-Act. To exclude Batchnorm module use
         `use_normalization=False`, to exclude activation use `activation_type=None`.
     For convolution arguments documentation see `nn.Conv2d`.
@@ -60,7 +62,26 @@
                 nn.BatchNorm2d(out_channels, eps=eps, momentum=momentum, affine=affine, track_running_stats=track_running_stats, device=device, dtype=dtype),
             )
         if activation_type is not None:
             self.seq.add_module("act", activation_type(**activation_kwargs))
 
     def forward(self, x):
         return self.seq(x)
+
+
+class Conv(nn.Module):
+    # STANDARD CONVOLUTION
+    # TODO: This class is illegaly similar to ConvBNAct, and the only reason it exists is due to fact that some models were using it
+    # previosly and one have to find a bulletproof way drop this class but still be able to load models that were using it. Perhaps
+    # it is possible through load_state_dict / save_state_dict magic.
+    def __init__(self, input_channels, output_channels, kernel, stride, activation_type: Type[nn.Module], padding: int = None, groups: int = None):
+        super().__init__()
+
+        self.conv = nn.Conv2d(input_channels, output_channels, kernel, stride, autopad(kernel, padding), groups=groups or 1, bias=False)
+        self.bn = nn.BatchNorm2d(output_channels)
+        self.act = activation_type()
+
+    def forward(self, x):
+        return self.act(self.bn(self.conv(x)))
+
+    def fuseforward(self, x):
+        return self.act(self.conv(x))
```

## super_gradients/modules/detection_modules.py

```diff
@@ -1,41 +1,34 @@
+from abc import ABC, abstractmethod
 from typing import Union, List
-from abc import abstractmethod, ABC
 
 import torch
-from torch import nn
-from omegaconf.listconfig import ListConfig
 from omegaconf import DictConfig
-
+from omegaconf.listconfig import ListConfig
 from super_gradients.common.registry.registry import register_detection_module
+from super_gradients.modules.base_modules import BaseDetectionModule
+from super_gradients.modules.multi_output_modules import MultiOutputModule
+from super_gradients.training.models import MobileNet, MobileNetV2
 from super_gradients.training.models.classification_models.mobilenetv2 import InvertedResidual
 from super_gradients.training.utils.utils import HpmStruct
-from super_gradients.training.models import MobileNet, MobileNetV2
-from super_gradients.modules.multi_output_modules import MultiOutputModule
-
-
-class BaseDetectionModule(nn.Module, ABC):
-    """
-    An interface for a module that is easy to integrate into a model with complex connections
-    """
-
-    def __init__(self, in_channels: Union[List[int], int], **kwargs):
-        """
-        :param in_channels: defines channels of tensor(s) that will be accepted by a module in forward
-        """
-        super().__init__()
-        self.in_channels = in_channels
+from torch import nn
 
-    @property
-    @abstractmethod
-    def out_channels(self) -> Union[List[int], int]:
-        """
-        :return: channels of tensor(s) that will be returned by a module  in forward
-        """
-        raise NotImplementedError()
+__all__ = [
+    "PANNeck",
+    "NHeads",
+    "MultiOutputBackbone",
+    "NStageBackbone",
+    "MobileNetV1Backbone",
+    "MobileNetV2Backbone",
+    "SSDNeck",
+    "SSDInvertedResidualNeck",
+    "SSDBottleneckNeck",
+    "SSDHead",
+    "BaseDetectionModule",
+]
 
 
 @register_detection_module()
 class NStageBackbone(BaseDetectionModule):
     """
     A backbone with a stem -> N stages -> context module
     Returns outputs of the layers listed in out_layers
```

## super_gradients/modules/pose_estimation_modules.py

```diff
@@ -1,15 +1,15 @@
 from typing import Type, Tuple, Union, List
 
 import torch
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.activations_type_factory import ActivationsTypeFactory
 from torch import nn, Tensor
 
-from super_gradients.modules.detection_modules import BaseDetectionModule
+from super_gradients.modules.base_modules import BaseDetectionModule
 from super_gradients.common.registry.registry import register_detection_module
 
 
 @register_detection_module()
 class LightweightDEKRHead(BaseDetectionModule):
     """
     Prediction head for pose estimation task that mimics approach from DEKR (https://arxiv.org/abs/2104.02300) paper,
```

## super_gradients/modules/sampling.py

```diff
@@ -1,29 +1,37 @@
 from typing import Union, Optional
 
 from torch import nn
 
 from super_gradients.common import UpsampleMode
 from super_gradients.common.data_types.enum import DownSampleMode
-from super_gradients.modules.anti_alias import AntiAliasDownsample
+from super_gradients.modules import AntiAliasDownsample, PixelShuffle
 
 
 def make_upsample_module(scale_factor: int, upsample_mode: Union[str, UpsampleMode], align_corners: Optional[bool] = None):
     """
     Factory method for creating upsampling modules.
     :param scale_factor: upsample scale factor
     :param upsample_mode: see UpsampleMode for supported options.
     :return: nn.Module
     """
     upsample_mode = upsample_mode.value if isinstance(upsample_mode, UpsampleMode) else upsample_mode
+
     if upsample_mode == UpsampleMode.NEAREST.value:
         # Prevent ValueError when passing align_corners with nearest mode.
         module = nn.Upsample(scale_factor=scale_factor, mode=upsample_mode)
+
     elif upsample_mode in [UpsampleMode.BILINEAR.value, UpsampleMode.BICUBIC.value]:
         module = nn.Upsample(scale_factor=scale_factor, mode=upsample_mode, align_corners=align_corners)
+
+    elif upsample_mode == UpsampleMode.PIXEL_SHUFFLE.value:
+        module = PixelShuffle(upscale_factor=scale_factor)
+
+    elif upsample_mode == UpsampleMode.NN_PIXEL_SHUFFLE.value:
+        module = nn.PixelShuffle(upscale_factor=scale_factor)
     else:
         raise NotImplementedError(f"Upsample mode: `{upsample_mode}` is not supported.")
     return module
 
 
 def make_downsample_module(in_channels: int, stride: int, downsample_mode: Union[str, DownSampleMode]):
     """
```

## super_gradients/modules/utils.py

```diff
@@ -1,8 +1,9 @@
 import copy
+import math
 from typing import List
 
 import torch
 from torch import nn
 
 
 def _replace_activations_recursive(module: nn.Module, new_activation: nn.Module, activations_to_replace: List[type]):
@@ -53,7 +54,21 @@
 
         self.additive = torch.nn.Parameter((mean_original - mean_required) / std_original)
         self.multiplier = torch.nn.Parameter(std_original / std_required)
 
     def forward(self, x):
         x = (x + self.additive) * self.multiplier
         return x
+
+
+def width_multiplier(original, factor, divisor: int = None):
+    if divisor is None:
+        return int(original * factor)
+    else:
+        return math.ceil(int(original * factor) / divisor) * divisor
+
+
+def autopad(kernel, padding=None):
+    # PAD TO 'SAME'
+    if padding is None:
+        padding = kernel // 2 if isinstance(kernel, int) else [x // 2 for x in kernel]
+    return padding
```

## super_gradients/recipes/cifar10_resnet.yaml

```diff
@@ -1,39 +1,24 @@
 # Cifar10 Classification Training:
 # Reaches ~94.9 Accuracy after 250 Epochs
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=cifar10_resnet +experiment_name=cifar10
+#       python -m super_gradients.train_from_recipe --config-name=cifar10_resnet +experiment_name=cifar10
 #
 #   To use equivalent Albumentations transforms pipeline set dataset_params to cifar10_albumentations_dataset_params:
-#     python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=cifar10_resnet dataset_params=cifar10_albumentations_dataset_params
+#     python -m super_gradients.train_from_recipe --config-name=cifar10_resnet dataset_params=cifar10_albumentations_dataset_params
 defaults:
   - training_hyperparams: cifar10_resnet_train_params
   - dataset_params: cifar10_dataset_params
   - arch_params: resnet18_cifar_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: cifar10_train
 val_dataloader: cifar10_val
-
-data_loader_num_workers: 8
-
-resume: False
-training_hyperparams:
-  resume: ${resume}
-
-ckpt_root_dir:
-
 architecture: resnet18_cifar
-
-experiment_name: resnet18_cifar
-
+experiment_name: resnet18_cifar_interpolation_check
 multi_gpu: Off
 num_gpus: 1
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/cityscapes_ddrnet.yaml

```diff
@@ -5,17 +5,17 @@
 #
 
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#      DDRNet23:        python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=cityscapes_ddrnet
-#      DDRNet23-Slim:   python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=cityscapes_ddrnet architecture=ddrnet_23_slim
-#      DDRNet39:        python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=cityscapes_ddrnet architecture=ddrnet_39
+#      DDRNet23:        python -m super_gradients.train_from_recipe --config-name=cityscapes_ddrnet
+#      DDRNet23-Slim:   python -m super_gradients.train_from_recipe --config-name=cityscapes_ddrnet architecture=ddrnet_23_slim
+#      DDRNet39:        python -m super_gradients.train_from_recipe --config-name=cityscapes_ddrnet architecture=ddrnet_39
 # Note: add "checkpoint_params.checkpoint_path=<ddrnet23-backbone-pretrained-path>" to use pretrained backbone
 #
 #  Validation mIoU - Cityscapes, training time:
 #      DDRNet23:        input-size: [1024, 2048]     mIoU: 80.26     4 X RTX A5000, 12 H
 #      DDRNet23-Slim:   input-size: [1024, 2048]     mIoU: 78.01     4 X RTX A5000, 9 H
 #      DDRNet39:        input-size: [1024, 2048]     mIoU: 81.32     4 X RTX A5000, 15 H
 #
@@ -42,14 +42,15 @@
 #      * Pretrained backbones were used.
 
 defaults:
   - training_hyperparams: cityscapes_default_train_params
   - dataset_params: cityscapes_ddrnet_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: cityscapes_train
 val_dataloader: cityscapes_val
 
 architecture: ddrnet_23
 
 training_hyperparams:
@@ -79,19 +80,9 @@
   load_checkpoint: ${load_checkpoint}
   checkpoint_path:
   load_backbone: True
   strict_load: no_key_matching
 
 experiment_name: ${architecture}_cityscapes
 
-
-ckpt_root_dir:
-
 multi_gpu: DDP
 num_gpus: 4
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/cityscapes_kd_base.yaml

```diff
@@ -1,15 +1,15 @@
 # Distillation for semantic segmentation on Cityscapes dataset.
 #
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#      DDRNet23:        python src/super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py --config-name=cityscapes_kd_base student_architecture=ddrnet_23
-#      DDRNet23-Slim:   python src/super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py --config-name=cityscapes_kd_base student_architecture=ddrnet_23_slim
+#      DDRNet23:        python -m super_gradients.train_from_kd_recipe --config-name=cityscapes_kd_base student_architecture=ddrnet_23
+#      DDRNet23-Slim:   python -m super_gradients.train_from_kd_recipe --config-name=cityscapes_kd_base student_architecture=ddrnet_23_slim
 # Note: add "student_checkpoint_params.checkpoint_path=<ddrnet23-backbone-pretrained-path>" to use pretrained backbone
 #
 #  Teachers specifications:
 #      DDRNet39-AL:     mIoU: 85.17     notes: trained with Cityscapes coarse data.
 #
 #  Validation mIoU results - Cityscapes, training time:
 #      DDRNet23:        teacher: DDRNet39-AL  input-size: [1024, 2048]     mIoU: 81.48     4 X RTX A5000, 13 H
@@ -35,14 +35,15 @@
 #      * Default hyper-parameters are based on DDRNet model train recipes, for full resolution training [1024 x 2048]
 
 defaults:
   - training_hyperparams: cityscapes_default_train_params
   - dataset_params: cityscapes_ddrnet_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: cityscapes_train
 val_dataloader: cityscapes_val
 
 resume: False
 training_hyperparams:
   sync_bn: True
@@ -92,14 +93,7 @@
 num_gpus: 4
 
 architecture: kd_module
 student_architecture: ???
 teacher_architecture: ddrnet_39
 
 experiment_name: ${student_architecture}_teacher-${teacher_architecture}
-ckpt_root_dir:
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/cityscapes_pplite_seg50.yaml

```diff
@@ -4,16 +4,16 @@
 #     Qingqing Dang,Baohua Lai, Qiwen Liu, Xiaoguang Hu, Dianhai Yu, Yanjun Ma.
 #     PP-LiteSeg: A Superior Real-Time Semantic Segmentation Model.
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       PPLite-T-Seg50: python src/super_gradients/examples/train_from_recipe.py --config-name=cityscapes_pplite_seg50 checkpoint_params.checkpoint_path=<stdc1-backbone-pretrained-path> architecture=pp_lite_t_seg
-#       PPLite-B-Seg50: python src/super_gradients/examples/train_from_recipe.py --config-name=cityscapes_pplite_seg50 checkpoint_params.checkpoint_path=<stdc2-backbone-pretrained-path> architecture=pp_lite_b_seg
+#       PPLite-T-Seg50: python -m super_gradients.train_from_recipe --config-name=cityscapes_pplite_seg50 checkpoint_params.checkpoint_path=<stdc1-backbone-pretrained-path> architecture=pp_lite_t_seg
+#       PPLite-B-Seg50: python -m super_gradients.train_from_recipe --config-name=cityscapes_pplite_seg50 checkpoint_params.checkpoint_path=<stdc2-backbone-pretrained-path> architecture=pp_lite_b_seg
 #
 #
 #  Validation mIoU - Cityscapes, training time:
 #      PPLite-T-Seg50:    input-size: [512, 1024]     mIoU: 74.92     4 X RTX A5000, 13 H
 #      PPLite-B-Seg50:    input-size: [512, 1024]     mIoU: 76.48     4 X RTX A5000, 14 H
 #
 #  Official git repo:
@@ -38,14 +38,15 @@
 #      * ImageNet Pretrained backbones were used.
 
 defaults:
   - training_hyperparams: cityscapes_default_train_params
   - dataset_params: cityscapes_stdc_seg50_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: cityscapes_train
 val_dataloader: cityscapes_val
 
 architecture: pp_lite_t_seg
 
 dataset_params:
@@ -77,15 +78,7 @@
       ce_edge_weights: [ .5, .5 ]
       edge_kernel: 5
 
 multi_gpu: DDP
 num_gpus: 4
 
 experiment_name: ${architecture}50_cityscapes
-ckpt_root_dir:
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/cityscapes_pplite_seg75.yaml

```diff
@@ -4,16 +4,16 @@
 #     Qingqing Dang,Baohua Lai, Qiwen Liu, Xiaoguang Hu, Dianhai Yu, Yanjun Ma.
 #     PP-LiteSeg: A Superior Real-Time Semantic Segmentation Model.
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       PPLite-T-Seg75: python src/super_gradients/examples/train_from_recipe.py --config-name=cityscapes_pplite_seg75 checkpoint_params.checkpoint_path=<stdc1-backbone-pretrained-path> architecture=pp_lite_t_seg
-#       PPLite-B-Seg75: python src/super_gradients/examples/train_from_recipe.py --config-name=cityscapes_pplite_seg75 checkpoint_params.checkpoint_path=<stdc2-backbone-pretrained-path> architecture=pp_lite_b_seg
+#       PPLite-T-Seg75: python -m super_gradients.train_from_recipe --config-name=cityscapes_pplite_seg75 checkpoint_params.checkpoint_path=<stdc1-backbone-pretrained-path> architecture=pp_lite_t_seg
+#       PPLite-B-Seg75: python -m super_gradients.train_from_recipe --config-name=cityscapes_pplite_seg75 checkpoint_params.checkpoint_path=<stdc2-backbone-pretrained-path> architecture=pp_lite_b_seg
 #
 #
 #  Validation mIoU - Cityscapes, training time:
 #      PPLite-T-Seg75:    input-size: [768, 1536]     mIoU: 77.56     4 X RTX A5000, 13 H
 #      PPLite-B-Seg75:    input-size: [768, 1536]     mIoU: 78.52     4 X RTX A5000, 14 H
 #
 #  Official git repo:
@@ -38,14 +38,15 @@
 #      * ImageNet Pretrained backbones were used.
 
 defaults:
   - training_hyperparams: cityscapes_default_train_params
   - dataset_params: cityscapes_ppliteseg_seg75_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: cityscapes_train
 val_dataloader: cityscapes_val
 
 
 architecture: pp_lite_t_seg
 
@@ -72,15 +73,7 @@
       ce_edge_weights: [ .5, .5 ]
       edge_kernel: 5
 
 multi_gpu: DDP
 num_gpus: 4
 
 experiment_name: ${architecture}75_cityscapes
-ckpt_root_dir:
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/cityscapes_regseg48.yaml

```diff
@@ -2,15 +2,15 @@
 #  Reproduction of paper: Rethink Dilated Convolution for Real-time Semantic Segmentation.
 #
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=cityscapes_regseg48
+#       python -m super_gradients.train_from_recipe --config-name=cityscapes_regseg48
 #
 #
 #  Validation mIoU - Cityscapes, training time:
 #      RegSeg48:    input-size: [1024, 2048]     mIoU: 78.15  using 4 GeForce RTX 2080 Ti with DDP, ~2 minutes / epoch
 #
 #  Official git repo:
 #      https://github.com/RolandGao/RegSeg
@@ -26,29 +26,30 @@
 #      RegSeg48:    input-size: [1024, 2048]     initial_lr: 0.02    batch-size: 4 * 4gpus = 16
 
 defaults:
   - training_hyperparams: default_train_params
   - dataset_params: cityscapes_regseg48_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: cityscapes_train
 val_dataloader: cityscapes_val
 
 cityscapes_ignored_label: 19    # convenience parameter since it is used in many places in the YAML
 
 architecture: regseg48
 
 arch_params:
   num_classes: 19
   strict_load: no_key_matching
 
 load_checkpoint: False
 
-ckpt_root_dir:
+
 
 resume: False
 training_hyperparams:
   sync_bn: True
   resume: ${resume}
   max_epochs: 800
   lr_mode: poly
@@ -85,14 +86,7 @@
   _convert_: all
 
 project_name: RegSeg
 experiment_name: ${architecture}_cityscapes
 
 multi_gpu: AUTO
 num_gpus: 4
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/cityscapes_segformer.yaml

```diff
@@ -16,15 +16,15 @@
 #      https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/Dataset_Setup_Instructions.md
 #   3. Note: if you change the dataset's internal directory structure, make changes to the fields "list_file" and
 #      "labels_csv_path" of both "train_dataset_params" and "val_dataset_params" accordingly
 #   4. Edit the "data_root_dir" field below to point to the absolute path of the data root directory
 #   5. Edit the "ckpt_root_dir" field to the path where you want to save checkpoints and logs
 #   6. Move to the project root (where you will find the ReadMe and src folder)
 #   7. Run the command (change:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=cityscapes_segformer
+#       python -m super_gradients.train_from_recipe --config-name=cityscapes_segformer
 #
 #
 # Imagenet-1K pre-trained backbone:
 #   MiT (Mix Transformer) B0:   https://deci-pretrained-models.s3.amazonaws.com/mit_backbones/mit_b0.pth
 #                         B1:   https://deci-pretrained-models.s3.amazonaws.com/mit_backbones/mit_b1.pth
 #                         B2:   https://deci-pretrained-models.s3.amazonaws.com/mit_backbones/mit_b2.pth
 #                         B3:   https://deci-pretrained-models.s3.amazonaws.com/mit_backbones/mit_b3.pth
@@ -41,26 +41,27 @@
 
 
 defaults:
   - training_hyperparams: default_train_params
   - dataset_params: cityscapes_segformer_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 architecture: segformer_b0    # segformer_b1, segformer_b2, segformer_b3, segformer_b4, segformer_b5
 
 data_root_dir: /data/cityscapes
 dataset_params:
   train_dataset_params:
     root_dir: ${data_root_dir}
   val_dataset_params:
     root_dir: ${data_root_dir}
 
 experiment_name: ${architecture}_cityscapes
-ckpt_root_dir:
+
 
 train_dataloader: cityscapes_train
 val_dataloader: cityscapes_val
 
 cityscapes_ignored_label: 19    # convenience parameter since it is used in many places in the YAML
 
 arch_params:
@@ -104,14 +105,7 @@
         ignore_index: ${cityscapes_ignored_label}
 
   metric_to_watch: IoU
   greater_metric_to_watch_is_better: True
 
 multi_gpu: DDP
 num_gpus: 4
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/cityscapes_stdc_base.yaml

```diff
@@ -1,14 +1,15 @@
 # STDC Base training params
 
 defaults:
   - training_hyperparams: cityscapes_default_train_params
   - dataset_params: cityscapes_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: cityscapes_train
 val_dataloader: cityscapes_val
 
 data_loader_num_workers: 10
 
 arch_params:
@@ -25,17 +26,10 @@
 experiment_name: ${architecture}_cityscapes
 
 training_hyperparams:
   sync_bn: True
 
 
 
-ckpt_root_dir:
-
-multi_gpu: DDP
 
 
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
+multi_gpu: DDP
```

## super_gradients/recipes/cityscapes_stdc_seg50.yaml

```diff
@@ -2,16 +2,16 @@
 #  Reproduction and refinement of paper: Rethinking BiSeNet For Real-time Semantic Segmentation.
 #
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       STDC1-Seg50: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=cityscapes_stdc_seg50
-#       STDC2-Seg50: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=cityscapes_stdc_seg50 architecture=stdc2_seg
+#       STDC1-Seg50: python -m super_gradients.train_from_recipe --config-name=cityscapes_stdc_seg50
+#       STDC2-Seg50: python -m super_gradients.train_from_recipe --config-name=cityscapes_stdc_seg50 architecture=stdc2_seg
 # Note: add "checkpoint_params.checkpoint_path=<stdc1-backbone-pretrained-path>" to use pretrained backbone
 #
 #
 #
 #  Validation mIoU - Cityscapes, training time:
 #      STDC1-Seg50:    input-size: [512, 1024]     mIoU: 75.11     2 X RTX A5000, 20 H
 #      STDC2-Seg50:    input-size: [512, 1024]     mIoU: 76.44     2 X RTX A5000, 23 H
@@ -38,14 +38,15 @@
 #      * Pretrained backbones were used.
 
 defaults:
   - training_hyperparams: cityscapes_default_train_params
   - dataset_params: cityscapes_stdc_seg50_dataset_params # TODO: uncomment after DatasetInterface refactor
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: cityscapes_train
 val_dataloader: cityscapes_val
 
 architecture: stdc1_seg
 
 arch_params:
@@ -69,15 +70,7 @@
       ce_edge_weights: [ .5, .5 ]
       edge_kernel: 3
 
 multi_gpu: DDP
 num_gpus: 2
 
 experiment_name: ${architecture}50_cityscapes
-ckpt_root_dir:
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/cityscapes_stdc_seg75.yaml

```diff
@@ -2,16 +2,16 @@
 #  Reproduction and refinement of paper: Rethinking BiSeNet For Real-time Semantic Segmentation.
 #
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       STDC1-Seg75: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=cityscapes_stdc_seg75
-#       STDC2-Seg75: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=cityscapes_stdc_seg75 architecture=stdc2_seg
+#       STDC1-Seg75: python -m super_gradients.train_from_recipe --config-name=cityscapes_stdc_seg75
+#       STDC2-Seg75: python -m super_gradients.train_from_recipe --config-name=cityscapes_stdc_seg75 architecture=stdc2_seg
 # Note: add "external_checkpoint_path=<stdc1-backbone-pretrained-path>" to use pretrained backbone
 #
 #
 #
 #  Validation mIoU - Cityscapes, training time:
 #      STDC1-Seg75:    input-size: [768, 1536]     mIoU: 76.87     4 X RTX A5000, 29 H, early stopped after 711 epochs
 #      STDC2-Seg75:    input-size: [768, 1536]     mIoU: 78.93     2 X RTX A5000, 29 H, early stopped after 530 epochs
@@ -41,14 +41,15 @@
 #          module, different auxiliary feature maps and different loss weights.
 
 defaults:
   - training_hyperparams: cityscapes_default_train_params
   - dataset_params: cityscapes_stdc_seg75_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: cityscapes_train
 val_dataloader: cityscapes_val
 
 
 architecture: stdc1_seg
 
@@ -73,16 +74,7 @@
       mining_percent: 0.0625 # mining percentage is 1/16 of pixels following original implementation.
       weights: [ 1., 0.6, 0.4, 1. ]
 
 multi_gpu: DDP
 num_gpus: 4
 
 experiment_name: ${architecture}75_cityscapes
-ckpt_root_dir:
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
-
```

## super_gradients/recipes/coco2017_pose_ddrnet39.yaml

```diff
@@ -2,26 +2,27 @@
 
 defaults:
   - training_hyperparams: coco2017_dekr_pose_train_params
   - dataset_params: coco_pose_estimation_dekr_dataset_params
   - arch_params: pose_ddrnet39_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 resume: False
 
 architecture: pose_ddrnet39
 
 multi_gpu: DDP
 num_gpus: 8
 
 experiment_suffix: ""
 experiment_name: coco2017_${architecture}${experiment_suffix}
 
-ckpt_root_dir:
+
 
 train_dataloader: coco2017_pose_train
 val_dataloader: coco2017_pose_val
 
 arch_params:
   num_classes: ${dataset_params.num_joints}
 
@@ -55,13 +56,7 @@
 #        phase:
 #          _target_: super_gradients.training.utils.callbacks.callbacks.Phase
 #          value: VALIDATION_BATCH_END
 #        prefix: "val_"
 #        mean: [ 0.485, 0.456, 0.406 ]
 #        std: [ 0.229, 0.224, 0.225 ]
 #        apply_sigmoid: False
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml

```diff
@@ -3,15 +3,15 @@
 #
 #  Recipe runs with batch size = 8 X 8 gpus = 64.
 #
 #  Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       DEKR-W32: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_pose_dekr_w32_no_dc
+#       DEKR-W32: python -m super_gradients.train_from_recipe --config-name=coco2017_pose_dekr_w32_no_dc
 #  NOTE: Add "checkpoint_params.checkpoint_path=<hrnet-pretrained-path>" to use pretrained backbone (See line 55).
 #
 #
 #  Validation AP (Without multiscale & flip augmentation) - COCO, training time:
 #      DEKR-W32:    input-size: [640, 640]     AP: TBD    8 X RTX A5000
 #
 #
@@ -28,26 +28,27 @@
 
 defaults:
   - training_hyperparams: coco2017_dekr_pose_train_params
   - dataset_params: coco_pose_estimation_dekr_dataset_params
   - arch_params: pose_dekr_w32_no_dc_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 resume: False
 
 architecture: dekr_w32_no_dc
 
 multi_gpu: DDP
 num_gpus: 8
 
 experiment_suffix: ""
 experiment_name: coco2017_pose_${architecture}_${experiment_suffix}
 
-ckpt_root_dir:
+
 
 train_dataloader: coco2017_pose_train
 val_dataloader: coco2017_pose_val
 
 arch_params:
   num_classes: ${dataset_params.num_joints}
 
@@ -90,13 +91,7 @@
 #        phase:
 #          _target_: super_gradients.training.utils.callbacks.callbacks.Phase
 #          value: VALIDATION_BATCH_END
 #        prefix: "val_"
 #        mean: [ 0.485, 0.456, 0.406 ]
 #        std: [ 0.229, 0.224, 0.225 ]
 #        apply_sigmoid: False
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/coco2017_pose_pppose_l.yaml

```diff
@@ -2,26 +2,27 @@
 
 defaults:
   - training_hyperparams: coco2017_dekr_pose_train_params
   - dataset_params: coco_pose_estimation_dekr_dataset_params
   - arch_params: pose_pppose_l_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 resume: False
 
 architecture: pose_ppyolo_l
 
 multi_gpu: DDP
 num_gpus: 8
 
 experiment_suffix: ""
 experiment_name: coco2017_${architecture}${experiment_suffix}
 
-ckpt_root_dir:
+
 
 train_dataloader: coco2017_pose_train
 val_dataloader: coco2017_pose_val
 
 arch_params:
   num_classes: ${dataset_params.num_joints}
 
@@ -59,13 +60,7 @@
 #        phase:
 #          _target_: super_gradients.training.utils.callbacks.callbacks.Phase
 #          value: VALIDATION_BATCH_END
 #        prefix: "val_"
 #        mean: [ 0.485, 0.456, 0.406 ]
 #        std: [ 0.229, 0.224, 0.225 ]
 #        apply_sigmoid: False
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/coco2017_ppyoloe_l.yaml

```diff
@@ -4,32 +4,33 @@
 # Recipe runs with batch size = 20 X 8 gpus = 160.
 
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command you want:
-#         ppyoloe_s: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_s
-#         ppyoloe_m: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_m
-#         ppyoloe_l: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_l
-#         ppyoloe_x: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_x
+#         ppyoloe_s: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_s
+#         ppyoloe_m: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_m
+#         ppyoloe_l: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_l
+#         ppyoloe_x: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_x
 #
 # Training times and accuracies (mAP@0.5-0.95 (COCO API, confidence 0.001, IoU threshold 0.6, test on 640x640 images):
 #         ppyoloe_s: 37h  on 8 NVIDIA GeForce RTX 3090, mAP: 42.52 (val)
 #         ppyoloe_m: 58h  on 8 NVIDIA GeForce RTX 3090, mAP: 47.11 (val)
 #         ppyoloe_l: 115h on 8 NVIDIA GeForce RTX 3090, mAP: 49.48 (val)
 #         ppyoloe_x: 240h on 8 NVIDIA GeForce RTX 3090, mAP: 51.15 (val)
 #
 
 defaults:
   - training_hyperparams: coco2017_ppyoloe_train_params
   - dataset_params: coco_detection_ppyoloe_dataset_params
   - arch_params: ppyoloe_l_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: coco2017_train_ppyoloe
 val_dataloader: coco2017_val_ppyoloe
 
 load_checkpoint: False
 resume: False
 
@@ -46,16 +47,7 @@
 architecture: pp_yoloe_l
 
 multi_gpu: DDP
 num_gpus: 8
 
 experiment_suffix: ""
 experiment_name: coco2017_${architecture}${experiment_suffix}
-
-ckpt_root_dir:
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/coco2017_ppyoloe_m.yaml

```diff
@@ -4,32 +4,33 @@
 # Recipe runs with batch size = 24 X 8 gpus = 192.
 
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command you want:
-#         ppyoloe_s: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_s
-#         ppyoloe_m: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_m
-#         ppyoloe_l: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_l
-#         ppyoloe_x: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_x
+#         ppyoloe_s: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_s
+#         ppyoloe_m: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_m
+#         ppyoloe_l: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_l
+#         ppyoloe_x: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_x
 #
 # Training times and accuracies (mAP@0.5-0.95 (COCO API, confidence 0.001, IoU threshold 0.6, test on 640x640 images):
 #         ppyoloe_s: 37h  on 8 NVIDIA GeForce RTX 3090, mAP: 42.52 (val)
 #         ppyoloe_m: 58h  on 8 NVIDIA GeForce RTX 3090, mAP: 47.11 (val)
 #         ppyoloe_l: 115h on 8 NVIDIA GeForce RTX 3090, mAP: 49.48 (val)
 #         ppyoloe_x: 240h on 8 NVIDIA GeForce RTX 3090, mAP: 51.15 (val)
 #
 
 defaults:
   - training_hyperparams: coco2017_ppyoloe_train_params
   - dataset_params: coco_detection_ppyoloe_dataset_params
   - arch_params: ppyoloe_m_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: coco2017_train_ppyoloe
 val_dataloader: coco2017_val_ppyoloe
 
 load_checkpoint: False
 resume: False
 
@@ -46,16 +47,7 @@
 architecture: pp_yoloe_m
 
 multi_gpu: DDP
 num_gpus: 8
 
 experiment_suffix: ""
 experiment_name: coco2017_${architecture}${experiment_suffix}
-
-ckpt_root_dir:
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/coco2017_ppyoloe_s.yaml

```diff
@@ -2,32 +2,33 @@
 # PP-Yolo-E trained in 640x640
 # Recipe runs with batch size = 32 X 8 gpus = 256.
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command you want:
-#         ppyoloe_s: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_s
-#         ppyoloe_m: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_m
-#         ppyoloe_l: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_l
-#         ppyoloe_x: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_x
+#         ppyoloe_s: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_s
+#         ppyoloe_m: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_m
+#         ppyoloe_l: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_l
+#         ppyoloe_x: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_x
 #
 # Training times and accuracies (mAP@0.5-0.95 (COCO API, confidence 0.001, IoU threshold 0.6, test on 640x640 images):
 #         ppyoloe_s: 37h  on 8 NVIDIA GeForce RTX 3090, mAP: 42.52 (val)
 #         ppyoloe_m: 58h  on 8 NVIDIA GeForce RTX 3090, mAP: 47.11 (val)
 #         ppyoloe_l: 115h on 8 NVIDIA GeForce RTX 3090, mAP: 49.48 (val)
 #         ppyoloe_x: 240h on 8 NVIDIA GeForce RTX 3090, mAP: 51.15 (val)
 #
 
 defaults:
   - training_hyperparams: coco2017_ppyoloe_train_params
   - dataset_params: coco_detection_ppyoloe_dataset_params
   - arch_params: ppyoloe_s_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: coco2017_train_ppyoloe
 val_dataloader: coco2017_val_ppyoloe
 
 load_checkpoint: False
 resume: False
 
@@ -42,16 +43,7 @@
 architecture: pp_yoloe_s
 
 multi_gpu: DDP
 num_gpus: 8
 
 experiment_suffix: ""
 experiment_name: coco2017_${architecture}${experiment_suffix}
-
-ckpt_root_dir:
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/coco2017_ppyoloe_x.yaml

```diff
@@ -4,32 +4,33 @@
 # Recipe runs with batch size = 16 X 8 gpus = 128.
 
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command you want:
-#         ppyoloe_s: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_s
-#         ppyoloe_m: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_m
-#         ppyoloe_l: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_l
-#         ppyoloe_x: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ppyoloe_x
+#         ppyoloe_s: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_s
+#         ppyoloe_m: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_m
+#         ppyoloe_l: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_l
+#         ppyoloe_x: python -m super_gradients.train_from_recipe --config-name=coco2017_ppyoloe_x
 #
 # Training times and accuracies (mAP@0.5-0.95 (COCO API, confidence 0.001, IoU threshold 0.6, test on 640x640 images):
 #         ppyoloe_s: 37h  on 8 NVIDIA GeForce RTX 3090, mAP: 42.52 (val)
 #         ppyoloe_m: 58h  on 8 NVIDIA GeForce RTX 3090, mAP: 47.11 (val)
 #         ppyoloe_l: 115h on 8 NVIDIA GeForce RTX 3090, mAP: 49.48 (val)
 #         ppyoloe_x: 240h on 8 NVIDIA GeForce RTX 3090, mAP: 51.15 (val)
 #
 
 defaults:
   - training_hyperparams: coco2017_ppyoloe_train_params
   - dataset_params: coco_detection_ppyoloe_dataset_params
   - arch_params: ppyoloe_x_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: coco2017_train_ppyoloe
 val_dataloader: coco2017_val_ppyoloe
 
 load_checkpoint: False
 resume: False
 
@@ -44,16 +45,7 @@
 architecture: pp_yoloe_x
 
 multi_gpu: DDP
 num_gpus: 8
 
 experiment_suffix: ""
 experiment_name: coco2017_${architecture}${experiment_suffix}
-
-ckpt_root_dir:
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml

```diff
@@ -7,29 +7,30 @@
 #
 
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ssd_lite_mobilenet_v2
+#       python -m super_gradients.train_from_recipe --config-name=coco2017_ssd_lite_mobilenet_v2
 
 
 # NOTE:
 # Anchors will be selected based on validation resolution and anchors_name
 # To switch between anchors, set anchors_name to something else defined in the anchors section
 # e.g.
-# python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_ssd_lite_mobilenet_v2 anchors_name=stride_16_plus
+# python -m super_gradients.train_from_recipe --config-name=coco2017_ssd_lite_mobilenet_v2 anchors_name=stride_16_plus
 
 
 defaults:
   - training_hyperparams: coco2017_ssd_lite_mobilenet_v2_train_params
   - dataset_params: coco_detection_ssd_lite_mobilenet_v2_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
   - anchors: ssd_anchors
 
 train_dataloader: coco2017_train
 val_dataloader: coco2017_val
 
 architecture: ssd_lite_mobilenet_v2
 
@@ -51,15 +52,7 @@
   resume: ${resume}
   criterion_params:
     alpha: 1.0
     dboxes: ${dboxes}
 
 multi_gpu: DDP
 num_gpus: 4
-
-ckpt_root_dir:
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/coco2017_yolox.yaml

```diff
@@ -4,20 +4,20 @@
 # Recipe runs with batch size = 16 X 8 gpus = 128.
 
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command you want:
-#         yolox_n: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_yolox architecture=yolox_n
-#         yolox_t: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_yolox architecture=yolox_t
-#         yolox_s: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_yolox architecture=yolox_s
-#         yolox_m: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_yolox architecture=yolox_m
-#         yolox_l: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_yolox architecture=yolox_l
-#         yolox_x: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco2017_yolox architecture=yolox_x
+#         yolox_n: python -m super_gradients.train_from_recipe --config-name=coco2017_yolox architecture=yolox_n
+#         yolox_t: python -m super_gradients.train_from_recipe --config-name=coco2017_yolox architecture=yolox_t
+#         yolox_s: python -m super_gradients.train_from_recipe --config-name=coco2017_yolox architecture=yolox_s
+#         yolox_m: python -m super_gradients.train_from_recipe --config-name=coco2017_yolox architecture=yolox_m
+#         yolox_l: python -m super_gradients.train_from_recipe --config-name=coco2017_yolox architecture=yolox_l
+#         yolox_x: python -m super_gradients.train_from_recipe --config-name=coco2017_yolox architecture=yolox_x
 #
 # Training times and accuracies (mAP@0.5-0.95 (COCO API, confidence 0.001, IoU threshold 0.6, test on 640x640 images):
 #         yolox_n: 1d 16h 33m 9s  on 8 NVIDIA GeForce RTX 3090, mAP: 26.77
 #         yolox_t: 20h 43m 37s    on 8 NVIDIA RTX A5000, mAP: 37.18
 #         yolox_s: 1d 17h 40m 30s on 8 NVIDIA RTX A5000, mAP: 40.47
 #         yolox_m: 1d 22h 23m 43s on 8 NVIDIA GeForce RTX 3090, mAP: 46.40
 #         yolox_l: 2d 14h 11m 41s on 8 NVIDIA GeForce RTX 3090, mAP: 49.25
@@ -33,14 +33,15 @@
 
 defaults:
   - training_hyperparams: coco2017_yolox_train_params
   - dataset_params: coco_detection_dataset_params
   - arch_params: yolox_s_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: coco2017_train
 val_dataloader: coco2017_val
 
 
 
 load_checkpoint: False
@@ -51,16 +52,7 @@
 architecture: yolox_s
 
 multi_gpu: DDP
 num_gpus: 8
 
 experiment_suffix: res${dataset_params.train_dataset_params.input_dim}
 experiment_name: ${architecture}_coco2017_${experiment_suffix}
-
-ckpt_root_dir:
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml

```diff
@@ -5,25 +5,26 @@
 # Logs and tensorboards: s3://deci-pretrained-models/shelfnet34_coco_segmentation_tensorboard/
 
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=coco_segmentation_shelfnet_lw
+#       python -m super_gradients.train_from_recipe --config-name=coco_segmentation_shelfnet_lw
 
 
 # /!\ THIS RECIPE IS NOT SUPPORTED AT THE MOMENT /!\
 
 defaults:
   - training_hyperparams: coco_segmentation_shelfnet_lw_train_params
   - dataset_params: coco_segmentation_dataset_params
   - arch_params: shelfnet34_lw_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: coco_segmentation_train
 val_dataloader: coco_segmentation_val
 
 checkpoint_params:
   strict_load: True
   load_backbone: False
@@ -34,17 +35,10 @@
   resume: ${resume}
 
 experiment_name: coco_segmentation_21_subclass_shelfnet34
 
 multi_gpu: DDP
 num_gpus: 4
 
-ckpt_root_dir:
-
-architecture: shelfnet34_lw
 
 
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
+architecture: shelfnet34_lw
```

## super_gradients/recipes/imagenet_efficientnet.yaml

```diff
@@ -2,22 +2,23 @@
 # This example trains with effective batch size = 64 * 4 gpus = 256.
 # Epoch time on 4 X 3090Ti distributed training is ~ 16:25 minutes
 # Logs and tensorboards: s3://deci-pretrained-models/efficientnet_b0/
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=imagenet_efficientnet
+#       python -m super_gradients.train_from_recipe --config-name=imagenet_efficientnet
 
 defaults:
   - training_hyperparams: imagenet_efficientnet_train_params
   - dataset_params: imagenet_efficientnet_dataset_params
   - arch_params: efficientnet_b0_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 arch_params:
   num_classes: 1000
 
 train_dataloader: imagenet_train
 val_dataloader: imagenet_val
 
@@ -25,20 +26,13 @@
 resume: False
 training_hyperparams:
   resume: ${resume}
 
 experiment_name: efficientnet_b0_imagenet
 
 
-ckpt_root_dir:
+
 
 multi_gpu: DDP
 num_gpus: 4
 
 architecture: efficientnet_b0
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/imagenet_mobilenetv2.yaml

```diff
@@ -3,22 +3,23 @@
 # Learning rate and batch size parameters, using 2 GPUs with DDP:
 #     initial_lr: 0.032    batch-size: 256 * 2gpus = 512
 #
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=imagenet_mobilenetv2
+#       python -m super_gradients.train_from_recipe --config-name=imagenet_mobilenetv2
 
 defaults:
   - training_hyperparams: imagenet_mobilenetv2_train_params
   - dataset_params: imagenet_mobilenetv2_dataset_params
   - arch_params: mobilenet_v2_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: imagenet_train
 val_dataloader: imagenet_val
 
 arch_params:
   num_classes: 1000
   dropout: 0.2
@@ -30,20 +31,13 @@
 resume: False
 training_hyperparams:
   resume: ${resume}
 
 experiment_name: mobileNetv2_training
 
 
-ckpt_root_dir:
+
 
 multi_gpu: DDP
 num_gpus: 2
 
 architecture: mobilenet_v2
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/imagenet_mobilenetv3_base.yaml

```diff
@@ -1,31 +1,25 @@
 # TODO: PRODUCE RESULTS AND ADD TENSORBOARDS, LOGS, TRAINING TIME ETC.
 
 defaults:
   - training_hyperparams: imagenet_mobilenetv3_train_params
   - dataset_params: imagenet_mobilenetv3_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: imagenet_train
 val_dataloader: imagenet_val
 
 
 resume: False
 training_hyperparams:
   resume: ${resume}
 
 experiment_name: mobileNetv3_large_training
 
-ckpt_root_dir:
+
 
 multi_gpu: DDP
 num_gpus: 2
 
 architecture: mobilenet_v3_large
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/imagenet_mobilenetv3_large.yaml

```diff
@@ -1,29 +1,23 @@
 # MobileNetV3 Large Imagenet classification training:
 # TODO: Add metrics
 #
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=imagenet_mobilenetv3_large
+#       python -m super_gradients.train_from_recipe --config-name=imagenet_mobilenetv3_large
 
 
 defaults:
   - imagenet_mobilenetv3_base
   - arch_params: mobilenet_v3_large_arch_params
   - _self_
+  - variable_setup
 
 arch_params:
   num_classes: 1000
   dropout: 0.2
 
 experiment_name: mobileNetv3_large_training
 
 architecture: mobilenet_v3_large
-ckpt_root_dir:
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/imagenet_mobilenetv3_small.yaml

```diff
@@ -1,29 +1,23 @@
 # MobileNetV3 Small Imagenet classification training:
 # TODO: Add metrics
 #
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=imagenet_mobilenetv3_small
+#       python -m super_gradients.train_from_recipe --config-name=imagenet_mobilenetv3_small
 
 
 defaults:
   - imagenet_mobilenetv3_base
   - arch_params: mobilenet_v3_small_arch_params
   - _self_
+  - variable_setup
 
 arch_params:
   num_classes: 1000
   dropout: 0.2
 
 experiment_name: mobileNetv3_small_training
 
 architecture: mobilenet_v3_small
-ckpt_root_dir:
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/imagenet_regnetY.yaml

```diff
@@ -13,25 +13,26 @@
 # https://deci-pretrained-models.s3.amazonaws.com/RegnetY400/
 # https://deci-pretrained-models.s3.amazonaws.com/RegnetY200/
 #
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#         regnetY200: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=imagenet_regnetY architecture=regnetY200
-#         regnetY400: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=imagenet_regnetY architecture=regnetY400
-#         regnetY600: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=imagenet_regnetY architecture=regnetY600
-#         regnetY800: python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=imagenet_regnetY architecture=regnetY800
+#         regnetY200: python -m super_gradients.train_from_recipe --config-name=imagenet_regnetY architecture=regnetY200
+#         regnetY400: python -m super_gradients.train_from_recipe --config-name=imagenet_regnetY architecture=regnetY400
+#         regnetY600: python -m super_gradients.train_from_recipe --config-name=imagenet_regnetY architecture=regnetY600
+#         regnetY800: python -m super_gradients.train_from_recipe --config-name=imagenet_regnetY architecture=regnetY800
 
 defaults:
   - training_hyperparams: imagenet_regnetY_train_params
   - dataset_params: imagenet_regnetY_dataset_params
   - arch_params: regnetY_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 arch_params:   
   num_classes: 1000
   dropout_prob: 0.5
   droppath_prob: 0.0
 
 train_dataloader: imagenet_train
@@ -40,21 +41,14 @@
 
 load_checkpoint: False
 resume: False
 training_hyperparams:
   resume: ${resume}
 
 
-ckpt_root_dir:
+
 
 multi_gpu: Off
 num_gpus: 1
 
 architecture: regnetY800
 experiment_name: ${architecture}
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/imagenet_repvgg.yaml

```diff
@@ -5,22 +5,23 @@
 #
 #  Log and tensorboard at s3://deci-pretrained-models/repvggg-a0-imagenet-tensorboard/
 #
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=imagenet_repvgg
+#       python -m super_gradients.train_from_recipe --config-name=imagenet_repvgg
 
 defaults:
   - training_hyperparams: imagenet_repvgg_train_params
   - dataset_params: imagenet_dataset_params
   - arch_params: repvgg_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 arch_params:
   num_classes: 1000
   build_residual_branches: True
 
 train_dataloader: imagenet_train
 val_dataloader: imagenet_val
@@ -33,14 +34,7 @@
 
 experiment_name: repvgg_a0_imagenet_reproduce_fix
 
 multi_gpu: DDP
 num_gpus: 4
 
 architecture: repvgg_a0
-ckpt_root_dir:
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/imagenet_resnet50.yaml

```diff
@@ -5,43 +5,37 @@
 #
 #  Log and tensorboard at s3://deci-pretrained-models/ResNet50_ImageNet/average_model.pth
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=imagenet_resnet50
+#       python -m super_gradients.train_from_recipe --config-name=imagenet_resnet50
 
 
 defaults:
   - training_hyperparams: imagenet_resnet50_train_params
   - dataset_params: imagenet_resnet50_dataset_params
   - arch_params: resnet50_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 arch_params:
   droppath_prob: 0.05
 
 train_dataloader: imagenet_train
 val_dataloader: imagenet_val
 
 
 resume: False
 training_hyperparams:
   resume: ${resume}
 
 experiment_name: resnet50_imagenet
 
-ckpt_root_dir:
+
 
 multi_gpu: DDP
 num_gpus: 4
 
 architecture: resnet50
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/imagenet_resnet50_kd.yaml

```diff
@@ -5,22 +5,23 @@
 #
 #  Log and tensorboard at s3://deci-pretrained-models/KD_ResNet50_Beit_Base_ImageNet/average_model.pth
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py --config-name=imagenet_resnet50_kd
+#       python -m super_gradients.train_from_kd_recipe --config-name=imagenet_resnet50_kd
 
 
 defaults:
   - training_hyperparams: imagenet_resnet50_kd_train_params
   - dataset_params: imagenet_resnet50_kd_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: imagenet_train
 val_dataloader: imagenet_val
 
 resume: False
 training_hyperparams:
   resume: ${resume}
@@ -69,22 +70,15 @@
 
 
 
 run_teacher_on_eval: True
 
 experiment_name: resnet50_imagenet_KD_Model
 
-ckpt_root_dir:
+
 
 multi_gpu: DDP
 num_gpus: 8
 
 architecture: kd_module
 student_architecture: resnet50
 teacher_architecture: beit_base_patch16_224
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/imagenet_vit_base.yaml

```diff
@@ -5,23 +5,24 @@
 #
 #  Log and tensorboard at s3://deci-pretrained-models/vit_base_imagenet1k/
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=imagenet_vit_base
+#       python -m super_gradients.train_from_recipe --config-name=imagenet_vit_base
 
 
 defaults:
   - training_hyperparams: imagenet_vit_train_params
   - dataset_params: imagenet_vit_base_dataset_params
   - arch_params: vit_base_arch_params
   - checkpoint_params: vit_base_imagenet_checkpoint_params
   - _self_
+  - variable_setup
 
 train_dataloader: imagenet_train
 val_dataloader: imagenet_val
 
 
 
 resume: False
@@ -29,14 +30,7 @@
   resume: ${resume}
 
 experiment_name: vit_base_imagenet1k
 
 architecture: vit_base
 multi_gpu: DDP
 num_gpus: 8
-ckpt_root_dir:
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/imagenet_vit_large.yaml

```diff
@@ -5,34 +5,28 @@
 #
 #  Log and tensorboard at s3://deci-pretrained-models/vit_large_cutmix_randaug_v2_lr=0.03/
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#       python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=imagenet_vit_large
+#       python -m super_gradients.train_from_recipe --config-name=imagenet_vit_large
 
 
 defaults:
   - imagenet_vit_base
   - _self_
+  - variable_setup
 
 dataset_params:
   train_dataloader_params:
     batch_size: 32
 
 training_hyperparams:
   initial_lr: 0.06
   average_best_models: True
 
 architecture: vit_large
 
 experiment_name: vit_large_imagenet1k
 multi_gpu: DDP
 num_gpus: 8
-ckpt_root_dir:
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/roboflow_ppyoloe.yaml

```diff
@@ -1,21 +1,22 @@
 # Checkout the datasets at https://universe.roboflow.com/roboflow-100?ref=blog.roboflow.com
 #
 # `dataset_name` refers to the official name of the dataset.
 # You can find it in the url of the dataset: https://universe.roboflow.com/roboflow-100/digits-t2eg6 -> digits-t2eg6
 #
-# Example: python train_from_recipe.py --config-name=roboflow_ppyoloe dataset_name=digits-t2eg6
+# Example: python -m super_gradients.train_from_recipe --config-name=roboflow_ppyoloe dataset_name=digits-t2eg6
 
 
 defaults:
   - training_hyperparams: coco2017_ppyoloe_train_params
   - dataset_params: roboflow_detection_dataset_params
   - checkpoint_params: default_checkpoint_params
   - arch_params: ppyoloe_m_arch_params
   - _self_
+  - variable_setup
 
 dataset_name: ??? # Placeholder for the name of the dataset you want to use (e.g. "digits-t2eg6")
 dataset_params:
   dataset_name: ${dataset_name}
 num_classes: ${roboflow_dataset_num_classes:${dataset_name}}
 
 
@@ -63,15 +64,7 @@
           max_predictions: 300
           nms_threshold: 0.7
 
 
 multi_gpu: DDP
 num_gpus:
 experiment_name: ${architecture}_roboflow_${dataset_name}
-ckpt_root_dir:
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/roboflow_yolox.yaml

```diff
@@ -1,19 +1,20 @@
 # Checkout the datasets at https://universe.roboflow.com/roboflow-100?ref=blog.roboflow.com
 #
 # `dataset_name` refers to the official name of the dataset.
 # You can find it in the url of the dataset: https://universe.roboflow.com/roboflow-100/digits-t2eg6 -> digits-t2eg6
 #
-# Example: python train_from_recipe.py --config-name=roboflow_yolox dataset_name=digits-t2eg6
+# Example: python -m super_gradients.train_from_recipe --config-name=roboflow_yolox dataset_name=digits-t2eg6
 
 defaults:
   - training_hyperparams: coco2017_yolox_train_params
   - dataset_params: roboflow_detection_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 dataset_name: ??? # Placeholder for the name of the dataset you want to use (e.g. "digits-t2eg6")
 dataset_params:
   dataset_name: ${dataset_name}
 num_classes: ${roboflow_dataset_num_classes:${dataset_name}}
 
 
@@ -57,15 +58,7 @@
           conf: 0.01
         num_cls: 80
 
 
 multi_gpu: DDP
 num_gpus: 3
 experiment_name: ${architecture}_roboflow_${dataset_name}
-ckpt_root_dir:
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/supervisely_unet.yaml

```diff
@@ -1,27 +1,28 @@
 # Binary segmentation training example of UNet model on the Supervisely person dataset.
 
 # Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
 #   2. Run the command:
-#      UNet:        python src/super_gradients/examples/train_from_recipe_example/train_from_recipe.py --config-name=supervisely_unet
+#      UNet:        python -m super_gradients.train_from_recipe --config-name=supervisely_unet
 #
 # Validation Target (Person class) IoU and training time:
 #      UNet:        input-size: [480, 320]     mIoU: 89.18     1 X RTX A5000, 4 H
 #
 # Logs, tensorboards and network checkpoints:
 #      UNet:       https://deci-pretrained-models.s3.amazonaws.com/unet/supervisely/
 #
 
 defaults:
   - training_hyperparams: supervisely_default_train_params
   - dataset_params: supervisely_persons_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 architecture: unet
 arch_params:
   num_classes: 1
   use_aux_heads: False
 
 training_hyperparams:
@@ -34,15 +35,7 @@
 
 dataset_params:
   batch_size: 16
 
 multi_gpu: OFF
 
 experiment_name: unet_supervisely
-ckpt_root_dir:
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml

```diff
@@ -8,14 +8,15 @@
 #   to the dataloader of our user's)
 
 defaults:
   - training_hyperparams: cifar10_resnet_train_params
   - dataset_params: cifar10_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 arch_params:
   num_classes: 10
   in_channels: 1
 
 dataset_params:
   train_dataset_params:
@@ -51,19 +52,12 @@
 
 resume: False
 training_hyperparams:
   resume: ${resume}
   max_epochs: 3
 
 
-ckpt_root_dir:
+
 
 architecture: mobilenet_v2
 
 experiment_name: mobilenet_v2_mnist
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/user_recipe_mnist_example.yaml

```diff
@@ -13,14 +13,15 @@
 #   train_dataloader_params, valid_dataloader_params.
 
 defaults:
   - training_hyperparams: cifar10_resnet_train_params
   - dataset_params: cifar10_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
+  - variable_setup
 
 arch_params:
   num_classes: 10
   in_channels: 1
 
 dataset_params:
   train_dataset_params:
@@ -55,19 +56,12 @@
 
 resume: False
 training_hyperparams:
   resume: ${resume}
   max_epochs: 3
 
 
-ckpt_root_dir:
+
 
 architecture: mobilenet_v2
 
 experiment_name: mobilenet_v2_mnist
-
-
-# THE FOLLOWING PARAMS ARE DIRECTLY USED BY HYDRA
-hydra:
-  run:
-    # Set the output directory (i.e. where .hydra folder that logs all the input params will be generated)
-    dir: ${hydra_output_dir:${ckpt_root_dir}, ${experiment_name}}
```

## super_gradients/recipes/arch_params/unet_default_arch_params.yaml

```diff
@@ -28,14 +28,15 @@
   # skip expansion ratio value, before fusing the skip features from the encoder with the decoder features, a projection
   # convolution is applied upon the encoder features to project the num_channels by skip_expansion.
   skip_expansion: 0.25
   decoder_scale: 0.25   # num_channels width ratio between encoder stages and decoder stages.
   up_block_types: [UpCatBlock, UpCatBlock, UpCatBlock, UpCatBlock]    # See unet_decoder.UpBlockType for options.
   up_block_repeat_list: [ 1, 1, 1, 1]   # num of blocks per decoder stage, the `block` implementation depends on the up-block type.
   mode: bilinear
+  fallback_mode:
   align_corners: False
   up_factor: 2
   is_skip_list: [True, True, True, True]    # List of flags whether to use feature-map from encoder stage as skip connection or not.
   min_decoder_channels: 1                   # The minimum num_channels of decoder stages. Useful i.e if we want to keep the width above the num of classes.
 
 dropout: 0.
 final_upsample_factor: 2    # Final upsample scale factor after the segmentation head.
```

## super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml

```diff
@@ -5,50 +5,62 @@
 train_dataset_params:
   data_dir: ${..data_dir} # root path to Robflow datasets
   dataset_name: ${..dataset_name}
   split: train
   input_dim: [640, 640]
   cache_dir:
   cache: False
+  ignore_empty_annotations: False
   transforms:
+    - DetectionMosaic:
+        input_dim: ${dataset_params.train_dataset_params.input_dim}
+        prob: 1.
     - DetectionRandomAffine:
         degrees: 0.                  # rotation degrees, randomly sampled from [-degrees, degrees]
         translate: 0.1                # image translation fraction
         scales: [ 0.5, 1.5 ]              # random rescale range (keeps size by padding/cropping) after mosaic transform.
         shear: 0.0                    # shear degrees, randomly sampled from [-degrees, degrees]
         target_size: ${dataset_params.train_dataset_params.input_dim}
-        filter_box_candidates: True   # whether to filter out transformed bboxes by edge size, area ratio, and aspect ratio.
+        filter_box_candidates: False  # whether to filter out transformed bboxes by edge size, area ratio, and aspect ratio.
         wh_thr: 2                     # edge size threshold when filter_box_candidates = True (pixels)
         area_thr: 0.1                 # threshold for area ratio between original image and the transformed one, when filter_box_candidates = True
         ar_thr: 20                    # aspect ratio threshold when filter_box_candidates = True
         border_value: 128
+#    - DetectionMixup:
+#        input_dim: ${dataset_params.train_dataset_params.input_dim}
+#        mixup_scale: [ 0.5, 1.5 ]         # random rescale range for the additional sample in mixup
+#        prob: 1.0                       # probability to apply per-sample mixup
+#        flip_prob: 0.5                  # probability to apply horizontal flip
     - DetectionHSV:
         prob: 1.0                       # probability to apply HSV transform
         hgain: 5                        # HSV transform hue gain (randomly sampled from [-hgain, hgain])
         sgain: 30                       # HSV transform saturation gain (randomly sampled from [-sgain, sgain])
         vgain: 30                       # HSV transform value gain (randomly sampled from [-vgain, vgain])
     - DetectionHorizontalFlip:
         prob: 0.5                       # probability to apply horizontal flip
     - DetectionPaddedRescale:
         input_dim: ${dataset_params.train_dataset_params.input_dim}
-        max_targets: 120
+        max_targets: 300
+    - DetectionStandardize:
+        max_value: 255.
     - DetectionTargetsFormatTransform:
+        max_targets: 300
         input_dim: ${dataset_params.train_dataset_params.input_dim}
         output_format: LABEL_CXCYWH
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: False
   verbose: 0
 
 train_dataloader_params:
   shuffle: True
   batch_size: 16
-  num_workers: 0
-  sampler:
+  min_samples: 512
+  num_workers: 4
   drop_last: False
   pin_memory: True
   worker_init_fn:
     _target_: super_gradients.training.utils.utils.load_func
     dotpath: super_gradients.training.datasets.datasets_utils.worker_init_reset_seed
   collate_fn: # collate function for trainset
     _target_: super_gradients.training.utils.detection_utils.DetectionCollateFN
@@ -56,31 +68,36 @@
 val_dataset_params:
   data_dir: ${..data_dir} # root path to Robflow datasets
   dataset_name: ${..dataset_name}
   split: valid
   input_dim: [640, 640]
   cache_dir:
   cache: False
+  ignore_empty_annotations: False
   transforms:
   - DetectionPaddedRescale:
       input_dim: ${dataset_params.val_dataset_params.input_dim}
+      max_targets: 300
+      pad_value: 114
+  - DetectionStandardize:
+      max_value: 255.
   - DetectionTargetsFormatTransform:
-      max_targets: 50
+      max_targets: 300
       input_dim: ${dataset_params.val_dataset_params.input_dim}
       output_format: LABEL_CXCYWH
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: True
   verbose: 0
 
 val_dataloader_params:
-  batch_size: 64
-  num_workers: 0
-  sampler:
+  batch_size: 32
+  num_workers: 4
   drop_last: False
+  shuffle: False
   pin_memory: True
   collate_fn: # collate function for valset
     _target_: super_gradients.training.utils.detection_utils.CrowdDetectionCollateFN
 
 
 _convert_: all
```

## super_gradients/training/pretrained_models.py

```diff
@@ -1,70 +1,59 @@
 # TODO: It would be nice to create keys here as: make_pretrained_model_key(Models.RESNET18, Dataset.COCO)
 # TODO: Not only this would reduce risk of making a typo error, it would bring more clarity how the key is created
 # TODO: And allow to "query" pretrained models by dataset
 MODEL_URLS = {
-    # RegNet-s
-    "regnetY800_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/RegnetY800/average_model.pth",
-    "regnetY600_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/RegnetY600/average_model_regnety600.pth",
-    "regnetY400_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/RegnetY400/average_model_regnety400.pth",
-    "regnetY200_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/RegnetY200/average_model_regnety200.pth",
-    # ResNet-s
-    "resnet50_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/KD_ResNet50_Beit_Base_ImageNet/resnet.pth",
-    "resnet34_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/resent_34/average_model.pth",
-    "resnet18_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/resnet18/average_model.pth",
-    #
-    "repvgg_a0_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/repvgg_a0_imagenet.pth",
-    #
-    "shelfnet34_lw_coco_segmentation_subclass": "https://deci-pretrained-models.s3.amazonaws.com" "/shelfnet34_coco_segmentation_subclass.pth",
-    #
-    "ddrnet_23_cityscapes": "https://deci-pretrained-models.s3.amazonaws.com/ddrnet/cityscapes/ddrnet23_cwd/average_model.pth",
-    "ddrnet_23_slim_cityscapes": "https://deci-pretrained-models.s3.amazonaws.com/ddrnet/cityscapes/ddrnet23_slim_cwd/ckpt_best.pth",
-    "ddrnet_39_cityscapes": "https://deci-pretrained-models.s3.amazonaws.com/ddrnet/cityscapes/ddrnet39_al/average_model_2023_02_20.pth",
-    #
-    "stdc1_seg50_cityscapes": "https://deci-pretrained-models.s3.amazonaws.com/cityscapes_stdc1_seg50_dice_edge/ckpt_best.pth",
-    "stdc1_seg75_cityscapes": "https://deci-pretrained-models.s3.amazonaws.com/stdc1_seg75_cityscapes/ckpt_best.pth",
-    "stdc2_seg50_cityscapes": "https://deci-pretrained-models.s3.amazonaws.com/cityscapes_stdc2_seg50_dice_edge/ckpt_best.pth",
-    "stdc2_seg75_cityscapes": "https://deci-pretrained-models.s3.amazonaws.com/stdc2_seg75_cityscapes/ckpt_best.pth",
-    #
-    "efficientnet_b0_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/efficientnet_b0/average_model-3.pth",
-    #
-    "ssd_lite_mobilenet_v2_coco": "https://deci-pretrained-models.s3.amazonaws.com/ssd_lite_mobilenet_v2/coco2017/2022-11-28/average_model.pth",
-    "ssd_mobilenet_v1_coco": "https://deci-pretrained-models.s3.amazonaws.com/ssd_mobilenet_v1_coco_res320/ckpt_best.pth",
-    #
-    "mobilenet_v3_large_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/mobilenetv3+large+300epoch/average_model.pth",
-    "mobilenet_v3_small_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/mobilenetv3+small/ckpt_best.pth",
-    "mobilenet_v2_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/mobilenetv2+w1/ckpt_best.pth",
-    #
-    "regseg48_cityscapes": "https://deci-pretrained-models.s3.amazonaws.com/regseg48_cityscapes/ckpt_best.pth",
-    #
-    "vit_base_imagenet21k": "https://deci-pretrained-models.s3.amazonaws.com/vit_pretrained_imagenet21k/vit_base_16_imagenet21K.pth",
-    "vit_large_imagenet21k": "https://deci-pretrained-models.s3.amazonaws.com/vit_pretrained_imagenet21k/vit_large_16_imagenet21K.pth",
-    "vit_base_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/vit_base_imagenet1k/ckpt_best.pth",
-    "vit_large_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/vit_large_cutmix_randaug_v2_lr%3D0.03/average_model.pth",
-    #
-    "beit_base_patch16_224_imagenet": "https://deci-pretrained-models.s3.amazonaws.com/beit_base_patch16_224_imagenet.pth",
-    "beit_base_patch16_224_cifar10": "https://deci-pretrained-models.s3.amazonaws.com/beit_cifar10.pth",
-    #
-    "yolox_s_coco": "https://deci-pretrained-models.s3.amazonaws.com/yolox_coco/yolox_s_coco/average_model.pth",
-    "yolox_m_coco": "https://deci-pretrained-models.s3.amazonaws.com/yolox_coco/yolox_m_coco/average_model.pth",
-    "yolox_l_coco": "https://deci-pretrained-models.s3.amazonaws.com/yolox_coco/yolox_l_coco/average_model.pth",
-    "yolox_t_coco": "https://deci-pretrained-models.s3.amazonaws.com/yolox_coco/yolox_tiny_coco/ckpt_best.pth",
-    "yolox_n_coco": "https://deci-pretrained-models.s3.amazonaws.com/yolox_coco/yolox_n_coco/ckpt_best.pth",
-    #
-    "pp_lite_t_seg50_cityscapes": "https://deci-pretrained-models.s3.amazonaws.com/ppliteseg/cityscapes/pplite_t_seg50/average_model.pth",
-    "pp_lite_t_seg75_cityscapes": "https://deci-pretrained-models.s3.amazonaws.com/ppliteseg/cityscapes/pplite_t_seg75/average_model.pth",
-    "pp_lite_b_seg50_cityscapes": "https://deci-pretrained-models.s3.amazonaws.com/ppliteseg/cityscapes/pplite_b_seg50/average_model.pth",
-    "pp_lite_b_seg75_cityscapes": "https://deci-pretrained-models.s3.amazonaws.com/ppliteseg/cityscapes/pplite_b_seg75/average_model.pth",
-    #
-    "ppyoloe_s_coco": "https://deci-pretrained-models.s3.amazonaws.com/ppyolo_e/coco2017_ppyoloe_s.pth",
-    "ppyoloe_m_coco": "https://deci-pretrained-models.s3.amazonaws.com/ppyolo_e/coco2017_ppyoloe_m.pth",
-    "ppyoloe_l_coco": "https://deci-pretrained-models.s3.amazonaws.com/ppyolo_e/coco2017_pp_yoloe_l_best_model_21uffbb8.pth",  # 0.4948
-    "ppyoloe_x_coco": "https://deci-pretrained-models.s3.amazonaws.com/ppyolo_e/coco2017_pp_yoloe_x_best_model_z03if91o.pth",  # 0.5115
+    "regnetY800_imagenet": "https://sghub.deci.ai/models/regnetY800_imagenet.pth",
+    "regnetY600_imagenet": "https://sghub.deci.ai/models/regnetY600_imagenet.pth",
+    "regnetY400_imagenet": "https://sghub.deci.ai/models/regnetY400_imagenet.pth",
+    "regnetY200_imagenet": "https://sghub.deci.ai/models/regnetY200_imagenet.pth",
+    "resnet50_imagenet": "https://sghub.deci.ai/models/resnet50_imagenet.pth",
+    "resnet34_imagenet": "https://sghub.deci.ai/models/resnet34_imagenet.pth",
+    "resnet18_imagenet": "https://sghub.deci.ai/models/resnet18_imagenet.pth",
+    "repvgg_a0_imagenet": "https://sghub.deci.ai/models/repvgg_a0_imagenet.pth",
+    "shelfnet34_lw_coco_segmentation_subclass": "https://sghub.deci.ai/models/shelfnet34_lw_coco_segmentation_subclass.pth",
+    "ddrnet_23_cityscapes": "https://sghub.deci.ai/models/ddrnet_23_cityscapes.pth",
+    "ddrnet_23_slim_cityscapes": "https://sghub.deci.ai/models/ddrnet_23_slim_cityscapes.pth",
+    "ddrnet_39_cityscapes": "https://sghub.deci.ai/models/ddrnet_39_cityscapes.pth",
+    "stdc1_seg50_cityscapes": "https://sghub.deci.ai/models/stdc1_seg50_cityscapes.pth",
+    "stdc1_seg75_cityscapes": "https://sghub.deci.ai/models/stdc1_seg75_cityscapes.pth",
+    "stdc2_seg50_cityscapes": "https://sghub.deci.ai/models/stdc2_seg50_cityscapes.pth",
+    "stdc2_seg75_cityscapes": "https://sghub.deci.ai/models/stdc2_seg75_cityscapes.pth",
+    "efficientnet_b0_imagenet": "https://sghub.deci.ai/models/efficientnet_b0_imagenet.pth",
+    "ssd_lite_mobilenet_v2_coco": "https://sghub.deci.ai/models/ssd_lite_mobilenet_v2_coco.pth",
+    "ssd_mobilenet_v1_coco": "https://sghub.deci.ai/models/ssd_mobilenet_v1_coco.pth",
+    "mobilenet_v3_large_imagenet": "https://sghub.deci.ai/models/mobilenet_v3_large_imagenet.pth",
+    "mobilenet_v3_small_imagenet": "https://sghub.deci.ai/models/mobilenet_v3_small_imagenet.pth",
+    "mobilenet_v2_imagenet": "https://sghub.deci.ai/models/mobilenet_v2_imagenet.pth",
+    "regseg48_cityscapes": "https://sghub.deci.ai/models/regseg48_cityscapes.pth",
+    "vit_base_imagenet21k": "https://sghub.deci.ai/models/vit_base_imagenet21k.pth",
+    "vit_large_imagenet21k": "https://sghub.deci.ai/models/vit_large_imagenet21k.pth",
+    "vit_base_imagenet": "https://sghub.deci.ai/models/vit_base_imagenet.pth",
+    "vit_large_imagenet": "https://sghub.deci.ai/models/vit_large_imagenet.pth",
+    "beit_base_patch16_224_imagenet": "https://sghub.deci.ai/models/beit_base_patch16_224_imagenet.pth",
+    "beit_base_patch16_224_cifar10": "https://sghub.deci.ai/models/beit_base_patch16_224_cifar10.pth",
+    "yolox_s_coco": "https://sghub.deci.ai/models/yolox_s_coco.pth",
+    "yolox_m_coco": "https://sghub.deci.ai/models/yolox_m_coco.pth",
+    "yolox_l_coco": "https://sghub.deci.ai/models/yolox_l_coco.pth",
+    "yolox_t_coco": "https://sghub.deci.ai/models/yolox_t_coco.pth",
+    "yolox_n_coco": "https://sghub.deci.ai/models/yolox_n_coco.pth",
+    "pp_lite_t_seg50_cityscapes": "https://sghub.deci.ai/models/pp_lite_t_seg50_cityscapes.pth",
+    "pp_lite_t_seg75_cityscapes": "https://sghub.deci.ai/models/pp_lite_t_seg75_cityscapes.pth",
+    "pp_lite_b_seg50_cityscapes": "https://sghub.deci.ai/models/pp_lite_b_seg50_cityscapes.pth",
+    "pp_lite_b_seg75_cityscapes": "https://sghub.deci.ai/models/pp_lite_b_seg75_cityscapes.pth",
+    "ppyoloe_s_coco": "https://sghub.deci.ai/models/ppyoloe_s_coco.pth",
+    "ppyoloe_m_coco": "https://sghub.deci.ai/models/ppyoloe_m_coco.pth",
+    "ppyoloe_l_coco": "https://sghub.deci.ai/models/ppyoloe_l_coco.pth",
+    "ppyoloe_x_coco": "https://sghub.deci.ai/models/ppyoloe_x_coco.pth",
+    "yolo_nas_s_coco": "https://sghub.deci.ai/models/yolo_nas_s_coco.pth",
+    "yolo_nas_m_coco": "https://sghub.deci.ai/models/yolo_nas_m_coco.pth",
+    "yolo_nas_l_coco": "https://sghub.deci.ai/models/yolo_nas_l_coco.pth",
 }
 
+
 PRETRAINED_NUM_CLASSES = {
     "imagenet": 1000,
     "imagenet21k": 21843,
     "coco_segmentation_subclass": 21,
     "cityscapes": 19,
     "coco": 80,
     "cifar10": 10,
```

## super_gradients/training/dataloaders/__init__.py

```diff
@@ -5,16 +5,16 @@
     coco2017_val_yolox,
     coco2017_train_ssd_lite_mobilenet_v2,
     coco2017_val_ssd_lite_mobilenet_v2,
     coco2017_train_ppyoloe,
     coco2017_val_ppyoloe,
     coco2017_pose_train,
     coco2017_pose_val,
-    coco2017_train_deci_yolo,
-    coco2017_val_deci_yolo,
+    coco2017_train_yolo_nas,
+    coco2017_val_yolo_nas,
     imagenet_train,
     imagenet_val,
     imagenet_efficientnet_train,
     imagenet_efficientnet_val,
     imagenet_mobilenetv2_train,
     imagenet_mobilenetv2_val,
     imagenet_mobilenetv3_train,
@@ -64,16 +64,16 @@
     "coco2017_val_yolox",
     "coco2017_train_ssd_lite_mobilenet_v2",
     "coco2017_val_ssd_lite_mobilenet_v2",
     "coco2017_train_ppyoloe",
     "coco2017_val_ppyoloe",
     "coco2017_pose_train",
     "coco2017_pose_val",
-    "coco2017_train_deci_yolo",
-    "coco2017_val_deci_yolo",
+    "coco2017_train_yolo_nas",
+    "coco2017_val_yolo_nas",
     "imagenet_train",
     "imagenet_val",
     "imagenet_efficientnet_train",
     "imagenet_efficientnet_val",
     "imagenet_mobilenetv2_train",
     "imagenet_mobilenetv2_val",
     "imagenet_mobilenetv3_train",
```

## super_gradients/training/dataloaders/dataloaders.py

```diff
@@ -13,15 +13,15 @@
 from super_gradients.common.factories.samplers_factory import SamplersFactory
 from super_gradients.common.object_names import Dataloaders
 from super_gradients.training.datasets import ImageNetDataset
 from super_gradients.training.datasets.classification_datasets.cifar import (
     Cifar10,
     Cifar100,
 )
-from super_gradients.training.datasets.detection_datasets import COCODetectionDataset, RoboflowDetectionDataset
+from super_gradients.training.datasets.detection_datasets import COCODetectionDataset, RoboflowDetectionDataset, YoloDarknetFormatDetectionDataset
 from super_gradients.training.datasets.detection_datasets.pascal_voc_detection import (
     PascalVOCUnifiedDetectionTrainDataset,
     PascalVOCDetectionDataset,
 )
 from super_gradients.training.datasets.pose_estimation_datasets import COCOKeypointsDataset
 from super_gradients.training.datasets.segmentation_datasets import (
     CityscapesDataset,
@@ -168,29 +168,29 @@
         dataset_cls=COCODetectionDataset,
         train=False,
         dataset_params=dataset_params,
         dataloader_params=dataloader_params,
     )
 
 
-@register_dataloader(Dataloaders.COCO2017_TRAIN_DECIYOLO)
-def coco2017_train_deci_yolo(dataset_params: Dict = None, dataloader_params: Dict = None) -> DataLoader:
+@register_dataloader(Dataloaders.COCO2017_TRAIN_YOLO_NAS)
+def coco2017_train_yolo_nas(dataset_params: Dict = None, dataloader_params: Dict = None) -> DataLoader:
     return get_data_loader(
-        config_name="coco_detection_deci_yolo_dataset_params",
+        config_name="coco_detection_yolo_nas_dataset_params",
         dataset_cls=COCODetectionDataset,
         train=True,
         dataset_params=dataset_params,
         dataloader_params=dataloader_params,
     )
 
 
-@register_dataloader(Dataloaders.COCO2017_VAL_DECIYOLO)
-def coco2017_val_deci_yolo(dataset_params: Dict = None, dataloader_params: Dict = None) -> DataLoader:
+@register_dataloader(Dataloaders.COCO2017_VAL_YOLO_NAS)
+def coco2017_val_yolo_nas(dataset_params: Dict = None, dataloader_params: Dict = None) -> DataLoader:
     return get_data_loader(
-        config_name="coco_detection_deci_yolo_dataset_params",
+        config_name="coco_detection_yolo_nas_dataset_params",
         dataset_cls=COCODetectionDataset,
         train=False,
         dataset_params=dataset_params,
         dataloader_params=dataloader_params,
     )
 
 
@@ -266,14 +266,36 @@
         dataset_cls=RoboflowDetectionDataset,
         train=False,
         dataset_params=dataset_params,
         dataloader_params=dataloader_params,
     )
 
 
+@register_dataloader(Dataloaders.COCO_DETECTION_YOLO_FORMAT_TRAIN)
+def coco_detection_yolo_format_train(dataset_params: Dict = None, dataloader_params: Dict = None) -> DataLoader:
+    return get_data_loader(
+        config_name="coco_detection_yolo_format_base_dataset_params",
+        dataset_cls=YoloDarknetFormatDetectionDataset,
+        train=True,
+        dataset_params=dataset_params,
+        dataloader_params=dataloader_params,
+    )
+
+
+@register_dataloader(Dataloaders.COCO_DETECTION_YOLO_FORMAT_VAL)
+def coco_detection_yolo_format_val(dataset_params: Dict = None, dataloader_params: Dict = None) -> DataLoader:
+    return get_data_loader(
+        config_name="coco_detection_yolo_format_base_dataset_params",
+        dataset_cls=YoloDarknetFormatDetectionDataset,
+        train=False,
+        dataset_params=dataset_params,
+        dataloader_params=dataloader_params,
+    )
+
+
 @register_dataloader(Dataloaders.IMAGENET_TRAIN)
 def imagenet_train(dataset_params: Dict = None, dataloader_params: Dict = None, config_name="imagenet_dataset_params"):
     return get_data_loader(
         config_name=config_name,
         dataset_cls=ImageNetDataset,
         train=True,
         dataset_params=dataset_params,
```

## super_gradients/training/datasets/detection_datasets/detection_dataset.py

```diff
@@ -80,14 +80,15 @@
         transforms: List[DetectionTransform] = [],
         all_classes_list: Optional[List[str]] = [],
         class_inclusion_list: Optional[List[str]] = None,
         ignore_empty_annotations: bool = True,
         target_fields: List[str] = None,
         output_fields: List[str] = None,
         verbose: bool = True,
+        show_all_warnings: bool = False,
     ):
         """Detection dataset.
 
         :param data_dir:                Where the data is stored
         :param input_dim:               Image size (when loaded, before transforms).
         :param original_target_format:  Format of targets stored on disk. raw data format, the output format might
                                         differ based on transforms.
@@ -102,28 +103,30 @@
         :param ignore_empty_annotations:        If True and class_inclusion_list not None, images without any target
                                                 will be ignored.
         :param target_fields:                   List of the fields target fields. This has to include regular target,
                                                 but can also include crowd target, segmentation target, ...
                                                 It has to include at least "target" but can include other.
         :param output_fields:                   Fields that will be outputed by __getitem__.
                                                 It has to include at least "image" and "target" but can include other.
-        :param verbose:                 Whether to show additional information or not, such as loading progress.
+        :param verbose:                 Whether to show additional information or not, such as loading progress. (doesnt include warnings)
+        :param show_all_warnings:       Whether to show all warnings or not.
         """
         super().__init__()
         self.verbose = verbose
+        self.show_all_warnings = show_all_warnings
 
         if isinstance(original_target_format, DetectionTargetsFormat):
             logger.warning(
                 "Deprecation: original_target_format should be of type ConcatenatedTensorFormat instead of DetectionTargetsFormat."
                 "Support for DetectionTargetsFormat will be removed in 3.1"
             )
 
         self.data_dir = data_dir
         if not Path(data_dir).exists():
-            raise FileNotFoundError(f"data_dir={data_dir} not found. Please make sure that data_dir points toward your dataset.")
+            raise RuntimeError(f"data_dir={data_dir} not found. Please make sure that data_dir points toward your dataset.")
 
         # Number of images that are available (regardless of ignored images)
         self.n_available_samples = self._setup_data_source()
         if not isinstance(self.n_available_samples, int) or self.n_available_samples < 1:
             raise ValueError(f"_setup_data_source() should return the number of available samples but got {self.n_available_samples}")
 
         self.input_dim = input_dim
@@ -182,21 +185,24 @@
         """
         raise NotImplementedError
 
     def _cache_annotations(self) -> List[Dict[str, Union[np.ndarray, Any]]]:
         """Load all the annotations to memory to avoid opening files back and forth.
         :return: List of annotations
         """
+        n_invalid_bbox = 0
         annotations = []
         for sample_id, img_id in enumerate(tqdm(range(self.n_available_samples), desc="Caching annotations", disable=not self.verbose)):
 
             if self.max_num_samples is not None and len(annotations) >= self.max_num_samples:
                 break
 
             img_annotation = self._load_annotation(img_id)
+            n_invalid_bbox += img_annotation.get("n_invalid_labels", 0)
+
             if not self._required_annotation_fields.issubset(set(img_annotation.keys())):
                 raise KeyError(
                     f"_load_annotation is expected to return at least the fields {self._required_annotation_fields} " f"but got {set(img_annotation.keys())}"
                 )
 
             if self.class_inclusion_list is not None:
                 img_annotation = self._sub_class_annotation(img_annotation)
@@ -204,16 +210,20 @@
             is_annotation_empty = all(len(img_annotation[field]) == 0 for field in self.target_fields)
             if self.ignore_empty_annotations and is_annotation_empty:
                 continue
             annotations.append(img_annotation)
 
         if len(annotations) == 0:
             raise EmptyDatasetException(
-                f"Out of {self.n_available_samples} images, not a single one was found with" f"any of these classes: {self.class_inclusion_list}"
+                f"Out of {self.n_available_samples} images, not a single one was found with any of these classes: {self.class_inclusion_list}"
             )
+
+        if n_invalid_bbox > 0:
+            logger.warning(f"Found {n_invalid_bbox} invalid bbox that were ignored. For more information, please set `show_all_warnings=True`.")
+
         return annotations
 
     def _sub_class_annotation(self, annotation: dict) -> Union[dict, None]:
         """Subclass every field listed in self.target_fields. It could be targets, crowd_targets, ...
 
         :param annotation: Dict representing the annotation of a specific image
         :return:           Subclassed annotation if non empty after subclassing, otherwise None
```

## super_gradients/training/datasets/detection_datasets/yolo_format_detection.py

```diff
@@ -1,12 +1,12 @@
 import os
 
 import imagesize
 import numpy as np
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.training.utils.media.image import is_image
 from super_gradients.training.datasets.detection_datasets.detection_dataset import DetectionDataset
 from super_gradients.training.datasets.data_formats import ConcatenatedTensorFormatConverter
 from super_gradients.training.datasets.data_formats.default_formats import XYXY_LABEL, LABEL_NORMALIZED_CXCYWH
 
@@ -92,35 +92,38 @@
         self,
         data_dir: str,
         images_dir: str,
         labels_dir: str,
         classes: List[str],
         class_ids_to_ignore: Optional[List[int]] = None,
         ignore_invalid_labels: bool = True,
+        show_all_warnings: bool = False,
         *args,
         **kwargs,
     ):
         """
         :param data_dir:                Where the data is stored.
         :param images_dir:              Local path to directory that includes all the images. Path relative to `data_dir`. Can be the same as `labels_dir`.
         :param labels_dir:              Local path to directory that includes all the labels. Path relative to `data_dir`. Can be the same as `images_dir`.
         :param classes:                 List of class names.
         :param class_ids_to_ignore:     List of class ids to ignore in the dataset. By default, doesnt ignore any class.
         :param ignore_invalid_labels:   Whether to ignore labels that fail to be parsed. If True ignores and logs a warning, otherwise raise an error.
+        :param show_all_warnings:       Whether to show every yolo format parser warnings or not.
         """
         self.images_dir = images_dir
         self.labels_dir = labels_dir
         self.class_ids_to_ignore = class_ids_to_ignore or []
         self.classes = classes
         self.ignore_invalid_labels = ignore_invalid_labels
+        self.show_all_warnings = show_all_warnings
 
         kwargs["target_fields"] = ["target"]
         kwargs["output_fields"] = ["image", "target"]
         kwargs["original_target_format"] = XYXY_LABEL  # We convert yolo format (LABEL_CXCYWH) to Coco format (XYXY_LABEL) when loading the annotation
-        super().__init__(data_dir=data_dir, *args, **kwargs)
+        super().__init__(data_dir=data_dir, show_all_warnings=show_all_warnings, *args, **kwargs)
 
     @property
     def _all_classes(self) -> List[str]:
         return self.classes
 
     def _setup_data_source(self) -> int:
         """Initialize img_and_target_path_list and warn if label file is missing
@@ -142,28 +145,29 @@
             logger.warning(f"{len(images_not_in_labels)} images are note associated to any label file")
 
         labels_not_in_images = unique_label_file_base_names - unique_image_file_base_names
         if labels_not_in_images:
             logger.warning(f"{len(labels_not_in_images)} label files are not associated to any image.")
 
         # Only keep names that are in both the images and the labels
-        valid_base_names = list(unique_image_file_base_names & unique_label_file_base_names)
+        valid_base_names = unique_image_file_base_names & unique_label_file_base_names
         if len(valid_base_names) != len(all_images_file_names):
             logger.warning(
                 f"As a consequence, "
                 f"{len(valid_base_names)}/{len(all_images_file_names)} images and "
                 f"{len(valid_base_names)}/{len(all_labels_file_names)} label files will be used."
             )
 
-        self.images_file_names = list(
-            sorted(image_full_name for image_full_name in all_images_file_names if remove_file_extension(image_full_name) in valid_base_names)
-        )
-        self.labels_file_names = list(
-            sorted(label_full_name for label_full_name in all_labels_file_names if remove_file_extension(label_full_name) in valid_base_names)
-        )
+        self.images_file_names = []
+        self.labels_file_names = []
+        for image_full_name in all_images_file_names:
+            base_name = remove_file_extension(image_full_name)
+            if base_name in valid_base_names:
+                self.images_file_names.append(image_full_name)
+                self.labels_file_names.append(base_name + ".txt")
         return len(self.images_file_names)
 
     def _load_annotation(self, sample_id: int) -> dict:
         """Load relevant information of a specific image.
 
         :param sample_id:   Sample_id in the dataset
         :return:            Dictionary with the following keys:
@@ -174,15 +178,19 @@
         """
         image_path = os.path.join(self.images_folder, self.images_file_names[sample_id])
         label_path = os.path.join(self.labels_folder, self.labels_file_names[sample_id])
 
         image_width, image_height = imagesize.get(image_path)
         image_shape = (image_height, image_width)
 
-        yolo_format_target = self._parse_yolo_label_file(label_path, ignore_invalid_labels=self.ignore_invalid_labels)
+        yolo_format_target, invalid_labels = self._parse_yolo_label_file(
+            label_file_path=label_path,
+            ignore_invalid_labels=self.ignore_invalid_labels,
+            show_warnings=self.show_all_warnings,
+        )
 
         converter = ConcatenatedTensorFormatConverter(input_format=LABEL_NORMALIZED_CXCYWH, output_format=XYXY_LABEL, image_shape=image_shape)
         target = converter(yolo_format_target)
 
         # The base class includes a feature to resize the image, so we need to resize the target as well when self.input_dim is set.
         if self.input_dim is not None:
             r = min(self.input_dim[0] / image_height, self.input_dim[1] / image_width)
@@ -193,34 +201,40 @@
 
         annotation = {
             "target": target,
             "initial_img_shape": image_shape,
             "resized_img_shape": resized_img_shape,
             "img_path": image_path,
             "id": np.array([sample_id]),
+            "n_invalid_labels": len(invalid_labels),
         }
         return annotation
 
     @staticmethod
-    def _parse_yolo_label_file(label_file_path: str, ignore_invalid_labels: bool = True) -> np.ndarray:
+    def _parse_yolo_label_file(label_file_path: str, ignore_invalid_labels: bool = True, show_warnings: bool = True) -> Tuple[np.ndarray, List[str]]:
         """Parse a single label file in yolo format.
 
         #TODO: Add support for additional fields (with ConcatenatedTensorFormat)
         :param label_file_path:         Path to the label file in yolo format.
         :param ignore_invalid_labels:   Whether to ignore labels that fail to be parsed. If True ignores and logs a warning, otherwise raise an error.
+        :param show_warnings:           Whether to show the warnings or not.
 
-        :return: np.ndarray of shape (n_labels, 5) in yolo format (LABEL_NORMALIZED_CXCYWH)
+        :return:
+            - labels:           np.ndarray of shape (n_labels, 5) in yolo format (LABEL_NORMALIZED_CXCYWH)
+            - invalid_labels:   List of lines that failed to be parsed
         """
         with open(label_file_path, "r") as f:
             lines = f.readlines()
 
-        labels_yolo_format = []
+        labels_yolo_format, invalid_labels = [], []
         for line in filter(lambda x: x != "\n", lines):
             try:
                 label_id, cx, cw, w, h = line.split(" ")
                 labels_yolo_format.append([int(label_id), float(cx), float(cw), float(w), float(h)])
             except Exception as e:
                 if ignore_invalid_labels:
-                    logger.warning(f"Line `{line}` of file {label_file_path} will be ignored because not in LABEL_NORMALIZED_CXCYWH format: {e}")
+                    invalid_labels.append(line)
+                    if show_warnings:
+                        logger.warning(f"Line `{line}` of file {label_file_path} will be ignored because not in LABEL_NORMALIZED_CXCYWH format: {e}")
                 else:
                     raise e
-        return np.array(labels_yolo_format) if labels_yolo_format else np.zeros((0, 5))
+        return np.array(labels_yolo_format) if labels_yolo_format else np.zeros((0, 5)), invalid_labels
```

## super_gradients/training/datasets/detection_datasets/roboflow/metadata.py

```diff
@@ -29,15 +29,15 @@
     "asbestos": {"category": "microscopic", "train": 932, "test": 133, "valid": 266, "size": 1331, "num_classes": 4, "num_classes_found": 4},
     "underwater-pipes-4ng4t": {"category": "underwater", "train": 5617, "test": 779, "valid": 1575, "size": 7971, "num_classes": 1, "num_classes_found": 1},
     "aquarium-qlnqy": {"category": "underwater", "train": 448, "test": 63, "valid": 127, "size": 638, "num_classes": 7, "num_classes_found": 7},
     "peixos-fish": {"category": "underwater", "train": 821, "test": 118, "valid": 261, "size": 1200, "num_classes": 12, "num_classes_found": 2},
     "underwater-objects-5v7p8": {"category": "underwater", "train": 5320, "test": 760, "valid": 1520, "size": 7600, "num_classes": 5, "num_classes_found": 5},
     "coral-lwptl": {"category": "underwater", "train": 427, "test": 74, "valid": 93, "size": 594, "num_classes": 14, "num_classes_found": 14},
     "tweeter-posts": {"category": "documents", "train": 87, "test": 9, "valid": 21, "size": 117, "num_classes": 2, "num_classes_found": 2},
-    "tweeter-profile": {"category": "documents", "train": 425, "test": 61, "valid": 121, "size": 607, "num_classes": 1, "num_classes_found": 0},
+    "tweeter-profile": {"category": "documents", "train": 425, "test": 61, "valid": 121, "size": 607, "num_classes": 1, "num_classes_found": 1},
     "document-parts": {"category": "documents", "train": 906, "test": 150, "valid": 318, "size": 1374, "num_classes": 2, "num_classes_found": 2},
     "activity-diagrams-qdobr": {"category": "documents", "train": 259, "test": 45, "valid": 74, "size": 378, "num_classes": 19, "num_classes_found": 19},
     "signatures-xc8up": {"category": "documents", "train": 257, "test": 37, "valid": 74, "size": 368, "num_classes": 1, "num_classes_found": 1},
     "paper-parts": {"category": "documents", "train": 8472, "test": 1209, "valid": 2359, "size": 12040, "num_classes": 46, "num_classes_found": 19},
     "tabular-data-wf9uh": {"category": "documents", "train": 3251, "test": 206, "valid": 409, "size": 3866, "num_classes": 12, "num_classes_found": 12},
     "paragraphs-co84b": {"category": "documents", "train": 4209, "test": 633, "valid": 1221, "size": 6063, "num_classes": 7, "num_classes_found": 7},
     "thermal-dogs-and-people-x6ejw": {
@@ -144,15 +144,15 @@
     "asbestos": 4,
     "underwater-pipes-4ng4t": 1,
     "aquarium-qlnqy": 7,
     "peixos-fish": 2,
     "underwater-objects-5v7p8": 5,
     "coral-lwptl": 14,
     "tweeter-posts": 2,
-    "tweeter-profile": 0,
+    "tweeter-profile": 1,
     "document-parts": 2,
     "activity-diagrams-qdobr": 19,
     "signatures-xc8up": 1,
     "paper-parts": 19,
     "tabular-data-wf9uh": 12,
     "paragraphs-co84b": 7,
     "thermal-dogs-and-people-x6ejw": 2,
```

## super_gradients/training/models/__init__.py

```diff
@@ -58,21 +58,34 @@
     CustomizedShuffleNetV2,
     ShufflenetV2_x2_0,
 )
 from super_gradients.training.models.classification_models.vgg import VGG
 from super_gradients.training.models.classification_models.vit import ViT, ViTBase, ViTLarge, ViTHuge
 
 # Detection models
-from super_gradients.training.models.detection_models.csp_darknet53 import CSPDarknet53
-from super_gradients.training.models.detection_models.pp_yolo_e.pp_yolo_e import PPYoloE, PPYoloE_S, PPYoloE_M, PPYoloE_L, PPYoloE_X
+from super_gradients.training.models.detection_models.csp_darknet53 import CSPDarknet53, SPP
+from super_gradients.training.models.detection_models.pp_yolo_e import PPYoloE, PPYoloE_S, PPYoloE_M, PPYoloE_L, PPYoloE_X
 from super_gradients.training.models.detection_models.darknet53 import Darknet53, Darknet53Base
 from super_gradients.training.models.detection_models.ssd import SSDMobileNetV1, SSDLiteMobileNetV2
 from super_gradients.training.models.detection_models.yolo_base import YoloBase, YoloPostPredictionCallback
 from super_gradients.training.models.detection_models.yolox import YoloX_N, YoloX_T, YoloX_S, YoloX_M, YoloX_L, YoloX_X, CustomYoloX
 from super_gradients.training.models.detection_models.customizable_detector import CustomizableDetector
+from super_gradients.training.models.detection_models.yolo_nas import (
+    YoloNASStage,
+    YoloNASStem,
+    YoloNASDownStage,
+    YoloNASUpStage,
+    YoloNASBottleneck,
+    YoloNASDFLHead,
+    NDFLHeads,
+    YoloNASPANNeckWithC2,
+    YoloNAS_S,
+    YoloNAS_M,
+    YoloNAS_L,
+)
 
 # Segmentation models
 from super_gradients.training.models.segmentation_models.shelfnet import (
     ShelfNet50,
     ShelfNet101,
     ShelfNetHW,
     ShelfNetLW,
@@ -92,15 +105,14 @@
     STDCClassification,
     STDC1Classification,
     STDCClassificationBase,
     STDC2Classification,
     STDCSegmentationBase,
     CustomSTDCSegmentation,
 )
-from super_gradients.training.models.segmentation_models.segformer import SegFormerB0, SegFormerB1, SegFormerB2, SegFormerB3, SegFormerB4, SegFormerB5
 
 # Pose estimation
 from super_gradients.training.models.pose_estimation_models.pose_ppyolo import PosePPYoloL
 from super_gradients.training.models.pose_estimation_models.pose_ddrnet39 import PoseDDRNet39
 from super_gradients.training.models.pose_estimation_models.dekr_hrnet import DEKRPoseEstimationModel, DEKRW32
 
 # KD
@@ -112,14 +124,26 @@
 from super_gradients.training.models.conversion import convert_to_onnx, convert_from_config
 
 
 from super_gradients.common.object_names import Models
 from super_gradients.common.registry.registry import ARCHITECTURES
 
 __all__ = [
+    "SPP",
+    "YoloNAS_S",
+    "YoloNAS_M",
+    "YoloNAS_L",
+    "YoloNASStage",
+    "YoloNASUpStage",
+    "YoloNASStem",
+    "YoloNASDownStage",
+    "YoloNASDFLHead",
+    "YoloNASBottleneck",
+    "NDFLHeads",
+    "YoloNASPANNeckWithC2",
     "SgModule",
     "Beit",
     "BeitLargePatch16_224",
     "BeitBasePatch16_224",
     "DenseNet",
     "CustomizedDensnet",
     "DenseNet121",
@@ -255,14 +279,8 @@
     "get_model_name",
     "get_arch_params",
     "convert_to_onnx",
     "convert_from_config",
     "ARCHITECTURES",
     "Models",
     "user_models",
-    "SegFormerB0",
-    "SegFormerB1",
-    "SegFormerB2",
-    "SegFormerB3",
-    "SegFormerB4",
-    "SegFormerB5",
 ]
```

## super_gradients/training/models/prediction_results.py

```diff
@@ -1,18 +1,19 @@
 import os
 from abc import ABC, abstractmethod
 from typing import List, Optional, Tuple, Iterator
 from dataclasses import dataclass
 
 import numpy as np
 
-from super_gradients.training.utils.detection_utils import DetectionVisualization
 from super_gradients.training.models.predictions import Prediction, DetectionPrediction
 from super_gradients.training.utils.media.video import show_video_from_frames, save_video
 from super_gradients.training.utils.media.image import show_image, save_image
+from super_gradients.training.utils.visualization.utils import generate_color_mapping
+from super_gradients.training.utils.visualization.detection import draw_bbox
 
 
 @dataclass
 class ImagePrediction(ABC):
     """Object wrapping an image and a model's prediction.
 
     :attr image:        Input image
@@ -49,53 +50,56 @@
     :attr class_names:  List of the class names to predict
     """
 
     image: np.ndarray
     prediction: DetectionPrediction
     class_names: List[str]
 
-    def draw(self, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int]]] = None) -> np.ndarray:
+    def draw(self, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int, int, int]]] = None) -> np.ndarray:
         """Draw the predicted bboxes on the image.
 
         :param box_thickness:   Thickness of bounding boxes.
         :param show_confidence: Whether to show confidence scores on the image.
         :param color_mapping:   List of tuples representing the colors for each class.
                                 Default is None, which generates a default color mapping based on the number of class names.
         :return:                Image with predicted bboxes. Note that this does not modify the original image.
         """
-        image_np = self.image.copy()
-        color_mapping = color_mapping or DetectionVisualization._generate_color_mapping(len(self.class_names))
+        image = self.image.copy()
+        color_mapping = color_mapping or generate_color_mapping(len(self.class_names))
 
         for pred_i in range(len(self.prediction)):
-            image_np = DetectionVisualization._draw_box_title(
-                color_mapping=color_mapping,
-                class_names=self.class_names,
+
+            class_id = int(self.prediction.labels[pred_i])
+            score = "" if not show_confidence else str(round(self.prediction.confidence[pred_i], 2))
+
+            image = draw_bbox(
+                image=image,
+                title=f"{self.class_names[class_id]} {score}",
+                color=color_mapping[class_id],
                 box_thickness=box_thickness,
-                image_np=image_np,
                 x1=int(self.prediction.bboxes_xyxy[pred_i, 0]),
                 y1=int(self.prediction.bboxes_xyxy[pred_i, 1]),
                 x2=int(self.prediction.bboxes_xyxy[pred_i, 2]),
                 y2=int(self.prediction.bboxes_xyxy[pred_i, 3]),
-                class_id=int(self.prediction.labels[pred_i]),
-                pred_conf=self.prediction.confidence[pred_i] if show_confidence else None,
             )
-        return image_np
 
-    def show(self, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int]]] = None) -> None:
+        return image
+
+    def show(self, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int, int, int]]] = None) -> None:
         """Display the image with predicted bboxes.
 
         :param box_thickness:   Thickness of bounding boxes.
         :param show_confidence: Whether to show confidence scores on the image.
         :param color_mapping:   List of tuples representing the colors for each class.
                                 Default is None, which generates a default color mapping based on the number of class names.
         """
         image = self.draw(box_thickness=box_thickness, show_confidence=show_confidence, color_mapping=color_mapping)
         show_image(image)
 
-    def save(self, output_path: str, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int]]] = None) -> None:
+    def save(self, output_path: str, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int, int, int]]] = None) -> None:
         """Save the predicted bboxes on the images.
 
         :param output_path:     Path to the output video file.
         :param box_thickness:   Thickness of bounding boxes.
         :param show_confidence: Whether to show confidence scores on the image.
         :param color_mapping:   List of tuples representing the colors for each class.
                                 Default is None, which generates a default color mapping based on the number of class names.
@@ -160,26 +164,28 @@
     """Object wrapping the list of image detection predictions.
 
     :attr _images_prediction_lst:  List of the predictions results
     """
 
     _images_prediction_lst: List[ImageDetectionPrediction]
 
-    def show(self, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int]]] = None) -> None:
+    def show(self, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int, int, int]]] = None) -> None:
         """Display the predicted bboxes on the images.
 
         :param box_thickness:   Thickness of bounding boxes.
         :param show_confidence: Whether to show confidence scores on the image.
         :param color_mapping:   List of tuples representing the colors for each class.
                                 Default is None, which generates a default color mapping based on the number of class names.
         """
         for prediction in self._images_prediction_lst:
             prediction.show(box_thickness=box_thickness, show_confidence=show_confidence, color_mapping=color_mapping)
 
-    def save(self, output_folder: str, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int]]] = None) -> None:
+    def save(
+        self, output_folder: str, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int, int, int]]] = None
+    ) -> None:
         """Save the predicted bboxes on the images.
 
         :param output_folder:     Folder path, where the images will be saved.
         :param box_thickness:   Thickness of bounding boxes.
         :param show_confidence: Whether to show confidence scores on the image.
         :param color_mapping:   List of tuples representing the colors for each class.
                                 Default is None, which generates a default color mapping based on the number of class names.
@@ -199,40 +205,40 @@
     :attr _images_prediction_lst:   List of the predictions results
     :att fps:                       Frames per second of the video
     """
 
     _images_prediction_lst: List[ImageDetectionPrediction]
     fps: int
 
-    def draw(self, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int]]] = None) -> List[np.ndarray]:
+    def draw(self, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int, int, int]]] = None) -> List[np.ndarray]:
         """Draw the predicted bboxes on the images.
 
         :param box_thickness:   Thickness of bounding boxes.
         :param show_confidence: Whether to show confidence scores on the image.
         :param color_mapping:   List of tuples representing the colors for each class.
                                 Default is None, which generates a default color mapping based on the number of class names.
         :return:                List of images with predicted bboxes. Note that this does not modify the original image.
         """
         frames_with_bbox = [
             result.draw(box_thickness=box_thickness, show_confidence=show_confidence, color_mapping=color_mapping) for result in self._images_prediction_lst
         ]
         return frames_with_bbox
 
-    def show(self, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int]]] = None) -> None:
+    def show(self, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int, int, int]]] = None) -> None:
         """Display the predicted bboxes on the images.
 
         :param box_thickness:   Thickness of bounding boxes.
         :param show_confidence: Whether to show confidence scores on the image.
         :param color_mapping:   List of tuples representing the colors for each class.
                                 Default is None, which generates a default color mapping based on the number of class names.
         """
         frames = self.draw(box_thickness=box_thickness, show_confidence=show_confidence, color_mapping=color_mapping)
         show_video_from_frames(window_name="Detection", frames=frames, fps=self.fps)
 
-    def save(self, output_path: str, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int]]] = None) -> None:
+    def save(self, output_path: str, box_thickness: int = 2, show_confidence: bool = True, color_mapping: Optional[List[Tuple[int, int, int]]] = None) -> None:
         """Save the predicted bboxes on the images.
 
         :param output_path:     Path to the output video file.
         :param box_thickness:   Thickness of bounding boxes.
         :param show_confidence: Whether to show confidence scores on the image.
         :param color_mapping:   List of tuples representing the colors for each class.
                                 Default is None, which generates a default color mapping based on the number of class names.
```

## super_gradients/training/models/classification_models/resnet.py

```diff
@@ -10,25 +10,22 @@
 Code adapted from https://github.com/pytorch/vision/blob/master/torchvision/models/resnet.py
 """
 
 import torch.nn as nn
 import torch.nn.functional as F
 from collections import OrderedDict
 
+from super_gradients.modules.utils import width_multiplier
 from super_gradients.training.models import SgModule
 from super_gradients.training.utils import get_param
 from super_gradients.training.utils.regularization_utils import DropPath
 from super_gradients.common.registry.registry import register_model
 from super_gradients.common.object_names import Models
 
 
-def width_multiplier(original, factor):
-    return int(original * factor)
-
-
 class BasicBlock(nn.Module):
     def __init__(self, in_planes, planes, stride=1, expansion=1, final_relu=True, droppath_prob=0.0):
         super(BasicBlock, self).__init__()
         self.expansion = expansion
         self.conv1 = nn.Conv2d(in_planes, planes, kernel_size=3, stride=stride, padding=1, bias=False)
         self.bn1 = nn.BatchNorm2d(planes)
         self.conv2 = nn.Conv2d(planes, planes, kernel_size=3, stride=1, padding=1, bias=False)
```

## super_gradients/training/models/detection_models/csp_darknet53.py

```diff
@@ -1,36 +1,24 @@
 """
 CSP Darknet
 
 """
-import math
 from typing import Tuple, Type
 
 import torch
 import torch.nn as nn
 
-from super_gradients.common.registry.registry import register_model
+from super_gradients.common.decorators.factory_decorator import resolve_param
+from super_gradients.common.factories.activations_type_factory import ActivationsTypeFactory
 from super_gradients.common.object_names import Models
-from super_gradients.modules import Residual
-from super_gradients.training.utils.utils import get_param, HpmStruct
+from super_gradients.common.registry.registry import register_model, register_detection_module
+from super_gradients.modules import Residual, Conv, BaseDetectionModule
+from super_gradients.modules.utils import width_multiplier
 from super_gradients.training.models.sg_module import SgModule
-
-
-def autopad(kernel, padding=None):
-    # PAD TO 'SAME'
-    if padding is None:
-        padding = kernel // 2 if isinstance(kernel, int) else [x // 2 for x in kernel]
-    return padding
-
-
-def width_multiplier(original, factor, divisor: int = None):
-    if divisor is None:
-        return int(original * factor)
-    else:
-        return math.ceil(int(original * factor) / divisor) * divisor
+from super_gradients.training.utils.utils import get_param, HpmStruct
 
 
 def get_yolo_type_params(yolo_type: str, width_mult_factor: float, depth_mult_factor: float):
     if yolo_type == "yoloX":
         struct = (3, 9, 9, 3)
         block = CSPLayer
         activation_type = nn.SiLU
@@ -42,30 +30,14 @@
     return struct, block, activation_type, width_mult, depth_mult
 
 
 class NumClassesMissingException(Exception):
     pass
 
 
-class Conv(nn.Module):
-    # STANDARD CONVOLUTION
-    def __init__(self, input_channels, output_channels, kernel, stride, activation_type: Type[nn.Module], padding: int = None, groups: int = None):
-        super().__init__()
-
-        self.conv = nn.Conv2d(input_channels, output_channels, kernel, stride, autopad(kernel, padding), groups=groups or 1, bias=False)
-        self.bn = nn.BatchNorm2d(output_channels)
-        self.act = activation_type()
-
-    def forward(self, x):
-        return self.act(self.bn(self.conv(x)))
-
-    def fuseforward(self, x):
-        return self.act(self.conv(x))
-
-
 class GroupedConvBlock(nn.Module):
     """
     Grouped Conv KxK -> usual Conv 1x1
     """
 
     def __init__(self, input_channels, output_channels, kernel, stride, activation_type: Type[nn.Module], padding: int = None, groups: int = None):
         """
@@ -153,28 +125,38 @@
 
     def forward(self, x):
         y1 = self.cv3(self.m(self.cv1(x)))
         y2 = self.cv2(x)
         return self.cv4(self.act(self.bn(torch.cat((y1, y2), dim=1))))
 
 
-class SPP(nn.Module):
+@register_detection_module()
+class SPP(BaseDetectionModule):
     # SPATIAL PYRAMID POOLING LAYER
-    def __init__(self, input_channels, output_channels, k: Tuple, activation_type: Type[nn.Module]):
-        super().__init__()
+    @resolve_param("activation_type", ActivationsTypeFactory())
+    def __init__(self, in_channels, output_channels, k: Tuple, activation_type: Type[nn.Module]):
+        super().__init__(in_channels)
+        self._output_channels = output_channels
 
-        hidden_channels = input_channels // 2
-        self.cv1 = Conv(input_channels, hidden_channels, 1, 1, activation_type)
+        hidden_channels = in_channels // 2
+        self.cv1 = Conv(in_channels, hidden_channels, 1, 1, activation_type)
         self.cv2 = Conv(hidden_channels * (len(k) + 1), output_channels, 1, 1, activation_type)
         self.m = nn.ModuleList([nn.MaxPool2d(kernel_size=x, stride=1, padding=x // 2) for x in k])
 
     def forward(self, x):
         x = self.cv1(x)
         return self.cv2(torch.cat([x] + [m(x) for m in self.m], 1))
 
+    @property
+    def out_channels(self):
+        """
+        :return: channels of tensor(s) that will be returned by a module  in forward
+        """
+        return self._output_channels
+
 
 class ViewModule(nn.Module):
     """
     Returns a reshaped version of the input, to be used in None-Backbone Mode
     """
 
     def __init__(self, features=1024):
```

## super_gradients/training/models/detection_models/customizable_detector.py

```diff
@@ -8,14 +8,16 @@
 from typing import Union, Optional, List
 
 from torch import nn
 from omegaconf import DictConfig
 
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.processing_factory import ProcessingFactory
+from super_gradients.module_interfaces import SupportsReplaceNumClasses
+from super_gradients.modules.head_replacement_utils import replace_num_classes_with_random_weights
 from super_gradients.training.utils.utils import HpmStruct
 from super_gradients.training.models.sg_module import SgModule
 import super_gradients.common.factories.detection_modules_factory as det_factory
 from super_gradients.training.models.prediction_results import ImagesDetectionPrediction
 from super_gradients.training.pipelines.pipelines import DetectionPipeline
 from super_gradients.training.processing.processing import Processing
 from super_gradients.training.utils.detection_utils import DetectionPostPredictionCallback
@@ -98,14 +100,16 @@
                 module.prep_model_for_conversion(input_size, **kwargs)
 
     def replace_head(self, new_num_classes: Optional[int] = None, new_head: Optional[nn.Module] = None):
         if new_num_classes is None and new_head is None:
             raise ValueError("At least one of new_num_classes, new_head must be given to replace output layer.")
         if new_head is not None:
             self.heads = new_head
+        elif isinstance(self.heads, SupportsReplaceNumClasses):
+            self.heads.replace_num_classes(new_num_classes, replace_num_classes_with_random_weights)
         else:
             factory = det_factory.DetectionModulesFactory()
             self.heads_params = factory.insert_module_param(self.heads_params, "num_classes", new_num_classes)
             self.heads = factory.get(factory.insert_module_param(self.heads_params, "in_channels", self.neck.out_channels))
             self._initialize_weights(self.bn_eps, self.bn_momentum, self.inplace_act)
 
     @staticmethod
```

## super_gradients/training/models/detection_models/yolo_base.py

```diff
@@ -2,17 +2,17 @@
 from typing import Union, Type, List, Tuple, Optional
 
 import torch
 import torch.nn as nn
 
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.processing_factory import ProcessingFactory
-from super_gradients.modules import CrossModelSkipConnection
+from super_gradients.modules import CrossModelSkipConnection, Conv
 from super_gradients.training.models.classification_models.regnet import AnyNetX, Stage
-from super_gradients.training.models.detection_models.csp_darknet53 import Conv, GroupedConvBlock, CSPDarknet53, get_yolo_type_params, SPP
+from super_gradients.training.models.detection_models.csp_darknet53 import GroupedConvBlock, CSPDarknet53, get_yolo_type_params, SPP
 from super_gradients.training.models.sg_module import SgModule
 from super_gradients.training.utils import torch_version_is_greater_or_equal
 from super_gradients.training.utils.detection_utils import non_max_suppression, matrix_non_max_suppression, NMS_Type, DetectionPostPredictionCallback, Anchors
 from super_gradients.training.utils.utils import HpmStruct, check_img_size_divisibility, get_param
 from super_gradients.training.models.prediction_results import ImagesDetectionPrediction
 from super_gradients.training.pipelines.pipelines import DetectionPipeline
 from super_gradients.training.processing.processing import Processing
```

## super_gradients/training/models/detection_models/pp_yolo_e/__init__.py

```diff
@@ -1,4 +1,4 @@
-from .pp_yolo_e import PPYoloE
+from .pp_yolo_e import PPYoloE, PPYoloE_S, PPYoloE_M, PPYoloE_L, PPYoloE_X
 from .post_prediction_callback import PPYoloEPostPredictionCallback
 
-__all__ = ["PPYoloE", "PPYoloEPostPredictionCallback"]
+__all__ = ["PPYoloE", "PPYoloEPostPredictionCallback", "PPYoloE_L", "PPYoloE_M", "PPYoloE_S", "PPYoloE_X"]
```

## super_gradients/training/models/detection_models/pp_yolo_e/pan.py

```diff
@@ -6,18 +6,18 @@
 
 from super_gradients.common.registry.registry import register_detection_module
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.activations_type_factory import ActivationsTypeFactory
 from super_gradients.training.models.detection_models.csp_resnet import CSPResNetBasicBlock
 from super_gradients.modules import ConvBNAct
 
-__all__ = ["CustomCSPPAN"]
+__all__ = ["PPYoloECSPPAN"]
 
 
-class SPP(nn.Module):
+class PPYoloESPP(nn.Module):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         kernel_size: int,
         pool_size: Tuple[int, ...],
         activation_type: Type[nn.Module],
@@ -48,15 +48,15 @@
         self.conv2 = ConvBNAct(in_channels, ch_mid, kernel_size=1, padding=0, activation_type=activation_type, stride=1, bias=False)
 
         convs = []
         next_ch_in = ch_mid
         for i in range(n):
             convs.append((str(i), CSPResNetBasicBlock(next_ch_in, ch_mid, activation_type=activation_type, use_residual_connection=False)))
             if i == (n - 1) // 2 and spp:
-                convs.append(("spp", SPP(ch_mid, ch_mid, 1, (5, 9, 13), activation_type=activation_type)))
+                convs.append(("spp", PPYoloESPP(ch_mid, ch_mid, 1, (5, 9, 13), activation_type=activation_type)))
             next_ch_in = ch_mid
 
         self.convs = nn.Sequential(collections.OrderedDict(convs))
         self.conv3 = ConvBNAct(ch_mid * 2, out_channels, kernel_size=1, padding=0, activation_type=activation_type, stride=1, bias=False)
 
     def forward(self, x):
         y1 = self.conv1(x)
@@ -64,15 +64,15 @@
         y2 = self.convs(y2)
         y = torch.cat([y1, y2], dim=1)
         y = self.conv3(y)
         return y
 
 
 @register_detection_module()
-class CustomCSPPAN(nn.Module):
+class PPYoloECSPPAN(nn.Module):
     @resolve_param("activation", ActivationsTypeFactory())
     def __init__(
         self,
         in_channels: Tuple[int, ...],
         out_channels: Tuple[int, ...],
         activation: Type[nn.Module],
         stage_num: int,
```

## super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py

```diff
@@ -1,18 +1,19 @@
 from typing import Union, Optional, List
 
 from torch import Tensor
+
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.processing_factory import ProcessingFactory
 from super_gradients.common.registry.registry import register_model
 from super_gradients.common.object_names import Models
 from super_gradients.modules import RepVGGBlock
 from super_gradients.training.models.sg_module import SgModule
 from super_gradients.training.models.detection_models.csp_resnet import CSPResNetBackbone
-from super_gradients.training.models.detection_models.pp_yolo_e.pan import CustomCSPPAN
+from super_gradients.training.models.detection_models.pp_yolo_e.pan import PPYoloECSPPAN
 from super_gradients.training.models.detection_models.pp_yolo_e.pp_yolo_head import PPYOLOEHead
 from super_gradients.training.utils import HpmStruct
 from super_gradients.training.models.arch_params_factory import get_arch_params
 from super_gradients.training.models.detection_models.pp_yolo_e.post_prediction_callback import PPYoloEPostPredictionCallback, DetectionPostPredictionCallback
 from super_gradients.training.models.prediction_results import ImagesDetectionPrediction
 from super_gradients.training.pipelines.pipelines import DetectionPipeline
 from super_gradients.training.processing.processing import Processing
@@ -22,15 +23,15 @@
 class PPYoloE(SgModule):
     def __init__(self, arch_params):
         super().__init__()
         if isinstance(arch_params, HpmStruct):
             arch_params = arch_params.to_dict()
 
         self.backbone = CSPResNetBackbone(**arch_params["backbone"], depth_mult=arch_params["depth_mult"], width_mult=arch_params["width_mult"])
-        self.neck = CustomCSPPAN(**arch_params["neck"], depth_mult=arch_params["depth_mult"], width_mult=arch_params["width_mult"])
+        self.neck = PPYoloECSPPAN(**arch_params["neck"], depth_mult=arch_params["depth_mult"], width_mult=arch_params["width_mult"])
         self.head = PPYOLOEHead(**arch_params["head"], width_mult=arch_params["width_mult"], num_classes=arch_params["num_classes"])
 
         self._class_names: Optional[List[str]] = None
         self._image_processor: Optional[Processing] = None
         self._default_nms_iou: Optional[float] = None
         self._default_nms_conf: Optional[float] = None
```

## super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py

```diff
@@ -171,19 +171,20 @@
             anchor_points, stride_tensor = self._generate_anchors()
             self.anchor_points = anchor_points
             self.stride_tensor = stride_tensor
 
     @torch.jit.ignore
     def replace_num_classes(self, num_classes: int):
         bias_cls = bias_init_with_prob(0.01)
+        device = self.pred_cls[0].weight.device
         self.pred_cls = nn.ModuleList()
         self.num_classes = num_classes
 
         for in_c in self.in_channels:
-            predict_layer = nn.Conv2d(in_c, num_classes, 3, padding=1)
+            predict_layer = nn.Conv2d(in_c, num_classes, 3, padding=1, device=device)
             torch.nn.init.constant_(predict_layer.weight, 0.0)
             torch.nn.init.constant_(predict_layer.bias, bias_cls)
             self.pred_cls.append(predict_layer)
 
     @torch.jit.ignore
     def forward_train(self, feats: Tuple[Tensor, ...]):
         anchors, anchor_points, num_anchors_list, stride_tensor = generate_anchors_for_grid_cell(
```

## super_gradients/training/models/segmentation_models/unet/unet_decoder.py

```diff
@@ -1,19 +1,20 @@
-from typing import List, Type
+from typing import List, Type, Union, Optional, Tuple
 from abc import ABC, abstractmethod
 
 import torch.nn as nn
 import torch
 
 from super_gradients.common.registry.registry import register_unet_up_block, UP_FUSE_BLOCKS
 from super_gradients.modules import ConvBNReLU, CrossModelSkipConnection, Residual
 from super_gradients.modules.sampling import make_upsample_module
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.list_factory import ListFactory
 from super_gradients.common.factories.type_factory import TypeFactory
+from super_gradients.common import UpsampleMode
 
 
 class AbstractUpFuseBlock(nn.Module, ABC):
     """
     Abstract class for upsample and fuse UNet decoder building block.
     """
 
@@ -25,46 +26,97 @@
         """
         super().__init__()
 
     @abstractmethod
     def forward(self, x, skip):
         raise NotImplementedError()
 
+    @staticmethod
+    def validate_upsample_mode(
+        in_channels: int, up_factor: int, upsample_mode: Union[UpsampleMode, str], fallback_mode: Optional[Union[UpsampleMode, str]] = None
+    ) -> Tuple[Union[UpsampleMode, str], int]:
+        """
+        Validate whether the upsample_mode is supported, and returns the upsample path output channels.
+        :return: tuple of upsample_mode and out_channels of the upsample module
+        """
+        out_channels = in_channels
+        upsample_mode = upsample_mode.value if isinstance(upsample_mode, UpsampleMode) else upsample_mode
+        if upsample_mode in [UpsampleMode.PIXEL_SHUFFLE.value, UpsampleMode.NN_PIXEL_SHUFFLE.value]:
+            # Check if in_channels is divisible by (up_factor ** 2) for pixel shuffle, else fallback to fallback_mode.
+            _in_ch = in_channels / (up_factor**2)
+            if _in_ch % 1 == 0:
+                out_channels = int(_in_ch)
+            elif fallback_mode is not None:
+                upsample_mode = fallback_mode
+            else:
+                raise ValueError(
+                    f"Upsample mode: {upsample_mode} can't be used, due to in_channels: {in_channels} "
+                    f"is not divisible by (up_factor ** 2) for up_factor: {up_factor}.\n"
+                    f"Consider setting a `fallback_mode`."
+                )
+        return upsample_mode, out_channels
+
 
 @register_unet_up_block()
 class UpFactorBlock(AbstractUpFuseBlock):
     """
     Ignore Skip features, simply apply upsampling and ConvBNRelu layers.
     """
 
-    def __init__(self, in_channels: int, skip_channels: int, out_channels: int, up_factor: int, mode: str, num_repeats: int, **kwargs):
+    def __init__(
+        self,
+        in_channels: int,
+        skip_channels: int,
+        out_channels: int,
+        up_factor: int,
+        mode: Union[UpsampleMode, str],
+        num_repeats: int,
+        fallback_mode: Optional[Union[UpsampleMode, str]] = None,
+        **kwargs,
+    ):
         super().__init__(in_channels=in_channels, skip_channels=0, out_channels=out_channels)
+
+        mode, up_out_channels = self.validate_upsample_mode(in_channels, up_factor=up_factor, upsample_mode=mode, fallback_mode=fallback_mode)
         self.up_path = make_upsample_module(scale_factor=up_factor, upsample_mode=mode, align_corners=False)
 
         self.last_convs = nn.Sequential(
-            ConvBNReLU(in_channels, out_channels, kernel_size=3, padding=1, bias=False),
+            ConvBNReLU(up_out_channels, out_channels, kernel_size=3, padding=1, bias=False),
             nn.Sequential(*[ConvBNReLU(out_channels, out_channels, kernel_size=3, padding=1, bias=False) for _ in range(num_repeats - 1)]),
         )
 
     def forward(self, x, skip):
         x = self.up_path(x)
         return self.last_convs(x)
 
 
 @register_unet_up_block()
 class UpCatBlock(AbstractUpFuseBlock):
     """
     Fuse features with concatenation and followed Convolutions.
     """
 
-    def __init__(self, in_channels: int, skip_channels: int, out_channels: int, up_factor: int, mode: str, num_repeats: int, **kwargs):
+    def __init__(
+        self,
+        in_channels: int,
+        skip_channels: int,
+        out_channels: int,
+        up_factor: int,
+        mode: Union[UpsampleMode, str],
+        num_repeats: int,
+        fallback_mode: Optional[Union[UpsampleMode, str]] = None,
+        **kwargs,
+    ):
         super().__init__(in_channels=in_channels, skip_channels=skip_channels, out_channels=out_channels)
+
+        mode, up_out_channels = self.validate_upsample_mode(in_channels, up_factor=up_factor, upsample_mode=mode, fallback_mode=fallback_mode)
+
         self.up_path = make_upsample_module(scale_factor=up_factor, upsample_mode=mode, align_corners=False)
+
         self.last_convs = nn.Sequential(
-            ConvBNReLU(in_channels + skip_channels, out_channels, kernel_size=3, padding=1, bias=False),
+            ConvBNReLU(up_out_channels + skip_channels, out_channels, kernel_size=3, padding=1, bias=False),
             nn.Sequential(*[ConvBNReLU(out_channels, out_channels, kernel_size=3, padding=1, bias=False) for _ in range(num_repeats - 1)]),
         )
 
     def forward(self, x, skip):
         x = self.up_path(x)
         x = torch.cat([x, skip], dim=1)
         return self.last_convs(x)
@@ -72,21 +124,36 @@
 
 @register_unet_up_block()
 class UpSumBlock(AbstractUpFuseBlock):
     """
     Fuse features with concatenation and followed Convolutions.
     """
 
-    def __init__(self, in_channels: int, skip_channels: int, out_channels: int, up_factor: int, mode: str, num_repeats: int, **kwargs):
+    def __init__(
+        self,
+        in_channels: int,
+        skip_channels: int,
+        out_channels: int,
+        up_factor: int,
+        mode: Union[UpsampleMode, str],
+        num_repeats: int,
+        fallback_mode: Optional[Union[UpsampleMode, str]] = None,
+        **kwargs,
+    ):
         super().__init__(in_channels=in_channels, skip_channels=skip_channels, out_channels=out_channels)
-        self.proj_conv = Residual() if skip_channels == in_channels else ConvBNReLU(skip_channels, in_channels, kernel_size=1, bias=False, use_activation=False)
+        mode, up_out_channels = self.validate_upsample_mode(in_channels, up_factor=up_factor, upsample_mode=mode, fallback_mode=fallback_mode)
+
         self.up_path = make_upsample_module(scale_factor=up_factor, upsample_mode=mode, align_corners=False)
 
+        self.proj_conv = (
+            Residual() if skip_channels == up_out_channels else ConvBNReLU(skip_channels, up_out_channels, kernel_size=1, bias=False, use_activation=False)
+        )
+
         self.last_convs = nn.Sequential(
-            ConvBNReLU(in_channels, out_channels, kernel_size=3, padding=1, bias=False),
+            ConvBNReLU(up_out_channels, out_channels, kernel_size=3, padding=1, bias=False),
             nn.Sequential(*[ConvBNReLU(out_channels, out_channels, kernel_size=3, padding=1, bias=False) for _ in range(num_repeats - 1)]),
         )
 
     def forward(self, x, skip):
         skip = self.proj_conv(skip)
         x = self.up_path(x)
         x = x + skip
```

## super_gradients/training/pipelines/pipelines.py

```diff
@@ -48,15 +48,15 @@
     :param image_processor: A single image processor or a list of image processors for preprocessing and postprocessing the images.
     :param device:          The device on which the model will be run. If None, will run on current model device. Use "cuda" for GPU support.
     """
 
     def __init__(self, model: SgModule, image_processor: Union[Processing, List[Processing]], class_names: List[str], device: Optional[str] = None):
         super().__init__()
         self.device = device or next(model.parameters()).device
-        self.model = model.to(device)
+        self.model = model.to(self.device)
         self.class_names = class_names
 
         if isinstance(image_processor, list):
             image_processor = ComposeProcessing(image_processor)
         self.image_processor = image_processor
 
     def __call__(self, inputs: Union[str, ImageSource, List[ImageSource]], batch_size: Optional[int] = 32) -> ImagesPredictions:
@@ -261,15 +261,20 @@
 
     def _instantiate_image_prediction(self, image: np.ndarray, prediction: DetectionPrediction) -> ImagePrediction:
         return ImageDetectionPrediction(image=image, prediction=prediction, class_names=self.class_names)
 
     def _combine_image_prediction_to_images(
         self, images_predictions: Iterable[ImageDetectionPrediction], n_images: Optional[int] = None
     ) -> ImagesDetectionPrediction:
-        images_predictions = [image_predictions for image_predictions in tqdm(images_predictions, total=n_images, desc="Predicting Images")]
+        if n_images is not None and n_images == 1:
+            # Do not show tqdm progress bar if there is only one image
+            pass
+        else:
+            images_predictions = [image_predictions for image_predictions in tqdm(images_predictions, total=n_images, desc="Predicting Images")]
+
         return ImagesDetectionPrediction(_images_prediction_lst=images_predictions)
 
     def _combine_image_prediction_to_video(
         self, images_predictions: Iterable[ImageDetectionPrediction], fps: float, n_images: Optional[int] = None
     ) -> VideoDetectionPrediction:
         images_predictions = [image_predictions for image_predictions in tqdm(images_predictions, total=n_images, desc="Predicting Video")]
         return VideoDetectionPrediction(_images_prediction_lst=images_predictions, fps=fps)
```

## super_gradients/training/processing/processing.py

```diff
@@ -301,16 +301,16 @@
         image_processor=image_processor,
         iou=0.65,
         conf=0.5,
     )
     return params
 
 
-def default_deciyolo_coco_processing_params() -> dict:
-    """Processing parameters commonly used for training DeciYolo on COCO dataset.
+def default_yolo_nas_coco_processing_params() -> dict:
+    """Processing parameters commonly used for training YoloNAS on COCO dataset.
     TODO: remove once we load it from the checkpoint
     """
 
     image_processor = ComposeProcessing(
         [
             DetectionLongestMaxSizeRescale(output_shape=(636, 636)),
             DetectionCenterPadding(output_shape=(640, 640), pad_value=114),
@@ -318,25 +318,25 @@
             ImagePermute(permutation=(2, 0, 1)),
         ]
     )
 
     params = dict(
         class_names=COCO_DETECTION_CLASSES_LIST,
         image_processor=image_processor,
-        iou=0.65,
-        conf=0.5,
+        iou=0.7,
+        conf=0.25,
     )
     return params
 
 
 def get_pretrained_processing_params(model_name: str, pretrained_weights: str) -> dict:
     """Get the processing parameters for a pretrained model.
     TODO: remove once we load it from the checkpoint
     """
     if pretrained_weights == "coco":
         if "yolox" in model_name:
             return default_yolox_coco_processing_params()
         elif "ppyoloe" in model_name:
             return default_ppyoloe_coco_processing_params()
-        elif "deciyolo" in model_name:
-            return default_deciyolo_coco_processing_params()
+        elif "yolo_nas" in model_name:
+            return default_yolo_nas_coco_processing_params()
     return dict()
```

## super_gradients/training/qat_trainer/qat_trainer.py

```diff
@@ -7,15 +7,14 @@
 from omegaconf import DictConfig
 from omegaconf import OmegaConf
 from torch import nn
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.environment.device_utils import device_config
 from super_gradients.training import utils as core_utils, models, dataloaders
-from super_gradients.training.metrics.metric_utils import get_metrics_dict
 from super_gradients.training.sg_trainer import Trainer
 from super_gradients.training.utils import get_param
 from super_gradients.training.utils.distributed_training_utils import setup_device
 from super_gradients.modules.repvgg_block import fuse_repvgg_blocks_residual_branches
 
 logger = get_logger(__name__)
 try:
@@ -154,16 +153,15 @@
             percentile=get_param(cfg.quantization_params.calib_params, "percentile", 99.99),
         )
         calibrator.reset_calibrators(model)  # release memory taken by calibrators
 
         # VALIDATE PTQ MODEL AND PRINT SUMMARY
         logger.info("Validating PTQ model...")
         trainer = Trainer(experiment_name=cfg.experiment_name, ckpt_root_dir=get_param(cfg, "ckpt_root_dir", default_val=None))
-        val_results_tuple = trainer.test(model=model, test_loader=val_dataloader, test_metrics_list=cfg.training_hyperparams.valid_metrics_list)
-        valid_metrics_dict = get_metrics_dict(val_results_tuple, trainer.test_metrics, trainer.loss_logging_items_names)
+        valid_metrics_dict = trainer.test(model=model, test_loader=val_dataloader, test_metrics_list=cfg.training_hyperparams.valid_metrics_list)
         results = ["PTQ Model Validation Results"]
         results += [f"   - {metric:10}: {value}" for metric, value in valid_metrics_dict.items()]
         logger.info("\n".join(results))
 
         # TRAIN
         if cfg.quantization_params.ptq_only:
             logger.info("cfg.quantization_params.ptq_only=True. Performing PTQ only!")
```

## super_gradients/training/sg_trainer/sg_trainer.py

```diff
@@ -325,22 +325,21 @@
             strict_load=cfg.checkpoint_params.strict_load,
             pretrained_weights=cfg.checkpoint_params.pretrained_weights,
             checkpoint_path=cfg.checkpoint_params.checkpoint_path,
             load_backbone=cfg.checkpoint_params.load_backbone,
         )
 
         # TEST
-        val_results_tuple = trainer.test(model=model, test_loader=val_dataloader, test_metrics_list=cfg.training_hyperparams.valid_metrics_list)
+        valid_metrics_dict = trainer.test(model=model, test_loader=val_dataloader, test_metrics_list=cfg.training_hyperparams.valid_metrics_list)
 
-        valid_metrics_dict = get_metrics_dict(val_results_tuple, trainer.test_metrics, trainer.loss_logging_items_names)
         results = ["Validate Results"]
         results += [f"   - {metric:10}: {value}" for metric, value in valid_metrics_dict.items()]
         logger.info("\n".join(results))
 
-        return model, val_results_tuple
+        return model, valid_metrics_dict
 
     @classmethod
     def evaluate_checkpoint(cls, experiment_name: str, ckpt_name: str = "ckpt_latest.pth", ckpt_root_dir: str = None) -> None:
         """
         Evaluate a checkpoint resulting from one of your previous experiment, using the same parameters (dataset, valid_metrics,...)
         as used during the training of the experiment
 
@@ -1744,14 +1743,16 @@
 
         # SWITCH BACK BETWEEN NETS SO AN ADDITIONAL TRAINING CAN BE DONE AFTER TEST
         if use_ema_net and self.ema_model is not None:
             self.net = keep_model
 
         self._first_backward = True
 
+        test_results = get_metrics_dict(test_results, self.test_metrics, self.loss_logging_items_names)
+
         return test_results
 
     def _validate_epoch(self, epoch: int, silent_mode: bool = False) -> tuple:
         """
         Runs evaluation on self.valid_loader, with self.valid_metrics.
 
         :param epoch: (int) epoch idx
```

## super_gradients/training/transforms/transforms.py

```diff
@@ -1162,15 +1162,15 @@
         corner_points = corner_points.reshape(num_gts_boxes, 8)
 
         # create new boxes
         corner_xs = corner_points[:, 0::2]
         corner_ys = corner_points[:, 1::2]
         new_bboxes = np.concatenate((np.min(corner_xs, 1), np.min(corner_ys, 1), np.max(corner_xs, 1), np.max(corner_ys, 1))).reshape(4, -1).T
     else:
-        new_bboxes = np.ones((0, 4), dtype=np.float)
+        new_bboxes = np.ones((0, 4), dtype=np.float32)
 
     if num_gts_masks:
         # warp segmentation points
         num_seg_points = targets_seg.shape[1] // 2
         corner_points_seg = np.ones((num_gts_masks * num_seg_points, 3))
         corner_points_seg[:, :2] = targets_seg[seg_is_present_mask].reshape(num_gts_masks * num_seg_points, 2)
         corner_points_seg = corner_points_seg @ M.T
@@ -1181,15 +1181,15 @@
         seg_points_ys = corner_points_seg[:, 1::2]
         new_tight_bboxes = (
             np.concatenate((np.nanmin(seg_points_xs, 1), np.nanmin(seg_points_ys, 1), np.nanmax(seg_points_xs, 1), np.nanmax(seg_points_ys, 1)))
             .reshape(4, -1)
             .T
         )
     else:
-        new_tight_bboxes = np.ones((0, 4), dtype=np.float)
+        new_tight_bboxes = np.ones((0, 4), dtype=np.float32)
 
     targets[~seg_is_present_mask, :4] = new_bboxes
     targets[seg_is_present_mask, :4] = new_tight_bboxes
 
     # clip boxes
     targets[:, [0, 2]] = targets[:, [0, 2]].clip(0, twidth)
     targets[:, [1, 3]] = targets[:, [1, 3]].clip(0, theight)
```

## super_gradients/training/utils/checkpoint_utils.py

```diff
@@ -287,20 +287,30 @@
     """
     Loads pretrained weights from the MODEL_URLS dictionary to model
     :param architecture: name of the model's architecture
     :param model: model to load pretrinaed weights for
     :param pretrained_weights: name for the pretrianed weights (i.e imagenet)
     :return: None
     """
+    from super_gradients.common.object_names import Models
+
     model_url_key = architecture + "_" + str(pretrained_weights)
     if model_url_key not in MODEL_URLS.keys():
         raise MissingPretrainedWeightsException(model_url_key)
 
     url = MODEL_URLS[model_url_key]
-    unique_filename = url.split("https://deci-pretrained-models.s3.amazonaws.com/")[1].replace("/", "_").replace(" ", "_")
+
+    if architecture in {Models.YOLO_NAS_S, Models.YOLO_NAS_M, Models.YOLO_NAS_L}:
+        logger.info(
+            "License Notification: YOLO-NAS pre-trained weights are subjected to the specific license terms and conditions detailed in \n"
+            "https://github.com/Deci-AI/super-gradients/blob/master/LICENSE.YOLONAS.md\n"
+            "By downloading the pre-trained weight files you agree to comply with these terms."
+        )
+
+    unique_filename = url.split("https://sghub.deci.ai/models/")[1].replace("/", "_").replace(" ", "_")
     map_location = torch.device("cpu")
     pretrained_state_dict = load_state_dict_from_url(url=url, map_location=map_location, file_name=unique_filename)
     _load_weights(architecture, model, pretrained_state_dict)
 
 
 def _load_weights(architecture, model, pretrained_state_dict):
     if "ema_net" in pretrained_state_dict.keys():
```

## super_gradients/training/utils/detection_utils.py

```diff
@@ -3,23 +3,25 @@
 import pathlib
 import random
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Callable, List, Union, Tuple, Optional, Dict
 
 import cv2
-import matplotlib.pyplot as plt
+
 import numpy as np
 import torch
 import torchvision
 from omegaconf import ListConfig
 from torch import nn
 from torch.utils.data.dataloader import default_collate
 
 from super_gradients.common.registry.registry import register_collate_function
+from super_gradients.training.utils.visualization.detection import draw_bbox
+from super_gradients.training.utils.visualization.utils import generate_color_mapping
 
 
 class DetectionTargetsFormat(Enum):
     """
     Enum class for the different detection output formats
 
     When NORMALIZED is not specified- the type refers to unnormalized image coordinates (of the bboxes).
@@ -360,17 +362,16 @@
 
 class DetectionVisualization:
     @staticmethod
     def _generate_color_mapping(num_classes: int) -> List[Tuple[int]]:
         """
         Generate a unique BGR color for each class
         """
-        cmap = plt.cm.get_cmap("gist_rainbow", num_classes)
-        colors = [cmap(i, bytes=True)[:3][::-1] for i in range(num_classes)]
-        return [tuple(int(v) for v in c) for c in colors]
+
+        return generate_color_mapping(num_classes=num_classes)
 
     @staticmethod
     def _draw_box_title(
         color_mapping: List[Tuple[int]],
         class_names: List[str],
         box_thickness: int,
         image_np: np.ndarray,
@@ -381,28 +382,20 @@
         class_id: int,
         pred_conf: float = None,
         is_target: bool = False,
     ):
         color = color_mapping[class_id]
         class_name = class_names[class_id]
 
-        # Draw the box
-        image_np = cv2.rectangle(image_np, (x1, y1), (x2, y2), color, box_thickness)
-
-        # Caption with class name and confidence if given
-        text_color = (255, 255, 255)  # white
-
         if is_target:
             title = f"[GT] {class_name}"
-        if not is_target:
+        else:
             title = f'[Pred] {class_name}  {str(round(pred_conf, 2)) if pred_conf is not None else ""}'
 
-        image_np = cv2.rectangle(image_np, (x1, y1 - 15), (x1 + len(title) * 10, y1), color, cv2.FILLED)
-        image_np = cv2.putText(image_np, title, (x1, y1 - box_thickness), 2, 0.5, text_color, 1, lineType=cv2.LINE_AA)
-
+        draw_bbox(image=image_np, title=title, x1=x1, y1=y1, x2=x2, y2=y2, box_thickness=box_thickness, color=color)
         return image_np
 
     @staticmethod
     def _visualize_image(
         image_np: np.ndarray,
         pred_boxes: np.ndarray,
         target_boxes: np.ndarray,
```

## super_gradients/training/utils/media/image.py

```diff
@@ -127,16 +127,18 @@
         return False
 
 
 def show_image(image: np.ndarray) -> None:
     """Show an image using matplotlib.
     :param image: Image to show in (H, W, C), RGB.
     """
+    plt.figure(figsize=(image.shape[1] / 100.0, image.shape[0] / 100.0), dpi=100)
     plt.imshow(image, interpolation="nearest")
     plt.axis("off")
+    plt.tight_layout()
     plt.show()
 
 
 def check_image_typing(image: ImageSource) -> bool:
     """Check if the given object respects typing of image.
     :param image: Image to check.
     :return: True if the object is an image, False otherwise.
```

## super_gradients/training/utils/media/video.py

```diff
@@ -1,16 +1,21 @@
 from typing import List, Optional, Tuple
 import cv2
+import PIL
 
 import numpy as np
 
 
+from super_gradients.common.abstractions.abstract_logger import get_logger
+
+logger = get_logger(__name__)
+
 __all__ = ["load_video", "save_video", "includes_video_extension", "show_video_from_disk", "show_video_from_frames"]
 
-VIDEO_EXTENSIONS = (".mp4", ".avi", ".mov", ".wmv", ".flv")
+VIDEO_EXTENSIONS = (".mp4", ".avi", ".mov", ".wmv", ".flv", ".gif")
 
 
 def load_video(file_path: str, max_frames: Optional[int] = None) -> Tuple[List[np.ndarray], int]:
     """Open a video file and extract each frame into numpy array.
 
     :param file_path:   Path to the video file.
     :param max_frames:  Optional, maximum number of frames to extract.
@@ -53,15 +58,45 @@
             break
         frames.append(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB))
 
     return frames
 
 
 def save_video(output_path: str, frames: List[np.ndarray], fps: int) -> None:
-    """Save a video locally.
+    """Save a video locally. Depending on the extension, the video will be saved as a .mp4 file or as a .gif file.
+
+    :param output_path: Where the video will be saved
+    :param frames:      Frames representing the video, each in (H, W, C), RGB. Note that all the frames are expected to have the same shape.
+    :param fps:         Frames per second
+    """
+    if not includes_video_extension(output_path):
+        logger.info(f'Output path "{output_path}" does not have a video extension, and therefore will be saved as {output_path}.mp4')
+        output_path += ".mp4"
+
+    if check_is_gif(output_path):
+        save_gif(output_path, frames, fps)
+    else:
+        save_mp4(output_path, frames, fps)
+
+
+def save_gif(output_path: str, frames: List[np.ndarray], fps: int) -> None:
+    """Save a video locally in .gif format.
+
+    :param output_path: Where the video will be saved
+    :param frames:      Frames representing the video, each in (H, W, C), RGB. Note that all the frames are expected to have the same shape.
+    :param fps:         Frames per second
+    """
+
+    frames_pil = [PIL.Image.fromarray(frame) for frame in frames]
+
+    frames_pil[0].save(output_path, save_all=True, append_images=frames_pil[1:], duration=int(1000 / fps), loop=0)
+
+
+def save_mp4(output_path: str, frames: List[np.ndarray], fps: int) -> None:
+    """Save a video locally in .mp4 format.
 
     :param output_path: Where the video will be saved
     :param frames:      Frames representing the video, each in (H, W, C), RGB. Note that all the frames are expected to have the same shape.
     :param fps:         Frames per second
     """
     video_height, video_width = _validate_frames(frames)
 
@@ -147,7 +182,11 @@
 
 def includes_video_extension(file_path: str) -> bool:
     """Check if a file includes a video extension.
     :param file_path:   Path to the video file.
     :return:            True if the file includes a video extension.
     """
     return isinstance(file_path, str) and file_path.lower().endswith(VIDEO_EXTENSIONS)
+
+
+def check_is_gif(file_path: str) -> bool:
+    return file_path.lower().endswith(".gif")
```

## Comparing `super_gradients/recipes/dataset_params/coco_detection_deci_yolo_dataset_params.yaml` & `super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     - DetectionHorizontalFlip:
         prob: 0.5                       # probability to apply horizontal flip
     - DetectionMixup:
         input_dim:
         mixup_scale: [ 0.5, 1.5 ]         # random rescale range for the additional sample in mixup
         prob: 0.5                       # probability to apply per-sample mixup
         flip_prob: 0.5                  # probability to apply horizontal flip
-    - DetectionStandardizeImage:
-        max_value: 255.
     - DetectionPaddedRescale:
         input_dim: [640, 640]
         max_targets: 120
         pad_value: 114
+    - DetectionStandardize:
+        max_value: 255.
     - DetectionTargetsFormatTransform:
         max_targets: 256
-        output_format: LABEL_NORMALIZED_CXCYWH
+        output_format: LABEL_CXCYWH
 
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: False
 
 train_dataloader_params:
@@ -63,28 +63,29 @@
   cache: False
   transforms:
     - DetectionRGB2BGR:
         prob: 1
     - DetectionPadToSize:
         output_size: [640, 640]
         pad_value: 114
-    - DetectionStandardizeImage:
+    - DetectionStandardize:
         max_value: 255.
     - DetectionImagePermute
     - DetectionTargetsFormatTransform:
         max_targets: 50
         input_dim: [640, 640]
-        output_format: LABEL_NORMALIZED_CXCYWH
+        output_format: LABEL_CXCYWH
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: True
 
 val_dataloader_params:
   batch_size: 25
   num_workers: 8
   drop_last: False
+  shuffle: False
   pin_memory: True
   collate_fn:
     _target_: super_gradients.training.utils.detection_utils.CrowdDetectionCollateFN
 
 _convert_: all
```

## Comparing `super_gradients-3.0.9.dist-info/LICENSE.md` & `super_gradients-3.1.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `super_gradients-3.0.9.dist-info/METADATA` & `super_gradients-3.1.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: super-gradients
-Version: 3.0.9
+Version: 3.1.0
 Summary: SuperGradients
-Home-page: https://deci-ai.github.io/super-gradients/welcome.html
+Home-page: https://docs.deci.ai/super-gradients/documentation/source/welcome.html
 Author: Deci AI
 Author-email: rnd@deci.ai
 License: UNKNOWN
 Keywords: Deci,AI,Training,Deep Learning,Computer Vision,PyTorch,SOTA,Recipes,Pre Trained,Models
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: torch (<1.14,>=1.9.0)
@@ -45,63 +45,74 @@
 Requires-Dist: rapidfuzz
 Requires-Dist: json-tricks (==3.16.1)
 Requires-Dist: onnx-simplifier (<1.0,>=0.3.6)
 Provides-Extra: pro
 Requires-Dist: deci-lab-client (==4.17.0) ; extra == 'pro'
 Requires-Dist: deci-common (==3.15.0) ; extra == 'pro'
 
-<div align="center">
+<div align="center" markdown="1">
   <img src="docs/assets/SG_img/SG - Horizontal Glow 2.png" width="600"/>
  <br/><br/>
 
 **Build, train, and fine-tune production-ready deep learning  SOTA vision models**
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Easily%20train%20or%20fine-tune%20SOTA%20computer%20vision%20models%20from%20one%20training%20repository&url=https://github.com/Deci-AI/super-gradients&via=deci_ai&hashtags=AI,deeplearning,computervision,training,opensource)
 
 #### Version 3 is out! Notebooks have been updated!
 ______________________________________________________________________
-
-  <p align="center">
+</div>  
+<div align="center">
+<p align="center">
   <a href="https://www.supergradients.com/">Website</a> •
-  <a href="https://deci-ai.github.io/super-gradients/welcome.html">Docs</a> •
+  <a href="https://docs.deci.ai/super-gradients/documentation/source/welcome.html">Docs</a> •
   <a href="#getting-started">Getting Started</a> •
   <a href="#implemented-model-architectures">Pretrained Models</a> •
   <a href="#community">Community</a> •
   <a href="#license">License</a> •
   <a href="#deci-platform">Deci Platform</a>
 </p>
 <p align="center">
   <a href="https://github.com/Deci-AI/super-gradients#prerequisites"><img src="https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue" />
   <a href="https://github.com/Deci-AI/super-gradients#prerequisites"><img src="https://img.shields.io/badge/pytorch-1.9%20%7C%201.10-blue" />
   <a href="https://pypi.org/project/super-gradients/"><img src="https://img.shields.io/pypi/v/super-gradients" />
   <a href="https://github.com/Deci-AI/super-gradients#computer-vision-models-pretrained-checkpoints" ><img src="https://img.shields.io/badge/pre--trained%20models-34-brightgreen" />
   <a href="https://github.com/Deci-AI/super-gradients/releases"><img src="https://img.shields.io/github/v/release/Deci-AI/super-gradients" />
   <a href="https://join.slack.com/t/supergradients-comm52/shared_invite/zt-10vz6o1ia-b_0W5jEPEnuHXm087K~t8Q"><img src="https://img.shields.io/badge/slack-community-blueviolet" />
   <a href="https://github.com/Deci-AI/super-gradients/blob/master/LICENSE.md"><img src="https://img.shields.io/badge/license-Apache%202.0-blue" />
-  <a href="https://deci-ai.github.io/super-gradients/welcome.html"><img src="https://img.shields.io/badge/docs-sphinx-brightgreen" />
+  <a href="https://docs.deci.ai/super-gradients/documentation/source/welcome.html"><img src="https://img.shields.io/badge/docs-mkdocs-brightgreen" /></a>
 </p>    
 </div>
 
+______________________________________________________________________
+
 ## Build with SuperGradients
 __________________________________________________________________________________________________________
 
 ### Support various computer vision tasks
 <div align="center">
 <img src="https://github.com/Deci-AI/super-gradients/raw/master/docs/assets/SG_img/Segmentation 1500x900 .png" width="250px">
 <img src="https://github.com/Deci-AI/super-gradients/raw/master/docs/assets/SG_img/Object detection 1500X900.png" width="250px">
 <img src="https://github.com/Deci-AI/super-gradients/raw/master/docs/assets/SG_img/Classification 1500x900.png" width="250px">
 </div>
 
 
 ### Ready to deploy pre-trained SOTA models
+
+YOLO-NAS architecture is out! The new YOLO-NAS delivers state-of-the-art performance with the unparalleled accuracy-speed performance, outperforming other models such as YOLOv5, YOLOv6, YOLOv7 and YOLOv8.
+Check it out here: [YOLO-NAS](YOLONAS.md).
+
+<div align="center">
+<img src="./documentation/source/images/yolo_nas_frontier.png" width="800px">
+</div>
+
 ```python
 # Load model with pretrained weights
 from super_gradients.training import models
 from super_gradients.common.object_names import Models
 
-model = models.get(Models.YOLOX_S, pretrained_weights="coco")
+model = models.get(Models.YOLO_NAS_M, pretrained_weights="coco")
 ```
 #### All Computer Vision Models - Pretrained Checkpoints can be found in the [Model Zoo](http://bit.ly/41dkt89)
 
 #### Classification
 <div align="center">
 <img src="./docs/assets/SG_img/Classification@2xDark.png" width="800px">
 </div>
@@ -120,38 +131,38 @@
 ### Easy to train SOTA Models
 
 Easily load and fine-tune production-ready, pre-trained SOTA models that incorporate best practices and validated hyper-parameters for achieving best-in-class accuracy. 
 For more information on how to do it go to [Getting Started](#getting-started)
 
 
 #### Plug and play recipes
-```python
-python -m super_gradients.examples.train_from_recipe_example.train_from_recipe architecture=regnetY800 dataset_interface.data_dir=<YOUR_Imagenet_LOCAL_PATH> ckpt_root_dir=<CHEKPOINT_DIRECTORY>
+```bash
+python -m super_gradients.train_from_recipe architecture=regnetY800 dataset_interface.data_dir=<YOUR_Imagenet_LOCAL_PATH> ckpt_root_dir=<CHEKPOINT_DIRECTORY>
 ```
 More example on how and why to use recipes can be found in [Recipes](#recipes)
 
 
 ### Production readiness
 All SuperGradients models’ are production ready in the sense that they are compatible with deployment tools such as TensorRT (Nvidia) and OpenVINO (Intel) and can be easily taken into production. With a few lines of code you can easily integrate the models into your codebase.
 ```python
 # Load model with pretrained weights
 from super_gradients.training import models
 from super_gradients.common.object_names import Models
 
-model = models.get(Models.YOLOX_S, pretrained_weights="coco")
+model = models.get(Models.YOLO_NAS_M, pretrained_weights="coco")
 
 # Prepare model for conversion
-# Input size is in format of [Batch x Channels x Width x Height] where 640 is the standart COCO dataset dimensions
+# Input size is in format of [Batch x Channels x Width x Height] where 640 is the standard COCO dataset dimensions
 model.eval()
 model.prep_model_for_conversion(input_size=[1, 3, 640, 640])
 
 # Create dummy_input
 
 # Convert model to onnx
-torch.onnx.export(model, dummy_input,  "yolox_s.onnx")
+torch.onnx.export(model, dummy_input,  "yolo_nas_m.onnx")
 ```
 More information on how to take your model to production can be found in [Getting Started](#getting-started) notebooks
 
 ## Quick Installation
 
 __________________________________________________________________________________________________________
 
@@ -205,15 +216,15 @@
 
 ### Start Training with Just 1 Command Line
 The most simple and straightforward way to start training SOTA performance models with SuperGradients reproducible recipes. Just define your dataset path and where you want your checkpoints to be saved and you are good to go from your terminal!
 
 Just make sure that you [setup your dataset](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/Dataset_Setup_Instructions.md) according to the data dir specified in the recipe.
 
 ```bash
-python -m super_gradients.examples.train_from_recipe_example.train_from_recipe --config-name=imagenet_regnetY architecture=regnetY800 dataset_interface.data_dir=<YOUR_Imagenet_LOCAL_PATH> ckpt_root_dir=<CHEKPOINT_DIRECTORY>
+python -m super_gradients.train_from_recipe --config-name=imagenet_regnetY architecture=regnetY800 dataset_interface.data_dir=<YOUR_Imagenet_LOCAL_PATH> ckpt_root_dir=<CHEKPOINT_DIRECTORY>
 ```
 ### Quickly Load Pre-Trained Weights for Your Desired Model with SOTA Performance
 Want to try our pre-trained models on your machine? Import SuperGradients, initialize your Trainer, and load your desired architecture and pre-trained weights from our [SOTA model zoo](http://bit.ly/41dkt89)
 
 ```python
 # The pretrained_weights argument will load a pre-trained architecture on the provided dataset
 
@@ -357,15 +368,15 @@
  <td width="200">  
 <a target="_blank" href="https://bit.ly/3QSrHbm"><img src="./docs/assets/SG_img/GitHub_logo.png" /> GitHub source</a>
  </td>
 </table>
  </br></br>
 
  </br>
-<details>
+<details markdown="1">
   <summary><h3>Using Distributed Data Parallel (DDP) </h3></summary>
 
 #### Why use DDP ?
 
 Recent Deep Learning models are growing larger and larger to an extent that training on a single GPU can take weeks.
 In order to train models in a timely fashion, it is necessary to train them with multiple GPUs.
 Using 100s GPUs can reduce training time of a model from a week to less than an hour.
@@ -469,15 +480,15 @@
 
 #### Good to know
 Your total batch size will be (number of gpus x batch size), so you might want to increase your learning rate.
 There is no clear rule, but a rule of thumb seems to be to [linearly increase the learning rate with the number of gpus](https://arxiv.org/pdf/1706.02677.pdf) 
 
 </details>
 
-<details>
+<details markdown="1">
 <summary><h3> Easily change architectures parameters </h3></summary>
 
 ```python
 from super_gradients.training import models
 
 # instantiate default pretrained resnet18
 default_resnet18 = models.get(model_name="resnet18", num_classes=100, pretrained_weights="imagenet")
@@ -487,15 +498,15 @@
 
 # instantiate pretrained resnet18, without classifier head. Output will be from the last stage before global pooling
 backbone_resnet18 = models.get(model_name="resnet18", arch_params={"backbone_mode": True}, pretrained_weights="imagenet")
 ```
 
 </details>
 
-<details>
+<details markdown="1">
 
 <summary><h3> Using phase callbacks </h3></summary>  
 
 ```python
 from super_gradients import Trainer
 from torch.optim.lr_scheduler import ReduceLROnPlateau
 from super_gradients.training.utils.callbacks import Phase, LRSchedulerCallback
@@ -516,14 +527,41 @@
 
 # define phase_callbacks as part of the training parameters
 train_params = {"phase_callbacks": phase_callbacks}
 ```
 
 </details>
 
+<details markdown="1">
+
+<summary><h3> Integration to DagsHub </h3></summary>    
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/11fW56pMpwOMHQSbQW6xxMRYvw1mEC-t-?usp=sharing) 
+
+```python
+from super_gradients import Trainer
+
+trainer = Trainer("experiment_name")
+model = ...
+
+training_params = { ...  # Your training params
+                   "sg_logger": "dagshub_sg_logger",  # DagsHub Logger, see class super_gradients.common.sg_loggers.dagshub_sg_logger.DagsHubSGLogger for details
+                   "sg_logger_params":  # Params that will be passes to __init__ of the logger super_gradients.common.sg_loggers.dagshub_sg_logger.DagsHubSGLogger
+                     {
+                       "dagshub_repository": "<REPO_OWNER>/<REPO_NAME>", # Optional: Your DagsHub project name, consisting of the owner name, followed by '/', and the repo name. If this is left empty, you'll be prompted in your run to fill it in manually.
+                       "log_mlflow_only": False, # Optional: Change to true to bypass logging to DVC, and log all artifacts only to MLflow  
+                       "save_checkpoints_remote": True,
+                       "save_tensorboard_remote": True,
+                       "save_logs_remote": True,
+                     }
+                   }
+```
+
+</details>
+
 <details>
 
 <summary><h3> Integration to Weights and Biases </h3></summary>    
 
 
 ```python
 from super_gradients import Trainer
@@ -541,15 +579,15 @@
                     "save_logs_remote": True
                   } 
                }
 ```
 
 </details>
 
-<details>
+<details markdown="1">
 
 <summary><h3> Integration to ClearML </h3></summary>    
 
 ```python
 from super_gradients import Trainer
 
 # create a trainer object, look the declaration for more parameters
@@ -569,51 +607,51 @@
 
   </details>
 
 
 ## Installation Methods
 __________________________________________________________________________________________________________
 ### Prerequisites
-<details>
+<details markdown="1">
 
 <summary>General requirements</summary>
 
 - Python 3.7, 3.8 or 3.9 installed.
 - 1.9.0 <= torch < 1.14 
   - https://pytorch.org/get-started/locally/
 - The python packages that are specified in requirements.txt;
 
 </details>
 
-<details>
+<details markdown="1">
 
 <summary>To train on nvidia GPUs</summary>
 
 - [Nvidia CUDA Toolkit >= 11.2](https://developer.nvidia.com/cuda-11.2.0-download-archive?target_os=Linux&target_arch=x86_64&target_distro=Ubuntu)
 - CuDNN >= 8.1.x
 - Nvidia Driver with CUDA >= 11.2 support (≥460.x)
 
 </details>
 
 ### Quick Installation
 
-<details>
+<details markdown="1">
 
 <summary>Install stable version using PyPi</summary>
 
 See in [PyPi](https://pypi.org/project/super-gradients/)
 ```bash
 pip install super-gradients
 ```
 
 That's it !
 
 </details>
 
-<details>
+<details markdown="1">
 
 <summary>Install using GitHub</summary>
 
 
 ```bash
 pip install git+https://github.com/Deci-AI/super-gradients.git@stable
 ```
@@ -697,15 +735,15 @@
 
 
 __________________________________________________________________________________________________________
 
 
 ## Documentation
 
-Check SuperGradients [Docs](https://deci-ai.github.io/super-gradients/welcome.html) for full documentation, user guide, and examples.
+Check SuperGradients [Docs](https://docs.deci.ai/super-gradients/documentation/source/welcome.html) for full documentation, user guide, and examples.
 
 ## Contributing
 
 To learn about making a contribution to SuperGradients, please see our [Contribution page](CONTRIBUTING.md).
 
 Our awesome contributors:
```

### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: super-gradients Version: 3.0.9 Summary:
-SuperGradients Home-page: https://deci-ai.github.io/super-gradients/
-welcome.html Author: Deci AI Author-email: rnd@deci.ai License: UNKNOWN
+Metadata-Version: 2.1 Name: super-gradients Version: 3.1.0 Summary:
+SuperGradients Home-page: https://docs.deci.ai/super-gradients/documentation/
+source/welcome.html Author: Deci AI Author-email: rnd@deci.ai License: UNKNOWN
 Keywords: Deci,AI,Training,Deep Learning,Computer
 Vision,PyTorch,SOTA,Recipes,Pre Trained,Models Platform: UNKNOWN Description-
 Content-Type: text/markdown Requires-Dist: torch (<1.14,>=1.9.0) Requires-Dist:
 tqdm (>=4.57.0) Requires-Dist: boto3 (>=1.17.15) Requires-Dist: jsonschema
 (>=3.2.0) Requires-Dist: Deprecated (>=1.2.11) Requires-Dist: opencv-python
 (>=4.5.1) Requires-Dist: scipy (>=1.6.1) Requires-Dist: matplotlib (>=3.3.4)
 Requires-Dist: psutil (>=5.8.0) Requires-Dist: tensorboard (>=2.4.1) Requires-
@@ -37,54 +37,58 @@
                            License â¢ Deci_Platform
 [https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue]_[https:/
  /img.shields.io/badge/pytorch-1.9%20%7C%201.10-blue]_[https://img.shields.io/
 pypi/v/super-gradients]_[https://img.shields.io/badge/pre--trained%20models-34-
 brightgreen]_[https://img.shields.io/github/v/release/Deci-AI/super-gradients]_
       [https://img.shields.io/badge/slack-community-blueviolet]_[https://
 img.shields.io/badge/license-Apache%202.0-blue]_[https://img.shields.io/badge/
-                           docs-sphinx-brightgreen]
-## Build with SuperGradients
+                           docs-mkdocs-brightgreen]
+______________________________________________________________________ ## Build
+with SuperGradients
 __________________________________________________________________________________________________________
 ### Support various computer vision tasks
   [https://github.com/Deci-AI/super-gradients/raw/master/docs/assets/SG_img/
  Segmentation 1500x900 .png] [https://github.com/Deci-AI/super-gradients/raw/
  master/docs/assets/SG_img/Object detection 1500X900.png] [https://github.com/
      Deci-AI/super-gradients/raw/master/docs/assets/SG_img/Classification
                                  1500x900.png]
-### Ready to deploy pre-trained SOTA models ```python # Load model with
-pretrained weights from super_gradients.training import models from
-super_gradients.common.object_names import Models model = models.get
-(Models.YOLOX_S, pretrained_weights="coco") ``` #### All Computer Vision Models
-- Pretrained Checkpoints can be found in the [Model Zoo](http://bit.ly/41dkt89)
-#### Classification
+### Ready to deploy pre-trained SOTA models YOLO-NAS architecture is out! The
+new YOLO-NAS delivers state-of-the-art performance with the unparalleled
+accuracy-speed performance, outperforming other models such as YOLOv5, YOLOv6,
+YOLOv7 and YOLOv8. Check it out here: [YOLO-NAS](YOLONAS.md).
+             [./documentation/source/images/yolo_nas_frontier.png]
+```python # Load model with pretrained weights from super_gradients.training
+import models from super_gradients.common.object_names import Models model =
+models.get(Models.YOLO_NAS_M, pretrained_weights="coco") ``` #### All Computer
+Vision Models - Pretrained Checkpoints can be found in the [Model Zoo](http://
+bit.ly/41dkt89) #### Classification
                [./docs/assets/SG_img/Classification@2xDark.png]
 #### Semantic Segmentation
             [./docs/assets/SG_img/Semantic Segmentation@2xDark.png]
 #### Object Detection
               [./docs/assets/SG_img/Object Detection@2xDark.png]
 ### Easy to train SOTA Models Easily load and fine-tune production-ready, pre-
 trained SOTA models that incorporate best practices and validated hyper-
 parameters for achieving best-in-class accuracy. For more information on how to
 do it go to [Getting Started](#getting-started) #### Plug and play recipes
-```python python -
-m super_gradients.examples.train_from_recipe_example.train_from_recipe
-architecture=regnetY800 dataset_interface.data_dir= ckpt_root_dir= ``` More
-example on how and why to use recipes can be found in [Recipes](#recipes) ###
-Production readiness All SuperGradients modelsâ are production ready in the
-sense that they are compatible with deployment tools such as TensorRT (Nvidia)
-and OpenVINO (Intel) and can be easily taken into production. With a few lines
-of code you can easily integrate the models into your codebase. ```python #
-Load model with pretrained weights from super_gradients.training import models
-from super_gradients.common.object_names import Models model = models.get
-(Models.YOLOX_S, pretrained_weights="coco") # Prepare model for conversion #
+```bash python -m super_gradients.train_from_recipe architecture=regnetY800
+dataset_interface.data_dir= ckpt_root_dir= ``` More example on how and why to
+use recipes can be found in [Recipes](#recipes) ### Production readiness All
+SuperGradients modelsâ are production ready in the sense that they are
+compatible with deployment tools such as TensorRT (Nvidia) and OpenVINO (Intel)
+and can be easily taken into production. With a few lines of code you can
+easily integrate the models into your codebase. ```python # Load model with
+pretrained weights from super_gradients.training import models from
+super_gradients.common.object_names import Models model = models.get
+(Models.YOLO_NAS_M, pretrained_weights="coco") # Prepare model for conversion #
 Input size is in format of [Batch x Channels x Width x Height] where 640 is the
-standart COCO dataset dimensions model.eval() model.prep_model_for_conversion
+standard COCO dataset dimensions model.eval() model.prep_model_for_conversion
 (input_size=[1, 3, 640, 640]) # Create dummy_input # Convert model to onnx
-torch.onnx.export(model, dummy_input, "yolox_s.onnx") ``` More information on
-how to take your model to production can be found in [Getting Started]
+torch.onnx.export(model, dummy_input, "yolo_nas_m.onnx") ``` More information
+on how to take your model to production can be found in [Getting Started]
 (#getting-started) notebooks ## Quick Installation
 __________________________________________________________________________________________________________
 ```bash pip install super-gradients ``` ## What's New - Version 3.0.8
 __________________________________________________________________________________________________________
 * [QAT&PTQ](https://bit.ly/41hC8uI) * [Pose estimation](http://bit.ly/3o0xHq2)
 * [New documentation](http://bit.ly/3KYVCiJ) * [New semantic segmentation
 dataset - Mapillary Vistas Dataset](https://github.com/Deci-AI/super-gradients/
@@ -111,24 +115,24 @@
 ### Start Training with Just 1 Command Line The most simple and straightforward
 way to start training SOTA performance models with SuperGradients reproducible
 recipes. Just define your dataset path and where you want your checkpoints to
 be saved and you are good to go from your terminal! Just make sure that you
 [setup your dataset](https://github.com/Deci-AI/super-gradients/blob/master/
 src/super_gradients/training/datasets/Dataset_Setup_Instructions.md) according
 to the data dir specified in the recipe. ```bash python -
-m super_gradients.examples.train_from_recipe_example.train_from_recipe --
-config-name=imagenet_regnetY architecture=regnetY800
-dataset_interface.data_dir= ckpt_root_dir= ``` ### Quickly Load Pre-Trained
-Weights for Your Desired Model with SOTA Performance Want to try our pre-
-trained models on your machine? Import SuperGradients, initialize your Trainer,
-and load your desired architecture and pre-trained weights from our [SOTA model
-zoo](http://bit.ly/41dkt89) ```python # The pretrained_weights argument will
-load a pre-trained architecture on the provided dataset import super_gradients
-model = models.get("model-name", pretrained_weights="pretrained-model-name")
-``` ### Classification #### Transfer Learning
+m super_gradients.train_from_recipe --config-name=imagenet_regnetY
+architecture=regnetY800 dataset_interface.data_dir= ckpt_root_dir= ``` ###
+Quickly Load Pre-Trained Weights for Your Desired Model with SOTA Performance
+Want to try our pre-trained models on your machine? Import SuperGradients,
+initialize your Trainer, and load your desired architecture and pre-trained
+weights from our [SOTA model zoo](http://bit.ly/41dkt89) ```python # The
+pretrained_weights argument will load a pre-trained architecture on the
+provided dataset import super_gradients model = models.get("model-name",
+pretrained_weights="pretrained-model-name") ``` ### Classification ####
+Transfer Learning
  ### Semantic Segmentation #### Quick Start
  #### Transfer Learning
  #### How to Connect Custom Dataset
  ### Object Detection #### Transfer Learning
  #### How to Connect Custom Dataset
  ### How to Predict Using Pre-trained Model #### Segmentation, Detection and
 Classification Prediction
@@ -233,14 +237,29 @@
 mode="max", patience=10, verbose=True) # define phase callbacks, they will fire
 as defined in Phase phase_callbacks = [LRSchedulerCallback
 (scheduler=rop_lr_scheduler, phase=Phase.VALIDATION_EPOCH_END,
 metric_name="Accuracy")] # create a trainer object, look the declaration for
 more parameters trainer = Trainer("experiment_name") # define phase_callbacks
 as part of the training parameters train_params = {"phase_callbacks":
 phase_callbacks} ```
+**** Integration to DagsHub ****
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/drive/11fW56pMpwOMHQSbQW6xxMRYvw1mEC-t-
+?usp=sharing) ```python from super_gradients import Trainer trainer = Trainer
+("experiment_name") model = ... training_params = { ... # Your training params
+"sg_logger": "dagshub_sg_logger", # DagsHub Logger, see class
+super_gradients.common.sg_loggers.dagshub_sg_logger.DagsHubSGLogger for details
+"sg_logger_params": # Params that will be passes to __init__ of the logger
+super_gradients.common.sg_loggers.dagshub_sg_logger.DagsHubSGLogger
+{ "dagshub_repository": "/", # Optional: Your DagsHub project name, consisting
+of the owner name, followed by '/', and the repo name. If this is left empty,
+you'll be prompted in your run to fill it in manually. "log_mlflow_only":
+False, # Optional: Change to true to bypass logging to DVC, and log all
+artifacts only to MLflow "save_checkpoints_remote": True,
+"save_tensorboard_remote": True, "save_logs_remote": True, } } ```
 **** Integration to Weights and Biases ****
 ```python from super_gradients import Trainer # create a trainer object, look
 the declaration for more parameters trainer = Trainer("experiment_name")
 train_params = { ... # training parameters "sg_logger": "wandb_sg_logger", #
 Weights&Biases Logger, see class WandBSGLogger for details "sg_logger_params":
 # paramenters that will be passes to __init__ of the logger { "project_name":
 "project_name", # W&B project name "save_checkpoints_remote": True
@@ -345,19 +364,20 @@
 master/src/super_gradients/training/datasets/segmentation_datasets/
 mapillary_dataset.py) ### Object Detection - [Coco](https://github.com/Deci-AI/
 super-gradients/blob/master/src/super_gradients/training/datasets/
 detection_datasets/coco_detection.py) - [PascalVOC 2007 & 2012](https://
 github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/
 datasets/detection_datasets/pascal_voc_detection.py)
 __________________________________________________________________________________________________________
-## Documentation Check SuperGradients [Docs](https://deci-ai.github.io/super-
-gradients/welcome.html) for full documentation, user guide, and examples. ##
-Contributing To learn about making a contribution to SuperGradients, please see
-our [Contribution page](CONTRIBUTING.md). Our awesome contributors: [https://
-contrib.rocks/image?repo=Deci-AI/super-gradients]
+## Documentation Check SuperGradients [Docs](https://docs.deci.ai/super-
+gradients/documentation/source/welcome.html) for full documentation, user
+guide, and examples. ## Contributing To learn about making a contribution to
+SuperGradients, please see our [Contribution page](CONTRIBUTING.md). Our
+awesome contributors: [https://contrib.rocks/image?repo=Deci-AI/super-
+gradients]
 Made with [contrib.rocks](https://contrib.rocks). ## Citation If you are using
 SuperGradients library or benchmarks in your research, please cite
 SuperGradients deep learning training library. ## Community If you want to be a
 part of SuperGradients growing community, hear about all the exciting news and
 updates, need help, request for advanced features, or want to file a bug or
 issue report, we would love to welcome you aboard! * Slack is the place to be
 and ask questions about SuperGradients and get support. [Click here to join our
```

## Comparing `super_gradients-3.0.9.dist-info/RECORD` & `super_gradients-3.1.0.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-super_gradients/__init__.py,sha256=e1PEJK3EaBHt27KXTY-kVQSBCVhq6e41ifYtuDk2SeE,932
+super_gradients/__init__.py,sha256=bwjT_UxykuA7BjB2FfWvbiWu6xtNB6YJXX5mqLPmp1I,711
+super_gradients/evaluate_checkpoint.py,sha256=cAB8pjlpxrpyJ2RhDp9jtV90TRvih7Axl0D2HVbfFKA,1657
+super_gradients/evaluate_from_recipe.py,sha256=aEUFWz0ue8tI55ChEivtABxUe7lhLCqT9aOywoenYfM,1807
+super_gradients/qat_from_recipe.py,sha256=Jb355vmclhurcOYN8Qgr6DFRMnnoxRB6N1uI5RLT9cM,702
 super_gradients/requirements.pro.txt,sha256=N4SNm12LMYBhOwA5ShEQlihV_6nJoveWkbEo1037idI,44
 super_gradients/requirements.txt,sha256=-hJEsVtZGOENWHmv4jiAUp-doNLwlJ_Ld4uhVULJf-U,729
-super_gradients/train_from_recipe.py,sha256=597R7Zw0-cyQA5fcuTr6r6HynEiEQnoe3ZLVXxQOkfI,654
+super_gradients/resume_experiment.py,sha256=VSmGBGaFOdz6hOTRkHm7un0MHolUk4_CvXfu2jtjGZM,537
+super_gradients/train_from_kd_recipe.py,sha256=OpRZsmleqXWQyFeaLzcnIooa_YEYEHFhkHr63Cs_QU8,693
+super_gradients/train_from_recipe.py,sha256=ZdCUpUlLPiCejcKff2FTfg33_TjZF0CwvZ-eaQlVyrA,650
 super_gradients/common/__init__.py,sha256=1F7pRDWoGs7wMWpbBw3iaTPWpeegxOroNPqUO3nzEMw,1098
-super_gradients/common/object_names.py,sha256=Upy33h3UfnvHsfdPStzcd_txUnCmymhGziN3vcFXZSc,15140
+super_gradients/common/object_names.py,sha256=si2UiliiCCsSULfT-6kBXNs98C6snrawOFlC0vPMsgU,15372
 super_gradients/common/abstractions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/abstractions/abstract_logger.py,sha256=MpEjg7PihMZb_qLBKC-R58wWFqNJdPJMlOkxEU25hCU,879
 super_gradients/common/abstractions/mute_processes.py,sha256=JxC3ofVySoiL7U7x9QYhzWLVYArkgqKQB2Kp3HyPOyE,3129
 super_gradients/common/auto_logging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/auto_logging/auto_logger.py,sha256=qH84FkmTe50L7Mg8kDjTKVHVxCsCi4DQTMV2V53jARU,4687
 super_gradients/common/auto_logging/console_logging.py,sha256=PEPSfHQ8incS13dkM9gzlWBeRdwbodo9qVqRSk32s_E,6625
 super_gradients/common/aws_connection/__init__.py,sha256=cZCFSeQHk8E6TTZHTjnAhezGATF5iSKiFR2dBof8vqg,142
@@ -28,29 +33,29 @@
 super_gradients/common/data_types/__init__.py,sha256=YfKs8C4Jtz2ZL-Y7ZKaTMKO0VSr1zWTK90CfVtgdXP4,220
 super_gradients/common/data_types/enum/__init__.py,sha256=3qhCLZTNtd5PK46HxDWRo0VDx2xX7Xo_m5TzcVQjRgQ,597
 super_gradients/common/data_types/enum/deep_learning_task.py,sha256=MEf3deKCYcmcIh88Pmc88xLj8TUU50ghN-2wGIv1AH4,309
 super_gradients/common/data_types/enum/downsample_mode.py,sha256=MAqGu6STlcSnbVw_rSJ_MMEo3LhBhhBuoocTGDrDpO0,108
 super_gradients/common/data_types/enum/evaluation_type.py,sha256=ldPEiV8I2KNR0U3dk-BC-wekGNybTWuk65RQk7qw4X0,317
 super_gradients/common/data_types/enum/multi_gpu_mode.py,sha256=CDS0_-Zp5XdgKI6ox4-GIMmK_M15d2foEb4MYY__LRU,1025
 super_gradients/common/data_types/enum/strict_load.py,sha256=9zhV8Eg75dG-Fqmn_gizLAsd4FSfxO8nWBgQArqQ9Ug,1200
-super_gradients/common/data_types/enum/upsample_mode.py,sha256=lqVfECHY40NSX_-TbFLr1wtk4oGzlbG6RJXj7Tetw9Q,160
+super_gradients/common/data_types/enum/upsample_mode.py,sha256=xXeYtdY7ybO4LJmv1L0DEAiybU_zFF6I20vHUIsgiRY,202
 super_gradients/common/decorators/__init__.py,sha256=0_l9pHZrtOWpfx6dThoLM-PBapfYr5tszzToG2sNmyU,257
 super_gradients/common/decorators/code_save_decorator.py,sha256=S5d1Jaop51HO7MtAD0dNunQKfZeY8it1-a_FR9rGJ1E,1567
 super_gradients/common/decorators/deci_logger.py,sha256=vyvodC1QCdLp_S05ELnBDnK1vCHBjtbvCsLRVnIdYHc,3663
 super_gradients/common/decorators/explicit_params_validator.py,sha256=EtW4ebI18tgPCBsA6v0Go3RY87iiqEEiQUQrujOb-y0,2921
 super_gradients/common/decorators/factory_decorator.py,sha256=PPHORVS_3fHGMqy7jbfTRwrHhDtXtHwWjR6hQe4J41s,1315
 super_gradients/common/decorators/singleton.py,sha256=6lVKPFSidDVRMOLeQ2YK-c7FRcxQEhrWU_AbuC7JXSc,1132
 super_gradients/common/environment/__init__.py,sha256=ljbYwQPDh8G0dCHjA6EGPSX5guFcsj-tUB6Ks0mHR-A,202
 super_gradients/common/environment/argparse_utils.py,sha256=c-XT11eDEZ42bWu2eKr4e6i30SF-OlM0a8xxgD08ob4,993
 super_gradients/common/environment/cfg_utils.py,sha256=_jUmcZ6HG7NK2R0H7edjNM62rDNzCTeRXBdAH2FFbq4,9170
 super_gradients/common/environment/checkpoints_dir_utils.py,sha256=UMQbSQ8tuZzYfTmwrqNef3KHElbZ3DC69B2L_hbGqNw,4218
 super_gradients/common/environment/ddp_utils.py,sha256=JMEzTKSrQ5pG9MGLd0xaIGIlg4Rlexh4soXhi0r6nzY,2682
 super_gradients/common/environment/device_utils.py,sha256=wV1pK5rjB4IShktrVdo9vx5mg_tF4XHIrRFssl2ftZA,752
 super_gradients/common/environment/env_variables.py,sha256=OxUpZ6aDt16d3rHPfw9u6wn-cmvdV4Zp67FIVc6n01c,1147
-super_gradients/common/environment/omegaconf_utils.py,sha256=4Pb6xm4LAqwiqyX_VhfIsnvCVtjI8ThLY5MhfyQzvu0,1768
+super_gradients/common/environment/omegaconf_utils.py,sha256=ycjvwGWxhhnBUwWXljqcSw-IJ8UH1BW1E3AznUSNN60,4047
 super_gradients/common/environment/path_utils.py,sha256=p6fBTLBdxdpsALaD0lanM2jEtZcbSdthuEXSoOmgT5Q,459
 super_gradients/common/environment/monitoring/__init__.py,sha256=QmJWRpVWwHOK0qjNPV6PlA5ZzKjgumxNbSoYDnhUzzo,112
 super_gradients/common/environment/monitoring/cpu.py,sha256=eGHnEDbci_jku-RTzgROxt_kPy9bUdydk_bUMin3Kxc,153
 super_gradients/common/environment/monitoring/data_models.py,sha256=t3Hky9Iu-qLKATdzyqb76j_6QxEVxamC7gnjh7Te5xk,2517
 super_gradients/common/environment/monitoring/disk.py,sha256=2XI7426eWGk_z3O_Fy_LWoVwUkLdK7ee7D8rqE6lmWE,1025
 super_gradients/common/environment/monitoring/monitoring.py,sha256=7c2anfycW-cHauTphi-ZaRH6CYVuEPLsGCbLz7BjHSQ,5427
 super_gradients/common/environment/monitoring/network.py,sha256=kfse7NZsOErzvkYmHKRbCP4g5hVW0ZNyZ0GbRTjtrw4,948
@@ -83,18 +88,19 @@
 super_gradients/common/factories/type_factory.py,sha256=HwIiWskEfoHZiEkN8batqIxATs_20TJqq8qR9W0_Has,2377
 super_gradients/common/plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/plugins/deci_client.py,sha256=CP0H4tvynauOmLOWmPLjTvu3ho-Cugu8gLhofFY08HA,10974
 super_gradients/common/registry/__init__.py,sha256=gYkyLBFQN2kIgt0YFzGJl7lXKyOHBHE67B-1_C_JS8I,271
 super_gradients/common/registry/albumentation.py,sha256=MU7ZkXX-qSM5A_2l2apl6njJECwuUn4U1bo22yovOIY,1231
 super_gradients/common/registry/registry.py,sha256=XNgmvUY3kV3oF7i-yz4aZqyoM42EG4cV_mwS1EIyNFw,6006
 super_gradients/common/registry/registry_utils.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/common/sg_loggers/__init__.py,sha256=yMh5um_t_0FsWFMDF3Gi2ncf-s-g8HcicBMw-VSTxY4,409
+super_gradients/common/sg_loggers/__init__.py,sha256=MJ9Gte7Zs_gGGge3zH7Tqv8iMm6Pic03YBHtrNqZUfc,508
 super_gradients/common/sg_loggers/abstract_sg_logger.py,sha256=OoGxOvQXwDfycg4A9wt_jgxI1zTS5XIS8GPFBQmY5rM,7355
 super_gradients/common/sg_loggers/base_sg_logger.py,sha256=W5IBmftH8M9b85t-F-mWsnRIo34_6CQ_vQd9owslUN8,14980
 super_gradients/common/sg_loggers/clearml_sg_logger.py,sha256=BWAJzubNT974xgcsOVckRsU8KLsYW2NLJ5x65tCeQ6w,10055
+super_gradients/common/sg_loggers/dagshub_sg_logger.py,sha256=H0DJKzKQoL3ooXWvvx3fnidRTkuhTcL7tzQ5-mW9TaI,10103
 super_gradients/common/sg_loggers/deci_platform_sg_logger.py,sha256=XLanzH_CwW4Nw6Mx-m4tS6rFkDH3xZ9P8rCIyYIxoGs,6618
 super_gradients/common/sg_loggers/wandb_sg_logger.py,sha256=DnGC3OmBcMSpK_wQ00KW0e7SLsgZ9vhDbhNhJYHRAtE,13073
 super_gradients/examples/SG_Walkthrough.ipynb,sha256=bhJ62ERSAchiroY49KiQiycgyDjlgPgHeXLwcZdUuNY,85509
 super_gradients/examples/SG_quickstart_classification.ipynb,sha256=aMGQCqFss-flEKvUaVj5WiKStr0S8TRKUsHwoyFcuko,69618
 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb,sha256=M9YZY9VpKJNFHxBz-IGSRvdAACQJ1n-wTQgWSpZVW78,54966
 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb,sha256=Gyx6LjKAwHwUdJsGiSiBn-AdbcgTdpD2DvRWB7IaGYk,65090
 super_gradients/examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -105,100 +111,108 @@
 super_gradients/examples/ddrnet_imagenet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/ddrnet_imagenet/ddrnet_classification_example.py,sha256=K0p9d0iJFpGTGqYXjxaODIoTH6MZeGOJLMeqJK8B0JA,3114
 super_gradients/examples/deci_lab_export_example/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py,sha256=k7XkE--u_YOQrGmaowbWRjbceX6BHbI9QysMwKtKiHE,3562
 super_gradients/examples/early_stop/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/early_stop/early_stop_example.py,sha256=QH3mQGObo3BmkZ7EQ394eDVmaABMmtEy3n9A51DfaOk,1596
 super_gradients/examples/evaluate_checkpoint_example/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py,sha256=230V4BkF2hNWUpWFV22ZuZGCK3-Nigp76YK6sHeT9ro,1683
+super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py,sha256=MNCuzc90O3d0TSVsFJZUSZQt-8V903pSHNUD7CdJ5Xo,289
 super_gradients/examples/evaluate_from_recipe_example/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py,sha256=AY-hADprZZMpGNE4KILMez6tqaL3qELOg1RhWcvt4qc,1779
+super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py,sha256=IipK4OmfwP77IaGpnhOaiHdzY9sE0KF3WZJ58ZtFLHU,292
 super_gradients/examples/loggers_examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/loggers_examples/clearml_logger_example.py,sha256=1lkEBZtjKUMV3UAHQwMmd0olWdSlDS7JFO4K07GssQo,1206
 super_gradients/examples/loggers_examples/deci_platform_logger_example.py,sha256=9aWl9ZLbk6LGxtYrYcC3pUgvBUcLmh6qQTIHD92G5yg,1088
 super_gradients/examples/qat_from_recipe_example/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py,sha256=4Q9MnoBKjG-GOjROzP4OR9qfTV2dDWmKfiX_x2Wy7Mc,700
+super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py,sha256=ZCs42MTAuOfSKox0-q_qV9NezcZ7R61gBq6igzWp9u0,277
 super_gradients/examples/quantization/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/quantization/non_default_calibrators_example.py,sha256=itD6V_aLhWtwcZHb7gRHHw8dN-DmASWuMVYU7n3OU_Q,1104
 super_gradients/examples/quantization/ptq_e2e_example.py,sha256=GUg5hEkAypTB-jeNpv55OxAWW2SAmYzraYN5pTPR4f8,2310
 super_gradients/examples/quantization/register_quantization_mapping_with_decorator_example.py,sha256=pknDBKiydxjqVeorTv4xIECW4h2uj0cSKIXdxwPBq7U,1850
-super_gradients/examples/quantization/resnet_qat_example.py,sha256=1lUE4UXyeSXah79d55nRjKNlPqu7BFP5hDTFJikAsq0,4923
+super_gradients/examples/quantization/resnet_qat_example.py,sha256=RRU1HOnK5xNnfCroX_hvrMDt_SEvPYA9XmX0CDYEwI0,4732
 super_gradients/examples/quantization/skipping_quantization_example.py,sha256=GB-W-DtcqGnHn6vfkjxkLqoirF7xuco2Tx3ew92kWJI,1163
 super_gradients/examples/quantization/vanilla_quantize_all_example.py,sha256=IiqMO9SOcj0AZ6LICeNsBUi6KHMB1AVep0mPb8OmiXI,832
 super_gradients/examples/regseg_transfer_learning_example/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/regseg_transfer_learning_example/regseg_transfer_learning_example.py,sha256=TT_Z20LiPsBe6mZ-XWaWiVp1_gnFRcao36T2pRg_bdA,2379
 super_gradients/examples/resume_experiment_example/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/examples/resume_experiment_example/resume_experiment.py,sha256=wavFHdyscGCHMrmdV6rfKKxRsS3brPVqotRxmG-NQ-E,534
+super_gradients/examples/resume_experiment_example/resume_experiment.py,sha256=Vc03F8IFs9mpisUVn3KJA8IlGiSFl5EXKESbFZD8w6U,283
 super_gradients/examples/train_from_kd_recipe_example/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py,sha256=5aKLAkw1WxKDMwKHKbZ-3PgwDlO2MTh7Ou1tGeXBPEs,655
+super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py,sha256=h7mpAjiBX-dXNwmN6Wq-HrmDCMiZ9VSSx-HxjuYKcNk,292
 super_gradients/examples/train_from_recipe_example/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/examples/train_from_recipe_example/train_from_recipe.py,sha256=l-PwJ3GKaKcnYIbTVdVL811-diMyYdcoY4HxoO9jb60,627
+super_gradients/examples/train_from_recipe_example/train_from_recipe.py,sha256=_BRwyPyR_y-uD47u7fpU0oKw4rUAINwKGqHG1qnBlWg,283
 super_gradients/examples/train_from_recipe_with_dataset_registry/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/train_from_recipe_with_dataset_registry/train.py,sha256=wRiGIkRqoD3HRTQt4hBxWMp97EQrF50aqT1Jct_Wtrk,1334
 super_gradients/examples/train_from_recipe_with_dataset_registry/user_dataset.py,sha256=fJscmGOW90V-4x3MshgVcfrez7_XThZnOoec6W2J-QM,1643
 super_gradients/examples/train_from_recipe_with_user_objects/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/train_from_recipe_with_user_objects/train.py,sha256=MX3SCfca8NLmiiHv7iO1GUKA8fgy5fCLk6tN93kH8vY,1326
 super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py,sha256=vX_3SS6ZVmUVbBA62L7tx6FamPnPN66PRoh8NNeXw-Y,2548
-super_gradients/module_interfaces/__init__.py,sha256=T2XfJNfNnFl5cuqk3picDTlOevEErG_6fUKyrjoTRFE,118
-super_gradients/module_interfaces/module_interfaces.py,sha256=VV-G11F_mcG29TzjUcpbuMUDq6yv-XVjn6ClClap_W4,958
-super_gradients/modules/__init__.py,sha256=TsT-xloLimGBxiwiVkqeX5YVesJq2zCacDxGl_RghwU,2589
+super_gradients/module_interfaces/__init__.py,sha256=fi4Bsu9QUF29TqqSE-P1GaKsKsOqxA1MJVEDQT7mMeg,174
+super_gradients/module_interfaces/module_interfaces.py,sha256=qck4ChG35StWJrzNPC4u56yARs4eTW4z23oqsDQU__s,2043
+super_gradients/modules/__init__.py,sha256=T0iXFUqVikChMnto7C8yva1q_M8OUwUiyH759b-oqrc,3366
 super_gradients/modules/all_detection_modules.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/modules/anti_alias.py,sha256=Qi4RW9_TuuJMtNV2sHfHfp0BLMMA0BgeTZcn9k6pXz4,617
-super_gradients/modules/conv_bn_act_block.py,sha256=jsV1AV-HcdErb8PV4ZG63CtumfJrpI7Xjw4DhY7KnOU,2073
+super_gradients/modules/base_modules.py,sha256=OhcjlGzj6vKjQkxQP40A2C535ScwVo9eU5DiQGrEB2I,776
+super_gradients/modules/conv_bn_act_block.py,sha256=uJgtSZbW_km3zvlS9hh2PzxgmHjeiINtNEC9RlffD6Y,3054
 super_gradients/modules/conv_bn_relu_block.py,sha256=pZ0OazMsoP7PxjV6-ltgR8IytjsF6tsC71GH4kRgEgE,1976
-super_gradients/modules/detection_modules.py,sha256=F8qgnSt-yAEk2i1xFimdCNc6PpvSo47AWczPyGlQEso,15129
+super_gradients/modules/detection_modules.py,sha256=srfbJXd4tWk4UL92Wu2Lq2l6qI3YvzSP_Khjtsn9fS0,14805
+super_gradients/modules/head_replacement_utils.py,sha256=sDXb1CiJN08-mpjrdzyY46s_FEG72yFx2YsF2Rl22Xw,2143
 super_gradients/modules/multi_output_modules.py,sha256=YLofR05Z56k4iHM460KRO-GQ4jMcP1MrrrgT-aOcew4,4362
-super_gradients/modules/pose_estimation_modules.py,sha256=ZBk-C40x87kG_ywfM8nN14MLXgD5pASsm3_LL2xpM7U,3958
+super_gradients/modules/pixel_shuffle.py,sha256=Rcka24mhF8fR5OuG3jgIGV1yUllaEOWZU4qFjKMheIg,860
+super_gradients/modules/pose_estimation_modules.py,sha256=PjYY28XkAz52KgREnCupoIbCCFM6TBYu1Shudmq7xxs,3953
 super_gradients/modules/qarepvgg_block.py,sha256=Ou0FbQGC4OfmGjRb7GN0fnhvg4Ib7bavlG4YhUTRjOM,11642
 super_gradients/modules/repvgg_block.py,sha256=uT107B_lO09aeqvg0z9uDeR3c-tmyvNqJEdVmWtV1cw,8544
-super_gradients/modules/sampling.py,sha256=V-_AQa5so8xyX8_CC-hXm2NNY45rjYbVmGEJuyG2Yfw,1887
+super_gradients/modules/sampling.py,sha256=xcGx0oIvQGyPjtZFGQko_vybYYtQk-mL2AFA0G4MULs,2138
 super_gradients/modules/se_blocks.py,sha256=itIUGGoqKNBYhAyj20aKcRKQlK_HdD0sqCsfK-a8yE4,1459
 super_gradients/modules/skip_connections.py,sha256=QR1V7AG9_4eK3xgywanDU4NpK5HMiv_jy2AMOgH0di4,1403
-super_gradients/modules/utils.py,sha256=GLEfooz4eyfw1Mx2gXb1kPXBPJd9HVgKrpCJNq3G1pU,2565
+super_gradients/modules/utils.py,sha256=B3h8_ABd15fS6yaozvG7xsAc0VfuDNmGBKm3ty-Yejg,2968
 super_gradients/modules/quantization/__init__.py,sha256=YNuNoitnDrNS30BBeadjiGZfqOTdZu_GPTbiHyLmPV4,716
 super_gradients/modules/quantization/quantized_skip_connections.py,sha256=0NaQ63tdFC9s7YL1VV9VLheUYaN4pb29kjw_etmzR_g,2649
 super_gradients/modules/quantization/quantized_stdc_blocks.py,sha256=aahisE-qutTEnfVH2rfRKhUYEKssuTJTPnuBIq7lYHY,4604
 super_gradients/modules/quantization/resnet_bottleneck.py,sha256=QxcKN-ogzI1lDD8EeYjD006mCNouFfyekLvIjnhnffs,1281
 super_gradients/recipes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/recipes/cifar10_resnet.yaml,sha256=M4RO1pDcd27U2NbPvJCWXQJiIbaUTAJGoh7RBSZYBbc,1516
-super_gradients/recipes/cityscapes_ddrnet.yaml,sha256=aacRQxOIDMUJl97XtBFutzGz1r-8qI78BXB2wlMionI,3856
-super_gradients/recipes/cityscapes_kd_base.yaml,sha256=6Py8Oc2VnxzIvDyZJWA7nRugMmgrBQ_xvB9C2rEyXvQ,4072
-super_gradients/recipes/cityscapes_pplite_seg50.yaml,sha256=Nfx-C6nJYcLVm7TLDPk1C2nPljY0lseW1yLWIyliXOI,3615
-super_gradients/recipes/cityscapes_pplite_seg75.yaml,sha256=l0Oyy3qSLPSutlwyjlwJtWGSBxSVt1R8-OG0fPCEYVA,3514
-super_gradients/recipes/cityscapes_regseg48.yaml,sha256=rbcNThYt8YqWbnjT69H0g-JfU-MYVyswny7McAMIh0c,2771
-super_gradients/recipes/cityscapes_segformer.yaml,sha256=7G29cYeKoIOFP0mUDmyV5XR8-gYul9Br8vNqAL-UWF4,4293
-super_gradients/recipes/cityscapes_stdc_base.yaml,sha256=4HtapSi082EfOsufJTToCFu-dPLoE3UGeN6j1UeUWcI,852
-super_gradients/recipes/cityscapes_stdc_seg50.yaml,sha256=DyLzvIRUwemcq2e1ZrVDEcRTILZ2X-PwgOaXgjXLk2E,3175
-super_gradients/recipes/cityscapes_stdc_seg75.yaml,sha256=i1IREG_2l_PQHWs_HgoG4ylSLV6mzHgY2BxdMlGbbLs,3369
-super_gradients/recipes/coco2017_pose_ddrnet39.yaml,sha256=HmQhrTODv7zMI_9qbmL42UBskAGKUQFQGheI0QGse5Q,2063
-super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml,sha256=wn1oRekmwMfclrg3wtqFbUPD28iah_GeS1SsupiKaTU,3821
-super_gradients/recipes/coco2017_pose_pppose_l.yaml,sha256=8cmmkZ-t-P8Tgv3-ZlbnvSCcy3mEcfDEm8AoEBycDsQ,2231
-super_gradients/recipes/coco2017_ppyoloe_l.yaml,sha256=-syEeGFn4GZS9h78I8-uBvHA_ryC9dhtrQt3qdgwnfU,2388
-super_gradients/recipes/coco2017_ppyoloe_m.yaml,sha256=jUz4dwIHVYj_LZvFOcQ_2pX4sWKZhDATWUCRmRivn9o,2388
-super_gradients/recipes/coco2017_ppyoloe_s.yaml,sha256=CeOn4qY0Y5NEf1GuePK0ZdVGase7m_1DxBWUkO65kn0,2274
-super_gradients/recipes/coco2017_ppyoloe_x.yaml,sha256=TGCW7-zRtERucnF0LMVOo0j1_8a_GVHz5IkPWE77V0s,2367
-super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml,sha256=vL2fNQuU6hRMl5hSNIe2U4mAOsjzzKyPnQcAldJqc04,2202
-super_gradients/recipes/coco2017_yolox.yaml,sha256=Vw_b9bzaPYDmx9Evbkkjg0gAyYWwlplx7bkLuVCfu6w,3053
-super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml,sha256=iV5n40o04ks8OPVJRORJhMQXnDJjD__7j_YP9mpFJrc,1649
-super_gradients/recipes/imagenet_efficientnet.yaml,sha256=ICrko3vilYUIMNiMPnXHehStViyLi19M2gESofht2sk,1418
-super_gradients/recipes/imagenet_mobilenetv2.yaml,sha256=VvEt1oTsL7zyIPjDZYJ0nZfgbmsCllZHZ4gIiANINlI,1402
-super_gradients/recipes/imagenet_mobilenetv3_base.yaml,sha256=jyeAtC64aGwDTrpR7V3JpkjvJH7XNweCSN3ThIKuNQI,741
-super_gradients/recipes/imagenet_mobilenetv3_large.yaml,sha256=fEjpcwR_g4i72vMlH1rF6nj8xPseZXANnn1rIr4cMxA,992
-super_gradients/recipes/imagenet_mobilenetv3_small.yaml,sha256=d5MyAZJHe_EOcHDfIH25MOzsL163Sfqhj_XUEoP6BJI,992
-super_gradients/recipes/imagenet_regnetY.yaml,sha256=RXCCk8__OR891tRH2UdeZ9qCLTCPLG7nNM6W7zXPZYI,2387
-super_gradients/recipes/imagenet_repvgg.yaml,sha256=ghGo2YoP5VzmW7fw9ouLKK1VkYmM4KcOD0EfWpcd-iU,1519
-super_gradients/recipes/imagenet_resnet50.yaml,sha256=xB7uBvqcLujZ5j4ZNbgEgSM7I5LjM7ahaE1jz_I7hh8,1442
-super_gradients/recipes/imagenet_resnet50_kd.yaml,sha256=-Hz22cJysjIJmOjyOB6dK5rklXQXFoKxlfS4V4qmiUY,2998
-super_gradients/recipes/imagenet_vit_base.yaml,sha256=V4xwcPI_1uDQDqIraN5TQZMMSQB5q_VeoVaXrHGLCqU,1409
-super_gradients/recipes/imagenet_vit_large.yaml,sha256=l_MkDxYYWmjN6a1Rs6LwYMAWfUj2yxfPYlOjGrbtP9w,1283
-super_gradients/recipes/roboflow_ppyoloe.yaml,sha256=gJMGuCgFU7UeARh8iE5YSadZmmO2Hh0_I90ZvXSRbh0,2226
-super_gradients/recipes/roboflow_yolox.yaml,sha256=igSc1HUa6plUIRTQg46mz4nfr0mFxHfzQ3B6415MvdA,2134
-super_gradients/recipes/supervisely_unet.yaml,sha256=GwBvE2vvOmdgpLr1bka3_83jQCi2ug8rzyjINKhYUr0,1520
-super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml,sha256=0qDPTZn_TfM5uFBpw5HawJ947223y8oBqH6wU96XRRc,1906
-super_gradients/recipes/user_recipe_mnist_example.yaml,sha256=RZ_Ja8ZKACL1xgoredVAd3LG33KJDJhTVfJyfELY_E4,2367
+super_gradients/recipes/cifar10_resnet.yaml,sha256=iwUtqtF5OU3Hm59HTZUGa6sw6bUmNYdV6HWsr5PJ7kA,1136
+super_gradients/recipes/cityscapes_ddrnet.yaml,sha256=vPqkLwq9wpdXDqI7EUyPWgsUjjdK_k4Qckvj-jjErsE,3502
+super_gradients/recipes/cityscapes_kd_base.yaml,sha256=xOLxh4xcZigl6b1tQMV_IgMV37q6sKbo5j6RNxHbx9o,3754
+super_gradients/recipes/cityscapes_pplite_seg50.yaml,sha256=_iADDPmvD18DzmbgTMp-r2n3DFt3pJer7FFG4i_MOok,3354
+super_gradients/recipes/cityscapes_pplite_seg75.yaml,sha256=febqi42cSfZ4om7H0lRh2Ow8W1wxIbobcUWbiQt4t_8,3253
+super_gradients/recipes/cityscapes_regseg48.yaml,sha256=4PryJjKoJThIUZpsjesGr69i0fAThS3JDBBjYfQ-raA,2498
+super_gradients/recipes/cityscapes_segformer.yaml,sha256=DFy2Ir5L0NsB8zG1QD4FevUzVRDCQmTUmGu0M4XSQto,4020
+super_gradients/recipes/cityscapes_stdc_base.yaml,sha256=FwZUsUiS75o2RTauG-r1LEVB8I7xYJhKr_0fJhUh4Vs,618
+super_gradients/recipes/cityscapes_stdc_seg50.yaml,sha256=lCxKTpftQbIwz00q3t6Tukl2hALIny8hkrAB4KJkAqQ,2862
+super_gradients/recipes/cityscapes_stdc_seg75.yaml,sha256=s3H7De5muLfu6kNjRbAOccF2_mHkch98HppPnDmSNig,3055
+super_gradients/recipes/coco2017_pose_ddrnet39.yaml,sha256=sfAmnASFeFoS0QQI-ou9BnsxjOP2xSvfslG9HdfWQQM,1830
+super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml,sha256=cOdwPOV46ISu8fEI690_nO0gsbgTwFqb5Z6lpUfzrEA,3549
+super_gradients/recipes/coco2017_pose_pppose_l.yaml,sha256=r3Y_9Mat5vsmQ4_Aq4sUz37rGuGe6ydHcwOo3H8O0-c,1998
+super_gradients/recipes/coco2017_ppyoloe_l.yaml,sha256=bW0yA0E4P91lqF3-9G-dQfVB3GZNaI40okJtgZ-F7O4,1996
+super_gradients/recipes/coco2017_ppyoloe_m.yaml,sha256=HV8O7WVRjgz33aD62zYPIBOErNW1sbSEMyusQoy7QkQ,1996
+super_gradients/recipes/coco2017_ppyoloe_s.yaml,sha256=a9LHnLPYKntNr50nZaNw6DAhBMOpqUrgjYdsjv_tNR0,1882
+super_gradients/recipes/coco2017_ppyoloe_x.yaml,sha256=9FfoIZzlzCjvzeif8N6Vr90IRclWzfE1V6i4p_3voDk,1975
+super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml,sha256=xbz3qng4_jBT0YeBImpmSWoXwYGY2X0USbfFRaArNOY,1889
+super_gradients/recipes/coco2017_yolo_nas_s.yaml,sha256=2_FpHOih3btRm7gX7Hok2W1ItpokXxTUHh6fp8b6yZI,1385
+super_gradients/recipes/coco2017_yolox.yaml,sha256=pLonL8nqJ87OAwNkbTP1VtPDlRN_4x1JbZ0z1INVPKs,2583
+super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml,sha256=Lilr6pfmnzAWRmGdyt545iTTdTYx8704dmoGgERA4u4,1376
+super_gradients/recipes/imagenet_efficientnet.yaml,sha256=VyQCb9nkNCeGPNMnON3VfuUaGwnPjz-H37W5hXBd6qA,1145
+super_gradients/recipes/imagenet_mobilenetv2.yaml,sha256=fMrslHFs_egdEJG86BFoxRom4bLJfScGfSmWhtwfV_M,1129
+super_gradients/recipes/imagenet_mobilenetv3_base.yaml,sha256=TdKEVG74r-egKhsh3Szo-j4E28XuV6x9J1HiylEz2H0,507
+super_gradients/recipes/imagenet_mobilenetv3_large.yaml,sha256=2P3tQiRWASLaANU6Dy7wPsgq7D_OaFAtfmIVblJOSKw,719
+super_gradients/recipes/imagenet_mobilenetv3_small.yaml,sha256=WI-lPLBp2R5vfXjm4Fg2l6CN6VmKfNakVZ8fQ3nut_4,719
+super_gradients/recipes/imagenet_regnetY.yaml,sha256=aBIgDkMzH25FzG6j7K5sIRydpW0u6u5ji9lcexRGjzY,1997
+super_gradients/recipes/imagenet_repvgg.yaml,sha256=awLg4Q4AzEgWiFc_o1NiQonAAC3W0Af-6caBZSGqGt4,1246
+super_gradients/recipes/imagenet_resnet50.yaml,sha256=nPaWJhY1GKn57rhLM5ulGkig3zDbntL9072lxqiOHno,1169
+super_gradients/recipes/imagenet_resnet50_kd.yaml,sha256=JuVQSpPYHuKfggQpdXXBEEKZhFMwBQf3W0ima5TO414,2722
+super_gradients/recipes/imagenet_vit_base.yaml,sha256=dnvr4h7-d1XHhF09Q9dZWoNLGZvdCZZys32siTH1Ta8,1136
+super_gradients/recipes/imagenet_vit_large.yaml,sha256=QuI6OVc5XAUcIUsOfnFpcO76jZ79HMhhwnk8Aq_azaU,1010
+super_gradients/recipes/roboflow_ppyoloe.yaml,sha256=ukl-e8Qze0hZ-ENcD93PTql5xaNHtcVIItzDJF3yGWI,2007
+super_gradients/recipes/roboflow_yolo_nas_m.yaml,sha256=qpOIQmV3mwelxK5Xn8RXPFhE6Cb2dlIPm42WlvP-eok,2347
+super_gradients/recipes/roboflow_yolo_nas_s.yaml,sha256=Gj1L8Ky92PcX8pQ5wKKgc353HGzJYun4xuoQkMgGfpk,2347
+super_gradients/recipes/roboflow_yolo_nas_s_qat.yaml,sha256=-zTGn37Y59d_9_z4HSsNfcEZ7eNr8j4Zi-VAv3-l3so,473
+super_gradients/recipes/roboflow_yolox.yaml,sha256=d6Y-nv_7p9SX63d8kJ1oiPS-U6Znu6DLye5IvIP9ypk,1915
+super_gradients/recipes/supervisely_unet.yaml,sha256=L1bl1QsgThj9iv5dEZSSGMBYFR1SmW9Mgr7cddaXOoE,1246
+super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml,sha256=XR86Cg1sGjgoT8RHjdpnhJA01tFXYTz3QqiLYmLO46E,1672
+super_gradients/recipes/user_recipe_mnist_example.yaml,sha256=JtzZebnnTPGQUgsqu6i73zb5uF0l6_LPNnuh2q3UYD4,2133
+super_gradients/recipes/variable_setup.yaml,sha256=189UzdcCcHLw37-W1XF0W-j1k80IGMcMd8JkHwBXI9E,2000
 super_gradients/recipes/anchors/ssd_anchors.yaml,sha256=iRsfDXt3bWyCvmZtOQK-Y2maAJEgfgXVWF5sos6r7RU,2222
 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml,sha256=dEn_jgEn_NA80xaugB6lY1mdRRjVcOTwnckMlVmdbXE,563
 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml,sha256=jQfnMGb1kcprnr6UnUbmYaNwslEn728j-8Ci5NpX63E,104
 super_gradients/recipes/arch_params/efficientnet_b1_arch_params.yaml,sha256=An9tm3_3uLY6veIA23sp9SoZDapgVZ-q2hH9XgdUThw,103
 super_gradients/recipes/arch_params/efficientnet_b2_arch_params.yaml,sha256=6asWEU3JwI62-m8wcoArJlQEOl0_kDZBU4md0G4kpXs,103
 super_gradients/recipes/arch_params/efficientnet_b3_arch_params.yaml,sha256=RnaEhzycWnm3-RgR9yAii0IQr5ka6DkYZCyJZbUe8Oo,103
 super_gradients/recipes/arch_params/efficientnet_b4_arch_params.yaml,sha256=lZB_5AwQxD-WibrQPRYWsYfs6sIpIlxHLJgHXByO6Rs,103
@@ -229,17 +243,20 @@
 super_gradients/recipes/arch_params/repvggb2_arch_params.yaml,sha256=d4ypbSJhfb4m_9PDvSsXXKBC0DO1okmklDojurpYVOc,92
 super_gradients/recipes/arch_params/resnet18_cifar_arch_params.yaml,sha256=xxsFVbQl1tPsOZZQ5C41mMOIcH7Fc5z9-f60a84ZmpI,15
 super_gradients/recipes/arch_params/resnet50_arch_params.yaml,sha256=IY_Ky1W1tSZqkFfii6PBs2YvWMjstOVKHmdS51_pqUM,17
 super_gradients/recipes/arch_params/shelfnet34_lw_arch_params.yaml,sha256=DIfTJiaYSnb9HiQ67sV4I0TRRz3bGjUIif3Enm5fmC0,32
 super_gradients/recipes/arch_params/ssd_lite_mobilenetv2_arch_params.yaml,sha256=mgc7pa4Do5BNpjklXwH5zYPPw9_fGU_U2O8CzT8Md_8,655
 super_gradients/recipes/arch_params/ssd_mobilenetv1_arch_params.yaml,sha256=HiuGU1M0fDqQVVJWkx5VpZJaO4XYShwQyzpPxqJO0Oo,605
 super_gradients/recipes/arch_params/unet_arch_params.yaml,sha256=U-7HSXzOXXr2-d6xQjNJF-8oD1KLhD1WqqaThI0atUk,1369
-super_gradients/recipes/arch_params/unet_default_arch_params.yaml,sha256=w8lhI0_oNU4wpBs3qcKf79yW2G1i8XLeFl9MT7Qrkno,3014
+super_gradients/recipes/arch_params/unet_default_arch_params.yaml,sha256=ONkf6v0Msq4b9Ucxkv3TZWgW_RXmvhomkmo_5HeXzaY,3031
 super_gradients/recipes/arch_params/vit_base_arch_params.yaml,sha256=Y6skbVr98NRSf5Ts4c47JPwsDMudqygFu5W4ZQiXkLo,63
 super_gradients/recipes/arch_params/yolo_arch_params.yaml,sha256=GroGr-T0l_puiM3nPIT3Y_RzuwhNrv3U5s4g5y1Pijo,2393
+super_gradients/recipes/arch_params/yolo_nas_l_arch_params.yaml,sha256=yYHct24_5vEwR4XuZwxhuSqMn3tZGV70NiIKiR8gaW4,2337
+super_gradients/recipes/arch_params/yolo_nas_m_arch_params.yaml,sha256=83LcAgVeVv1PZjf3_fOOs4b27Y0PUpoHT2zLWBZCCWA,2346
+super_gradients/recipes/arch_params/yolo_nas_s_arch_params.yaml,sha256=IGC8VN-OuFCasSMUTEOKoukSQDt6N_-b9VUrc7mVZNU,2341
 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml,sha256=lmtcOUvHlhQf9anw1ybaks25GETvHu2QpH2D9jJqEUg,235
 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml,sha256=atByNWwQqnpaZ7SXEW2Q5cKo0T99V447xLhh1NoShFs,237
 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml,sha256=1yJcwDkZwKlL_6MeWjyypFtsPyyC9CdNWquRG7gQoXI,237
 super_gradients/recipes/arch_params/yolox_s_arch_params.yaml,sha256=J2qgjwp6VxRcNsRomCyZtdV5Ht3RruMZmYJagtlzttU,237
 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml,sha256=rxYvMOUeT5jnGhZ9-OTZ4ohHgheLDdHyNJ4_-m6JSQU,229
 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml,sha256=Wsg5AnPiqHZTnbTLFGUr90eS5a45F9ko0dfT8XTZbPQ,228
 super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml,sha256=XpQsqckADGZgsZHxW6bc0vF971bRz0kpyuP_1dH6aRI,611
@@ -254,17 +271,18 @@
 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml,sha256=HUr8IaV0IIfuxK-fibY42yKUHe04kUCBFnYAE5E3rGI,525
 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml,sha256=CKSennwvRG1a-swVvL1he18vdtNRnCStH3LFhruGSnQ,706
 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml,sha256=dtbvoxt9IR9cBaslNOWCcsX7s_gjHRnWK5Ayl1ElzmI,644
 super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml,sha256=i7l9LXea216Y2RB8e3FxhlGNBR_a1tLJKCg2Ix8JsTI,721
 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml,sha256=WK7UH73r-nuHMKepBVyykR0tf306s-P5NgQNGI-dZWk,709
 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml,sha256=wBHhYk6Q6kdmLDk9tTi0vpREr0fhTz4r1Zh0ybrRPGw,708
 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml,sha256=x8wk7EC6eKGlxSyaBTxKGJidss5BbgX1MTG9KLCnU0M,3946
-super_gradients/recipes/dataset_params/coco_detection_deci_yolo_dataset_params.yaml,sha256=S7uKClewyJSp-NJn7oOWfM583KpfpRwSNYod_pz2Fcs,3661
 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml,sha256=GeCdBxnGf5WqQ165WIVCg4jz4vmjqT2LzofdvXB6bAs,4202
 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml,sha256=PqQ6fBINO3sHHAAGx4rHKz4PAURkd67qPrVLWu1WM5Y,3590
+super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml,sha256=kbFd4bvfi8bhpX1qALfyjLZ3At9eHdC0J80w-a3OUkM,5568
+super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml,sha256=un_vfACn98dmTwPXS1AlpC6I3uRnZKTlE4MbZUGITsY,3646
 super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml,sha256=qHBh-kCmrXr5ICR0Ww_C1B2RywSEOz4nVSZSt96K-aU,2461
 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml,sha256=q8s65W76DEu9XWRY_gR9fyr5Xp5HH1vLh8eG9ZvR7fA,405
 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml,sha256=SC_nc2CyZqQ7R-z4pcqoTyZlBZB7JlmT_5hzgMjHCRc,1466
 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml,sha256=9JnbyZjCkZ3ZdMHj0CwVkQdzi7QBevwmoK1KQlxlymU,931
 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml,sha256=CILfhTGk4ne0wk0L7gbD95EjBTKGGTR8UjCaTW79Joc,732
 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml,sha256=lp64i0smov-lT6Xko9-fzVsxWO0UWdimXQnwrx0D3sY,794
 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml,sha256=YH7UxRgDjcR3qWs0yifxlgHsckHRqEYWx-kYRwNhPVo,142
@@ -272,23 +290,24 @@
 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml,sha256=SiPRDxzkwoOMDtKqzM7p0c5M658dQNEMQRvFH24K3aA,1059
 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml,sha256=C5-HGDjjDbnDWy43zM5byBmZicVqey-YQdoTkqKA7nw,1093
 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml,sha256=YvXeTTMlK8hEOu6HoedazdFtkk81icNHBg81yNGKmSw,845
 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml,sha256=mgexC2b4s-uabJsT2v51GdifhDg67WZfnexTMo-_NTY,1762
 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml,sha256=KzOrZe-NRkZ3XGkixGkUTA6Pd9aO2fTtnIhpaQOdIvU,149
 super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml,sha256=exEzH6LsS7KdvC975vG7TiA5byADG4YSfLUpCss58uI,1571
 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml,sha256=eIHwt4ZsVYKtpQbNSk1ZbsdneEZ6twlZkpxVG9LLt84,1414
-super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml,sha256=M6x8EzF8yDIKZ8ifPX11OmA_DAtbIQLimKxaRZRZ8R0,3398
+super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml,sha256=k9D4xbYMsuJv88r6m7MOeB3vQ37sUSnD94BQMMMExSM,4112
 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml,sha256=GshRG6Jqdb1S9uoBjWbckkSajIPo6Avuf46WXFMcC5w,961
 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml,sha256=4_4HkNjzZDKFHpgSV1-S0s9rRrZJUj5S-7zUk1wOFaY,559
 super_gradients/recipes/quantization_params/default_quantization_params.yaml,sha256=OVewy7FMpSUpheoL7_eAzbJVpcfy5O2eIwpEri0tUc8,1155
 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml,sha256=jZV1VVe3Lda96Mq-hb8zHfR3EATHt0kSGLOpcdxssFg,591
 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml,sha256=NUOLRusDJ9H6Nxp-NGVsie7tPuRXKE493jwzI_U8rqE,700
 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml,sha256=vh7Ej8ViU6qH7B87femqWgoxkE2WYxYhTFNsR-8JzK0,877
 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml,sha256=Ah9iuCKngV2Bri_R0PPB-p5SB0oPpVYGs38yG83X-kU,1302
 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml,sha256=vuTXdVTzwM52w1n44mGBB-kJKluXtmxymgmbdLg85Jw,723
+super_gradients/recipes/training_hyperparams/coco2017_yolo_nas_train_params.yaml,sha256=wjpqncCxlCxTg2zH30OoqqdctXYcoWz8nDOkD7DPTyM,1121
 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml,sha256=hMDTZejrlTXQxuSJPXyW6jdxTrd5De5IoilzpP-Fmis,956
 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml,sha256=4k8cytIVPZH37ALyCqhziIA9i8HDrSwyvK1nrk1et8w,461
 super_gradients/recipes/training_hyperparams/default_train_params.yaml,sha256=ZR6x6QR1Bc0YGwj-dKPITmxM7Qkava0du6RGhUC8n4s,5459
 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml,sha256=ueqNFnlvkCj78yA70mPDPp0n6AcikQkfCl35XLLE12c,794
 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml,sha256=xrCPTtKoJ85TjCART4sOLWMc7b5p2X2ZARt41WYScj0,742
 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml,sha256=xLXjLxQUyh6RJzBEtvrBPhKRAZre7OuVSZyAvErk3XA,549
 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml,sha256=A5j4hUflhQHwIPR8awxs64GuEH3AAFJbWT-Wo3g_nAs,795
@@ -297,17 +316,17 @@
 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml,sha256=DO5N9jxrfn-jEoJS74JMghZB5ZN_nvLA3llRLe7NTLY,522
 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml,sha256=_-n1iLYFwhEDBxCnO8L5OTa8A5gKvVgTPC19g5wVx9A,602
 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml,sha256=NoLNnoAVy7-P7IJAymyPY7sjhiNuy973WHttv_Hh8eI,519
 super_gradients/sanity_check/__init__.py,sha256=IrTB1Lxw15cKFjxV8bGraUxj5d_pmEqYk7FHa01nuvk,107
 super_gradients/sanity_check/env_sanity_check.py,sha256=2_55JKDSsL1krMuXrWbF_qpz3Ob5SHP8lTYvSO5Ie-Q,5262
 super_gradients/training/__init__.py,sha256=LaqXsoTNBBFvGcV14K7tjt0iMbQdEy5NINJEycpcrPw,666
 super_gradients/training/params.py,sha256=I62jGc85o5YZeQDfvv9uUDyDKFeUnwXpR_i5rSZ2aZs,4155
-super_gradients/training/pretrained_models.py,sha256=fbXHJRWmx_7azXkOUXNgDEORdsaVQ6jjp0jYfkO_dbU,5696
-super_gradients/training/dataloaders/__init__.py,sha256=tlQw2GmkFPEMK3FA-_eODb1LHhDVKbl12BL6G1GEMak,3228
-super_gradients/training/dataloaders/dataloaders.py,sha256=uMi6Ld8nVj-sxPFsWeJuAIzqnhNGW9gpPFvhmmtQR5M,31443
+super_gradients/training/pretrained_models.py,sha256=I1cVvTBgbZj4gTvFxm55BrREuBJhAr7JlJa_KkoGyw4,4301
+super_gradients/training/dataloaders/__init__.py,sha256=fnGUu4drH1B6VLb2efrJLV0s4DnoTEbyKHDcHmEH5qA,3224
+super_gradients/training/dataloaders/dataloaders.py,sha256=7Qvjr9-aSiXmHpD6anjCiwHzCklCJVnJP0FR-XCeLSE,32361
 super_gradients/training/datasets/__init__.py,sha256=nptSnL6f7srktNihvAqw5polrwp4K-IrhTWPQ9vFLEM,1811
 super_gradients/training/datasets/auto_augment.py,sha256=VHw-Wq4ecHSKcqe9l63RUGpNa6JygUP3N7B6hbnTPxg,14162
 super_gradients/training/datasets/data_augmentation.py,sha256=TJOIT7j6ZWaNW6E4VvkJ-ARIWBY7Y4210NqrZbzKJJ8,3705
 super_gradients/training/datasets/datasets_conf.py,sha256=U2FTTYwCFp3cFZkzliWSGCHuCUUrns57AX7uS5Wn5NY,3484
 super_gradients/training/datasets/datasets_utils.py,sha256=oZnyLGBkfibkczYP2t69xf2OtqPU8ixyWDlc3iXQJh0,30279
 super_gradients/training/datasets/mixup.py,sha256=WDHoqTFbq-PGemKxE0eZ10Q03mpH8GIj-vFBNIZEg1U,14663
 super_gradients/training/datasets/sg_dataset.py,sha256=xVqf-7vvGk96TkshGHIcqiQfIVXdOCs12U1fcJjWrX0,11746
@@ -328,19 +347,19 @@
 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py,sha256=nCCohobPvCOtQ_SF2BAyyVyuSV68ZjjxrUurGfwNXMs,575
 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py,sha256=LChhVCXQ9-d9Zp3sa_PzAOrUBa15f_QKtxHdW51ocwg,1792
 super_gradients/training/datasets/data_formats/output_adapters/__init__.py,sha256=n7aH5WQzk_awjpei_GY-yOktBTw7LtzekY-gHJ8_AKE,92
 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py,sha256=qH0LPewt8hvKE5jVaZl0HunzONd7UHErbBcCuK_rjZk,8373
 super_gradients/training/datasets/detection_datasets/__init__.py,sha256=g86eRhqJoDs-9snO7QR6zejTmqhF2Amq71O-ZZQLPZc,683
 super_gradients/training/datasets/detection_datasets/coco_detection.py,sha256=EUTVRS0igoBFeUDhXg_tqxJSDhGUEU45jdL8YYko2ng,2505
 super_gradients/training/datasets/detection_datasets/coco_format_detection.py,sha256=OJ0JEQLClxRgdMZlUpuVEH0jxRqwfTbhOZnHK4rzjuY,9258
-super_gradients/training/datasets/detection_datasets/detection_dataset.py,sha256=7J4vM6N5MIsmWf9gFx3G0Kn1rHWCdbwAlYA_HsBilD8,25694
+super_gradients/training/datasets/detection_datasets/detection_dataset.py,sha256=x5vDIU_XP2764cTm2EV6btQ76UALTWO9cFGv8Opsv8I,26159
 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py,sha256=pAtuVBRVO_Y0Q-diaHQz3tWyjW7U3xR04ohzPx-vkbo,11353
-super_gradients/training/datasets/detection_datasets/yolo_format_detection.py,sha256=Z96cYyHxzpYO3m5OQNNehU3iixtm60Wc11cZWkkpQs4,10390
+super_gradients/training/datasets/detection_datasets/yolo_format_detection.py,sha256=ZP8zw0vvQ5CK-RkZ7EOGaLyLCAAzjuEev34SJQYVxag,11120
 super_gradients/training/datasets/detection_datasets/roboflow/__init__.py,sha256=Kw_KF41iHBr9tHrg6I6T6gdy8fgKLlG0NLCtXOyNpEs,328
-super_gradients/training/datasets/detection_datasets/roboflow/metadata.py,sha256=PTwZuphA1HyeYtxDnio6kmbcV6aM8VPD0AM4gk3_JCU,18882
+super_gradients/training/datasets/detection_datasets/roboflow/metadata.py,sha256=Ccxl7kt5F3E58oU4qJftnxIRaOc2iRyfCiyz_X4_lBc,18882
 super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py,sha256=9UEctKh8WxBLxdRP8wqfg3KDFq_KDYTr5AX4qD2Om7I,3504
 super_gradients/training/datasets/detection_datasets/roboflow/utils.py,sha256=_7mtuGnTHUVqfUqWlC9zpKGutBdaYJCGGj9pSbItfxI,1997
 super_gradients/training/datasets/pose_estimation_datasets/__init__.py,sha256=BeCVpXLn0FV9Oo_8iWtHz9n1GxdhXqTzymGT97_bdCA,502
 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py,sha256=6xNszBrqqOOdIKgM2ZFOZ4Crwssfh096_AcLZL5R1q4,4910
 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py,sha256=aADh3OLNLBLCk-3_nxLHjrrHniqr-tfbIHjKzJf-REA,9066
 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py,sha256=uMq0vV22npZqz21L_preyhbyKSHiBqS14Mp2UuEb-_4,5929
 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py,sha256=McVUG3sWR9Lxgk_ca8ECqvYieQwZApsFRfLNABES51Q,10167
@@ -392,20 +411,21 @@
 super_gradients/training/metrics/all_metrics.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/metrics/classification_metrics.py,sha256=Zopby8WBumdoJxZLJv5YgL7W_ZQODN4hKs55UJKO_H0,3262
 super_gradients/training/metrics/detection_metrics.py,sha256=XXneeuIzFCMwQfiGQcZZCN9cWhD6v3Cj_25HJTZ93nE,10741
 super_gradients/training/metrics/metric_utils.py,sha256=WT1TmuARbVKDLhw4Z1rJt38JM6jnSLAqO6gJa8rKWWY,3973
 super_gradients/training/metrics/pose_estimation_metrics.py,sha256=rw2gFnRSe1tET_TD4rdvt-8DWAvfSoAZwTaT5FZY_og,15346
 super_gradients/training/metrics/pose_estimation_utils.py,sha256=aOv42gu29NiWLihv6kmDBoFBXf0heVUsICF75dmM0l4,11454
 super_gradients/training/metrics/segmentation_metrics.py,sha256=B24ivTj53cF2COHeyDutxGohDLYcFT_eiKEqXpjDMXk,11935
-super_gradients/training/models/__init__.py,sha256=XZlJndgVtaqOjpv_3Gns6ixTdvmCn-FwhibEra8RICE,8368
+super_gradients/training/models/__init__.py,sha256=fz3k7vfa380OiiUMDnP9RA1XrAAOqU9ZWOmHGfg-3uA,8617
 super_gradients/training/models/arch_params_factory.py,sha256=ufy6mCMPUm1b9s3wm-AVMIbX2irytPoZpeXELgtCROs,1226
 super_gradients/training/models/conversion.py,sha256=kucMPr5HGUVn_xL06BaQU7vXzcgvUaqjZF5jiGgupqE,7060
 super_gradients/training/models/model_factory.py,sha256=z2vsf1_zjK2wgWYimHxRxA-bpOHG3ZQx2bC1o0Nhz6s,11875
-super_gradients/training/models/prediction_results.py,sha256=KB0vc3zhL_-is3LN4eeMqwoEtyvjlwFJ4msvv-OM6-8,10850
+super_gradients/training/models/prediction_results.py,sha256=YX2P0ENHNZODBQRKN-GwrszMn3tD1C-DFFIlX5PlT2s,10986
 super_gradients/training/models/predictions.py,sha256=-i4fUfLThPPTpSPiyFj-3TS_MRQWwXwQm5QZG1GD754,2054
+super_gradients/training/models/results.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/sg_module.py,sha256=JalNA0oIrW5IqV6Fl-SkAaq1qmcdLcAS8jx9QC84zMk,2998
 super_gradients/training/models/classification_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/classification_models/beit.py,sha256=kAq50cBeBteSF3uE3SW4TwYqfVn6edxPNXQEvOXc1Xg,20025
 super_gradients/training/models/classification_models/densenet.py,sha256=kDFzSB95Zk9OES501IiAyZmUlOnT03M3BEDaxlFONjM,7472
 super_gradients/training/models/classification_models/dpn.py,sha256=B5wPjPhPGp2PhTRxbC3w4VheCqVVs_8s9swqtwWnNKQ,3707
 super_gradients/training/models/classification_models/efficientnet.py,sha256=t9Rc9DveDC99iin-Xsv6UQ_Oy43SMOx3WjykTziqRgA,36745
 super_gradients/training/models/classification_models/googlenet.py,sha256=H57hvNMY7fqOV4v7Ezre-QVvawD1U9wuyAKUmpC1A4o,8862
@@ -413,34 +433,39 @@
 super_gradients/training/models/classification_models/mobilenet.py,sha256=JuABaCD_b6_Sh1EzigrBKqOniTTnI9RQ-a1V_YGaS6g,2407
 super_gradients/training/models/classification_models/mobilenetv2.py,sha256=V8FF_9Ibrn9LCf_4ybvQVKr5wVs1LEhpbXOff_XE0pY,9472
 super_gradients/training/models/classification_models/mobilenetv3.py,sha256=2aVzTJOufcdqthtSbjVHE7ViT3iaZcvvwTE9l-GiiKA,8696
 super_gradients/training/models/classification_models/pnasnet.py,sha256=DAo76uXefiCtOUTJ8uiuwAKSDN0nasSSOsCHg-sCkP0,4339
 super_gradients/training/models/classification_models/preact_resnet.py,sha256=24X4Zz00jj3Tj_l3BlLZOl-Z-dLJQ17mf7WKcpYcMtw,4209
 super_gradients/training/models/classification_models/regnet.py,sha256=TqBLs0lkE8yot9CEwtus16KPRHwn5X-HToqF9UGfU3A,13599
 super_gradients/training/models/classification_models/repvgg.py,sha256=gh9vB8y6ZUF8t-dUzxjy5_vpL8RMy6NbzYAYppL4ZoA,7924
-super_gradients/training/models/classification_models/resnet.py,sha256=mJhm-O5gnAs-cYVbeXahC8sH0UZ4_UsesCrVdomQC4E,15042
+super_gradients/training/models/classification_models/resnet.py,sha256=_P09wEFC_MPfTaVpXFGhjvoVhmoN3iDkSE5T5NVpTTQ,15025
 super_gradients/training/models/classification_models/resnext.py,sha256=oK78roHfDVm0dZA88ZaLgx8ml9tQkvwU95kRGtfsyGI,6294
 super_gradients/training/models/classification_models/senet.py,sha256=QypzG-XPOvY7HzannhLaT2wtyDeLhT5PZReopJRqgAA,4134
 super_gradients/training/models/classification_models/shufflenet.py,sha256=-57ZOa75ul4eEUMi3fnNbEff2AJGCXJaXQ9npLzETa4,3660
 super_gradients/training/models/classification_models/shufflenetv2.py,sha256=hHMYew6ET-QV8bYhwyCfCoXwIGn1uAJjSyQ9F6EJ9Kw,9768
 super_gradients/training/models/classification_models/vgg.py,sha256=byU29VjwL79efNtIC_ETLXhBLSe8qn_4Wm2RJ4BQYlo,1538
 super_gradients/training/models/classification_models/vit.py,sha256=NwtBiuhcO8dFTXwRb7h66phGDyrQuztdAM_nO5--1UA,9210
 super_gradients/training/models/detection_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/training/models/detection_models/csp_darknet53.py,sha256=mn3ndQ4JDVsMM_N1q6wI8fnEYu3JnaX1RWDNJqm-GaM,9502
+super_gradients/training/models/detection_models/csp_darknet53.py,sha256=4EIj_ptbYiRu1hNYDPut9cQcUwetuVplpilj4sQHkpk,9130
 super_gradients/training/models/detection_models/csp_resnet.py,sha256=OVL-DXEWj7e5B873jujeKxYvhs7Nhy6ViXOcLDHr49E,9814
-super_gradients/training/models/detection_models/customizable_detector.py,sha256=E02Mx-8ehqZwV6GTnJ-uBgWMQGNBN_lW1gC6b-no0k4,8784
+super_gradients/training/models/detection_models/customizable_detector.py,sha256=WuI9niU0ndl41fFA4vYeAcPtrCLgo52vZZan86pZmfE,9120
 super_gradients/training/models/detection_models/darknet53.py,sha256=FBFqJjU01A1l94HW7u7gCBmnRhSUvRVjlXZCsqyR4X8,4746
 super_gradients/training/models/detection_models/ssd.py,sha256=wvl6t3ltL6y5tjwqiFzBl8KmkwBOyUh07VS_7yVDfjs,2315
-super_gradients/training/models/detection_models/yolo_base.py,sha256=gLF2ohfGLVA6x_a5b2CI8GPZNgcp-SHk7I1XUb-khBI,29459
+super_gradients/training/models/detection_models/yolo_base.py,sha256=8HlHamlhgCaj0kstQfzs87D4WsZ81VtspGwEvMjOmHw,29459
 super_gradients/training/models/detection_models/yolox.py,sha256=Wjz2H7NwX3j_YkUzLWMSmcDbnEqee59dCXLrd4jRJ-Q,2459
-super_gradients/training/models/detection_models/pp_yolo_e/__init__.py,sha256=kKdYZ8QRFvcXymQyiO30nRuf--sHEt1uncYowhNT6Kg,155
-super_gradients/training/models/detection_models/pp_yolo_e/pan.py,sha256=WJmWjmTzqNBlf0kmznhduaAGmNaTrxns6-1qro0KKaY,6984
+super_gradients/training/models/detection_models/pp_yolo_e/__init__.py,sha256=kdGGMgi8qmk8vjKKGVk5Ap46e1yjdNmtdQFALb8eiFo,251
+super_gradients/training/models/detection_models/pp_yolo_e/pan.py,sha256=zndJicizLwqjLdAtfWsKd2GnuPv2IoTf4YZW3wcjV1U,7000
 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py,sha256=D4V9FAX5_VoxoPcwbuvYDtxaTfPRxFfvM5Ds0frO6js,3487
-super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py,sha256=bZkjWOiKH3MXtEW3bnVFPa68LzX2LOZHQEQRGPyGBhw,8240
-super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py,sha256=dMdGGlREeqFBOB5J3FmOnHad7cs6N5zKhOt-Hz15NV0,12334
+super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py,sha256=5tD_49PK3Ll30jlcrB7YQJ1QtP8HHCoGxoKkZN5Kx1w,8243
+super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py,sha256=lSKZgvbXW2sD0Kd6ImzeOLN7d-kEiBjlB8dDsWc4cKM,12397
+super_gradients/training/models/detection_models/yolo_nas/__init__.py,sha256=TJ9gQeZO8gmsZm0K-hyGxXyIZA8fwYuEaDheRMbXLUk,756
+super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py,sha256=P0TqYiqLgpQpJcaMeGIkT_A9jZrikQ6pVwxzzP_iTlI,12084
+super_gradients/training/models/detection_models/yolo_nas/panneck.py,sha256=qt0ChEAfmYU7Yc5Om7qQW4JMpRVQhMYW9hb-bLWsx2Q,2646
+super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py,sha256=eZWuODf8QttWJAR_WYyH9j7GjTzoR6jpC-24Pa_QZaw,4124
+super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py,sha256=yEPlfJoqCAHtFhKebaj89vIt2DMjM5VHg5zqaiX6-bo,13329
 super_gradients/training/models/kd_modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/kd_modules/kd_module.py,sha256=urOyHbsubq615UiGJo4-CAFpKvdKxHLrTFMzp1TlM5c,3553
 super_gradients/training/models/pose_estimation_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/pose_estimation_models/dekr_hrnet.py,sha256=1WeqAspQseBaECT42iGbKnVfFJ2hHPx-63eublI_dgQ,21231
 super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py,sha256=vQUuvQO6JDdW4tNKYL7k_iDfRf1h28j7aj-n_Xr0UPo,1294
 super_gradients/training/models/pose_estimation_models/pose_ppyolo.py,sha256=pLLHoTF_V2rJKmJ0gLQmcQC0wt7TSfb9RrFA4VoYSaU,1335
 super_gradients/training/models/segmentation_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -453,42 +478,42 @@
 super_gradients/training/models/segmentation_models/regseg.py,sha256=V-Vc4zZcoigUlFD8-p4K9_p-BLuhYWmrPyZX8di8_QI,14424
 super_gradients/training/models/segmentation_models/segformer.py,sha256=hNSunP6CtOcwxczuwQRQxY1sZdc0R1OnxatCW2aHBPA,20334
 super_gradients/training/models/segmentation_models/segmentation_module.py,sha256=ypc_zQRfeuP6YEoY3Kc-tcRRVLLuOaY0uJuWpQRTzKo,2256
 super_gradients/training/models/segmentation_models/shelfnet.py,sha256=bcSLs0d1ulhjWUbgAtdmG6hR_vN4IXMXCkwK0r2Dp98,24833
 super_gradients/training/models/segmentation_models/stdc.py,sha256=m2oXqSvRV-lM8Rl_51ebP_6xcQt0pX8imkL59nzJp6A,29005
 super_gradients/training/models/segmentation_models/unet/__init__.py,sha256=WZp8BByl8QZpdPlnLwvW7QF5qfODj_-yo4UbtoScPng,260
 super_gradients/training/models/segmentation_models/unet/unet.py,sha256=x5Zu2Z7rw6i4LXyxcyxfL2uOzt3DuofWo7uKX_utTCw,12324
-super_gradients/training/models/segmentation_models/unet/unet_decoder.py,sha256=PdmnBOjv8MrreWEEphMJsMqS3MuxeNDqvRf0ls-uqvY,8305
+super_gradients/training/models/segmentation_models/unet/unet_decoder.py,sha256=nqwXOlJkAddqNHBQOgaBIJQdPExMwNWZQrlEqUMP8ME,10718
 super_gradients/training/models/segmentation_models/unet/unet_encoder.py,sha256=auTtUn6jkKWUOdW_wKvOyKC9DpVSi7Y-LjoZY1POA3g,13292
 super_gradients/training/models/user_models/__init__.py,sha256=WNfXGheDVebPB3XmC9ce-wkyh0qXHRlINW43JIdnY6E,119
 super_gradients/training/pipelines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/training/pipelines/pipelines.py,sha256=ML0ylHisBvP9wwhg33NoEw8U8N4ZADDQZ_bYZF5E3Lo,14399
+super_gradients/training/pipelines/pipelines.py,sha256=5RBdZVCQkjSeuwyfDmuHccOO5F_R3Hn73Gc8exL9aR4,14562
 super_gradients/training/pre_launch_callbacks/__init__.py,sha256=SZtn0Kq5PJ_GIMfFT5bBb0Pck6r5mAnBAfgpDaX5Cdk,393
 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py,sha256=E3UsNalAFR0-7pwga-OjFCTp4m7SuO9BEy04Lwt18kk,13955
 super_gradients/training/processing/__init__.py,sha256=L_S3KapcujiBTXjHcMZxQz5aCwJM9Xxurbhs08oy0_o,517
-super_gradients/training/processing/processing.py,sha256=Z-CvRtbGgEYtvT9N6S3-8NfOwSetFTZkCk1DzrdIRZc,13178
+super_gradients/training/processing/processing.py,sha256=xx6q2nO2VXC-FGX4rYVp9Otbipbv43gToYepKe0jQyk,13177
 super_gradients/training/qat_trainer/__init__.py,sha256=GZRdCf6P1Ximp-eoVw8kHv5Zb4AjBqxV0E2NwO1OmNo,98
-super_gradients/training/qat_trainer/qat_trainer.py,sha256=PY3-7_vEJN8mgVIsD17K1qZ-DT6PETe7KuvoN2tFnls,9896
+super_gradients/training/qat_trainer/qat_trainer.py,sha256=wrdK5ao9S1EJpufOtg_rJjI-qExzlHUa_ybsTNOVdTA,9701
 super_gradients/training/sg_trainer/__init__.py,sha256=dug-p1erLN2SzYFQytJzPWDLOCmfvE94kFtcFLOTqj0,184
-super_gradients/training/sg_trainer/sg_trainer.py,sha256=9Nk2wyMgrEAMGEcgkjONQms3_WHcEN8Hudbf54I9Ro8,97370
+super_gradients/training/sg_trainer/sg_trainer.py,sha256=XXLM3D_c-XVQW4j-G7sJRAfjD7DgMuFJf75N85Gm8jY,97356
 super_gradients/training/training_hyperparams/__init__.py,sha256=R5pvZNSQgDNxRp23qAlAAhGdPT7u_e78QiztqQDqosc,1685
 super_gradients/training/training_hyperparams/training_hyperparams.py,sha256=pZIOz9L6vf-tgCMUbvf2WLch1zCCfDevhfYPnL3QR7A,3774
 super_gradients/training/transforms/__init__.py,sha256=SMLfPEp8zqooiV6mB4byOzk5SprUUo77LIUNgTTB7A8,1024
 super_gradients/training/transforms/all_transforms.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/transforms/keypoint_transforms.py,sha256=-lTR8tHtWGmK6THZvyI52OpH5yhWXDGJeUJM_FwcZhE,16193
 super_gradients/training/transforms/pipeline_adaptors.py,sha256=ukVHjcx-XaCEGZ3I_afIb9Uj73vwYtkmgrLJw9jr7oU,1134
-super_gradients/training/transforms/transforms.py,sha256=OcqekeLDMA7_TUrtuo_wJG6XrUCwaEJ9qty2Ouxu0bk,55085
+super_gradients/training/transforms/transforms.py,sha256=uDbuGhNmEL0Mo_FvO4R9NhUf3nH9yQygGIxSgciqV60,55089
 super_gradients/training/transforms/utils.py,sha256=WkgT9-2hZm7IBS_HZzy1kOE0EOb-k0t8gypuPhpC5Z4,6048
 super_gradients/training/utils/__init__.py,sha256=hveHoDSb03rQ0jXc0SLWD7Pvwd9gCnaISEgc_oikTOE,1104
 super_gradients/training/utils/activations_utils.py,sha256=LNgR7SUWOehjBbvtHvU8PtgazsbxX9ztvIUNAQ4nB64,1673
 super_gradients/training/utils/bbox_utils.py,sha256=tvDIJ5TkShshteJAzXVtQZaZFMtIHrYS98U5bpcc0sU,1111
-super_gradients/training/utils/checkpoint_utils.py,sha256=jqphMTl_izp2nW41Fu9gj7iMVxVBZwyvgLxfnEju4vg,14834
+super_gradients/training/utils/checkpoint_utils.py,sha256=A3d7dhAhHqwDG_39iK1e4QcWNEfC5k3IFrJWFudIrGo,15315
 super_gradients/training/utils/config_utils.py,sha256=jDS_SaRfIEvAXzPB5ZerzVtKaDxD8mgKesUI4M2ERdo,9794
 super_gradients/training/utils/deprecated_utils.py,sha256=YtKScFu62sn2IDBtzC2cPmdSFQ_UfeQZ3CrPDuOZpO4,1132
-super_gradients/training/utils/detection_utils.py,sha256=EzzS372c8jPTOcOY50R5b7giRKkypXNFXcU9cBCbeTk,53611
+super_gradients/training/utils/detection_utils.py,sha256=heb7irv25BHi8erxfS5msqI9yA_VH28qk1zJa0PMgOA,53278
 super_gradients/training/utils/distributed_training_utils.py,sha256=1hUkc_OE3CCvBtcWlUsGbB8kmgjAUWtgXFJs9QORX-I,16195
 super_gradients/training/utils/early_stopping.py,sha256=FGv-bFT6N1WrtEmZ2Q0xmmijmOI_IKoTvxQcua0LK9g,6352
 super_gradients/training/utils/ema.py,sha256=xPjihYYtpKqrOth0KoRyTeFarCTEH-AVnh0J9M767PM,9322
 super_gradients/training/utils/ema_decay_schedules.py,sha256=lV9zLoVvfPPWJajPpNBnkn8d5ahLJIAjHtv3rZsDU1E,2610
 super_gradients/training/utils/export_utils.py,sha256=Ci9yz8OiK0oVEBHaG74-YuPqBANciWpFf17w-IVYvRc,1072
 super_gradients/training/utils/get_model_stats.py,sha256=nMKVdVxsLPSKDXD7qnTWk60f0B3F1-Ct-XdZchFbsJM,7508
 super_gradients/training/utils/kd_trainer_utils.py,sha256=j-RWPU7_0rKX-4Cf9RiyGk3GuH6j7_cGeBLKYhuXYOk,771
@@ -503,27 +528,31 @@
 super_gradients/training/utils/weight_averaging_utils.py,sha256=a9rw30CWTfp-QCDysObSC-yd-W_XQYJeX12SfvyH8TQ,6209
 super_gradients/training/utils/callbacks/__init__.py,sha256=IW4hEmiLvmSqcvYMQn6D0e8qcI-avUnHUcMI8Mv9gvg,2030
 super_gradients/training/utils/callbacks/all_callbacks.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/utils/callbacks/base_callbacks.py,sha256=pCMNK9iUQm8jqSAm5elZrG9Oy3AYD62L-_qj8e9du8U,20126
 super_gradients/training/utils/callbacks/callbacks.py,sha256=UCHS-mkHzEqqoORL2OiVa23Zab1inMLfytJnnioOkkE,32630
 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py,sha256=7-EaXO3ipczQw9H6NIGqZ-3cR3n-ZN6oAEcnCsv-VtE,1169
 super_gradients/training/utils/media/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/training/utils/media/image.py,sha256=F47OIx3s23gJDxujpHOd0Vw_YpN_aJj-abUeraFyA9M,5775
+super_gradients/training/utils/media/image.py,sha256=CZ6_K-yifXXNqGe3grp1e5hl-Ug_0lFUGH5CIm_1Glo,5880
 super_gradients/training/utils/media/stream.py,sha256=wgVafnzRXnZvSxaiquNXUC6PqSMlLI4A6YS6_b4A04Y,4046
-super_gradients/training/utils/media/video.py,sha256=XnoV6dnd6--iNT4JhT0e671DlQIfnN03nO7TrBBfkgQ,5360
+super_gradients/training/utils/media/video.py,sha256=DC9xdQX5g2JCWalBeHAGh3VWtvBRvxOs3dIgIuqURtw,6926
 super_gradients/training/utils/optimizers/__init__.py,sha256=Z-kZTiqwHe-KFYP0BTFsX0TNms8-CfRrc6iKEfewopM,396
 super_gradients/training/utils/optimizers/lamb.py,sha256=zdvmfKHGen7_rwMohoEs6DOSDEH95ELFCKezD1fN1v0,9760
 super_gradients/training/utils/optimizers/lion.py,sha256=ivMkwLg0vpOyfD4h226wScYXYDwTdCh0o_zkOeyrdcs,3008
 super_gradients/training/utils/optimizers/rmsprop_tf.py,sha256=5gzx0uy3x4c8G8UgfDnOTLjASwT1enBAcfUkgzrOOJU,6834
 super_gradients/training/utils/pose_estimation/__init__.py,sha256=V0xjHNxc1OeJUE2QOTlAV298wmQwgRWwXLx5Pq6p5Gw,213
 super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py,sha256=1y-85e33A9mKokm4ER_HpwuRqWpbY2pjm6gAjjy4WXc,11167
 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py,sha256=HEdNaksgnzoXh1RWRvB5rd_tniZWkk6Ro-6D2-Abv1Q,7140
 super_gradients/training/utils/quantization/__init__.py,sha256=FsLDGZR4MT_1tTIcnyOhIqUTfCf178tU7Y72och-Fws,387
 super_gradients/training/utils/quantization/calibrator.py,sha256=vfXnyPxLdHjk5e5CF3-lBwofRDjX-ZCyDaRreuu6_h4,6271
 super_gradients/training/utils/quantization/core.py,sha256=CYykLasziH9YT0h_utxWj6WZ6tXi4KUSKaiBf1N2YZM,8417
 super_gradients/training/utils/quantization/export.py,sha256=GW22x2GMQJMEp1iZcJ63qcxev6Etay_FI6taKbJpmv8,2196
 super_gradients/training/utils/quantization/selective_quantization_utils.py,sha256=hQ8uZliyAK21pguj0aSybxINffXrj0R2YCHCWIRV7Z4,17062
-super_gradients-3.0.9.dist-info/LICENSE.md,sha256=jWCBQN-JmCX0hwvn3MqItDj18W3riP4zda31ncMkcfA,11341
-super_gradients-3.0.9.dist-info/METADATA,sha256=qEEElq7wG2GUcVgeJE1foQ9XbaK5E-F9j4AzZimz3ug,34221
-super_gradients-3.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-super_gradients-3.0.9.dist-info/top_level.txt,sha256=k8ZbuOXtbEm0O2O3MCG-rnUyDilV2FYLXMbeXUspUXI,16
-super_gradients-3.0.9.dist-info/RECORD,,
+super_gradients/training/utils/visualization/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+super_gradients/training/utils/visualization/detection.py,sha256=348rm6aggC_RLn9Zsnr9FC0AJu5zieHVhTzQGJs6sfk,1698
+super_gradients/training/utils/visualization/utils.py,sha256=LXh2fmdauApUJEn62a0yEXwKQ6G1ySlWvqkK9Ap8ybU,2847
+super_gradients-3.1.0.dist-info/LICENSE.YOLONAS.md,sha256=mPgPXAN-RoGSYLzisdBu2uJx2HyJHd8enqEUlpO5mmQ,2218
+super_gradients-3.1.0.dist-info/LICENSE.md,sha256=jWCBQN-JmCX0hwvn3MqItDj18W3riP4zda31ncMkcfA,11341
+super_gradients-3.1.0.dist-info/METADATA,sha256=Zu_Yq27JlSrrBb214F99EmW_9UWoh0lxi52IJVsh7tk,36159
+super_gradients-3.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+super_gradients-3.1.0.dist-info/top_level.txt,sha256=k8ZbuOXtbEm0O2O3MCG-rnUyDilV2FYLXMbeXUspUXI,16
+super_gradients-3.1.0.dist-info/RECORD,,
```

