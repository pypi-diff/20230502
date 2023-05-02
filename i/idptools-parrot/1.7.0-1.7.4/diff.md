# Comparing `tmp/idptools-parrot-1.7.0.tar.gz` & `tmp/idptools-parrot-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idptools-parrot-1.7.0.tar", last modified: Fri Jul 15 21:51:06 2022, max compression
+gzip compressed data, was "dist/idptools-parrot-1.7.4.tar", last modified: Tue May  2 14:39:45 2023, max compression
```

## Comparing `idptools-parrot-1.7.0.tar` & `idptools-parrot-1.7.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2022-07-15 21:51:06.742381 idptools-parrot-1.7.0/
--rw-r--r--   0 dan        (501) staff       (20)     1071 2020-06-17 16:59:26.000000 idptools-parrot-1.7.0/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)      116 2020-06-17 16:59:26.000000 idptools-parrot-1.7.0/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)     6569 2022-07-15 21:51:06.742626 idptools-parrot-1.7.0/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     6321 2022-07-15 21:33:48.000000 idptools-parrot-1.7.0/README.md
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2022-07-15 21:51:06.724859 idptools-parrot-1.7.0/idptools_parrot.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     6569 2022-07-15 21:51:06.000000 idptools-parrot-1.7.0/idptools_parrot.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      884 2022-07-15 21:51:06.000000 idptools-parrot-1.7.0/idptools_parrot.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2022-07-15 21:51:06.000000 idptools-parrot-1.7.0/idptools_parrot.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2020-06-18 21:46:59.000000 idptools-parrot-1.7.0/idptools_parrot.egg-info/not-zip-safe
--rw-r--r--   0 dan        (501) staff       (20)      118 2022-07-15 21:51:06.000000 idptools-parrot-1.7.0/idptools_parrot.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       13 2022-07-15 21:51:06.000000 idptools-parrot-1.7.0/idptools_parrot.egg-info/top_level.txt
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2022-07-15 21:51:06.744568 idptools-parrot-1.7.0/parrot/
--rw-r--r--   0 dan        (501) staff       (20)      664 2022-01-16 18:30:55.000000 idptools-parrot-1.7.0/parrot/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)      498 2022-07-15 21:51:06.744712 idptools-parrot-1.7.0/parrot/_version.py
--rw-r--r--   0 dan        (501) staff       (20)    10767 2022-07-15 21:20:54.000000 idptools-parrot-1.7.0/parrot/bayesian_optimization.py
--rw-r--r--   0 dan        (501) staff       (20)     8760 2021-08-05 18:22:06.000000 idptools-parrot-1.7.0/parrot/brnn_architecture.py
--rw-r--r--   0 dan        (501) staff       (20)    20920 2021-08-12 20:27:10.000000 idptools-parrot-1.7.0/parrot/brnn_plot.py
--rw-r--r--   0 dan        (501) staff       (20)     8735 2021-07-22 19:26:58.000000 idptools-parrot-1.7.0/parrot/encode_sequence.py
--rw-r--r--   0 dan        (501) staff       (20)       90 2022-01-16 18:30:55.000000 idptools-parrot-1.7.0/parrot/parrot_exceptions.py
--rw-r--r--   0 dan        (501) staff       (20)    32029 2022-07-15 21:41:15.000000 idptools-parrot-1.7.0/parrot/process_input_data.py
--rw-r--r--   0 dan        (501) staff       (20)     4820 2021-08-05 18:38:11.000000 idptools-parrot-1.7.0/parrot/py_predictor.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2022-07-15 21:51:06.737218 idptools-parrot-1.7.0/parrot/tools/
--rw-r--r--   0 dan        (501) staff       (20)        0 2021-05-24 16:04:27.000000 idptools-parrot-1.7.0/parrot/tools/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    30180 2022-01-16 18:30:55.000000 idptools-parrot-1.7.0/parrot/tools/class_balancing.py
--rw-r--r--   0 dan        (501) staff       (20)     4213 2022-01-16 18:30:55.000000 idptools-parrot-1.7.0/parrot/tools/cli.py
--rw-r--r--   0 dan        (501) staff       (20)     5489 2022-01-16 18:30:55.000000 idptools-parrot-1.7.0/parrot/tools/dataset_warnings.py
--rw-r--r--   0 dan        (501) staff       (20)     8249 2022-01-16 18:30:55.000000 idptools-parrot-1.7.0/parrot/tools/preproc.py
--rw-r--r--   0 dan        (501) staff       (20)     3222 2021-08-02 21:40:30.000000 idptools-parrot-1.7.0/parrot/tools/validate_args.py
--rw-r--r--   0 dan        (501) staff       (20)    17042 2021-08-11 18:57:36.000000 idptools-parrot-1.7.0/parrot/train_network.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2022-07-15 21:51:06.740107 idptools-parrot-1.7.0/scripts/
--rwxr--r--   0 dan        (501) staff       (20)     3114 2021-08-09 20:06:46.000000 idptools-parrot-1.7.0/scripts/parrot-cvsplit
--rwxr-xr-x   0 dan        (501) staff       (20)    12440 2021-08-13 21:24:47.000000 idptools-parrot-1.7.0/scripts/parrot-optimize
--rwxr-xr-x   0 dan        (501) staff       (20)     8058 2021-08-05 22:01:30.000000 idptools-parrot-1.7.0/scripts/parrot-predict
--rwxr-xr-x   0 dan        (501) staff       (20)     7827 2022-07-15 21:41:15.000000 idptools-parrot-1.7.0/scripts/parrot-preprocess
--rwxr-xr-x   0 dan        (501) staff       (20)    12077 2021-08-13 20:38:54.000000 idptools-parrot-1.7.0/scripts/parrot-train
--rw-r--r--   0 dan        (501) staff       (20)      345 2022-07-15 21:51:06.744016 idptools-parrot-1.7.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     2434 2022-07-15 20:07:14.000000 idptools-parrot-1.7.0/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2022-07-15 21:51:06.741865 idptools-parrot-1.7.0/tests/
--rw-r--r--   0 dan        (501) staff       (20)      112 2020-06-17 16:59:26.000000 idptools-parrot-1.7.0/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     1719 2022-07-15 21:41:15.000000 idptools-parrot-1.7.0/tests/test_file_io.py
--rw-r--r--   0 dan        (501) staff       (20)     5025 2022-07-15 21:22:36.000000 idptools-parrot-1.7.0/tests/test_parrot.py
--rw-r--r--   0 dan        (501) staff       (20)    68611 2020-06-17 16:59:26.000000 idptools-parrot-1.7.0/versioneer.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/
+-rw-r--r--   0 dan        (501) staff       (20)     1071 2020-06-17 16:59:26.000000 idptools-parrot-1.7.4/LICENSE
+-rw-r--r--   0 dan        (501) staff       (20)      116 2020-06-17 16:59:26.000000 idptools-parrot-1.7.4/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)     7583 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     6442 2023-05-02 14:34:16.000000 idptools-parrot-1.7.4/README.md
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/idptools_parrot.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)     7583 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/idptools_parrot.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      884 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/idptools_parrot.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/idptools_parrot.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2020-06-18 21:46:59.000000 idptools-parrot-1.7.4/idptools_parrot.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)      118 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/idptools_parrot.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       13 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/idptools_parrot.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/parrot/
+-rw-r--r--   0 dan        (501) staff       (20)      664 2022-01-16 18:30:55.000000 idptools-parrot-1.7.4/parrot/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)      498 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/parrot/_version.py
+-rw-r--r--   0 dan        (501) staff       (20)    10767 2022-07-15 21:20:54.000000 idptools-parrot-1.7.4/parrot/bayesian_optimization.py
+-rw-r--r--   0 dan        (501) staff       (20)     8760 2021-08-05 18:22:06.000000 idptools-parrot-1.7.4/parrot/brnn_architecture.py
+-rw-r--r--   0 dan        (501) staff       (20)    20920 2021-08-12 20:27:10.000000 idptools-parrot-1.7.4/parrot/brnn_plot.py
+-rw-r--r--   0 dan        (501) staff       (20)     8735 2021-07-22 19:26:58.000000 idptools-parrot-1.7.4/parrot/encode_sequence.py
+-rw-r--r--   0 dan        (501) staff       (20)       90 2022-01-16 18:30:55.000000 idptools-parrot-1.7.4/parrot/parrot_exceptions.py
+-rw-r--r--   0 dan        (501) staff       (20)    32029 2022-07-15 21:41:15.000000 idptools-parrot-1.7.4/parrot/process_input_data.py
+-rw-r--r--   0 dan        (501) staff       (20)     4820 2021-08-05 18:38:11.000000 idptools-parrot-1.7.4/parrot/py_predictor.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/parrot/tools/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2021-05-24 16:04:27.000000 idptools-parrot-1.7.4/parrot/tools/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    30180 2022-01-16 18:30:55.000000 idptools-parrot-1.7.4/parrot/tools/class_balancing.py
+-rw-r--r--   0 dan        (501) staff       (20)     4213 2022-01-16 18:30:55.000000 idptools-parrot-1.7.4/parrot/tools/cli.py
+-rw-r--r--   0 dan        (501) staff       (20)     5489 2022-01-16 18:30:55.000000 idptools-parrot-1.7.4/parrot/tools/dataset_warnings.py
+-rw-r--r--   0 dan        (501) staff       (20)     8249 2022-01-16 18:30:55.000000 idptools-parrot-1.7.4/parrot/tools/preproc.py
+-rw-r--r--   0 dan        (501) staff       (20)     3222 2021-08-02 21:40:30.000000 idptools-parrot-1.7.4/parrot/tools/validate_args.py
+-rw-r--r--   0 dan        (501) staff       (20)    17042 2021-08-11 18:57:36.000000 idptools-parrot-1.7.4/parrot/train_network.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/scripts/
+-rwxr--r--   0 dan        (501) staff       (20)     3114 2021-08-09 20:06:46.000000 idptools-parrot-1.7.4/scripts/parrot-cvsplit
+-rwxr-xr-x   0 dan        (501) staff       (20)    12440 2021-08-13 21:24:47.000000 idptools-parrot-1.7.4/scripts/parrot-optimize
+-rwxr-xr-x   0 dan        (501) staff       (20)     8058 2021-08-05 22:01:30.000000 idptools-parrot-1.7.4/scripts/parrot-predict
+-rwxr-xr-x   0 dan        (501) staff       (20)     7827 2022-07-15 21:41:15.000000 idptools-parrot-1.7.4/scripts/parrot-preprocess
+-rwxr-xr-x   0 dan        (501) staff       (20)    12077 2021-08-13 20:38:54.000000 idptools-parrot-1.7.4/scripts/parrot-train
+-rw-r--r--   0 dan        (501) staff       (20)      345 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)     2434 2023-05-02 14:34:16.000000 idptools-parrot-1.7.4/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-05-02 14:39:45.000000 idptools-parrot-1.7.4/tests/
+-rw-r--r--   0 dan        (501) staff       (20)      112 2020-06-17 16:59:26.000000 idptools-parrot-1.7.4/tests/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     1719 2022-07-15 21:41:15.000000 idptools-parrot-1.7.4/tests/test_file_io.py
+-rw-r--r--   0 dan        (501) staff       (20)     5025 2022-07-15 21:22:36.000000 idptools-parrot-1.7.4/tests/test_parrot.py
+-rw-r--r--   0 dan        (501) staff       (20)    68611 2020-06-17 16:59:26.000000 idptools-parrot-1.7.4/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `idptools-parrot-1.7.0/LICENSE` & `idptools-parrot-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/PKG-INFO` & `idptools-parrot-1.7.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-Metadata-Version: 2.1
-Name: idptools-parrot
-Version: 1.7.0
-Author: Holehouse Lab
-Author-email: degriffith@wustl.edu
-License: MIT
-Requires-Python: >=3.9,<3.10.0
-Description-Content-Type: text/markdown
-Provides-Extra: optimize
-License-File: LICENSE
-
 ![PARROT_logo_full](https://user-images.githubusercontent.com/54642153/122615183-b274f280-d04d-11eb-88bf-1530d18d310c.png)
 
 # PARROT: Protein Analysis using RecuRrent neural networks On Training data
 
-**PARROT** encodes a computationally-robust bidirectional recurrent neural network (BRNN) behind an easy-to-use commandline interface. PARROT is well-suited for a variety of protein bioinformatics tasks. With only an input datafile containing sequences and mapped values, the user can automatically train a network for whatever purpose. This trained network can then be applied to new, unlabeled data to generate predictions and generate biological hypotheses.
+**PARROT** encodes a computationally-robust bidirectional recurrent neural network (BRNN) behind an easy-to-use commandline interface. PARROT is well-suited for a variety of protein bioinformatics tasks. With only an input data file containing sequences and mapped values, the user can automatically train a network for whatever purpose. This trained network can then be applied to new, unlabeled data to generate predictions and generate biological hypotheses.
 
 This package can handle regression and classification ML problems, as well as sequence-mapped and residue-mapped input data.
 
 ## Installation:
 
 PARROT is available through GitHub or the Python Package Index (PyPI). To install the base version of PARROT through PyPI, run
 
@@ -76,54 +65,42 @@
 	.
 	.
 	.  
 	seqIDM seqM seqMdata1 <seqMdata2> <seqMdata3> ... <seqMdataNM>
   
 Where Ni is the length of sequence i, and M is the total number of labeled sequences. Items must be whitespace-separated.
 For **sequence-mapped data** (i.e. each sequence constitutes a *single datapoint*), each row will only contain three columns.
-Note that it is not required that sequences are the same length. For example, if Sequence #1 has 12 amino acids and Sequence #2
-has 15 amino acids, then these two rows in the input file will contain 14 and 17 fields respectively.
 
-Optionally, you may use datasets that exclude the first column containing the ID of each sequence. In this case, be sure to 
-use the `--excludeSeqID` flag.
+Note that it is not required that sequences are the same length. For example, if Sequence #1 has 12 amino acids and Sequence #2 has 15 amino acids, these two rows in the input file will contain 14 and 17 fields, respectively.
+
+Optionally, you may use datasets that exclude the first column containing the ID of each sequence. In this case, be sure to use the `--excludeSeqID` flag.
 
-**Classification problem:** the labeled data should be integer class labels. For example, if there are 3 classes, then each
-datapoint should be either a '0', '1', or '2' (with no quote marks).
+**Classification problem:** the labeled data should be integer class labels. For example, if there are 3 classes, then each datapoint should be either a '0', '1', or '2' (with no quotation marks).
   
-**Regression problem:** If the user wishes to map each sequence or residue to a continuous real number, then each datapoint 
-should be a float
+**Regression problem:** If the user wishes to map each sequence or residue to a continuous real number, then each datapoint should be a float
 
-For example datasets, see the TSV files provided in the **/data** folder.
+For example, datasets, see the TSV files provided in the **/data** folder.
 
 ### 1. Train a network with provided hyperparameters: ``parrot-train``
 
-The ``parrot-train`` command is the primary command for training a network with PARROT. By default, users need only to specify 
-their data, where they want to save their output, and some basic information on the type of machine learning problem the are 
-tackling. Beyond this, there are a suite of other options that users can provide to tailor their network to their particular 
-needs. Users can provide specific hyperparameters to craft their network, they can manually specify what samples in their
-data set are trained on and which are held out as test data, they can choose to output information and figures on their network's
-performance on the test data, and much more!
+The ``parrot-train`` command is the primary command for training a network with PARROT. By default, users need only to specify their data, where they want to save their output, and some basic information on the type of machine learning problem they are tackling. Beyond this, there are a suite of other options that users can provide to tailor their network to their particular needs. Users can provide specific hyperparameters to craft their network, they can manually specify what samples in their data set are trained on and which are held out as test data, they can choose to output information and figures on their network's performance on the test data, and much more!
 
 ### 2. Optimize hyperparameters and train a network: ``parrot-optimize``
 
-The ``parrot-optimize`` command initiates an extensive search for the best-performing network hyperparameters for a given
-dataset using Bayesian optimiztion. Three hyperparameters, the learning rate, number of hidden layers, and hidden vector size
-can greatly impact network performance and training speed, so it is important to tune these for each particular dataset. This
-command will search across hyperparameter space by iteratively training and validating network performance (with 5-fold cross
-validation). The best performing hyperparameters will be selected, and used to train a network from scratch as if running
-``parrot_train`` with these parameters. Note that since this command take a significant amount of time to run since it involves
-searching for the best hyperparameters.
+The ``parrot-optimize`` command initiates an extensive search for the best-performing network hyperparameters for a given dataset using Bayesian optimization. Three hyperparameters, the learning rate, the number of hidden layers, and hidden vector size can greatly impact network performance and training speed, so it is important to tune these for each particular dataset. This command will search across hyperparameter space by iteratively training and validating network performance (with 5-fold cross-validation). The best-performing hyperparameters will be selected and used to train a network from scratch as if running ``parrot_train`` with these parameters. Note that since this command takes a significant amount of time to run since it involvessearching for the best hyperparameters.
 
 ### 3. Generate predictions with a trained network: ``parrot-predict``
 
-Once a network has been trained for a particular machine learning task, the user can generate predictions on new sequences
-with this network using the ``parrot-predict`` command. The user provides a list of sequences they would like to predict and
-the saved network, and a file is outputted with the predictions.
+Once a network has been trained for a particular machine learning task, the user can generate predictions on new sequences with this network using the ``parrot-predict`` command. The user provides a list of sequences they would like to predict and the saved network, and a file is outputted with the predictions.
 
 ### Copyright
 
-Copyright (c) 2020-2022, Holehouse Lab
+Copyright (c) 2020-2023, Holehouse Lab
+
+### Change log 
+
+* Version 1.7.2: Updated Python dependency so PARROT is compatible with Python 3.8, 3.9, and 3.10. 
 
 #### Acknowledgements
  
 Project based on the 
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.3.
```

