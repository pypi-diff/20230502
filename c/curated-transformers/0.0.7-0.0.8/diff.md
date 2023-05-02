# Comparing `tmp/curated-transformers-0.0.7.tar.gz` & `tmp/curated-transformers-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-transformers-0.0.7.tar", last modified: Tue Apr 18 10:23:30 2023, max compression
+gzip compressed data, was "curated-transformers-0.0.8.tar", last modified: Tue May  2 15:19:14 2023, max compression
```

## Comparing `curated-transformers-0.0.7.tar` & `curated-transformers-0.0.8.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.058464 curated-transformers-0.0.7/
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      101 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1267 2023-04-18 10:23:30.058464 curated-transformers-0.0.7/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      954 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.034464 curated-transformers-0.0.7/curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)       41 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      570 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.034464 curated-transformers-0.0.7/curated_transformers/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4050 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/cli/debug_pieces.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4697 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/cli/quantize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4688 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.038464 curated-transformers-0.0.7/curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      438 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24143 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/architectures.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1206 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19182 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/listeners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4102 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/output.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4016 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pooling.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.042464 curated-transformers-0.0.7/curated_transformers/models/pytorch/
--rw-r--r--   0 vsts      (1001) docker     (122)      194 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      583 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/activations.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.042464 curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/
--rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2251 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2364 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)      949 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/layer_group.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2259 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/attention.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.042464 curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3795 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1739 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4775 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/layer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1240 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/curated_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      890 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10982 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/hf_util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.046464 curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1392 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1781 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1882 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/pytorch/scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/remove_eos_bos.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4650 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2271 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/types.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7876 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10279 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/models/with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.046464 curated-transformers-0.0.7/curated_transformers/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       37 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17281 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/pipeline/transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.046464 curated-transformers-0.0.7/curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2204 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.050464 curated-transformers-0.0.7/curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3207 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_hf_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2608 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_listeners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4550 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_pooling.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1419 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6139 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_transformer_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3176 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4313 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/models/test_with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.050464 curated-transformers-0.0.7/curated_transformers/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17306 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/pipeline/test_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2703 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/pipeline/toy-en-corpus.spacy
--rw-r--r--   0 vsts      (1001) docker     (122)      406 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/test_cli_app.py
--rw-r--r--   0 vsts      (1001) docker     (122)      794 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/test_torchscript_wrapper.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.054464 curated-transformers-0.0.7/curated_transformers/tests/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3369 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4054 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1275 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2737 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7925 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4819 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_xlmr_adapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)      138 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy-chars.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy-vocab.json
--rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy.model
--rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy.wordpieces
--rw-r--r--   0 vsts      (1001) docker     (122)      482 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.058464 curated-transformers-0.0.7/curated_transformers/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3612 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3713 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5394 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2500 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/sentencepiece_adapters.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3823 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)      557 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/types.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5890 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/tokenization/wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2711 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/curated_transformers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-18 10:23:30.034464 curated-transformers-0.0.7/curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1267 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4184 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     3136 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       56 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-18 10:23:30.000000 curated-transformers-0.0.7/curated_transformers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     3858 2023-04-18 10:23:30.058464 curated-transformers-0.0.7/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-04-18 10:21:24.000000 curated-transformers-0.0.7/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.819089 curated-transformers-0.0.8/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      101 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1267 2023-05-02 15:19:14.819089 curated-transformers-0.0.8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      954 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.799089 curated-transformers-0.0.8/curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)       41 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      570 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.803089 curated-transformers-0.0.8/curated_transformers/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4050 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/cli/debug_pieces.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4697 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/cli/quantize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4688 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.803089 curated-transformers-0.0.8/curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      438 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24143 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/architectures.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1206 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19182 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4102 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/output.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4016 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pooling.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.807089 curated-transformers-0.0.8/curated_transformers/models/pytorch/
+-rw-r--r--   0 vsts      (1001) docker     (122)      194 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      583 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/activations.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.807089 curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/
+-rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2251 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2364 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      949 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/layer_group.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2259 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/attention.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.811089 curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3795 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1739 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4775 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/layer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1240 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/curated_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      890 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10982 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/hf_util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.811089 curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1392 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1781 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1882 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/remove_eos_bos.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4650 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2271 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7876 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10279 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.811089 curated-transformers-0.0.8/curated_transformers/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       37 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17281 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/pipeline/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.811089 curated-transformers-0.0.8/curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2204 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.811089 curated-transformers-0.0.8/curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3207 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_hf_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2608 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4550 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_pooling.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1419 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6139 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_transformer_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3176 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4313 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.811089 curated-transformers-0.0.8/curated_transformers/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17306 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/pipeline/test_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2703 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/pipeline/toy-en-corpus.spacy
+-rw-r--r--   0 vsts      (1001) docker     (122)      406 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/test_cli_app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      794 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/test_torchscript_wrapper.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.815089 curated-transformers-0.0.8/curated_transformers/tests/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3369 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4054 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1275 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2737 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7925 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4819 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_xlmr_adapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      138 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy-chars.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy-vocab.json
+-rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy.wordpieces
+-rw-r--r--   0 vsts      (1001) docker     (122)      482 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.819089 curated-transformers-0.0.8/curated_transformers/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3612 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3713 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5394 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2500 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/sentencepiece_adapters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3823 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      557 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5890 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2711 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.803089 curated-transformers-0.0.8/curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1267 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4184 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     3136 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       56 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3858 2023-05-02 15:19:14.819089 curated-transformers-0.0.8/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/setup.py
```

### Comparing `curated-transformers-0.0.7/LICENSE` & `curated-transformers-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/PKG-INFO` & `curated-transformers-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 0.0.7
+Version: 0.0.8
 Summary: Curated transformer models
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `curated-transformers-0.0.7/README.md` & `curated-transformers-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/_compat.py` & `curated-transformers-0.0.8/curated_transformers/_compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/cli/debug_pieces.py` & `curated-transformers-0.0.8/curated_transformers/cli/debug_pieces.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/cli/quantize.py` & `curated-transformers-0.0.8/curated_transformers/cli/quantize.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/errors.py` & `curated-transformers-0.0.8/curated_transformers/errors.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/architectures.py` & `curated-transformers-0.0.8/curated_transformers/models/architectures.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/hf_loader.py` & `curated-transformers-0.0.8/curated_transformers/models/hf_loader.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/listeners.py` & `curated-transformers-0.0.8/curated_transformers/models/listeners.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/output.py` & `curated-transformers-0.0.8/curated_transformers/models/output.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pooling.py` & `curated-transformers-0.0.8/curated_transformers/models/pooling.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/activations.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/activations.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/config.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/encoder.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/albert/layer_group.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/layer_group.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/attention.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/attention.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/config.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/embeddings.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/encoder.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/bert/layer.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/layer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/curated_transformer.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/curated_transformer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/embeddings.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/hf_util.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/hf_util.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/config.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/embeddings.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/roberta/encoder.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/pytorch/scalar_weight.py` & `curated-transformers-0.0.8/curated_transformers/models/pytorch/scalar_weight.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/remove_eos_bos.py` & `curated-transformers-0.0.8/curated_transformers/models/remove_eos_bos.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/scalar_weight.py` & `curated-transformers-0.0.8/curated_transformers/models/scalar_weight.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/types.py` & `curated-transformers-0.0.8/curated_transformers/models/types.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/with_non_ws_tokens.py` & `curated-transformers-0.0.8/curated_transformers/models/with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/models/with_strided_spans.py` & `curated-transformers-0.0.8/curated_transformers/models/with_strided_spans.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/pipeline/transformer.py` & `curated-transformers-0.0.8/curated_transformers/pipeline/transformer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/conftest.py` & `curated-transformers-0.0.8/curated_transformers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/models/test_hf_model.py` & `curated-transformers-0.0.8/curated_transformers/tests/models/test_hf_model.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/models/test_listeners.py` & `curated-transformers-0.0.8/curated_transformers/tests/models/test_listeners.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/models/test_pooling.py` & `curated-transformers-0.0.8/curated_transformers/tests/models/test_pooling.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/models/test_scalar_weight.py` & `curated-transformers-0.0.8/curated_transformers/tests/models/test_scalar_weight.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/models/test_transformer_model.py` & `curated-transformers-0.0.8/curated_transformers/tests/models/test_transformer_model.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/models/test_with_non_ws_tokens.py` & `curated-transformers-0.0.8/curated_transformers/tests/models/test_with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/models/test_with_strided_spans.py` & `curated-transformers-0.0.8/curated_transformers/tests/models/test_with_strided_spans.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/pipeline/test_transformer.py` & `curated-transformers-0.0.8/curated_transformers/tests/pipeline/test_transformer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/pipeline/toy-en-corpus.spacy` & `curated-transformers-0.0.8/curated_transformers/tests/pipeline/toy-en-corpus.spacy`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/test_torchscript_wrapper.py` & `curated-transformers-0.0.8/curated_transformers/tests/test_torchscript_wrapper.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_bbpe_encoder.py` & `curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_bbpe_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from curated_transformers.tokenization.hf_loader import build_hf_piece_encoder_loader_v1
 from curated_transformers._compat import has_hf_transformers
 
 
 @pytest.fixture
 def toy_encoder(test_dir):
     encoder = build_byte_bpe_encoder_v1()
