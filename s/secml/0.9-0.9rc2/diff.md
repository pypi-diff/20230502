# Comparing `tmp/secml-0.9.zip` & `tmp/secml-0.9rc2.zip`

## zipinfo {}

```diff
@@ -1,220 +1,220 @@
-Zip file size: 401755 bytes, number of entries: 218
--rw-r--r--  2.0 unx    13907 b- defN 19-Oct-11 18:29 secml-0.9/PKG-INFO
--rw-rw-rw-  2.0 unx     6168 b- defN 19-Oct-11 18:29 secml-0.9/setup.py
--rw-rw-rw-  2.0 unx    10617 b- defN 19-Oct-11 18:29 secml-0.9/README.md
--rw-r--r--  2.0 unx       38 b- defN 19-Oct-11 18:29 secml-0.9/setup.cfg
--rw-rw-rw-  2.0 unx     1289 b- defN 19-Oct-11 18:29 secml-0.9/CHANGELOG.md
--rw-rw-rw-  2.0 unx      165 b- defN 19-Oct-11 18:29 secml-0.9/MANIFEST.in
--rw-rw-rw-  2.0 unx      141 b- defN 19-Oct-11 18:29 secml-0.9/requirements.txt
--rw-r--r--  2.0 unx        1 b- defN 19-Oct-11 18:29 secml-0.9/src/secml.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        1 b- defN 19-Oct-11 18:29 secml-0.9/src/secml.egg-info/not-zip-safe
--rw-r--r--  2.0 unx    13907 b- defN 19-Oct-11 18:29 secml-0.9/src/secml.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     9314 b- defN 19-Oct-11 18:29 secml-0.9/src/secml.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      197 b- defN 19-Oct-11 18:29 secml-0.9/src/secml.egg-info/requires.txt
--rw-r--r--  2.0 unx        6 b- defN 19-Oct-11 18:29 secml-0.9/src/secml.egg-info/top_level.txt
--rw-rw-rw-  2.0 unx        3 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/VERSION
--rw-rw-rw-  2.0 unx      181 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/test_simple.py
--rw-rw-rw-  2.0 unx      614 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/secml.conf
--rw-rw-rw-  2.0 unx     5018 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/__init__.py
--rw-rw-rw-  2.0 unx    10562 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/settings.py
--rw-rw-rw-  2.0 unx     1368 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/_globals.py
--rw-rw-rw-  2.0 unx    74225 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/array/c_sparse.py
--rw-rw-rw-  2.0 unx       28 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/array/__init__.py
--rw-rw-rw-  2.0 unx     2678 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/array/array_utils.py
--rw-rw-rw-  2.0 unx    73348 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/array/c_dense.py
--rw-rw-rw-  2.0 unx   179872 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/array/c_array.py
--rw-rw-rw-  2.0 unx    20535 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/array/c_array_interface.py
--rwxrwxrwx  2.0 unx     6995 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/c_dataset_header.py
--rwxrwxrwx  2.0 unx       77 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/__init__.py
--rwxrwxrwx  2.0 unx    13538 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/c_dataset.py
--rw-rw-rw-  2.0 unx     2740 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/c_dataset_pytorch.py
--rw-rw-rw-  2.0 unx     1036 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/data_utils.py
--rw-rw-rw-  2.0 unx     2781 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/splitter/c_datasplitter.py
--rw-rw-rw-  2.0 unx     3058 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/splitter/c_datasplitter_stratkfold.py
--rw-rw-rw-  2.0 unx     5313 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/splitter/c_train_test_split.py
--rw-rw-rw-  2.0 unx      487 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/splitter/__init__.py
--rw-rw-rw-  2.0 unx     7106 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/splitter/c_chronological_splitter.py
--rw-rw-rw-  2.0 unx     2821 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/splitter/c_datasplitter_kfold.py
--rw-rw-rw-  2.0 unx     6640 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/splitter/c_datasplitter_openworld.py
--rw-rw-rw-  2.0 unx     3548 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/splitter/c_datasplitter_labelkfold.py
--rw-rw-rw-  2.0 unx     4377 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/splitter/c_datasplitter_shuffle.py
--rw-rw-rw-  2.0 unx     1616 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/selection/c_ps_random.py
--rw-rw-rw-  2.0 unx     2266 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/selection/c_prototypes_selector.py
--rw-rw-rw-  2.0 unx     1932 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/selection/c_ps_border.py
--rw-rw-rw-  2.0 unx     2493 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/selection/c_ps_kmedians.py
--rw-rw-rw-  2.0 unx      238 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/selection/__init__.py
--rw-rw-rw-  2.0 unx     2140 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/selection/c_ps_spanning.py
--rw-rw-rw-  2.0 unx     1929 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/selection/c_ps_center.py
--rw-rw-rw-  2.0 unx     2171 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/loader/c_dataloader.py
--rw-rw-rw-  2.0 unx     8668 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/loader/c_dataloader_icubworld.py
--rw-rw-rw-  2.0 unx     4716 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/loader/c_dataloader_imgclients.py
--rw-rw-rw-  2.0 unx      930 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/loader/c_dataloader_pytorch.py
--rw-rw-rw-  2.0 unx     2218 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/loader/loader_utils.py
--rw-rw-rw-  2.0 unx    12836 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/loader/c_dataloader_cifar.py
--rw-rw-rw-  2.0 unx     7043 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/loader/c_dataloader_imgfolders.py
--rw-rw-rw-  2.0 unx      620 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/loader/__init__.py
--rw-rw-rw-  2.0 unx     7272 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/loader/c_dataloader_mnist.py
--rw-rw-rw-  2.0 unx     7150 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/loader/c_dataloader_svmlight.py
--rwxrwxrwx  2.0 unx    26623 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/loader/c_dataloader_sklearn.py
--rw-rw-rw-  2.0 unx     3223 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/data/loader/c_dataloader_lfw.py
--rw-rw-rw-  2.0 unx       35 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/__init__.py
--rwxrwxrwx  2.0 unx       79 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/attacks/__init__.py
--rw-rw-rw-  2.0 unx    13279 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/attacks/c_attack.py
--rw-rw-rw-  2.0 unx     5442 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/attacks/evasion/c_attack_evasion_pgd.py
--rw-rw-rw-  2.0 unx     4765 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/attacks/evasion/c_attack_evasion.py
--rw-rw-rw-  2.0 unx      154 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/attacks/evasion/__init__.py
--rw-rw-rw-  2.0 unx    16335 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/attacks/evasion/c_attack_evasion_pgd_ls.py
--rw-rw-rw-  2.0 unx    11259 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/attacks/poisoning/c_attack_poisoning_svm.py
--rw-rw-rw-  2.0 unx     7099 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/attacks/poisoning/c_attack_poisoning_logistic_regression.py
--rw-rw-rw-  2.0 unx      258 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/attacks/poisoning/__init__.py
--rw-rw-rw-  2.0 unx     7060 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/attacks/poisoning/c_attack_poisoning_ridge.py
--rw-rw-rw-  2.0 unx    23838 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/attacks/poisoning/c_attack_poisoning.py
--rw-rw-rw-  2.0 unx       75 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/seceval/__init__.py
--rw-rw-rw-  2.0 unx     5547 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/seceval/c_sec_eval_data.py
--rw-rw-rw-  2.0 unx     6421 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/adv/seceval/c_sec_eval.py
--rw-rw-rw-  2.0 unx     2668 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/parallel/parfor.py
--rw-rw-rw-  2.0 unx       36 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/parallel/__init__.py
--rw-rw-rw-  2.0 unx     1009 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/core/constants.py
--rwxrwxrwx  2.0 unx    20185 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/core/c_creator.py
--rwxrwxrwx  2.0 unx       32 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/core/__init__.py
--rw-rw-rw-  2.0 unx    11210 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/core/attr_utils.py
--rw-rw-rw-  2.0 unx      824 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/core/exceptions.py
--rw-rw-rw-  2.0 unx     3568 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/core/decorators.py
--rw-rw-rw-  2.0 unx     7504 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/core/type_utils.py
--rw-rw-rw-  2.0 unx    11736 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/figure/c_figure.py
--rw-rw-rw-  2.0 unx       30 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/figure/__init__.py
--rw-rw-rw-  2.0 unx     1398 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/figure/_plots/plot_utils.py
--rw-rw-rw-  2.0 unx     2934 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/figure/_plots/c_plot_classifier.py
--rw-rw-rw-  2.0 unx     3321 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/figure/_plots/c_plot_ds.py
--rw-rw-rw-  2.0 unx    79744 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/figure/_plots/c_plot.py
--rw-rw-rw-  2.0 unx    12154 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/figure/_plots/c_plot_metric.py
--rw-rw-rw-  2.0 unx     5691 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/figure/_plots/c_plot_sec_eval.py
--rw-rw-rw-  2.0 unx     1380 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/figure/_plots/c_plot_constraint.py
--rw-rw-rw-  2.0 unx      312 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/figure/_plots/__init__.py
--rw-rw-rw-  2.0 unx     8318 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/figure/_plots/c_plot_fun.py
--rw-rw-rw-  2.0 unx     1328 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/figure/_plots/c_plot_stats.py
--rwxrwxrwx  2.0 unx       19 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/__init__.py
--rw-rw-rw-  2.0 unx     7143 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/optimizers/c_optimizer_scipy.py
--rw-rw-rw-  2.0 unx     5509 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/optimizers/c_optimizer_pgd.py
--rw-rw-rw-  2.0 unx      174 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/optimizers/__init__.py
--rw-rw-rw-  2.0 unx     5577 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/optimizers/c_optimizer.py
--rw-rw-rw-  2.0 unx    11340 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/optimizers/c_optimizer_pgd_ls.py
--rw-rw-rw-  2.0 unx     1399 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/optimizers/line_search/c_line_search.py
--rw-rw-rw-  2.0 unx       91 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/optimizers/line_search/__init__.py
--rw-rw-rw-  2.0 unx    12701 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/optimizers/line_search/c_line_search_bisect.py
--rw-rw-rw-  2.0 unx     2589 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/function/c_function_3hcamel.py
--rw-rw-rw-  2.0 unx     3228 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/function/c_function_rosenbrock.py
--rw-rw-rw-  2.0 unx     1263 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/function/c_function_linear.py
--rw-rw-rw-  2.0 unx     2954 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/function/c_function_beale.py
--rw-rw-rw-  2.0 unx      343 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/function/__init__.py
--rw-rw-rw-  2.0 unx    10076 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/function/c_function.py
--rw-rw-rw-  2.0 unx     2814 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/function/c_function_mccormick.py
--rw-rw-rw-  2.0 unx     1772 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/function/c_function_quadratic.py
--rw-rw-rw-  2.0 unx     5673 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/constraints/c_constraint_l1.py
--rw-rw-rw-  2.0 unx     2708 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/constraints/c_constraint_l2.py
--rw-rw-rw-  2.0 unx      169 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/constraints/__init__.py
--rw-rw-rw-  2.0 unx     4483 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/constraints/c_constraint.py
--rw-rw-rw-  2.0 unx     7633 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/optim/constraints/c_constraint_box.py
--rw-rw-rw-  2.0 unx     3537 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/utils/download_utils.py
--rw-rw-rw-  2.0 unx     7620 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/utils/dict_utils.py
--rwxrwxrwx  2.0 unx    16782 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/utils/c_log.py
--rw-rw-rw-  2.0 unx     4981 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/utils/mixed_utils.py
--rw-rw-rw-  2.0 unx      982 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/utils/list_utils.py
--rwxrwxrwx  2.0 unx      209 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/utils/__init__.py
--rwxrwxrwx  2.0 unx    12948 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/utils/c_file_manager.py
--rw-rw-rw-  2.0 unx     1926 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/utils/pickle_utils.py
--rw-rw-rw-  2.0 unx       23 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/__init__.py
--rw-rw-rw-  2.0 unx     1460 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/clf_utils.py
--rw-rw-rw-  2.0 unx     5261 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/c_classifier_kde.py
--rwxrwxrwx  2.0 unx     4507 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/c_classifier_linear.py
--rwxrwxrwx  2.0 unx    11461 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/c_classifier.py
--rwxrwxrwx  2.0 unx      911 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/__init__.py
--rw-rw-rw-  2.0 unx     5453 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/c_classifier_mcs_linear.py
--rw-rw-rw-  2.0 unx     1347 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_kde.py
--rw-rw-rw-  2.0 unx     5434 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_linear.py
--rw-rw-rw-  2.0 unx     1986 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_logistic.py
--rw-rw-rw-  2.0 unx     6084 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_svm.py
--rw-rw-rw-  2.0 unx     3402 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_ridge.py
--rw-rw-rw-  2.0 unx      690 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/gradients/__init__.py
--rw-rw-rw-  2.0 unx     5499 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_pytorch.py
--rw-rw-rw-  2.0 unx     2882 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_sgd.py
--rw-rw-rw-  2.0 unx     4991 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient.py
--rwxrwxrwx  2.0 unx     3457 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/loss/c_loss_cross_entropy.py
--rw-rw-rw-  2.0 unx      405 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/loss/__init__.py
--rw-rw-rw-  2.0 unx     2604 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/loss/c_softmax.py
--rwxrwxrwx  2.0 unx     4781 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/loss/c_loss_squared.py
--rw-rw-rw-  2.0 unx     5752 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/loss/c_loss.py
--rwxrwxrwx  2.0 unx     4170 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/loss/c_loss_logistic.py
--rwxrwxrwx  2.0 unx     6353 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/loss/c_loss_hinge.py
--rwxrwxrwx  2.0 unx     5501 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/loss/c_loss_epsilon_insensitive.py
--rw-rw-rw-  2.0 unx     1579 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/reject/mixin_classifier_gradient_reject_threshold.py
--rw-rw-rw-  2.0 unx      121 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/reject/__init__.py
--rw-rw-rw-  2.0 unx     2388 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/reject/c_classifier_reject.py
--rw-rw-rw-  2.0 unx     9447 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/reject/c_classifier_reject_threshold.py
--rw-rw-rw-  2.0 unx     2572 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_knn.py
--rw-rw-rw-  2.0 unx     3769 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_sklearn.py
--rw-rw-rw-  2.0 unx     3451 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_logistic.py
--rwxrwxrwx  2.0 unx    14782 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_svm.py
--rw-rw-rw-  2.0 unx     9772 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_sgd.py
--rw-rw-rw-  2.0 unx       13 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/sklearn/__init__.py
--rw-rw-rw-  2.0 unx     2246 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_nearest_centroid.py
--rw-rw-rw-  2.0 unx     1303 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_random_forest.py
--rw-rw-rw-  2.0 unx     1179 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_decision_tree.py
--rw-rw-rw-  2.0 unx     6996 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_ridge.py
--rw-rw-rw-  2.0 unx       13 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/pytorch/__init__.py
--rw-rw-rw-  2.0 unx    19384 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/pytorch/c_classifier_pytorch.py
--rw-rw-rw-  2.0 unx     5362 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/multiclass/c_classifier_multi_ova.py
--rw-rw-rw-  2.0 unx     1292 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/multiclass/mixin_classifier_gradient_multiclass_ova.py
--rw-rw-rw-  2.0 unx      115 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/multiclass/__init__.py
--rw-rw-rw-  2.0 unx    10540 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/multiclass/c_classifier_multi.py
--rwxrwxrwx  2.0 unx      922 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/regularizer/c_regularizer_l1.py
--rw-rw-rw-  2.0 unx      725 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/regularizer/c_regularizer.py
--rwxrwxrwx  2.0 unx     1565 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/regularizer/c_regularizer_elastic_net.py
--rw-rw-rw-  2.0 unx      192 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/regularizer/__init__.py
--rwxrwxrwx  2.0 unx      918 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/classifiers/regularizer/c_regularizer_l2.py
--rw-rw-rw-  2.0 unx       93 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/features/__init__.py
--rw-rw-rw-  2.0 unx     7796 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/features/c_preprocess.py
--rw-rw-rw-  2.0 unx     6420 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/features/normalization/c_normalizer_minmax.py
--rw-rw-rw-  2.0 unx      475 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/features/normalization/c_normalizer.py
--rw-rw-rw-  2.0 unx     4422 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/features/normalization/c_normalizer_linear.py
--rw-rw-rw-  2.0 unx      249 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/features/normalization/__init__.py
--rw-rw-rw-  2.0 unx     8106 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/features/normalization/c_normalizer_mean_std.py
--rw-rw-rw-  2.0 unx     7388 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/features/normalization/c_normalizer_unitnorm.py
--rw-rw-rw-  2.0 unx       96 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/features/reduction/__init__.py
--rw-rw-rw-  2.0 unx    10398 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/features/reduction/c_reducer_pca.py
--rw-rw-rw-  2.0 unx     5908 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/features/reduction/c_reducer_lda.py
--rw-rw-rw-  2.0 unx      390 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/features/reduction/c_reducer.py
--rwxrwxrwx  2.0 unx     5213 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/c_perfevaluator_xval.py
--rwxrwxrwx  2.0 unx     6537 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/c_perfevaluator_xval_multiclass.py
--rw-rw-rw-  2.0 unx      171 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/__init__.py
--rwxrwxrwx  2.0 unx     7568 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/c_perfevaluator.py
--rw-rw-rw-  2.0 unx      902 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_confusion_matrix.py
--rw-rw-rw-  2.0 unx     2092 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_metric_tpr_at_fpr.py
--rw-rw-rw-  2.0 unx     2144 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_metric_auc_wmw.py
--rw-rw-rw-  2.0 unx     1397 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_metric_mae.py
--rw-rw-rw-  2.0 unx     1392 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_metric_mse.py
--rw-rw-rw-  2.0 unx     1448 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_metric_test_error.py
--rw-rw-rw-  2.0 unx      650 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/__init__.py
--rw-rw-rw-  2.0 unx     2652 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_metric_pauc.py
--rwxrwxrwx  2.0 unx     3377 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_metric.py
--rw-rw-rw-  2.0 unx     1711 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_metric_precision.py
--rw-rw-rw-  2.0 unx    15874 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_roc.py
--rw-rw-rw-  2.0 unx     1758 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_metric_auc.py
--rw-rw-rw-  2.0 unx     1744 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_metric_recall.py
--rw-rw-rw-  2.0 unx     1402 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_metric_accuracy.py
--rw-rw-rw-  2.0 unx     1751 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/peval/metrics/c_metric_f1.py
--rw-rw-rw-  2.0 unx     3389 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/stats/c_density_estimation.py
--rw-rw-rw-  2.0 unx      112 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/stats/__init__.py
--rw-rw-rw-  2.0 unx     1852 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/stats/c_distribution_gaussian.py
--rwxrwxrwx  2.0 unx     5713 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/kernel/c_kernel_poly.py
--rwxrwxrwx  2.0 unx     1784 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/kernel/c_kernel_hamming.py
--rwxrwxrwx  2.0 unx     6033 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/kernel/c_kernel_euclidean.py
--rwxrwxrwx  2.0 unx     5720 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/kernel/c_kernel_rbf.py
--rw-rw-rw-  2.0 unx     5404 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/kernel/c_kernel_laplacian.py
--rwxrwxrwx  2.0 unx      415 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/kernel/__init__.py
--rw-rw-rw-  2.0 unx     3526 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/kernel/c_kernel_chebyshev_distance.py
--rwxrwxrwx  2.0 unx     3295 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/kernel/c_kernel_linear.py
--rwxrwxrwx  2.0 unx     2794 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/kernel/c_kernel_histintersect.py
--rwxrwxrwx  2.0 unx     7025 b- defN 19-Oct-11 18:29 secml-0.9/src/secml/ml/kernel/c_kernel.py
--rw-rw-rw-  2.0 unx     1166 b- defN 19-Oct-11 18:29 secml-0.9/update/0.8-to-0.9.md
-218 files, 1351267 bytes uncompressed, 362573 bytes compressed:  73.2%
+Zip file size: 402647 bytes, number of entries: 218
+-rw-r--r--  2.0 unx    13910 b- defN 19-Oct-11 16:14 secml-0.9rc2/PKG-INFO
+-rw-rw-rw-  2.0 unx     6168 b- defN 19-Oct-11 16:14 secml-0.9rc2/setup.py
+-rw-rw-rw-  2.0 unx    10617 b- defN 19-Oct-11 16:14 secml-0.9rc2/README.md
+-rw-r--r--  2.0 unx       38 b- defN 19-Oct-11 16:14 secml-0.9rc2/setup.cfg
+-rw-rw-rw-  2.0 unx      267 b- defN 19-Oct-11 16:14 secml-0.9rc2/CHANGELOG.md
+-rw-rw-rw-  2.0 unx      165 b- defN 19-Oct-11 16:14 secml-0.9rc2/MANIFEST.in
+-rw-rw-rw-  2.0 unx      141 b- defN 19-Oct-11 16:14 secml-0.9rc2/requirements.txt
+-rw-r--r--  2.0 unx        1 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        1 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx    13910 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     9314 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      197 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml.egg-info/requires.txt
+-rw-r--r--  2.0 unx        6 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml.egg-info/top_level.txt
+-rw-rw-rw-  2.0 unx        7 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/VERSION
+-rw-rw-rw-  2.0 unx      181 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/test_simple.py
+-rw-rw-rw-  2.0 unx      614 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/secml.conf
+-rw-rw-rw-  2.0 unx     5018 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/__init__.py
+-rw-rw-rw-  2.0 unx    10562 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/settings.py
+-rw-rw-rw-  2.0 unx     1368 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/_globals.py
+-rw-rw-rw-  2.0 unx    74225 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/array/c_sparse.py
+-rw-rw-rw-  2.0 unx       28 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/array/__init__.py
+-rw-rw-rw-  2.0 unx     2678 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/array/array_utils.py
+-rw-rw-rw-  2.0 unx    73348 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/array/c_dense.py
+-rw-rw-rw-  2.0 unx   179872 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/array/c_array.py
+-rw-rw-rw-  2.0 unx    20535 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/array/c_array_interface.py
+-rwxrwxrwx  2.0 unx     6995 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/c_dataset_header.py
+-rwxrwxrwx  2.0 unx       77 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/__init__.py
+-rwxrwxrwx  2.0 unx    13538 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/c_dataset.py
+-rw-rw-rw-  2.0 unx     2740 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/c_dataset_pytorch.py
+-rw-rw-rw-  2.0 unx     1036 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/data_utils.py
+-rw-rw-rw-  2.0 unx     2781 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/splitter/c_datasplitter.py
+-rw-rw-rw-  2.0 unx     3058 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/splitter/c_datasplitter_stratkfold.py
+-rw-rw-rw-  2.0 unx     5313 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/splitter/c_train_test_split.py
+-rw-rw-rw-  2.0 unx      487 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/splitter/__init__.py
+-rw-rw-rw-  2.0 unx     7106 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/splitter/c_chronological_splitter.py
+-rw-rw-rw-  2.0 unx     2821 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/splitter/c_datasplitter_kfold.py
+-rw-rw-rw-  2.0 unx     6640 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/splitter/c_datasplitter_openworld.py
+-rw-rw-rw-  2.0 unx     3548 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/splitter/c_datasplitter_labelkfold.py
+-rw-rw-rw-  2.0 unx     4377 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/splitter/c_datasplitter_shuffle.py
+-rw-rw-rw-  2.0 unx     1616 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/selection/c_ps_random.py
+-rw-rw-rw-  2.0 unx     2266 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/selection/c_prototypes_selector.py
+-rw-rw-rw-  2.0 unx     1932 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/selection/c_ps_border.py
+-rw-rw-rw-  2.0 unx     2493 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/selection/c_ps_kmedians.py
+-rw-rw-rw-  2.0 unx      238 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/selection/__init__.py
+-rw-rw-rw-  2.0 unx     2140 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/selection/c_ps_spanning.py
+-rw-rw-rw-  2.0 unx     1929 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/selection/c_ps_center.py
+-rw-rw-rw-  2.0 unx     2171 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/loader/c_dataloader.py
+-rw-rw-rw-  2.0 unx     8668 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/loader/c_dataloader_icubworld.py
+-rw-rw-rw-  2.0 unx     4716 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/loader/c_dataloader_imgclients.py
+-rw-rw-rw-  2.0 unx      930 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/loader/c_dataloader_pytorch.py
+-rw-rw-rw-  2.0 unx     2218 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/loader/loader_utils.py
+-rw-rw-rw-  2.0 unx    12836 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/loader/c_dataloader_cifar.py
+-rw-rw-rw-  2.0 unx     7043 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/loader/c_dataloader_imgfolders.py
+-rw-rw-rw-  2.0 unx      620 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/loader/__init__.py
+-rw-rw-rw-  2.0 unx     7272 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/loader/c_dataloader_mnist.py
+-rw-rw-rw-  2.0 unx     7150 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/loader/c_dataloader_svmlight.py
+-rwxrwxrwx  2.0 unx    26623 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/loader/c_dataloader_sklearn.py
+-rw-rw-rw-  2.0 unx     3223 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/data/loader/c_dataloader_lfw.py
+-rw-rw-rw-  2.0 unx       35 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/__init__.py
+-rwxrwxrwx  2.0 unx       79 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/attacks/__init__.py
+-rw-rw-rw-  2.0 unx    13279 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/attacks/c_attack.py
+-rw-rw-rw-  2.0 unx     5442 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/attacks/evasion/c_attack_evasion_pgd.py
+-rw-rw-rw-  2.0 unx     4765 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/attacks/evasion/c_attack_evasion.py
+-rw-rw-rw-  2.0 unx      154 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/attacks/evasion/__init__.py
+-rw-rw-rw-  2.0 unx    16335 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/attacks/evasion/c_attack_evasion_pgd_ls.py
+-rw-rw-rw-  2.0 unx    11259 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/attacks/poisoning/c_attack_poisoning_svm.py
+-rw-rw-rw-  2.0 unx     7099 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/attacks/poisoning/c_attack_poisoning_logistic_regression.py
+-rw-rw-rw-  2.0 unx      258 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/attacks/poisoning/__init__.py
+-rw-rw-rw-  2.0 unx     7060 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/attacks/poisoning/c_attack_poisoning_ridge.py
+-rw-rw-rw-  2.0 unx    23838 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/attacks/poisoning/c_attack_poisoning.py
+-rw-rw-rw-  2.0 unx       75 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/seceval/__init__.py
+-rw-rw-rw-  2.0 unx     5547 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/seceval/c_sec_eval_data.py
+-rw-rw-rw-  2.0 unx     6421 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/adv/seceval/c_sec_eval.py
+-rw-rw-rw-  2.0 unx     2668 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/parallel/parfor.py
+-rw-rw-rw-  2.0 unx       36 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/parallel/__init__.py
+-rw-rw-rw-  2.0 unx     1009 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/core/constants.py
+-rwxrwxrwx  2.0 unx    20185 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/core/c_creator.py
+-rwxrwxrwx  2.0 unx       32 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/core/__init__.py
+-rw-rw-rw-  2.0 unx    11210 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/core/attr_utils.py
+-rw-rw-rw-  2.0 unx      824 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/core/exceptions.py
+-rw-rw-rw-  2.0 unx     3568 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/core/decorators.py
+-rw-rw-rw-  2.0 unx     7504 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/core/type_utils.py
+-rw-rw-rw-  2.0 unx    11736 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/figure/c_figure.py
+-rw-rw-rw-  2.0 unx       30 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/figure/__init__.py
+-rw-rw-rw-  2.0 unx     1398 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/figure/_plots/plot_utils.py
+-rw-rw-rw-  2.0 unx     2934 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/figure/_plots/c_plot_classifier.py
+-rw-rw-rw-  2.0 unx     3321 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/figure/_plots/c_plot_ds.py
+-rw-rw-rw-  2.0 unx    79744 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/figure/_plots/c_plot.py
+-rw-rw-rw-  2.0 unx    12154 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/figure/_plots/c_plot_metric.py
+-rw-rw-rw-  2.0 unx     5691 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/figure/_plots/c_plot_sec_eval.py
+-rw-rw-rw-  2.0 unx     1380 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/figure/_plots/c_plot_constraint.py
+-rw-rw-rw-  2.0 unx      312 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/figure/_plots/__init__.py
+-rw-rw-rw-  2.0 unx     8318 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/figure/_plots/c_plot_fun.py
+-rw-rw-rw-  2.0 unx     1328 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/figure/_plots/c_plot_stats.py
+-rwxrwxrwx  2.0 unx       19 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/__init__.py
+-rw-rw-rw-  2.0 unx     7143 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/optimizers/c_optimizer_scipy.py
+-rw-rw-rw-  2.0 unx     5509 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/optimizers/c_optimizer_pgd.py
+-rw-rw-rw-  2.0 unx      174 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/optimizers/__init__.py
+-rw-rw-rw-  2.0 unx     5577 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/optimizers/c_optimizer.py
+-rw-rw-rw-  2.0 unx    11340 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/optimizers/c_optimizer_pgd_ls.py
+-rw-rw-rw-  2.0 unx     1399 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/optimizers/line_search/c_line_search.py
+-rw-rw-rw-  2.0 unx       91 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/optimizers/line_search/__init__.py
+-rw-rw-rw-  2.0 unx    12701 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/optimizers/line_search/c_line_search_bisect.py
+-rw-rw-rw-  2.0 unx     2589 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/function/c_function_3hcamel.py
+-rw-rw-rw-  2.0 unx     3228 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/function/c_function_rosenbrock.py
+-rw-rw-rw-  2.0 unx     1263 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/function/c_function_linear.py
+-rw-rw-rw-  2.0 unx     2954 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/function/c_function_beale.py
+-rw-rw-rw-  2.0 unx      343 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/function/__init__.py
+-rw-rw-rw-  2.0 unx    10076 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/function/c_function.py
+-rw-rw-rw-  2.0 unx     2814 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/function/c_function_mccormick.py
+-rw-rw-rw-  2.0 unx     1772 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/function/c_function_quadratic.py
+-rw-rw-rw-  2.0 unx     5673 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/constraints/c_constraint_l1.py
+-rw-rw-rw-  2.0 unx     2708 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/constraints/c_constraint_l2.py
+-rw-rw-rw-  2.0 unx      169 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/constraints/__init__.py
+-rw-rw-rw-  2.0 unx     4483 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/constraints/c_constraint.py
+-rw-rw-rw-  2.0 unx     7633 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/optim/constraints/c_constraint_box.py
+-rw-rw-rw-  2.0 unx     3537 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/utils/download_utils.py
+-rw-rw-rw-  2.0 unx     7620 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/utils/dict_utils.py
+-rwxrwxrwx  2.0 unx    16782 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/utils/c_log.py
+-rw-rw-rw-  2.0 unx     4981 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/utils/mixed_utils.py
+-rw-rw-rw-  2.0 unx      982 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/utils/list_utils.py
+-rwxrwxrwx  2.0 unx      209 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/utils/__init__.py
+-rwxrwxrwx  2.0 unx    12948 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/utils/c_file_manager.py
+-rw-rw-rw-  2.0 unx     1926 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/utils/pickle_utils.py
+-rw-rw-rw-  2.0 unx       23 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/__init__.py
+-rw-rw-rw-  2.0 unx     1460 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/clf_utils.py
+-rw-rw-rw-  2.0 unx     5261 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/c_classifier_kde.py
+-rwxrwxrwx  2.0 unx     4507 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/c_classifier_linear.py
+-rwxrwxrwx  2.0 unx    11461 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/c_classifier.py
+-rwxrwxrwx  2.0 unx      911 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/__init__.py
+-rw-rw-rw-  2.0 unx     5453 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/c_classifier_mcs_linear.py
+-rw-rw-rw-  2.0 unx     1347 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_kde.py
+-rw-rw-rw-  2.0 unx     5434 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_linear.py
+-rw-rw-rw-  2.0 unx     1986 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_logistic.py
+-rw-rw-rw-  2.0 unx     6084 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_svm.py
+-rw-rw-rw-  2.0 unx     3402 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_ridge.py
+-rw-rw-rw-  2.0 unx      690 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/gradients/__init__.py
+-rw-rw-rw-  2.0 unx     5499 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_pytorch.py
+-rw-rw-rw-  2.0 unx     2882 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_sgd.py
+-rw-rw-rw-  2.0 unx     4991 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient.py
+-rwxrwxrwx  2.0 unx     3457 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_cross_entropy.py
+-rw-rw-rw-  2.0 unx      405 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/loss/__init__.py
+-rw-rw-rw-  2.0 unx     2604 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/loss/c_softmax.py
+-rwxrwxrwx  2.0 unx     4781 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_squared.py
+-rw-rw-rw-  2.0 unx     5752 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss.py
+-rwxrwxrwx  2.0 unx     4170 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_logistic.py
+-rwxrwxrwx  2.0 unx     6353 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_hinge.py
+-rwxrwxrwx  2.0 unx     5501 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_epsilon_insensitive.py
+-rw-rw-rw-  2.0 unx     1579 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/reject/mixin_classifier_gradient_reject_threshold.py
+-rw-rw-rw-  2.0 unx      121 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/reject/__init__.py
+-rw-rw-rw-  2.0 unx     2388 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/reject/c_classifier_reject.py
+-rw-rw-rw-  2.0 unx     9447 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/reject/c_classifier_reject_threshold.py
+-rw-rw-rw-  2.0 unx     2572 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_knn.py
+-rw-rw-rw-  2.0 unx     3769 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_sklearn.py
+-rw-rw-rw-  2.0 unx     3451 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_logistic.py
+-rwxrwxrwx  2.0 unx    14782 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_svm.py
+-rw-rw-rw-  2.0 unx     9772 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_sgd.py
+-rw-rw-rw-  2.0 unx       13 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/sklearn/__init__.py
+-rw-rw-rw-  2.0 unx     2246 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_nearest_centroid.py
+-rw-rw-rw-  2.0 unx     1303 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_random_forest.py
+-rw-rw-rw-  2.0 unx     1179 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_decision_tree.py
+-rw-rw-rw-  2.0 unx     6996 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_ridge.py
+-rw-rw-rw-  2.0 unx       13 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/pytorch/__init__.py
+-rw-rw-rw-  2.0 unx    19384 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/pytorch/c_classifier_pytorch.py
+-rw-rw-rw-  2.0 unx     5362 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/multiclass/c_classifier_multi_ova.py
+-rw-rw-rw-  2.0 unx     1292 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/multiclass/mixin_classifier_gradient_multiclass_ova.py
+-rw-rw-rw-  2.0 unx      115 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/multiclass/__init__.py
+-rw-rw-rw-  2.0 unx    10540 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/multiclass/c_classifier_multi.py
+-rwxrwxrwx  2.0 unx      922 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/regularizer/c_regularizer_l1.py
+-rw-rw-rw-  2.0 unx      725 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/regularizer/c_regularizer.py
+-rwxrwxrwx  2.0 unx     1565 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/regularizer/c_regularizer_elastic_net.py
+-rw-rw-rw-  2.0 unx      192 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/regularizer/__init__.py
+-rwxrwxrwx  2.0 unx      918 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/classifiers/regularizer/c_regularizer_l2.py
+-rw-rw-rw-  2.0 unx       93 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/features/__init__.py
+-rw-rw-rw-  2.0 unx     7796 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/features/c_preprocess.py
+-rw-rw-rw-  2.0 unx     6420 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer_minmax.py
+-rw-rw-rw-  2.0 unx      475 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer.py
+-rw-rw-rw-  2.0 unx     4422 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer_linear.py
+-rw-rw-rw-  2.0 unx      249 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/features/normalization/__init__.py
+-rw-rw-rw-  2.0 unx     8106 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer_mean_std.py
+-rw-rw-rw-  2.0 unx     7388 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer_unitnorm.py
+-rw-rw-rw-  2.0 unx       96 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/features/reduction/__init__.py
+-rw-rw-rw-  2.0 unx    10398 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/features/reduction/c_reducer_pca.py
+-rw-rw-rw-  2.0 unx     5908 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/features/reduction/c_reducer_lda.py
+-rw-rw-rw-  2.0 unx      390 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/features/reduction/c_reducer.py
+-rwxrwxrwx  2.0 unx     5213 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/c_perfevaluator_xval.py
+-rwxrwxrwx  2.0 unx     6537 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/c_perfevaluator_xval_multiclass.py
+-rw-rw-rw-  2.0 unx      171 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/__init__.py
+-rwxrwxrwx  2.0 unx     7568 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/c_perfevaluator.py
+-rw-rw-rw-  2.0 unx      902 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_confusion_matrix.py
+-rw-rw-rw-  2.0 unx     2092 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_tpr_at_fpr.py
+-rw-rw-rw-  2.0 unx     2144 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_auc_wmw.py
+-rw-rw-rw-  2.0 unx     1397 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_mae.py
+-rw-rw-rw-  2.0 unx     1392 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_mse.py
+-rw-rw-rw-  2.0 unx     1448 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_test_error.py
+-rw-rw-rw-  2.0 unx      650 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/__init__.py
+-rw-rw-rw-  2.0 unx     2652 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_pauc.py
+-rwxrwxrwx  2.0 unx     3377 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_metric.py
+-rw-rw-rw-  2.0 unx     1711 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_precision.py
+-rw-rw-rw-  2.0 unx    15874 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_roc.py
+-rw-rw-rw-  2.0 unx     1758 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_auc.py
+-rw-rw-rw-  2.0 unx     1744 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_recall.py
+-rw-rw-rw-  2.0 unx     1402 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_accuracy.py
+-rw-rw-rw-  2.0 unx     1751 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_f1.py
+-rw-rw-rw-  2.0 unx     3389 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/stats/c_density_estimation.py
+-rw-rw-rw-  2.0 unx      112 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/stats/__init__.py
+-rw-rw-rw-  2.0 unx     1852 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/stats/c_distribution_gaussian.py
+-rwxrwxrwx  2.0 unx     5713 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/kernel/c_kernel_poly.py
+-rwxrwxrwx  2.0 unx     1784 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/kernel/c_kernel_hamming.py
+-rwxrwxrwx  2.0 unx     6033 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/kernel/c_kernel_euclidean.py
+-rwxrwxrwx  2.0 unx     5720 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/kernel/c_kernel_rbf.py
+-rw-rw-rw-  2.0 unx     5404 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/kernel/c_kernel_laplacian.py
+-rwxrwxrwx  2.0 unx      415 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/kernel/__init__.py
+-rw-rw-rw-  2.0 unx     3526 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/kernel/c_kernel_chebyshev_distance.py
+-rwxrwxrwx  2.0 unx     3295 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/kernel/c_kernel_linear.py
+-rwxrwxrwx  2.0 unx     2794 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/kernel/c_kernel_histintersect.py
+-rwxrwxrwx  2.0 unx     7025 b- defN 19-Oct-11 16:14 secml-0.9rc2/src/secml/ml/kernel/c_kernel.py
+-rw-rw-rw-  2.0 unx     1166 b- defN 19-Oct-11 16:14 secml-0.9rc2/update/0.8-to-0.9.md
+218 files, 1350255 bytes uncompressed, 362157 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -1,655 +1,655 @@
-Filename: secml-0.9/PKG-INFO
+Filename: secml-0.9rc2/PKG-INFO
 Comment: 
 
-Filename: secml-0.9/setup.py
+Filename: secml-0.9rc2/setup.py
 Comment: 
 
-Filename: secml-0.9/README.md
+Filename: secml-0.9rc2/README.md
 Comment: 
 
-Filename: secml-0.9/setup.cfg
+Filename: secml-0.9rc2/setup.cfg
 Comment: 
 
-Filename: secml-0.9/CHANGELOG.md
+Filename: secml-0.9rc2/CHANGELOG.md
 Comment: 
 
-Filename: secml-0.9/MANIFEST.in
+Filename: secml-0.9rc2/MANIFEST.in
 Comment: 
 
-Filename: secml-0.9/requirements.txt
+Filename: secml-0.9rc2/requirements.txt
 Comment: 
 
-Filename: secml-0.9/src/secml.egg-info/dependency_links.txt
+Filename: secml-0.9rc2/src/secml.egg-info/dependency_links.txt
 Comment: 
 
-Filename: secml-0.9/src/secml.egg-info/not-zip-safe
+Filename: secml-0.9rc2/src/secml.egg-info/not-zip-safe
 Comment: 
 
-Filename: secml-0.9/src/secml.egg-info/PKG-INFO
+Filename: secml-0.9rc2/src/secml.egg-info/PKG-INFO
 Comment: 
 
-Filename: secml-0.9/src/secml.egg-info/SOURCES.txt
+Filename: secml-0.9rc2/src/secml.egg-info/SOURCES.txt
 Comment: 
 
-Filename: secml-0.9/src/secml.egg-info/requires.txt
+Filename: secml-0.9rc2/src/secml.egg-info/requires.txt
 Comment: 
 
-Filename: secml-0.9/src/secml.egg-info/top_level.txt
+Filename: secml-0.9rc2/src/secml.egg-info/top_level.txt
 Comment: 
 
-Filename: secml-0.9/src/secml/VERSION
+Filename: secml-0.9rc2/src/secml/VERSION
 Comment: 
 
-Filename: secml-0.9/src/secml/test_simple.py
+Filename: secml-0.9rc2/src/secml/test_simple.py
 Comment: 
 
-Filename: secml-0.9/src/secml/secml.conf
+Filename: secml-0.9rc2/src/secml/secml.conf
 Comment: 
 
-Filename: secml-0.9/src/secml/__init__.py
+Filename: secml-0.9rc2/src/secml/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/settings.py
+Filename: secml-0.9rc2/src/secml/settings.py
 Comment: 
 
-Filename: secml-0.9/src/secml/_globals.py
+Filename: secml-0.9rc2/src/secml/_globals.py
 Comment: 
 
-Filename: secml-0.9/src/secml/array/c_sparse.py
+Filename: secml-0.9rc2/src/secml/array/c_sparse.py
 Comment: 
 
-Filename: secml-0.9/src/secml/array/__init__.py
+Filename: secml-0.9rc2/src/secml/array/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/array/array_utils.py
+Filename: secml-0.9rc2/src/secml/array/array_utils.py
 Comment: 
 
-Filename: secml-0.9/src/secml/array/c_dense.py
+Filename: secml-0.9rc2/src/secml/array/c_dense.py
 Comment: 
 
-Filename: secml-0.9/src/secml/array/c_array.py
+Filename: secml-0.9rc2/src/secml/array/c_array.py
 Comment: 
 
-Filename: secml-0.9/src/secml/array/c_array_interface.py
+Filename: secml-0.9rc2/src/secml/array/c_array_interface.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/c_dataset_header.py
+Filename: secml-0.9rc2/src/secml/data/c_dataset_header.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/__init__.py
+Filename: secml-0.9rc2/src/secml/data/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/c_dataset.py
+Filename: secml-0.9rc2/src/secml/data/c_dataset.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/c_dataset_pytorch.py
+Filename: secml-0.9rc2/src/secml/data/c_dataset_pytorch.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/data_utils.py
+Filename: secml-0.9rc2/src/secml/data/data_utils.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/splitter/c_datasplitter.py
+Filename: secml-0.9rc2/src/secml/data/splitter/c_datasplitter.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/splitter/c_datasplitter_stratkfold.py
+Filename: secml-0.9rc2/src/secml/data/splitter/c_datasplitter_stratkfold.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/splitter/c_train_test_split.py
+Filename: secml-0.9rc2/src/secml/data/splitter/c_train_test_split.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/splitter/__init__.py
+Filename: secml-0.9rc2/src/secml/data/splitter/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/splitter/c_chronological_splitter.py
+Filename: secml-0.9rc2/src/secml/data/splitter/c_chronological_splitter.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/splitter/c_datasplitter_kfold.py
+Filename: secml-0.9rc2/src/secml/data/splitter/c_datasplitter_kfold.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/splitter/c_datasplitter_openworld.py
+Filename: secml-0.9rc2/src/secml/data/splitter/c_datasplitter_openworld.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/splitter/c_datasplitter_labelkfold.py
+Filename: secml-0.9rc2/src/secml/data/splitter/c_datasplitter_labelkfold.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/splitter/c_datasplitter_shuffle.py
+Filename: secml-0.9rc2/src/secml/data/splitter/c_datasplitter_shuffle.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/selection/c_ps_random.py
+Filename: secml-0.9rc2/src/secml/data/selection/c_ps_random.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/selection/c_prototypes_selector.py
+Filename: secml-0.9rc2/src/secml/data/selection/c_prototypes_selector.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/selection/c_ps_border.py
+Filename: secml-0.9rc2/src/secml/data/selection/c_ps_border.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/selection/c_ps_kmedians.py
+Filename: secml-0.9rc2/src/secml/data/selection/c_ps_kmedians.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/selection/__init__.py
+Filename: secml-0.9rc2/src/secml/data/selection/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/selection/c_ps_spanning.py
+Filename: secml-0.9rc2/src/secml/data/selection/c_ps_spanning.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/selection/c_ps_center.py
+Filename: secml-0.9rc2/src/secml/data/selection/c_ps_center.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/loader/c_dataloader.py
+Filename: secml-0.9rc2/src/secml/data/loader/c_dataloader.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/loader/c_dataloader_icubworld.py
+Filename: secml-0.9rc2/src/secml/data/loader/c_dataloader_icubworld.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/loader/c_dataloader_imgclients.py
+Filename: secml-0.9rc2/src/secml/data/loader/c_dataloader_imgclients.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/loader/c_dataloader_pytorch.py
+Filename: secml-0.9rc2/src/secml/data/loader/c_dataloader_pytorch.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/loader/loader_utils.py
+Filename: secml-0.9rc2/src/secml/data/loader/loader_utils.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/loader/c_dataloader_cifar.py
+Filename: secml-0.9rc2/src/secml/data/loader/c_dataloader_cifar.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/loader/c_dataloader_imgfolders.py
+Filename: secml-0.9rc2/src/secml/data/loader/c_dataloader_imgfolders.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/loader/__init__.py
+Filename: secml-0.9rc2/src/secml/data/loader/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/loader/c_dataloader_mnist.py
+Filename: secml-0.9rc2/src/secml/data/loader/c_dataloader_mnist.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/loader/c_dataloader_svmlight.py
+Filename: secml-0.9rc2/src/secml/data/loader/c_dataloader_svmlight.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/loader/c_dataloader_sklearn.py
+Filename: secml-0.9rc2/src/secml/data/loader/c_dataloader_sklearn.py
 Comment: 
 
-Filename: secml-0.9/src/secml/data/loader/c_dataloader_lfw.py
+Filename: secml-0.9rc2/src/secml/data/loader/c_dataloader_lfw.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/__init__.py
+Filename: secml-0.9rc2/src/secml/adv/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/attacks/__init__.py
+Filename: secml-0.9rc2/src/secml/adv/attacks/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/attacks/c_attack.py
+Filename: secml-0.9rc2/src/secml/adv/attacks/c_attack.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/attacks/evasion/c_attack_evasion_pgd.py
+Filename: secml-0.9rc2/src/secml/adv/attacks/evasion/c_attack_evasion_pgd.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/attacks/evasion/c_attack_evasion.py
+Filename: secml-0.9rc2/src/secml/adv/attacks/evasion/c_attack_evasion.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/attacks/evasion/__init__.py
+Filename: secml-0.9rc2/src/secml/adv/attacks/evasion/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/attacks/evasion/c_attack_evasion_pgd_ls.py
+Filename: secml-0.9rc2/src/secml/adv/attacks/evasion/c_attack_evasion_pgd_ls.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/attacks/poisoning/c_attack_poisoning_svm.py
+Filename: secml-0.9rc2/src/secml/adv/attacks/poisoning/c_attack_poisoning_svm.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/attacks/poisoning/c_attack_poisoning_logistic_regression.py
+Filename: secml-0.9rc2/src/secml/adv/attacks/poisoning/c_attack_poisoning_logistic_regression.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/attacks/poisoning/__init__.py
+Filename: secml-0.9rc2/src/secml/adv/attacks/poisoning/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/attacks/poisoning/c_attack_poisoning_ridge.py
+Filename: secml-0.9rc2/src/secml/adv/attacks/poisoning/c_attack_poisoning_ridge.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/attacks/poisoning/c_attack_poisoning.py
+Filename: secml-0.9rc2/src/secml/adv/attacks/poisoning/c_attack_poisoning.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/seceval/__init__.py
+Filename: secml-0.9rc2/src/secml/adv/seceval/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/seceval/c_sec_eval_data.py
+Filename: secml-0.9rc2/src/secml/adv/seceval/c_sec_eval_data.py
 Comment: 
 
-Filename: secml-0.9/src/secml/adv/seceval/c_sec_eval.py
+Filename: secml-0.9rc2/src/secml/adv/seceval/c_sec_eval.py
 Comment: 
 
-Filename: secml-0.9/src/secml/parallel/parfor.py
+Filename: secml-0.9rc2/src/secml/parallel/parfor.py
 Comment: 
 
-Filename: secml-0.9/src/secml/parallel/__init__.py
+Filename: secml-0.9rc2/src/secml/parallel/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/core/constants.py
+Filename: secml-0.9rc2/src/secml/core/constants.py
 Comment: 
 
-Filename: secml-0.9/src/secml/core/c_creator.py
+Filename: secml-0.9rc2/src/secml/core/c_creator.py
 Comment: 
 
-Filename: secml-0.9/src/secml/core/__init__.py
+Filename: secml-0.9rc2/src/secml/core/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/core/attr_utils.py
+Filename: secml-0.9rc2/src/secml/core/attr_utils.py
 Comment: 
 
-Filename: secml-0.9/src/secml/core/exceptions.py
+Filename: secml-0.9rc2/src/secml/core/exceptions.py
 Comment: 
 
-Filename: secml-0.9/src/secml/core/decorators.py
+Filename: secml-0.9rc2/src/secml/core/decorators.py
 Comment: 
 
-Filename: secml-0.9/src/secml/core/type_utils.py
+Filename: secml-0.9rc2/src/secml/core/type_utils.py
 Comment: 
 
-Filename: secml-0.9/src/secml/figure/c_figure.py
+Filename: secml-0.9rc2/src/secml/figure/c_figure.py
 Comment: 
 
-Filename: secml-0.9/src/secml/figure/__init__.py
+Filename: secml-0.9rc2/src/secml/figure/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/figure/_plots/plot_utils.py
+Filename: secml-0.9rc2/src/secml/figure/_plots/plot_utils.py
 Comment: 
 
-Filename: secml-0.9/src/secml/figure/_plots/c_plot_classifier.py
+Filename: secml-0.9rc2/src/secml/figure/_plots/c_plot_classifier.py
 Comment: 
 
-Filename: secml-0.9/src/secml/figure/_plots/c_plot_ds.py
+Filename: secml-0.9rc2/src/secml/figure/_plots/c_plot_ds.py
 Comment: 
 
-Filename: secml-0.9/src/secml/figure/_plots/c_plot.py
+Filename: secml-0.9rc2/src/secml/figure/_plots/c_plot.py
 Comment: 
 
-Filename: secml-0.9/src/secml/figure/_plots/c_plot_metric.py
+Filename: secml-0.9rc2/src/secml/figure/_plots/c_plot_metric.py
 Comment: 
 
-Filename: secml-0.9/src/secml/figure/_plots/c_plot_sec_eval.py
+Filename: secml-0.9rc2/src/secml/figure/_plots/c_plot_sec_eval.py
 Comment: 
 
-Filename: secml-0.9/src/secml/figure/_plots/c_plot_constraint.py
+Filename: secml-0.9rc2/src/secml/figure/_plots/c_plot_constraint.py
 Comment: 
 
-Filename: secml-0.9/src/secml/figure/_plots/__init__.py
+Filename: secml-0.9rc2/src/secml/figure/_plots/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/figure/_plots/c_plot_fun.py
+Filename: secml-0.9rc2/src/secml/figure/_plots/c_plot_fun.py
 Comment: 
 
-Filename: secml-0.9/src/secml/figure/_plots/c_plot_stats.py
+Filename: secml-0.9rc2/src/secml/figure/_plots/c_plot_stats.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/__init__.py
+Filename: secml-0.9rc2/src/secml/optim/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/optimizers/c_optimizer_scipy.py
+Filename: secml-0.9rc2/src/secml/optim/optimizers/c_optimizer_scipy.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/optimizers/c_optimizer_pgd.py
+Filename: secml-0.9rc2/src/secml/optim/optimizers/c_optimizer_pgd.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/optimizers/__init__.py
+Filename: secml-0.9rc2/src/secml/optim/optimizers/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/optimizers/c_optimizer.py
+Filename: secml-0.9rc2/src/secml/optim/optimizers/c_optimizer.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/optimizers/c_optimizer_pgd_ls.py
+Filename: secml-0.9rc2/src/secml/optim/optimizers/c_optimizer_pgd_ls.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/optimizers/line_search/c_line_search.py
+Filename: secml-0.9rc2/src/secml/optim/optimizers/line_search/c_line_search.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/optimizers/line_search/__init__.py
+Filename: secml-0.9rc2/src/secml/optim/optimizers/line_search/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/optimizers/line_search/c_line_search_bisect.py
+Filename: secml-0.9rc2/src/secml/optim/optimizers/line_search/c_line_search_bisect.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/function/c_function_3hcamel.py
+Filename: secml-0.9rc2/src/secml/optim/function/c_function_3hcamel.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/function/c_function_rosenbrock.py
+Filename: secml-0.9rc2/src/secml/optim/function/c_function_rosenbrock.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/function/c_function_linear.py
+Filename: secml-0.9rc2/src/secml/optim/function/c_function_linear.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/function/c_function_beale.py
+Filename: secml-0.9rc2/src/secml/optim/function/c_function_beale.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/function/__init__.py
+Filename: secml-0.9rc2/src/secml/optim/function/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/function/c_function.py
+Filename: secml-0.9rc2/src/secml/optim/function/c_function.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/function/c_function_mccormick.py
+Filename: secml-0.9rc2/src/secml/optim/function/c_function_mccormick.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/function/c_function_quadratic.py
+Filename: secml-0.9rc2/src/secml/optim/function/c_function_quadratic.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/constraints/c_constraint_l1.py
+Filename: secml-0.9rc2/src/secml/optim/constraints/c_constraint_l1.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/constraints/c_constraint_l2.py
+Filename: secml-0.9rc2/src/secml/optim/constraints/c_constraint_l2.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/constraints/__init__.py
+Filename: secml-0.9rc2/src/secml/optim/constraints/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/constraints/c_constraint.py
+Filename: secml-0.9rc2/src/secml/optim/constraints/c_constraint.py
 Comment: 
 
-Filename: secml-0.9/src/secml/optim/constraints/c_constraint_box.py
+Filename: secml-0.9rc2/src/secml/optim/constraints/c_constraint_box.py
 Comment: 
 
-Filename: secml-0.9/src/secml/utils/download_utils.py
+Filename: secml-0.9rc2/src/secml/utils/download_utils.py
 Comment: 
 
-Filename: secml-0.9/src/secml/utils/dict_utils.py
+Filename: secml-0.9rc2/src/secml/utils/dict_utils.py
 Comment: 
 
-Filename: secml-0.9/src/secml/utils/c_log.py
+Filename: secml-0.9rc2/src/secml/utils/c_log.py
 Comment: 
 
-Filename: secml-0.9/src/secml/utils/mixed_utils.py
+Filename: secml-0.9rc2/src/secml/utils/mixed_utils.py
 Comment: 
 
-Filename: secml-0.9/src/secml/utils/list_utils.py
+Filename: secml-0.9rc2/src/secml/utils/list_utils.py
 Comment: 
 
-Filename: secml-0.9/src/secml/utils/__init__.py
+Filename: secml-0.9rc2/src/secml/utils/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/utils/c_file_manager.py
+Filename: secml-0.9rc2/src/secml/utils/c_file_manager.py
 Comment: 
 
-Filename: secml-0.9/src/secml/utils/pickle_utils.py
+Filename: secml-0.9rc2/src/secml/utils/pickle_utils.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/clf_utils.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/clf_utils.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/c_classifier_kde.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/c_classifier_kde.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/c_classifier_linear.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/c_classifier_linear.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/c_classifier.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/c_classifier.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/c_classifier_mcs_linear.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/c_classifier_mcs_linear.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_kde.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_kde.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_linear.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_linear.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_logistic.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_logistic.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_svm.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_svm.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_ridge.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_ridge.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/gradients/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/gradients/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_pytorch.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_pytorch.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_sgd.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_sgd.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/loss/c_loss_cross_entropy.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_cross_entropy.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/loss/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/loss/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/loss/c_softmax.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/loss/c_softmax.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/loss/c_loss_squared.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_squared.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/loss/c_loss.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/loss/c_loss_logistic.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_logistic.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/loss/c_loss_hinge.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_hinge.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/loss/c_loss_epsilon_insensitive.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_epsilon_insensitive.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/reject/mixin_classifier_gradient_reject_threshold.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/reject/mixin_classifier_gradient_reject_threshold.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/reject/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/reject/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/reject/c_classifier_reject.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/reject/c_classifier_reject.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/reject/c_classifier_reject_threshold.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/reject/c_classifier_reject_threshold.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_knn.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_knn.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_sklearn.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_sklearn.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_logistic.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_logistic.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_svm.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_svm.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_sgd.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_sgd.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/sklearn/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/sklearn/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_nearest_centroid.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_nearest_centroid.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_random_forest.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_random_forest.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_decision_tree.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_decision_tree.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_ridge.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_ridge.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/pytorch/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/pytorch/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/pytorch/c_classifier_pytorch.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/pytorch/c_classifier_pytorch.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/multiclass/c_classifier_multi_ova.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/multiclass/c_classifier_multi_ova.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/multiclass/mixin_classifier_gradient_multiclass_ova.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/multiclass/mixin_classifier_gradient_multiclass_ova.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/multiclass/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/multiclass/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/multiclass/c_classifier_multi.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/multiclass/c_classifier_multi.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/regularizer/c_regularizer_l1.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/regularizer/c_regularizer_l1.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/regularizer/c_regularizer.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/regularizer/c_regularizer.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/regularizer/c_regularizer_elastic_net.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/regularizer/c_regularizer_elastic_net.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/regularizer/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/regularizer/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/classifiers/regularizer/c_regularizer_l2.py
+Filename: secml-0.9rc2/src/secml/ml/classifiers/regularizer/c_regularizer_l2.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/features/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/features/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/features/c_preprocess.py
+Filename: secml-0.9rc2/src/secml/ml/features/c_preprocess.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/features/normalization/c_normalizer_minmax.py
+Filename: secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer_minmax.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/features/normalization/c_normalizer.py
+Filename: secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/features/normalization/c_normalizer_linear.py
+Filename: secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer_linear.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/features/normalization/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/features/normalization/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/features/normalization/c_normalizer_mean_std.py
+Filename: secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer_mean_std.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/features/normalization/c_normalizer_unitnorm.py
+Filename: secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer_unitnorm.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/features/reduction/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/features/reduction/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/features/reduction/c_reducer_pca.py
+Filename: secml-0.9rc2/src/secml/ml/features/reduction/c_reducer_pca.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/features/reduction/c_reducer_lda.py
+Filename: secml-0.9rc2/src/secml/ml/features/reduction/c_reducer_lda.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/features/reduction/c_reducer.py
+Filename: secml-0.9rc2/src/secml/ml/features/reduction/c_reducer.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/c_perfevaluator_xval.py
+Filename: secml-0.9rc2/src/secml/ml/peval/c_perfevaluator_xval.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/c_perfevaluator_xval_multiclass.py
+Filename: secml-0.9rc2/src/secml/ml/peval/c_perfevaluator_xval_multiclass.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/peval/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/c_perfevaluator.py
+Filename: secml-0.9rc2/src/secml/ml/peval/c_perfevaluator.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_confusion_matrix.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_confusion_matrix.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_metric_tpr_at_fpr.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_tpr_at_fpr.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_metric_auc_wmw.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_auc_wmw.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_metric_mae.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_mae.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_metric_mse.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_mse.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_metric_test_error.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_test_error.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_metric_pauc.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_pauc.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_metric.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_metric.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_metric_precision.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_precision.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_roc.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_roc.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_metric_auc.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_auc.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_metric_recall.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_recall.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_metric_accuracy.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_accuracy.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/peval/metrics/c_metric_f1.py
+Filename: secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_f1.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/stats/c_density_estimation.py
+Filename: secml-0.9rc2/src/secml/ml/stats/c_density_estimation.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/stats/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/stats/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/stats/c_distribution_gaussian.py
+Filename: secml-0.9rc2/src/secml/ml/stats/c_distribution_gaussian.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/kernel/c_kernel_poly.py
+Filename: secml-0.9rc2/src/secml/ml/kernel/c_kernel_poly.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/kernel/c_kernel_hamming.py
+Filename: secml-0.9rc2/src/secml/ml/kernel/c_kernel_hamming.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/kernel/c_kernel_euclidean.py
+Filename: secml-0.9rc2/src/secml/ml/kernel/c_kernel_euclidean.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/kernel/c_kernel_rbf.py
+Filename: secml-0.9rc2/src/secml/ml/kernel/c_kernel_rbf.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/kernel/c_kernel_laplacian.py
+Filename: secml-0.9rc2/src/secml/ml/kernel/c_kernel_laplacian.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/kernel/__init__.py
+Filename: secml-0.9rc2/src/secml/ml/kernel/__init__.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/kernel/c_kernel_chebyshev_distance.py
+Filename: secml-0.9rc2/src/secml/ml/kernel/c_kernel_chebyshev_distance.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/kernel/c_kernel_linear.py
+Filename: secml-0.9rc2/src/secml/ml/kernel/c_kernel_linear.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/kernel/c_kernel_histintersect.py
+Filename: secml-0.9rc2/src/secml/ml/kernel/c_kernel_histintersect.py
 Comment: 
 
-Filename: secml-0.9/src/secml/ml/kernel/c_kernel.py
+Filename: secml-0.9rc2/src/secml/ml/kernel/c_kernel.py
 Comment: 
 
-Filename: secml-0.9/update/0.8-to-0.9.md
+Filename: secml-0.9rc2/update/0.8-to-0.9.md
 Comment: 
 
 Zip file comment:
```