### Comparing `idptools-parrot-1.7.0/README.md` & `idptools-parrot-1.7.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,119 @@
-![PARROT_logo_full](https://user-images.githubusercontent.com/54642153/122615183-b274f280-d04d-11eb-88bf-1530d18d310c.png)
-
-# PARROT: Protein Analysis using RecuRrent neural networks On Training data
-
-**PARROT** encodes a computationally-robust bidirectional recurrent neural network (BRNN) behind an easy-to-use commandline interface. PARROT is well-suited for a variety of protein bioinformatics tasks. With only an input datafile containing sequences and mapped values, the user can automatically train a network for whatever purpose. This trained network can then be applied to new, unlabeled data to generate predictions and generate biological hypotheses.
-
-This package can handle regression and classification ML problems, as well as sequence-mapped and residue-mapped input data.
-
-## Installation:
-
-PARROT is available through GitHub or the Python Package Index (PyPI). To install the base version of PARROT through PyPI, run
-
-	$ pip install idptools-parrot
-
-It is possible that you may experience errors depending on what Python packages are already installed on your machine. If you encounter this, try installing PARROT in a "clean" virtual environment using conda:
-
-	$ conda create --name <env_name> python=3.9
-	$ conda activate <env_name>
-
-Then install PARROT with pip.
-
-Alternatively, to clone the GitHub repository and gain the ability to modify a local copy of the code, run:
-
-	$ git clone https://github.com/idptools/parrot.git
-	$ cd parrot
-	$ pip install .
-
-This will install PARROT locally. If you modify the source code in the local repository, be sure to reinstall with pip.
-
-**JULY 2022 UPDATE**
-
-To mitigate package version dependency issues involving Python, GPy, and PyTorch, new releases of PARROT have separated 
-`parrot-optimize` as an optional add-on installation. All of the documentation for using `parrot-optimize` is unchanged.
-However, if you wish to use the hyperparameter optimization, there are now slight differences in how you install PARROT.
-
-To install the PARROT that is compatible with `parrot-optimize` install via pip using:
-
-	$ pip install idptools-parrot[optimize]
-
-or
-
-	$ pip install "idptools-parrot[optimize]"
-
-Alternatively if you have the PARROT repository cloned locally you can install using
-
-	$ pip install ".[optimize]"
-
-
-## Usage:
-
-For detailed information on installation and examples, please visit the [documentation pages](https://idptools-parrot.readthedocs.io/en/latest/).
-
-There are three primary commands that can be run within the parrot package:
-
-1. Train a network with user-specified hyperparameters
-2. Train a network with automatically-determined, optimal hyperparameters
-3. Generate predictions on unlabeled sequences using a trained network
-
-### Input data format:
-
-Before data can be integrated into training a PARROT network, it must be formatted in the following manner:
-
-	seqID1 seq1 seq1data1 <seq1data2> <seq1data3> ... <seq1dataN1>  
-	seqID2 seq2 seq2data1 <seq2data2> <seq2data3> ... <seq2dataN2>  
-	.
-	.
-	.  
-	seqIDM seqM seqMdata1 <seqMdata2> <seqMdata3> ... <seqMdataNM>
-  
-Where Ni is the length of sequence i, and M is the total number of labeled sequences. Items must be whitespace-separated.
-For **sequence-mapped data** (i.e. each sequence constitutes a *single datapoint*), each row will only contain three columns.
-Note that it is not required that sequences are the same length. For example, if Sequence #1 has 12 amino acids and Sequence #2
-has 15 amino acids, then these two rows in the input file will contain 14 and 17 fields respectively.
-
-Optionally, you may use datasets that exclude the first column containing the ID of each sequence. In this case, be sure to 
-use the `--excludeSeqID` flag.
-
-**Classification problem:** the labeled data should be integer class labels. For example, if there are 3 classes, then each
-datapoint should be either a '0', '1', or '2' (with no quote marks).
-  
-**Regression problem:** If the user wishes to map each sequence or residue to a continuous real number, then each datapoint 
-should be a float
-
-For example datasets, see the TSV files provided in the **/data** folder.
-
-### 1. Train a network with provided hyperparameters: ``parrot-train``
-
-The ``parrot-train`` command is the primary command for training a network with PARROT. By default, users need only to specify 
-their data, where they want to save their output, and some basic information on the type of machine learning problem the are 
-tackling. Beyond this, there are a suite of other options that users can provide to tailor their network to their particular 
-needs. Users can provide specific hyperparameters to craft their network, they can manually specify what samples in their
-data set are trained on and which are held out as test data, they can choose to output information and figures on their network's
-performance on the test data, and much more!
-
-### 2. Optimize hyperparameters and train a network: ``parrot-optimize``
-
-The ``parrot-optimize`` command initiates an extensive search for the best-performing network hyperparameters for a given
-dataset using Bayesian optimiztion. Three hyperparameters, the learning rate, number of hidden layers, and hidden vector size
-can greatly impact network performance and training speed, so it is important to tune these for each particular dataset. This
-command will search across hyperparameter space by iteratively training and validating network performance (with 5-fold cross
-validation). The best performing hyperparameters will be selected, and used to train a network from scratch as if running
-``parrot_train`` with these parameters. Note that since this command take a significant amount of time to run since it involves
-searching for the best hyperparameters.
-
-### 3. Generate predictions with a trained network: ``parrot-predict``
-
-Once a network has been trained for a particular machine learning task, the user can generate predictions on new sequences
-with this network using the ``parrot-predict`` command. The user provides a list of sequences they would like to predict and
-the saved network, and a file is outputted with the predictions.
-
-### Copyright
-
-Copyright (c) 2020-2022, Holehouse Lab
-
-#### Acknowledgements
- 
-Project based on the 
-[Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.3.
+Metadata-Version: 2.1
+Name: idptools-parrot
+Version: 1.7.4
+Summary: UNKNOWN
+Home-page: UNKNOWN
+Author: Holehouse Lab
+Author-email: degriffith@wustl.edu
+License: MIT
+Description: ![PARROT_logo_full](https://user-images.githubusercontent.com/54642153/122615183-b274f280-d04d-11eb-88bf-1530d18d310c.png)
+        
+        # PARROT: Protein Analysis using RecuRrent neural networks On Training data
+        
+        **PARROT** encodes a computationally-robust bidirectional recurrent neural network (BRNN) behind an easy-to-use commandline interface. PARROT is well-suited for a variety of protein bioinformatics tasks. With only an input data file containing sequences and mapped values, the user can automatically train a network for whatever purpose. This trained network can then be applied to new, unlabeled data to generate predictions and generate biological hypotheses.
+        
+        This package can handle regression and classification ML problems, as well as sequence-mapped and residue-mapped input data.
+        
+        ## Installation:
+        
+        PARROT is available through GitHub or the Python Package Index (PyPI). To install the base version of PARROT through PyPI, run
+        
+        	$ pip install idptools-parrot
+        
+        It is possible that you may experience errors depending on what Python packages are already installed on your machine. If you encounter this, try installing PARROT in a "clean" virtual environment using conda:
+        
+        	$ conda create --name <env_name> python=3.9
+        	$ conda activate <env_name>
+        
+        Then install PARROT with pip.
+        
+        Alternatively, to clone the GitHub repository and gain the ability to modify a local copy of the code, run:
+        
+        	$ git clone https://github.com/idptools/parrot.git
+        	$ cd parrot
+        	$ pip install .
+        
+        This will install PARROT locally. If you modify the source code in the local repository, be sure to reinstall with pip.
+        
+        **JULY 2022 UPDATE**
+        
+        To mitigate package version dependency issues involving Python, GPy, and PyTorch, new releases of PARROT have separated 
+        `parrot-optimize` as an optional add-on installation. All of the documentation for using `parrot-optimize` is unchanged.
+        However, if you wish to use the hyperparameter optimization, there are now slight differences in how you install PARROT.
+        
+        To install the PARROT that is compatible with `parrot-optimize` install via pip using:
+        
+        	$ pip install idptools-parrot[optimize]
+        
+        or
+        
+        	$ pip install "idptools-parrot[optimize]"
+        
+        Alternatively if you have the PARROT repository cloned locally you can install using
+        
+        	$ pip install ".[optimize]"
+        
+        
+        ## Usage:
+        
+        For detailed information on installation and examples, please visit the [documentation pages](https://idptools-parrot.readthedocs.io/en/latest/).
+        
+        There are three primary commands that can be run within the parrot package:
+        
+        1. Train a network with user-specified hyperparameters
+        2. Train a network with automatically-determined, optimal hyperparameters
+        3. Generate predictions on unlabeled sequences using a trained network
+        
+        ### Input data format:
+        
+        Before data can be integrated into training a PARROT network, it must be formatted in the following manner:
+        
+        	seqID1 seq1 seq1data1 <seq1data2> <seq1data3> ... <seq1dataN1>  
+        	seqID2 seq2 seq2data1 <seq2data2> <seq2data3> ... <seq2dataN2>  
+        	.
+        	.
+        	.  
+        	seqIDM seqM seqMdata1 <seqMdata2> <seqMdata3> ... <seqMdataNM>
+          
+        Where Ni is the length of sequence i, and M is the total number of labeled sequences. Items must be whitespace-separated.
+        For **sequence-mapped data** (i.e. each sequence constitutes a *single datapoint*), each row will only contain three columns.
+        
+        Note that it is not required that sequences are the same length. For example, if Sequence #1 has 12 amino acids and Sequence #2 has 15 amino acids, these two rows in the input file will contain 14 and 17 fields, respectively.
+        
+        Optionally, you may use datasets that exclude the first column containing the ID of each sequence. In this case, be sure to use the `--excludeSeqID` flag.
+        
+        **Classification problem:** the labeled data should be integer class labels. For example, if there are 3 classes, then each datapoint should be either a '0', '1', or '2' (with no quotation marks).
+          
+        **Regression problem:** If the user wishes to map each sequence or residue to a continuous real number, then each datapoint should be a float
+        
+        For example, datasets, see the TSV files provided in the **/data** folder.
+        
+        ### 1. Train a network with provided hyperparameters: ``parrot-train``
+        
+        The ``parrot-train`` command is the primary command for training a network with PARROT. By default, users need only to specify their data, where they want to save their output, and some basic information on the type of machine learning problem they are tackling. Beyond this, there are a suite of other options that users can provide to tailor their network to their particular needs. Users can provide specific hyperparameters to craft their network, they can manually specify what samples in their data set are trained on and which are held out as test data, they can choose to output information and figures on their network's performance on the test data, and much more!
+        
+        ### 2. Optimize hyperparameters and train a network: ``parrot-optimize``
+        
+        The ``parrot-optimize`` command initiates an extensive search for the best-performing network hyperparameters for a given dataset using Bayesian optimization. Three hyperparameters, the learning rate, the number of hidden layers, and hidden vector size can greatly impact network performance and training speed, so it is important to tune these for each particular dataset. This command will search across hyperparameter space by iteratively training and validating network performance (with 5-fold cross-validation). The best-performing hyperparameters will be selected and used to train a network from scratch as if running ``parrot_train`` with these parameters. Note that since this command takes a significant amount of time to run since it involvessearching for the best hyperparameters.
+        
+        ### 3. Generate predictions with a trained network: ``parrot-predict``
+        
+        Once a network has been trained for a particular machine learning task, the user can generate predictions on new sequences with this network using the ``parrot-predict`` command. The user provides a list of sequences they would like to predict and the saved network, and a file is outputted with the predictions.
+        
+        ### Copyright
+        
+        Copyright (c) 2020-2023, Holehouse Lab
+        
+        ### Change log 
+        
+        * Version 1.7.2: Updated Python dependency so PARROT is compatible with Python 3.8, 3.9, and 3.10. 
+        
+        #### Acknowledgements
+         
+        Project based on the 
+        [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.3.
+        
+Platform: UNKNOWN
+Requires-Python: >=3.7,<3.11.0
+Description-Content-Type: text/markdown
+Provides-Extra: optimize
```

### Comparing `idptools-parrot-1.7.0/idptools_parrot.egg-info/PKG-INFO` & `idptools-parrot-1.7.4/idptools_parrot.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,129 +1,119 @@
 Metadata-Version: 2.1
 Name: idptools-parrot
-Version: 1.7.0
+Version: 1.7.4
+Summary: UNKNOWN
+Home-page: UNKNOWN
 Author: Holehouse Lab
 Author-email: degriffith@wustl.edu
 License: MIT
-Requires-Python: >=3.9,<3.10.0
+Description: ![PARROT_logo_full](https://user-images.githubusercontent.com/54642153/122615183-b274f280-d04d-11eb-88bf-1530d18d310c.png)
+        
+        # PARROT: Protein Analysis using RecuRrent neural networks On Training data
+        
+        **PARROT** encodes a computationally-robust bidirectional recurrent neural network (BRNN) behind an easy-to-use commandline interface. PARROT is well-suited for a variety of protein bioinformatics tasks. With only an input data file containing sequences and mapped values, the user can automatically train a network for whatever purpose. This trained network can then be applied to new, unlabeled data to generate predictions and generate biological hypotheses.
+        
+        This package can handle regression and classification ML problems, as well as sequence-mapped and residue-mapped input data.
+        
+        ## Installation:
+        
+        PARROT is available through GitHub or the Python Package Index (PyPI). To install the base version of PARROT through PyPI, run
+        
+        	$ pip install idptools-parrot
+        
+        It is possible that you may experience errors depending on what Python packages are already installed on your machine. If you encounter this, try installing PARROT in a "clean" virtual environment using conda:
+        
+        	$ conda create --name <env_name> python=3.9
+        	$ conda activate <env_name>
+        
+        Then install PARROT with pip.
+        
+        Alternatively, to clone the GitHub repository and gain the ability to modify a local copy of the code, run:
+        
+        	$ git clone https://github.com/idptools/parrot.git
+        	$ cd parrot
+        	$ pip install .
+        
+        This will install PARROT locally. If you modify the source code in the local repository, be sure to reinstall with pip.
+        
+        **JULY 2022 UPDATE**
+        
+        To mitigate package version dependency issues involving Python, GPy, and PyTorch, new releases of PARROT have separated 
+        `parrot-optimize` as an optional add-on installation. All of the documentation for using `parrot-optimize` is unchanged.
+        However, if you wish to use the hyperparameter optimization, there are now slight differences in how you install PARROT.
+        
+        To install the PARROT that is compatible with `parrot-optimize` install via pip using:
+        
+        	$ pip install idptools-parrot[optimize]
+        
+        or
+        
+        	$ pip install "idptools-parrot[optimize]"
+        
+        Alternatively if you have the PARROT repository cloned locally you can install using
+        
+        	$ pip install ".[optimize]"
+        
+        
+        ## Usage:
+        
+        For detailed information on installation and examples, please visit the [documentation pages](https://idptools-parrot.readthedocs.io/en/latest/).
+        
+        There are three primary commands that can be run within the parrot package:
+        
+        1. Train a network with user-specified hyperparameters
+        2. Train a network with automatically-determined, optimal hyperparameters
+        3. Generate predictions on unlabeled sequences using a trained network
+        
+        ### Input data format:
+        
+        Before data can be integrated into training a PARROT network, it must be formatted in the following manner:
+        
+        	seqID1 seq1 seq1data1 <seq1data2> <seq1data3> ... <seq1dataN1>  
+        	seqID2 seq2 seq2data1 <seq2data2> <seq2data3> ... <seq2dataN2>  
+        	.
+        	.
+        	.  
+        	seqIDM seqM seqMdata1 <seqMdata2> <seqMdata3> ... <seqMdataNM>
+          
+        Where Ni is the length of sequence i, and M is the total number of labeled sequences. Items must be whitespace-separated.
+        For **sequence-mapped data** (i.e. each sequence constitutes a *single datapoint*), each row will only contain three columns.
+        
+        Note that it is not required that sequences are the same length. For example, if Sequence #1 has 12 amino acids and Sequence #2 has 15 amino acids, these two rows in the input file will contain 14 and 17 fields, respectively.
+        
+        Optionally, you may use datasets that exclude the first column containing the ID of each sequence. In this case, be sure to use the `--excludeSeqID` flag.
+        
+        **Classification problem:** the labeled data should be integer class labels. For example, if there are 3 classes, then each datapoint should be either a '0', '1', or '2' (with no quotation marks).
+          
+        **Regression problem:** If the user wishes to map each sequence or residue to a continuous real number, then each datapoint should be a float
+        
+        For example, datasets, see the TSV files provided in the **/data** folder.
+        
+        ### 1. Train a network with provided hyperparameters: ``parrot-train``
+        
+        The ``parrot-train`` command is the primary command for training a network with PARROT. By default, users need only to specify their data, where they want to save their output, and some basic information on the type of machine learning problem they are tackling. Beyond this, there are a suite of other options that users can provide to tailor their network to their particular needs. Users can provide specific hyperparameters to craft their network, they can manually specify what samples in their data set are trained on and which are held out as test data, they can choose to output information and figures on their network's performance on the test data, and much more!
+        
+        ### 2. Optimize hyperparameters and train a network: ``parrot-optimize``
+        
+        The ``parrot-optimize`` command initiates an extensive search for the best-performing network hyperparameters for a given dataset using Bayesian optimization. Three hyperparameters, the learning rate, the number of hidden layers, and hidden vector size can greatly impact network performance and training speed, so it is important to tune these for each particular dataset. This command will search across hyperparameter space by iteratively training and validating network performance (with 5-fold cross-validation). The best-performing hyperparameters will be selected and used to train a network from scratch as if running ``parrot_train`` with these parameters. Note that since this command takes a significant amount of time to run since it involvessearching for the best hyperparameters.
+        
+        ### 3. Generate predictions with a trained network: ``parrot-predict``
+        
+        Once a network has been trained for a particular machine learning task, the user can generate predictions on new sequences with this network using the ``parrot-predict`` command. The user provides a list of sequences they would like to predict and the saved network, and a file is outputted with the predictions.
+        
+        ### Copyright
+        
+        Copyright (c) 2020-2023, Holehouse Lab
+        
+        ### Change log 
+        
+        * Version 1.7.2: Updated Python dependency so PARROT is compatible with Python 3.8, 3.9, and 3.10. 
+        
+        #### Acknowledgements
+         
+        Project based on the 
+        [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.3.
+        
+Platform: UNKNOWN
+Requires-Python: >=3.7,<3.11.0
 Description-Content-Type: text/markdown
 Provides-Extra: optimize
-License-File: LICENSE
-
-![PARROT_logo_full](https://user-images.githubusercontent.com/54642153/122615183-b274f280-d04d-11eb-88bf-1530d18d310c.png)
-
-# PARROT: Protein Analysis using RecuRrent neural networks On Training data
-
-**PARROT** encodes a computationally-robust bidirectional recurrent neural network (BRNN) behind an easy-to-use commandline interface. PARROT is well-suited for a variety of protein bioinformatics tasks. With only an input datafile containing sequences and mapped values, the user can automatically train a network for whatever purpose. This trained network can then be applied to new, unlabeled data to generate predictions and generate biological hypotheses.
-
-This package can handle regression and classification ML problems, as well as sequence-mapped and residue-mapped input data.
-
-## Installation:
-
-PARROT is available through GitHub or the Python Package Index (PyPI). To install the base version of PARROT through PyPI, run
-
-	$ pip install idptools-parrot
-
-It is possible that you may experience errors depending on what Python packages are already installed on your machine. If you encounter this, try installing PARROT in a "clean" virtual environment using conda:
-
-	$ conda create --name <env_name> python=3.9
-	$ conda activate <env_name>
-
-Then install PARROT with pip.
-
-Alternatively, to clone the GitHub repository and gain the ability to modify a local copy of the code, run:
-
-	$ git clone https://github.com/idptools/parrot.git
-	$ cd parrot
-	$ pip install .
-
-This will install PARROT locally. If you modify the source code in the local repository, be sure to reinstall with pip.
-
-**JULY 2022 UPDATE**
-
-To mitigate package version dependency issues involving Python, GPy, and PyTorch, new releases of PARROT have separated 
-`parrot-optimize` as an optional add-on installation. All of the documentation for using `parrot-optimize` is unchanged.
-However, if you wish to use the hyperparameter optimization, there are now slight differences in how you install PARROT.
-
-To install the PARROT that is compatible with `parrot-optimize` install via pip using:
-
-	$ pip install idptools-parrot[optimize]
-
-or
-
-	$ pip install "idptools-parrot[optimize]"
-
-Alternatively if you have the PARROT repository cloned locally you can install using
-
-	$ pip install ".[optimize]"
-
-
-## Usage:
-
-For detailed information on installation and examples, please visit the [documentation pages](https://idptools-parrot.readthedocs.io/en/latest/).
-
-There are three primary commands that can be run within the parrot package:
-
-1. Train a network with user-specified hyperparameters
-2. Train a network with automatically-determined, optimal hyperparameters
-3. Generate predictions on unlabeled sequences using a trained network
-
-### Input data format:
-
-Before data can be integrated into training a PARROT network, it must be formatted in the following manner:
-
-	seqID1 seq1 seq1data1 <seq1data2> <seq1data3> ... <seq1dataN1>  
-	seqID2 seq2 seq2data1 <seq2data2> <seq2data3> ... <seq2dataN2>  
-	.
-	.
-	.  
-	seqIDM seqM seqMdata1 <seqMdata2> <seqMdata3> ... <seqMdataNM>
-  
-Where Ni is the length of sequence i, and M is the total number of labeled sequences. Items must be whitespace-separated.
-For **sequence-mapped data** (i.e. each sequence constitutes a *single datapoint*), each row will only contain three columns.
-Note that it is not required that sequences are the same length. For example, if Sequence #1 has 12 amino acids and Sequence #2
-has 15 amino acids, then these two rows in the input file will contain 14 and 17 fields respectively.
-
-Optionally, you may use datasets that exclude the first column containing the ID of each sequence. In this case, be sure to 
-use the `--excludeSeqID` flag.
-
-**Classification problem:** the labeled data should be integer class labels. For example, if there are 3 classes, then each
-datapoint should be either a '0', '1', or '2' (with no quote marks).
-  
-**Regression problem:** If the user wishes to map each sequence or residue to a continuous real number, then each datapoint 
-should be a float
-
-For example datasets, see the TSV files provided in the **/data** folder.
-
-### 1. Train a network with provided hyperparameters: ``parrot-train``
-
-The ``parrot-train`` command is the primary command for training a network with PARROT. By default, users need only to specify 
-their data, where they want to save their output, and some basic information on the type of machine learning problem the are 
-tackling. Beyond this, there are a suite of other options that users can provide to tailor their network to their particular 
-needs. Users can provide specific hyperparameters to craft their network, they can manually specify what samples in their
-data set are trained on and which are held out as test data, they can choose to output information and figures on their network's
-performance on the test data, and much more!
-
-### 2. Optimize hyperparameters and train a network: ``parrot-optimize``
-
-The ``parrot-optimize`` command initiates an extensive search for the best-performing network hyperparameters for a given
-dataset using Bayesian optimiztion. Three hyperparameters, the learning rate, number of hidden layers, and hidden vector size
-can greatly impact network performance and training speed, so it is important to tune these for each particular dataset. This
-command will search across hyperparameter space by iteratively training and validating network performance (with 5-fold cross
-validation). The best performing hyperparameters will be selected, and used to train a network from scratch as if running
-``parrot_train`` with these parameters. Note that since this command take a significant amount of time to run since it involves
-searching for the best hyperparameters.
-
-### 3. Generate predictions with a trained network: ``parrot-predict``
-
-Once a network has been trained for a particular machine learning task, the user can generate predictions on new sequences
-with this network using the ``parrot-predict`` command. The user provides a list of sequences they would like to predict and
-the saved network, and a file is outputted with the predictions.
-
-### Copyright
-
-Copyright (c) 2020-2022, Holehouse Lab
-
-#### Acknowledgements
- 
-Project based on the 
-[Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.3.
```

### Comparing `idptools-parrot-1.7.0/idptools_parrot.egg-info/SOURCES.txt` & `idptools-parrot-1.7.4/idptools_parrot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/__init__.py` & `idptools-parrot-1.7.4/parrot/__init__.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/bayesian_optimization.py` & `idptools-parrot-1.7.4/parrot/bayesian_optimization.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/brnn_architecture.py` & `idptools-parrot-1.7.4/parrot/brnn_architecture.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/brnn_plot.py` & `idptools-parrot-1.7.4/parrot/brnn_plot.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/encode_sequence.py` & `idptools-parrot-1.7.4/parrot/encode_sequence.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/process_input_data.py` & `idptools-parrot-1.7.4/parrot/process_input_data.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/py_predictor.py` & `idptools-parrot-1.7.4/parrot/py_predictor.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/tools/class_balancing.py` & `idptools-parrot-1.7.4/parrot/tools/class_balancing.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/tools/cli.py` & `idptools-parrot-1.7.4/parrot/tools/cli.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/tools/dataset_warnings.py` & `idptools-parrot-1.7.4/parrot/tools/dataset_warnings.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/tools/preproc.py` & `idptools-parrot-1.7.4/parrot/tools/preproc.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/tools/validate_args.py` & `idptools-parrot-1.7.4/parrot/tools/validate_args.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/parrot/train_network.py` & `idptools-parrot-1.7.4/parrot/train_network.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/scripts/parrot-cvsplit` & `idptools-parrot-1.7.4/scripts/parrot-cvsplit`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/scripts/parrot-optimize` & `idptools-parrot-1.7.4/scripts/parrot-optimize`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/scripts/parrot-predict` & `idptools-parrot-1.7.4/scripts/parrot-predict`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/scripts/parrot-preprocess` & `idptools-parrot-1.7.4/scripts/parrot-preprocess`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/scripts/parrot-train` & `idptools-parrot-1.7.4/scripts/parrot-train`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/setup.py` & `idptools-parrot-1.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,13 +65,13 @@
             'seaborn',
             'pandas'],
 
     extras_require={
             'optimize': ['GPy', 'GPyOpt'] },
 
 
-    python_requires=">=3.9,<3.10.0",          # Python version restrictions
+    python_requires=">=3.7,<3.11.0",          # Python version restrictions
 
     # Manual control if final package is compressible or not, set False to prevent the .egg from being made
     zip_safe=False,
 
 )
```

### Comparing `idptools-parrot-1.7.0/tests/test_file_io.py` & `idptools-parrot-1.7.4/tests/test_file_io.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/tests/test_parrot.py` & `idptools-parrot-1.7.4/tests/test_parrot.py`

 * *Files identical despite different names*

### Comparing `idptools-parrot-1.7.0/versioneer.py` & `idptools-parrot-1.7.4/versioneer.py`

 * *Files identical despite different names*