-    encoder.init = registry.model_loaders.get("curated-transformers.ByteBPELoader.v1")(
+    encoder.init = registry.model_loaders.get("curated-transformers.ByteBpeLoader.v1")(
         vocab_path=test_dir / "toy-vocab.json", merges_path=test_dir / "toy-merges.txt"
     )
     encoder.initialize()
     return encoder
 
 
 @pytest.mark.slow
```

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_char_encoder.py` & `curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_char_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_registry.py` & `curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_registry.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from curated_transformers.util import registry
 
 
 @pytest.mark.parametrize(
     "encoder_name",
     [
         "curated-transformers.BertWordpieceEncoder.v1",
-        "curated-transformers.ByteBPEEncoder.v1",
+        "curated-transformers.ByteBpeEncoder.v1",
         "curated-transformers.CamembertSentencepieceEncoder.v1",
         "curated-transformers.CharEncoder.v1",
         "curated-transformers.SentencepieceEncoder.v1",
         "curated-transformers.WordpieceEncoder.v1",
         "curated-transformers.XlmrSentencepieceEncoder.v1",
     ],
 )
 def test_encoder_from_registry(encoder_name):
     spacy_registry.architectures.get(encoder_name)()
 
 
 @pytest.mark.parametrize(
     "loader_name",
     [
-        "curated-transformers.ByteBPELoader.v1",
+        "curated-transformers.ByteBpeLoader.v1",
         "curated-transformers.CharEncoderLoader.v1",
         "curated-transformers.HFTransformerEncoderLoader.v1",
         "curated-transformers.HFPieceEncoderLoader.v1",
         "curated-transformers.PyTorchCheckpointLoader.v1",
         "curated-transformers.SentencepieceLoader.v1",
         "curated-transformers.WordpieceLoader.v1",
     ],
```

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_sentencepiece_encoder.py` & `curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_sentencepiece_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_wordpiece_encoder.py` & `curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_wordpiece_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/tokenization/test_xlmr_adapter.py` & `curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_xlmr_adapter.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy-merges.txt` & `curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy-merges.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy-vocab.json` & `curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy-vocab.json`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy.model` & `curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy.model`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tests/tokenization/toy.wordpieces` & `curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy.wordpieces`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tokenization/__init__.py` & `curated-transformers-0.0.8/curated_transformers/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tokenization/bbpe_encoder.py` & `curated-transformers-0.0.8/curated_transformers/tokenization/bbpe_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tokenization/char_encoder.py` & `curated-transformers-0.0.8/curated_transformers/tokenization/char_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tokenization/hf_loader.py` & `curated-transformers-0.0.8/curated_transformers/tokenization/hf_loader.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tokenization/sentencepiece_adapters.py` & `curated-transformers-0.0.8/curated_transformers/tokenization/sentencepiece_adapters.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tokenization/sentencepiece_encoder.py` & `curated-transformers-0.0.8/curated_transformers/tokenization/sentencepiece_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tokenization/types.py` & `curated-transformers-0.0.8/curated_transformers/tokenization/types.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/tokenization/wordpiece_encoder.py` & `curated-transformers-0.0.8/curated_transformers/tokenization/wordpiece_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers/util.py` & `curated-transformers-0.0.8/curated_transformers/util.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers.egg-info/PKG-INFO` & `curated-transformers-0.0.8/curated_transformers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 0.0.7
+Version: 0.0.8
 Summary: Curated transformer models
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `curated-transformers-0.0.7/curated_transformers.egg-info/SOURCES.txt` & `curated-transformers-0.0.8/curated_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.7/curated_transformers.egg-info/entry_points.txt` & `curated-transformers-0.0.8/curated_transformers.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [spacy_architectures]
 curated-transformers.AlbertTransformer.v1 = curated_transformers.models:build_albert_transformer_model_v1
 curated-transformers.BertTransformer.v1 = curated_transformers.models:build_bert_transformer_model_v1
 curated-transformers.BertWordpieceEncoder.v1 = curated_transformers.tokenization:build_bert_wordpiece_encoder_v1
-curated-transformers.ByteBPEEncoder.v1 = curated_transformers.tokenization:build_byte_bpe_encoder_v1
+curated-transformers.ByteBpeEncoder.v1 = curated_transformers.tokenization:build_byte_bpe_encoder_v1
 curated-transformers.CamembertSentencepieceEncoder.v1 = curated_transformers.tokenization:build_camembert_sentencepiece_encoder_v1
 curated-transformers.CamembertTransformer.v1 = curated_transformers.models:build_camembert_transformer_model_v1
 curated-transformers.CharEncoder.v1 = curated_transformers.tokenization:build_char_encoder_v1
 curated-transformers.LastTransformerLayerListener.v1 = curated_transformers.models.listeners:build_last_transformer_layer_listener_v1
 curated-transformers.RobertaTransformer.v1 = curated_transformers.models:build_roberta_transformer_model_v1
 curated-transformers.ScalarWeight.v1 = curated_transformers.models:build_scalar_weight_v1
 curated-transformers.ScalarWeightingListener.v1 = curated_transformers.models.listeners:build_scalar_weighting_listener_v1
@@ -24,14 +24,14 @@
 curated-transformers.debug_pieces = curated_transformers.cli.debug_pieces:debug_pieces_cli
 curated-transformers.quantize = curated_transformers.cli.quantize:quantize_cli
 
 [spacy_factories]
 curated_transformer = curated_transformers.pipeline.transformer:make_transformer
 
 [thinc_model_loaders]
-curated-transformers.ByteBPELoader.v1 = curated_transformers.tokenization:build_byte_bpe_encoder_loader_v1
+curated-transformers.ByteBpeLoader.v1 = curated_transformers.tokenization:build_byte_bpe_encoder_loader_v1
 curated-transformers.CharEncoderLoader.v1 = curated_transformers.tokenization:build_char_encoder_loader_v1
 curated-transformers.HFPieceEncoderLoader.v1 = curated_transformers.tokenization:build_hf_piece_encoder_loader_v1
 curated-transformers.HFTransformerEncoderLoader.v1 = curated_transformers.models:build_hf_transformer_encoder_loader_v1
 curated-transformers.PyTorchCheckpointLoader.v1 = curated_transformers.models:build_pytorch_checkpoint_loader_v1
 curated-transformers.SentencepieceLoader.v1 = curated_transformers.tokenization:build_sentencepiece_encoder_loader_v1
 curated-transformers.WordpieceLoader.v1 = curated_transformers.tokenization:build_wordpiece_encoder_loader_v1
```

### Comparing `curated-transformers-0.0.7/setup.cfg` & `curated-transformers-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.7
+version = 0.0.8
 description = Curated transformer models
 url = https://github.com/explosion/curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
@@ -29,27 +29,27 @@
 	curated-transformers.XlmrTransformer.v1 = curated_transformers.models:build_xlmr_transformer_model_v1
 	curated-transformers.WithStridedSpans.v1 = curated_transformers.models:build_with_strided_spans_v1
 	curated-transformers.ScalarWeight.v1 = curated_transformers.models:build_scalar_weight_v1
 	curated-transformers.TransformerLayersListener.v1 = curated_transformers.models.listeners:build_transformer_layers_listener_v1
 	curated-transformers.LastTransformerLayerListener.v1 = curated_transformers.models.listeners:build_last_transformer_layer_listener_v1
 	curated-transformers.ScalarWeightingListener.v1 = curated_transformers.models.listeners:build_scalar_weighting_listener_v1
 	curated-transformers.BertWordpieceEncoder.v1 = curated_transformers.tokenization:build_bert_wordpiece_encoder_v1
-	curated-transformers.ByteBPEEncoder.v1 = curated_transformers.tokenization:build_byte_bpe_encoder_v1
+	curated-transformers.ByteBpeEncoder.v1 = curated_transformers.tokenization:build_byte_bpe_encoder_v1
 	curated-transformers.CamembertSentencepieceEncoder.v1 = curated_transformers.tokenization:build_camembert_sentencepiece_encoder_v1
 	curated-transformers.CharEncoder.v1 = curated_transformers.tokenization:build_char_encoder_v1
 	curated-transformers.SentencepieceEncoder.v1 = curated_transformers.tokenization:build_sentencepiece_encoder_v1
 	curated-transformers.WordpieceEncoder.v1 = curated_transformers.tokenization:build_wordpiece_encoder_v1
 	curated-transformers.XlmrSentencepieceEncoder.v1 = curated_transformers.tokenization:build_xlmr_sentencepiece_encoder_v1
 spacy_callbacks = 
 	curated-transformers.gradual_transformer_unfreezing.v1 = curated_transformers.util:create_gradual_transformer_unfreezing
 spacy_cli = 
 	curated-transformers.debug_pieces = curated_transformers.cli.debug_pieces:debug_pieces_cli
 	curated-transformers.quantize = curated_transformers.cli.quantize:quantize_cli
 thinc_model_loaders = 
-	curated-transformers.ByteBPELoader.v1 = curated_transformers.tokenization:build_byte_bpe_encoder_loader_v1
+	curated-transformers.ByteBpeLoader.v1 = curated_transformers.tokenization:build_byte_bpe_encoder_loader_v1
 	curated-transformers.CharEncoderLoader.v1 = curated_transformers.tokenization:build_char_encoder_loader_v1
 	curated-transformers.HFTransformerEncoderLoader.v1 = curated_transformers.models:build_hf_transformer_encoder_loader_v1
 	curated-transformers.HFPieceEncoderLoader.v1 = curated_transformers.tokenization:build_hf_piece_encoder_loader_v1
 	curated-transformers.PyTorchCheckpointLoader.v1 = curated_transformers.models:build_pytorch_checkpoint_loader_v1
 	curated-transformers.SentencepieceLoader.v1 = curated_transformers.tokenization:build_sentencepiece_encoder_loader_v1
 	curated-transformers.WordpieceLoader.v1 = curated_transformers.tokenization:build_wordpiece_encoder_loader_v1
```