## Comparing `secml-0.9/PKG-INFO` & `secml-0.9rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: secml
-Version: 0.9
+Version: 0.9rc2
 Summary: A library for Secure and Explainable Machine Learning
 Home-page: https://secml.gitlab.io
 Maintainer: Marco Melis
 Maintainer-email: marco.melis@unica.it
 License: Apache License 2.0
 Download-URL: https://pypi.python.org/pypi/secml#files
-Project-URL: Bug Tracker, https://gitlab.com/secml/secml/issues
 Project-URL: Source Code, https://gitlab.com/secml/secml
+Project-URL: Bug Tracker, https://gitlab.com/secml/secml/issues
 Description: # SecML: A library for Secure and Explainable Machine Learning
         
         SecML is an open-source Python library for the **security evaluation** of
         Machine Learning (ML) algorithms.
         
         It comes with a set of powerful features:
         - **Dense/Sparse data support.** We provide full, transparent support for both
```

## Comparing `secml-0.9/setup.py` & `secml-0.9rc2/setup.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/README.md` & `secml-0.9rc2/README.md`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml.egg-info/PKG-INFO` & `secml-0.9rc2/src/secml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: secml
-Version: 0.9
+Version: 0.9rc2
 Summary: A library for Secure and Explainable Machine Learning
 Home-page: https://secml.gitlab.io
 Maintainer: Marco Melis
 Maintainer-email: marco.melis@unica.it
 License: Apache License 2.0
 Download-URL: https://pypi.python.org/pypi/secml#files
-Project-URL: Bug Tracker, https://gitlab.com/secml/secml/issues
 Project-URL: Source Code, https://gitlab.com/secml/secml
+Project-URL: Bug Tracker, https://gitlab.com/secml/secml/issues
 Description: # SecML: A library for Secure and Explainable Machine Learning
         
         SecML is an open-source Python library for the **security evaluation** of
         Machine Learning (ML) algorithms.
         
         It comes with a set of powerful features:
         - **Dense/Sparse data support.** We provide full, transparent support for both
```

## Comparing `secml-0.9/src/secml.egg-info/SOURCES.txt` & `secml-0.9rc2/src/secml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/secml.conf` & `secml-0.9rc2/src/secml/secml.conf`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/__init__.py` & `secml-0.9rc2/src/secml/__init__.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/settings.py` & `secml-0.9rc2/src/secml/settings.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/_globals.py` & `secml-0.9rc2/src/secml/_globals.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/array/c_sparse.py` & `secml-0.9rc2/src/secml/array/c_sparse.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/array/array_utils.py` & `secml-0.9rc2/src/secml/array/array_utils.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/array/c_dense.py` & `secml-0.9rc2/src/secml/array/c_dense.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/array/c_array.py` & `secml-0.9rc2/src/secml/array/c_array.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/array/c_array_interface.py` & `secml-0.9rc2/src/secml/array/c_array_interface.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/c_dataset_header.py` & `secml-0.9rc2/src/secml/data/c_dataset_header.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/c_dataset.py` & `secml-0.9rc2/src/secml/data/c_dataset.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/c_dataset_pytorch.py` & `secml-0.9rc2/src/secml/data/c_dataset_pytorch.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/data_utils.py` & `secml-0.9rc2/src/secml/data/data_utils.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/splitter/c_datasplitter.py` & `secml-0.9rc2/src/secml/data/splitter/c_datasplitter.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/splitter/c_datasplitter_stratkfold.py` & `secml-0.9rc2/src/secml/data/splitter/c_datasplitter_stratkfold.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/splitter/c_train_test_split.py` & `secml-0.9rc2/src/secml/data/splitter/c_train_test_split.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/splitter/c_chronological_splitter.py` & `secml-0.9rc2/src/secml/data/splitter/c_chronological_splitter.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/splitter/c_datasplitter_kfold.py` & `secml-0.9rc2/src/secml/data/splitter/c_datasplitter_kfold.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/splitter/c_datasplitter_openworld.py` & `secml-0.9rc2/src/secml/data/splitter/c_datasplitter_openworld.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/splitter/c_datasplitter_labelkfold.py` & `secml-0.9rc2/src/secml/data/splitter/c_datasplitter_labelkfold.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/splitter/c_datasplitter_shuffle.py` & `secml-0.9rc2/src/secml/data/splitter/c_datasplitter_shuffle.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/selection/c_ps_random.py` & `secml-0.9rc2/src/secml/data/selection/c_ps_random.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/selection/c_prototypes_selector.py` & `secml-0.9rc2/src/secml/data/selection/c_prototypes_selector.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/selection/c_ps_border.py` & `secml-0.9rc2/src/secml/data/selection/c_ps_border.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/selection/c_ps_kmedians.py` & `secml-0.9rc2/src/secml/data/selection/c_ps_kmedians.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/selection/c_ps_spanning.py` & `secml-0.9rc2/src/secml/data/selection/c_ps_spanning.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/selection/c_ps_center.py` & `secml-0.9rc2/src/secml/data/selection/c_ps_center.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/loader/c_dataloader.py` & `secml-0.9rc2/src/secml/data/loader/c_dataloader.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/loader/c_dataloader_icubworld.py` & `secml-0.9rc2/src/secml/data/loader/c_dataloader_icubworld.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/loader/c_dataloader_imgclients.py` & `secml-0.9rc2/src/secml/data/loader/c_dataloader_imgclients.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/loader/c_dataloader_pytorch.py` & `secml-0.9rc2/src/secml/data/loader/c_dataloader_pytorch.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/loader/loader_utils.py` & `secml-0.9rc2/src/secml/data/loader/loader_utils.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/loader/c_dataloader_cifar.py` & `secml-0.9rc2/src/secml/data/loader/c_dataloader_cifar.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/loader/c_dataloader_imgfolders.py` & `secml-0.9rc2/src/secml/data/loader/c_dataloader_imgfolders.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/loader/__init__.py` & `secml-0.9rc2/src/secml/data/loader/__init__.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/loader/c_dataloader_mnist.py` & `secml-0.9rc2/src/secml/data/loader/c_dataloader_mnist.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/loader/c_dataloader_svmlight.py` & `secml-0.9rc2/src/secml/data/loader/c_dataloader_svmlight.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/loader/c_dataloader_sklearn.py` & `secml-0.9rc2/src/secml/data/loader/c_dataloader_sklearn.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/data/loader/c_dataloader_lfw.py` & `secml-0.9rc2/src/secml/data/loader/c_dataloader_lfw.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/adv/attacks/c_attack.py` & `secml-0.9rc2/src/secml/adv/attacks/c_attack.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/adv/attacks/evasion/c_attack_evasion_pgd.py` & `secml-0.9rc2/src/secml/adv/attacks/evasion/c_attack_evasion_pgd.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/adv/attacks/evasion/c_attack_evasion.py` & `secml-0.9rc2/src/secml/adv/attacks/evasion/c_attack_evasion.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/adv/attacks/evasion/c_attack_evasion_pgd_ls.py` & `secml-0.9rc2/src/secml/adv/attacks/evasion/c_attack_evasion_pgd_ls.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/adv/attacks/poisoning/c_attack_poisoning_svm.py` & `secml-0.9rc2/src/secml/adv/attacks/poisoning/c_attack_poisoning_svm.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/adv/attacks/poisoning/c_attack_poisoning_logistic_regression.py` & `secml-0.9rc2/src/secml/adv/attacks/poisoning/c_attack_poisoning_logistic_regression.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/adv/attacks/poisoning/c_attack_poisoning_ridge.py` & `secml-0.9rc2/src/secml/adv/attacks/poisoning/c_attack_poisoning_ridge.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/adv/attacks/poisoning/c_attack_poisoning.py` & `secml-0.9rc2/src/secml/adv/attacks/poisoning/c_attack_poisoning.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/adv/seceval/c_sec_eval_data.py` & `secml-0.9rc2/src/secml/adv/seceval/c_sec_eval_data.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/adv/seceval/c_sec_eval.py` & `secml-0.9rc2/src/secml/adv/seceval/c_sec_eval.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/parallel/parfor.py` & `secml-0.9rc2/src/secml/parallel/parfor.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/core/constants.py` & `secml-0.9rc2/src/secml/core/constants.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/core/c_creator.py` & `secml-0.9rc2/src/secml/core/c_creator.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/core/attr_utils.py` & `secml-0.9rc2/src/secml/core/attr_utils.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/core/exceptions.py` & `secml-0.9rc2/src/secml/core/exceptions.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/core/decorators.py` & `secml-0.9rc2/src/secml/core/decorators.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/core/type_utils.py` & `secml-0.9rc2/src/secml/core/type_utils.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/figure/c_figure.py` & `secml-0.9rc2/src/secml/figure/c_figure.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/figure/_plots/plot_utils.py` & `secml-0.9rc2/src/secml/figure/_plots/plot_utils.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/figure/_plots/c_plot_classifier.py` & `secml-0.9rc2/src/secml/figure/_plots/c_plot_classifier.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/figure/_plots/c_plot_ds.py` & `secml-0.9rc2/src/secml/figure/_plots/c_plot_ds.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/figure/_plots/c_plot.py` & `secml-0.9rc2/src/secml/figure/_plots/c_plot.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/figure/_plots/c_plot_metric.py` & `secml-0.9rc2/src/secml/figure/_plots/c_plot_metric.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/figure/_plots/c_plot_sec_eval.py` & `secml-0.9rc2/src/secml/figure/_plots/c_plot_sec_eval.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/figure/_plots/c_plot_constraint.py` & `secml-0.9rc2/src/secml/figure/_plots/c_plot_constraint.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/figure/_plots/c_plot_fun.py` & `secml-0.9rc2/src/secml/figure/_plots/c_plot_fun.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/figure/_plots/c_plot_stats.py` & `secml-0.9rc2/src/secml/figure/_plots/c_plot_stats.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/optimizers/c_optimizer_scipy.py` & `secml-0.9rc2/src/secml/optim/optimizers/c_optimizer_scipy.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/optimizers/c_optimizer_pgd.py` & `secml-0.9rc2/src/secml/optim/optimizers/c_optimizer_pgd.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/optimizers/c_optimizer.py` & `secml-0.9rc2/src/secml/optim/optimizers/c_optimizer.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/optimizers/c_optimizer_pgd_ls.py` & `secml-0.9rc2/src/secml/optim/optimizers/c_optimizer_pgd_ls.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/optimizers/line_search/c_line_search.py` & `secml-0.9rc2/src/secml/optim/optimizers/line_search/c_line_search.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/optimizers/line_search/c_line_search_bisect.py` & `secml-0.9rc2/src/secml/optim/optimizers/line_search/c_line_search_bisect.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/function/c_function_3hcamel.py` & `secml-0.9rc2/src/secml/optim/function/c_function_3hcamel.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/function/c_function_rosenbrock.py` & `secml-0.9rc2/src/secml/optim/function/c_function_rosenbrock.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/function/c_function_linear.py` & `secml-0.9rc2/src/secml/optim/function/c_function_linear.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/function/c_function_beale.py` & `secml-0.9rc2/src/secml/optim/function/c_function_beale.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/function/c_function.py` & `secml-0.9rc2/src/secml/optim/function/c_function.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/function/c_function_mccormick.py` & `secml-0.9rc2/src/secml/optim/function/c_function_mccormick.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/function/c_function_quadratic.py` & `secml-0.9rc2/src/secml/optim/function/c_function_quadratic.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/constraints/c_constraint_l1.py` & `secml-0.9rc2/src/secml/optim/constraints/c_constraint_l1.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/constraints/c_constraint_l2.py` & `secml-0.9rc2/src/secml/optim/constraints/c_constraint_l2.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/constraints/c_constraint.py` & `secml-0.9rc2/src/secml/optim/constraints/c_constraint.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/optim/constraints/c_constraint_box.py` & `secml-0.9rc2/src/secml/optim/constraints/c_constraint_box.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/utils/download_utils.py` & `secml-0.9rc2/src/secml/utils/download_utils.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/utils/dict_utils.py` & `secml-0.9rc2/src/secml/utils/dict_utils.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/utils/c_log.py` & `secml-0.9rc2/src/secml/utils/c_log.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/utils/mixed_utils.py` & `secml-0.9rc2/src/secml/utils/mixed_utils.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/utils/list_utils.py` & `secml-0.9rc2/src/secml/utils/list_utils.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/utils/c_file_manager.py` & `secml-0.9rc2/src/secml/utils/c_file_manager.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/utils/pickle_utils.py` & `secml-0.9rc2/src/secml/utils/pickle_utils.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/clf_utils.py` & `secml-0.9rc2/src/secml/ml/classifiers/clf_utils.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/c_classifier_kde.py` & `secml-0.9rc2/src/secml/ml/classifiers/c_classifier_kde.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/c_classifier_linear.py` & `secml-0.9rc2/src/secml/ml/classifiers/c_classifier_linear.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/c_classifier.py` & `secml-0.9rc2/src/secml/ml/classifiers/c_classifier.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/__init__.py` & `secml-0.9rc2/src/secml/ml/classifiers/__init__.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/c_classifier_mcs_linear.py` & `secml-0.9rc2/src/secml/ml/classifiers/c_classifier_mcs_linear.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_kde.py` & `secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_kde.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_linear.py` & `secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_linear.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_logistic.py` & `secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_logistic.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_svm.py` & `secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_svm.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_ridge.py` & `secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_ridge.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/gradients/__init__.py` & `secml-0.9rc2/src/secml/ml/classifiers/gradients/__init__.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_pytorch.py` & `secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_pytorch.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_sgd.py` & `secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient_sgd.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/gradients/mixin_classifier_gradient.py` & `secml-0.9rc2/src/secml/ml/classifiers/gradients/mixin_classifier_gradient.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/loss/c_loss_cross_entropy.py` & `secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_cross_entropy.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/loss/c_softmax.py` & `secml-0.9rc2/src/secml/ml/classifiers/loss/c_softmax.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/loss/c_loss_squared.py` & `secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_squared.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/loss/c_loss.py` & `secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/loss/c_loss_logistic.py` & `secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_logistic.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/loss/c_loss_hinge.py` & `secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_hinge.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/loss/c_loss_epsilon_insensitive.py` & `secml-0.9rc2/src/secml/ml/classifiers/loss/c_loss_epsilon_insensitive.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/reject/mixin_classifier_gradient_reject_threshold.py` & `secml-0.9rc2/src/secml/ml/classifiers/reject/mixin_classifier_gradient_reject_threshold.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/reject/c_classifier_reject.py` & `secml-0.9rc2/src/secml/ml/classifiers/reject/c_classifier_reject.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/reject/c_classifier_reject_threshold.py` & `secml-0.9rc2/src/secml/ml/classifiers/reject/c_classifier_reject_threshold.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_knn.py` & `secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_knn.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_sklearn.py` & `secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_sklearn.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_logistic.py` & `secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_logistic.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_svm.py` & `secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_svm.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_sgd.py` & `secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_sgd.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_nearest_centroid.py` & `secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_nearest_centroid.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_random_forest.py` & `secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_random_forest.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_decision_tree.py` & `secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_decision_tree.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/sklearn/c_classifier_ridge.py` & `secml-0.9rc2/src/secml/ml/classifiers/sklearn/c_classifier_ridge.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/pytorch/c_classifier_pytorch.py` & `secml-0.9rc2/src/secml/ml/classifiers/pytorch/c_classifier_pytorch.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/multiclass/c_classifier_multi_ova.py` & `secml-0.9rc2/src/secml/ml/classifiers/multiclass/c_classifier_multi_ova.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/multiclass/mixin_classifier_gradient_multiclass_ova.py` & `secml-0.9rc2/src/secml/ml/classifiers/multiclass/mixin_classifier_gradient_multiclass_ova.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/multiclass/c_classifier_multi.py` & `secml-0.9rc2/src/secml/ml/classifiers/multiclass/c_classifier_multi.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/regularizer/c_regularizer_l1.py` & `secml-0.9rc2/src/secml/ml/classifiers/regularizer/c_regularizer_l1.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/regularizer/c_regularizer.py` & `secml-0.9rc2/src/secml/ml/classifiers/regularizer/c_regularizer.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/regularizer/c_regularizer_elastic_net.py` & `secml-0.9rc2/src/secml/ml/classifiers/regularizer/c_regularizer_elastic_net.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/classifiers/regularizer/c_regularizer_l2.py` & `secml-0.9rc2/src/secml/ml/classifiers/regularizer/c_regularizer_l2.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/features/c_preprocess.py` & `secml-0.9rc2/src/secml/ml/features/c_preprocess.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/features/normalization/c_normalizer_minmax.py` & `secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer_minmax.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/features/normalization/c_normalizer_linear.py` & `secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer_linear.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/features/normalization/c_normalizer_mean_std.py` & `secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer_mean_std.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/features/normalization/c_normalizer_unitnorm.py` & `secml-0.9rc2/src/secml/ml/features/normalization/c_normalizer_unitnorm.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/features/reduction/c_reducer_pca.py` & `secml-0.9rc2/src/secml/ml/features/reduction/c_reducer_pca.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/features/reduction/c_reducer_lda.py` & `secml-0.9rc2/src/secml/ml/features/reduction/c_reducer_lda.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/c_perfevaluator_xval.py` & `secml-0.9rc2/src/secml/ml/peval/c_perfevaluator_xval.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/c_perfevaluator_xval_multiclass.py` & `secml-0.9rc2/src/secml/ml/peval/c_perfevaluator_xval_multiclass.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/c_perfevaluator.py` & `secml-0.9rc2/src/secml/ml/peval/c_perfevaluator.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_confusion_matrix.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_confusion_matrix.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_metric_tpr_at_fpr.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_tpr_at_fpr.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_metric_auc_wmw.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_auc_wmw.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_metric_mae.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_mae.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_metric_mse.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_mse.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_metric_test_error.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_test_error.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/__init__.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/__init__.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_metric_pauc.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_pauc.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_metric.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_metric.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_metric_precision.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_precision.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_roc.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_roc.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_metric_auc.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_auc.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_metric_recall.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_recall.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_metric_accuracy.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_accuracy.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/peval/metrics/c_metric_f1.py` & `secml-0.9rc2/src/secml/ml/peval/metrics/c_metric_f1.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/stats/c_density_estimation.py` & `secml-0.9rc2/src/secml/ml/stats/c_density_estimation.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/stats/c_distribution_gaussian.py` & `secml-0.9rc2/src/secml/ml/stats/c_distribution_gaussian.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/kernel/c_kernel_poly.py` & `secml-0.9rc2/src/secml/ml/kernel/c_kernel_poly.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/kernel/c_kernel_hamming.py` & `secml-0.9rc2/src/secml/ml/kernel/c_kernel_hamming.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/kernel/c_kernel_euclidean.py` & `secml-0.9rc2/src/secml/ml/kernel/c_kernel_euclidean.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/kernel/c_kernel_rbf.py` & `secml-0.9rc2/src/secml/ml/kernel/c_kernel_rbf.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/kernel/c_kernel_laplacian.py` & `secml-0.9rc2/src/secml/ml/kernel/c_kernel_laplacian.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/kernel/c_kernel_chebyshev_distance.py` & `secml-0.9rc2/src/secml/ml/kernel/c_kernel_chebyshev_distance.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/kernel/c_kernel_linear.py` & `secml-0.9rc2/src/secml/ml/kernel/c_kernel_linear.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/kernel/c_kernel_histintersect.py` & `secml-0.9rc2/src/secml/ml/kernel/c_kernel_histintersect.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/src/secml/ml/kernel/c_kernel.py` & `secml-0.9rc2/src/secml/ml/kernel/c_kernel.py`

 * *Files identical despite different names*

## Comparing `secml-0.9/update/0.8-to-0.9.md` & `secml-0.9rc2/update/0.8-to-0.9.md`

 * *Files identical despite different names*

