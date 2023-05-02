# Comparing `tmp/transition_neural_parser-0.5.3.tar.gz` & `tmp/transition_neural_parser-0.5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transition_neural_parser-0.5.3.tar", last modified: Tue May  2 14:57:40 2023, max compression
+gzip compressed data, was "transition_neural_parser-0.5.3.1.tar", last modified: Thu Apr 27 04:44:36 2023, max compression
```

## Comparing `transition_neural_parser-0.5.3.tar` & `transition_neural_parser-0.5.3.1.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:40.018119 transition_neural_parser-0.5.3/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10776 2023-04-24 13:10:54.000000 transition_neural_parser-0.5.3/LICENSE
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10711 2023-05-02 14:57:40.017552 transition_neural_parser-0.5.3/PKG-INFO
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9958 2023-05-02 14:04:51.000000 transition_neural_parser-0.5.3/README.md
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      980 2023-05-02 14:57:33.000000 transition_neural_parser-0.5.3/pyproject.toml
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       38 2023-05-02 14:57:40.018202 transition_neural_parser-0.5.3/setup.cfg
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1794 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/setup.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.750837 transition_neural_parser-0.5.3/src/
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.801142 transition_neural_parser-0.5.3/src/fairseq_ext/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      165 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/__init__.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.802989 transition_neural_parser-0.5.3/src/fairseq_ext/amr_reform/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_reform/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    19730 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_reform/o10_action_reformer_subtok.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.822813 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10043 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8788 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15698 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15835 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    21406 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize_graphmp.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    21411 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize_graphmp_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10755 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_graphmp.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10336 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_graphmp_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8638 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/old_action_info.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    28857 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/old_action_info_binarize.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6018 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/average_checkpoints.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1100 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/binarize.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.827197 transition_neural_parser-0.5.3/src/fairseq_ext/criterions/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      679 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/criterions/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12919 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12636 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer_alignment.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.843203 transition_neural_parser-0.5.3/src/fairseq_ext/data/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    29683 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_bartsv_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    29892 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30695 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_goldamr_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30770 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_graphmp_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10918 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_bpe.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9147 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/data_utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16218 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/indexed_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18120 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/language_pair_dataset.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.851013 transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6506 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/binarize_encodings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9588 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/composite_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5255 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/mapavg_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8609 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/sentence_encoding.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15450 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/generate.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16901 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/generate_sliding.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.872908 transition_neural_parser-0.5.3/src/fairseq_ext/models/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      796 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8953 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/attention_masks.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5741 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/graph_attention_masks.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8485 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/graphmp_attention_masks.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    79650 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    84503 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bart.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    79562 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bart_sattn.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    75031 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    73280 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bartsv_sattn.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    64589 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_graph.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    84683 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_graphmp.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.883112 transition_neural_parser-0.5.3/src/fairseq_ext/modules/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/modules/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6304 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/modules/factored_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23865 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/modules/multihead_attention.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23312 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/modules/multihead_attention_old.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    17425 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/modules/transformer_layer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12391 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/modules/transformer_layer_old.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    31215 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/options.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    20449 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/options_train.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15142 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/preprocess.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18504 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/preprocess_bart.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    14481 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/preprocess_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13349 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/preprocess_graphmp.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.889815 transition_neural_parser-0.5.3/src/fairseq_ext/roberta/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/roberta/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4761 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/roberta/binarize_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9693 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/roberta/pretrained_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9316 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/roberta/pretrained_embeddings_bert.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    65291 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    65757 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    57973 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator_graph.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62664 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator_graphmp.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.902379 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      580 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    22251 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    27439 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_bart.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    55372 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_bart_dyo.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    28086 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    24602 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_graphmp.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    24616 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_graphmp_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       81 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tokenizer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23242 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/train.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7661 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1052 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/utils_font.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1748 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/utils_import.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.950107 transition_neural_parser-0.5.3/src/ibm_neural_aligner/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1226 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/README.md
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6389 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/align_leamr.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8746 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/align_utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1980 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/alignment_decoder.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5840 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/amr_utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7611 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/ccc.launch_many_jobs.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9753 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/ccc.summarize.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      687 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/dummy_align.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    26107 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/evaluation.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5402 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/formatter.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4784 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/gcn.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      485 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/leamr_align.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     2991 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/lexicon.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    60552 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/main.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1158 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/make_splits.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1752 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/metric_utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4322 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/pretrained_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13907 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/resolve_manual_alignments.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3752 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_detailed_eval.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      874 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_eval.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    11929 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_model_selection.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7781 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_sampler.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    34661 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/standalone_elmo.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1145 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/tokenize_amr.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4869 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/transformer_lm.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    19700 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/tree_lstm.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8380 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/tree_rnn.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3709 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/view_manual_alignments.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3202 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/vocab.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      380 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/vocab_definitions.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.981478 transition_neural_parser-0.5.3/src/transition_amr_parser/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      867 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/__init__.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:40.010840 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3749 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/amr_parser.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    37837 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_data_oracle.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13849 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_fake_parse.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62718 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62580 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15856 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine_reformer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15861 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine_reformer_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    20120 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/parse.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4040 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/roberta_utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1355 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/add_id_to_amr.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      635 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/add_sentence_amrs_to_file.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    52645 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/amr.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    46594 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/amr_aligner.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5278 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/amr_constituents.py
--rwxrwxr-x   0 gxxu     (700773) gxxu     (606684)     6746 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/amr_latex.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    74725 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/amr_machine.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4756 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/clbar.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5057 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/force_overlap_actions.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    45407 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/gold_subgraph_align.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18047 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/io.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10706 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/make_sliding_splits.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5548 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/merge_sliding_splits.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    50558 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/parse.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6358 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/plots.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:40.016978 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10711 2023-05-02 14:57:39.000000 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/PKG-INFO
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6377 2023-05-02 14:57:39.000000 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        1 2023-05-02 14:57:39.000000 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      116 2023-05-02 14:57:39.000000 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/entry_points.txt
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      241 2023-05-02 14:57:39.000000 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/requires.txt
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       53 2023-05-02 14:57:39.000000 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/top_level.txt
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.326697 transition_neural_parser-0.5.3.1/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10776 2023-04-24 13:10:54.000000 transition_neural_parser-0.5.3.1/LICENSE
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16136 2023-04-27 04:44:36.326094 transition_neural_parser-0.5.3.1/PKG-INFO
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15543 2023-04-25 17:50:32.000000 transition_neural_parser-0.5.3.1/README.md
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      704 2023-04-27 04:39:47.000000 transition_neural_parser-0.5.3.1/pyproject.toml
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       38 2023-04-27 04:44:36.326807 transition_neural_parser-0.5.3.1/setup.cfg
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1816 2023-04-27 04:43:18.000000 transition_neural_parser-0.5.3.1/setup.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.115540 transition_neural_parser-0.5.3.1/src/
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.151945 transition_neural_parser-0.5.3.1/src/fairseq_ext/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      165 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/__init__.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.153529 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_reform/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_reform/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    19730 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_reform/o10_action_reformer_subtok.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.172583 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10043 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8788 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15698 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15835 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    21406 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize_graphmp.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    21411 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize_graphmp_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10755 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_graphmp.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10336 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_graphmp_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8638 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/old_action_info.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    28857 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/old_action_info_binarize.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6018 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/average_checkpoints.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1100 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/binarize.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.176730 transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      679 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12919 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12636 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer_alignment.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.190420 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    29683 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_bartsv_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    29892 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30695 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_goldamr_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30770 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_graphmp_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10918 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_bpe.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9147 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/data_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16218 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/indexed_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18120 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/language_pair_dataset.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.198269 transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6506 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/binarize_encodings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9588 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/composite_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5255 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/mapavg_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8609 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/sentence_encoding.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15450 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/generate.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16901 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/generate_sliding.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.216327 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      796 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8953 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/attention_masks.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5741 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/graph_attention_masks.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8485 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/graphmp_attention_masks.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    79650 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    84503 2023-04-24 15:25:46.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bart.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    79562 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bart_sattn.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    75031 2023-04-24 15:25:04.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    73280 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bartsv_sattn.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    64589 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_graph.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    84683 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_graphmp.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.226376 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6304 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/factored_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23865 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/multihead_attention.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23312 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/multihead_attention_old.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    17425 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/transformer_layer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12391 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/transformer_layer_old.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    31215 2023-04-24 14:16:48.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/options.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    20449 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/options_train.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15142 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18504 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess_bart.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    14481 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13349 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess_graphmp.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.231622 transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4761 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/binarize_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9693 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/pretrained_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9316 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/pretrained_embeddings_bert.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    65291 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    65757 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    57973 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator_graph.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62664 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator_graphmp.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.243154 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      580 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    22251 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    27439 2023-04-24 15:25:16.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_bart.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    55372 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_bart_dyo.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    28086 2023-04-24 15:25:25.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    24602 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_graphmp.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    24616 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_graphmp_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       81 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tokenizer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23251 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/train.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7661 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1052 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/utils_font.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1748 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/utils_import.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.283621 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1226 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/README.md
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6389 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/align_leamr.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8746 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/align_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1958 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/alignment_decoder.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5840 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/amr_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7611 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/ccc.launch_many_jobs.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9753 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/ccc.summarize.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      687 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/dummy_align.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    26107 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/evaluation.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5402 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/formatter.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4784 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/gcn.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      485 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/leamr_align.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     2991 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/lexicon.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    60552 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/main.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1158 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/make_splits.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1752 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/metric_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4322 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/pretrained_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13907 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/resolve_manual_alignments.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3752 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/run_detailed_eval.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      874 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/run_eval.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    11929 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/run_model_selection.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7781 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/run_sampler.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    34661 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/standalone_elmo.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1145 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/tokenize_amr.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4869 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/transformer_lm.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    19700 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/tree_lstm.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8380 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/tree_rnn.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3709 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/view_manual_alignments.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3202 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/vocab.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      380 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/vocab_definitions.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.305271 transition_neural_parser-0.5.3.1/src/transition_amr_parser/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      867 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/__init__.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.319685 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3749 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/amr_parser.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    37837 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_data_oracle.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13849 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_fake_parse.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62718 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62580 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15856 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine_reformer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15861 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine_reformer_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    20120 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/parse.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4040 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/roberta_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1355 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/add_id_to_amr.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      635 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/add_sentence_amrs_to_file.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    52645 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    46594 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_aligner.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5278 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_constituents.py
+-rwxrwxr-x   0 gxxu     (700773) gxxu     (606684)     6746 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_latex.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    74725 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_machine.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4756 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/clbar.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5057 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/force_overlap_actions.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    45407 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/gold_subgraph_align.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18047 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/io.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10706 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/make_sliding_splits.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5548 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/merge_sliding_splits.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    50199 2023-04-26 18:24:35.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/parse.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6358 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/plots.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.324556 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16136 2023-04-27 04:44:36.321212 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6377 2023-04-27 04:44:36.321879 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        1 2023-04-27 04:44:36.322376 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      116 2023-04-27 04:44:36.323086 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/entry_points.txt
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      235 2023-04-27 04:44:36.323949 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/requires.txt
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       53 2023-04-27 04:44:36.324652 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/top_level.txt
```

### Comparing `transition_neural_parser-0.5.3/LICENSE` & `transition_neural_parser-0.5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/PKG-INFO` & `transition_neural_parser-0.5.3.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,97 @@
-Metadata-Version: 2.1
-Name: transition_neural_parser
-Version: 0.5.3
-Summary: The package for transition based nueral AMR parser
-Author-email: Ramon <ramon.astudillo@ibm.com>, Young-Suk <ysuklee@us.ibm.com>, Tahira <tnaseem@us.ibm.com>, Sadhana <sadhana.kumaravel1@ibm.com>, GX <GX.Xu@ibm.com>, Hans <raduf@us.ibm.com>, Salim <roukos@us.ibm.com>
-Project-URL: homepage, https://github.ibm.com/mnlp/transition-amr-parser/tree/master
-Project-URL: tracker, https://github.ibm.com/mnlp/transition-amr-parser/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: ~=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Transition-based Neural Parser
 ============================
 
-State-of-the-Art Abstract Meaning Representation (AMR) parsing, see [papers
-with code](https://paperswithcode.com/task/amr-parsing). Models both
-distribution over graphs and aligments with a transition-based approach. Parser
-supports any other graph formalism as long as it is expressed in [Penman
-notation](https://penman.readthedocs.io/en/latest/notation.html).
-
-Some of the main features
-
-- [Smatch](https://github.com/snowblink14/smatch) wrapper providing [significance testing](scripts/README.md#paired-boostrap-significance-test-for-Smatch) for Smatch and [MBSE](scripts/README.md#maximum-bayesian-smatch-ensemble-mbse) ensembling.
-- `Structured-BART` [(Zhou et al 2021b)](https://aclanthology.org/2021.emnlp-main.507/) with [trained checkpoints](#available-pretrained-model-checkpoints) for document-level AMR [(Naseem et al 2022)](https://aclanthology.org/2022.naacl-main.256), MBSE [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) and latent alignments training [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464)
-- `Structured-mBART` for multi-lingual support (EN, DE, Zh, IT) [(Lee et al 2022)](https://arxiv.org/abs/2112.07790)
-- Action-Pointer Transformer (`APT`) [(Zhou et al 2021)](https://www.aclweb.org/anthology/2021.naacl-main.443), checkout `action-pointer` branch 
-- `Stack-Transformer` [(Fernandez Astudillo et al 2020)](https://www.aclweb.org/anthology/2020.findings-emnlp.89), checkout `stack-Transformer` branch
 
-## Install Instructions
+## transition-neural-parser
+**transition-neural-parser** is a powerful and easy-to-use Python package that provides a state-of-the-art neural transition-based parser for Abstract Meaning Representation (AMR). 
+
+AMR is a semantic formalism used to represent the meaning of natural language sentences in a structured and machine-readable format. The package is designed to enable users to perform AMR parsing with high accuracy and generate reliable token-to-node alignments, which are crucial for various natural language understanding and generation tasks.
+
 
-create and activate a virtual environment with python 3.8, for example
+## Pip Installation Instructions
+**Step 1: Create and activate a new conda environment;**
+
+To ensure compatibility and prevent potential conflicts, create a new conda environment with Python 3.8:
 
 ```
 conda create -y -p ./cenv_x86 python=3.8
-conda activate ./cenv_x86
 ```
 
-or alternatively use `virtualenv` and `pyenv` for python versions. Note that
-all scripts source a `set_environment.sh` script that you can use to activate
-your virtual environment as above and set environment variables. If not used,
-just create an empty version
+Activate the newly created environment:
 
 ```
-# or e.g. put inside conda activate ./cenv_x86
-touch set_environment.sh
+conda activate ./cenv_x86
 ```
 
-Then install the parser package using pip. You will need to install
-`torch-scatter` by separate since it is custom built for CUDA. Here we specify the
-call for `torch 1.13.1` and `cuda 11.7`. See [torch-scatter
-repository](https://pypi.org/project/torch-scatter/) to find the appropriate
-installation instructions.
+**Step 2: Install the package**
+
+Install the transition-neural-parser package using pip:
 
 ```
 pip install transition-neural-parser
 pip install torch-scatter -f https://data.pyg.org/whl/torch-1.13.1+cu117.html
 ```
 
-If you plan to edit the code, clone and install instead
+Alternatively, you can install locally; 
+Go to the root directory of the project and then run the following:
 
 ```
-# clone this repo (see link above), then
-cd transition-neural-parser
-pip install --editable .
-pip install torch-scatter -f https://data.pyg.org/whl/torch-1.13.1+cu117.html
+pip install -e .
 ```
 
-If you want to train a document-level AMR parser you will also need 
+Note: The torch-scatter package is automatically set-up for most users using our default torch-1.13.1 and cu117 environment. However, in case you are choosing to use different environment set-up, or using non-linux servers, please visit the official [torch-scatter repository](https://pypi.org/project/torch-scatter/) to find the appropriate installation instructions.
+
+
+**Step 3: Install docAMR for document level parsing**
+
+For document-level AMR training and testing , the docAMR repo must be cloned and installed.
+
+[Link](https://aclanthology.org/2022.naacl-main.256.pdf) to NAACL 2022 paper DOCAMR: Multi-Sentence AMR Representation and Evaluation
 
 ```
 git clone https://github.com/IBM/docAMR.git
 cd docAMR
 pip install .
 cd ..
+
+```
+
+
+**(Optional) Step 4: Set a environment file (only for bash script training and evaluation)**
+
+We use a set_environment.sh script inside of which we activate conda environment; it is used for model training.
+
+First create the file at top-level directory of the project.
+```
+touch set_environment.sh
 ```
 
-## Parse with a pretrained model
+An example would be following, where the only line to change is where to source the conda.sh file. 
+```
+# inside set_environment.sh
+if [ ! -d cenv_x86 ];then
+    echo "Environment cenv_x86 not found"
+    exit 1
+else
+    printf "\033[94mconda activate ./cenv_x86\033[0m\n"
+    # replace the below line with the path your local conda location. 
+    source /dccstor/gxamr/anaconda3/etc/profile.d/conda.sh.  # Please change this line
+    conda activate ./cenv_x86
+fi
+```
+Note that all bash scripts always source set_environment.sh, so you do not need to source it yourself anymore. 
 
-Here is an example of how to download and use a pretrained AMR parser in Python
 
-```python
+## Decode with pretrained model
+**Python Option:** Download a pretrained AMR parser and run inference;
+
+Here is an example of how to download and use a pretrained AMR parser:
+
+```
 from transition_amr_parser.parse import AMRParser
 
 # Download and save a model named AMR3.0 to cache
 parser = AMRParser.from_pretrained('AMR3-structbart-L')
 tokens, positions = parser.tokenize('The girl travels and visits places')
 
 # Use parse_sentence() for single sentences or parse_sentences() for a batch
@@ -99,37 +105,20 @@
 print(amr.to_penman(jamr=False, isi=True))
 
 # Plot the graph (requires matplotlib)
 amr.plot()
 
 ```
 
-Note that Smatch does not support ISI-type alignments and gives worse results.
-Set `isi=False` to remove them. 
+This example demonstrates how to tokenize a document (list of sentences), parse it using the pretrained DocAMR parser, and print the resulting DocAMR graph in Penman notation. If you have matplotlib installed, you can also visualize the graph.
+The resulting graph represents coreference using *:same-as* edges. To change the representation and merge the coreferent nodes as in the paper, please refer to [the DocAMR repo](https://github.com/IBM/docAMR.git)
 
-You can also use the command line to run a pretrained model to parse a file:
+*DocAMR*
 
-```bash
-amr-parse -c $in_checkpoint -i $input_file -o file.amr
 ```
-
-Download models can invoked with `-m <config>` can be used as well.
-
-Note that Smatch does not support ISI and gives worse results. Use `--no-isi`
-to store alignments in `::alignments` meta data. Also use `--jamr` to add JAMR
-annotations in meta-data. Use `--no-isi` to store alignments in `::alignments`
-meta data. Also use `--jamr` to add JAMR annotations in meta-data.
-
-## Document-level Parsing
-
-This represents co-reference using `:same-as` edges. To change
-the representation and merge the co-referent nodes as in the paper, please refer
-to [the DocAMR repo](https://github.com/IBM/docAMR.git)
-
-```python
 from transition_amr_parser.parse import AMRParser
 
 # Download and save the docamr model to cache
 parser = AMRParser.from_pretrained('doc-sen-conll-amr-seed42')
 
 # Sentences in the doc
 doc = ["Hailey likes to travel." ,"She is going to London tomorrow.", "She will walk to Big Ben when she goes to London."]
@@ -151,63 +140,61 @@
 print(amr.to_penman(jamr=False, isi=True))
 
 # Plot the graph (requires matplotlib)
 amr.plot()
 
 ```
 
-To parse a document from the command line the input file `$doc_input_file` is a
-text file where each line is a sentence in the document and there is a newline
-('\n') separating every doc (even at the end) 
+**Command Line Option:** Use the command line to run a pretrained model to parse a file:
+
+```bash
+amr-parse -c $in_checkpoint -i $input_file -o file.amr
+```
+
+It will parse each line of `$input_file` separately. It assumes tokenization,
+use `--tokenize` otherwise. Once a model is unzipped, `-m <config>` can be used
+instead of `-c`. The `file.amr` will contain the PENMAN notation with ISI
+alignment annotations (`<node name>~<token position>`). Note that Smatch does
+not support ISI and gives worse results. Use `--no-isi` to store alignments in
+`::alignments` meta data. Also use `--jamr` to add JAMR annotations in
+meta-data.
+
+*DocAMR*
+
+To parse a document , 
+the input file ($doc_input_file) is a text file where each line is a sentence in the document and there is a newline ('\n') separating every doc (even at the end) 
 
 
 ```bash
-amr-parse -c $in_checkpoint --in-doc $doc_input_file -o file.docamr
+amr-parse -c $in_checkpoint --in-doc $doc_input_file -o file.docamr --sliding
 ```
 
+This will output a ".force_actions" file to the same directory as input , containing the actions needed to force sentence ends in the document as well as the output docamr "file.docamr"
 
-## Available Pretrained Model Checkpoints
 
-The models downloaded using `from_pretrained()` will be stored to the pytorch
-cache folder under:
-```python
+## Available Pretrained Model Checkpoints
+The models downloaded using from_pretrained() method will be stored to the pytorch cache folder as follows:
+```
 cache_dir = torch.hub._get_torch_home()
 ```
 
 This table shows you available pretrained model names to download;
 
-| pretrained model name      | corresponding file name                               | paper                                                           | beam10-Smatch |
-|:--------------------------:|:-----------------------------------------------------:|:---------------------------------------------------------------:|:-------------:|
-| AMR3-structbart-L-smpl     | amr3.0-structured-bart-large-neur-al-sampling5-seed42 | [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464) PR     | 82.9 (beam1)  |
-| AMR3-structbart-L          | amr3.0-structured-bart-large-neur-al-seed42           | [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464) MAP    | 82.6          |
-| AMR2-structbart-L          | amr2.0-structured-bart-large-neur-al-seed42           | [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464) MAP    | 84.0          |
-| AMR2-joint-ontowiki-seed42 | amr2joint_ontowiki2_g2g-structured-bart-large-seed42  | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 85.9          |
-| AMR2-joint-ontowiki-seed43 | amr2joint_ontowiki2_g2g-structured-bart-large-seed43  | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 85.9          |
-| AMR2-joint-ontowiki-seed44 | amr2joint_ontowiki2_g2g-structured-bart-large-seed44  | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 85.9          |
-| AMR3-joint-ontowiki-seed42 | amr3joint_ontowiki2_g2g-structured-bart-large-seed42  | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 84.4          |
-| AMR3-joint-ontowiki-seed43 | amr3joint_ontowiki2_g2g-structured-bart-large-seed43  | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 84.4          |
-| AMR3-joint-ontowiki-seed44 | amr3joint_ontowiki2_g2g-structured-bart-large-seed44  | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 84.4          |
-| doc-sen-conll-amr-seed42   | both_doc+sen_trainsliding_ws400x100-seed42            |                                                                 | 82.3<sup>1</sup>/71.8 <sup>2</sup>|              |
-
-<sup>1 Smatch on AMR3.0 sentences</sup>
-
-<sup>2 Smatch on AMR3.0 Multi-Sentence dataset </sup>
-
-we also provide the trained `ibm-neural-aligner` under names
-`AMR2.0_ibm_neural_aligner.zip` and `AMR3.0_ibm_neural_aligner.zip`. For the
-ensemble we provide the three seeds. Following fairseq conventions, to run the
-ensemble just give the three checkpoint paths joined by `:` to the normal
-checkpoint argument `-c`. Note that the checkpoints were trained with the
-`v0.5.1` tokenizer, this reduces performance by `0.1` on `v0.5.2` tokenized
-data.
-
-Note that we allways report average of three seeds in papers while these are
-individual models. A fast way to test models standalone is
-
-    bash tests/standalone.sh configs/<config>.sh
+| pretrained model name                       | corresponding file name| paper  |beam10-Smatch  |
+|:----------------------------------------|:-----------:|:-----------:|:-----------:|
+| AMR3-structbart-L-smpl                | amr3.0-structured-bart-large-neur-al-sampling5-seed42.zip      | [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464) PR  | 82.9(beam1)  |
+| AMR3-structbart-L                     | amr3.0-structured-bart-large-neur-al-seed42.zip      | [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464) MAP    |82.6  |
+| AMR2-structbart-L                     | amr2.0-structured-bart-large-neur-al-seed42.zip      |[(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464) MAP    |84.0  |
+| AMR2-joint-ontowiki-seed42            | amr2joint_ontowiki2_g2g-structured-bart-large-seed42.zip       | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 85.9  | 
+| AMR2-joint-ontowiki-seed43            | amr2joint_ontowiki2_g2g-structured-bart-large-seed43.zip      | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 85.9  | 
+| AMR2-joint-ontowiki-seed44            | amr2joint_ontowiki2_g2g-structured-bart-large-seed44.zip      | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 85.9  | 
+| AMR3-joint-ontowiki-seed42            | amr3joint_ontowiki2_g2g-structured-bart-large-seed42.zip      | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 84.4  | 
+| AMR3-joint-ontowiki-seed43            | amr3joint_ontowiki2_g2g-structured-bart-large-seed43.zip      | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 84.4  | 
+| AMR3-joint-ontowiki-seed44            | amr3joint_ontowiki2_g2g-structured-bart-large-seed44.zip      | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 84.4  | 
+| doc-sen-conll-amr-seed42              |both_doc+sen_trainsliding_ws400x100-seed42.zip                |||
 
 
 ## Training a model
 
 You first need to pre-process and align the data. For AMR2.0 do
 
 ```bash
@@ -243,14 +230,63 @@
 ```
 
 use `--results` to check for scores once models are finished.
 
 We include code to launch parallel jobs in the LSF job schedules. This can be
 adapted for other schedulers e.g. Slurm, see [here](run/lsf/README.md)
 
+
 ## Initialize with WatBART
+WatBART is an IBM internal BART architecture model. Our repo supports training AMR parsers with WatBART by simply passing a configuration argument. 
 
-To load WatBART instead of BART just uncomment and provide the path on
+For example, in the AMR2.0 joint-vocabulary training configs/amr2.0-structured-bart-large-joint-voc.sh file, uncomment #L132 to set **initialize_with_watbart** to a checkpoint path on ccc cluster. 
 
-```
-initialize_with_watbart=/path/to/checkpoint_best.pt
-```
+The final training result using WatBART is comparable to the Facebook BART model. 
+
+
+## Upcoming Features
+
+The current release primarily supports model inference using Python scripts. In future versions, we plan to expand the capabilities of this package by:
+
+- Adding python training and evaluation scripts for a more comprehensive user experience. Interested users can refer to the [IBM/transition-amr-parser](https://github.com/IBM/transition-amr-parser) repository for training and evaluation in the meantime.
+- Broadening platform support to include M1 MacOS and higher versions of Python, in addition to the current support for the Linux operating system and Python 3.8.
+
+
+## Research and Evaluation Results
+### Structured-BART 
+
+Current version (`0.5.2`). Structured-BART [(Zhou et al 2021b)](https://aclanthology.org/2021.emnlp-main.507/) encodes the parser state using specialized cross and self-attention heads and leverages BART's language model to replace the use of subgraph actions and lemmatizer, thus enabling a much simpler oracle with 100% coverage. It yields `84.2` Smatch (`84.7` with silver data and `84.9` with ensemble). Version `0.5.2` introduces the ibm-neural-aligner [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464) yielding a base AMR3.0 performance of `82.7` (`83.1` with latent alignment training). Structured-BART is also used for [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) which yields a new single model SoTA of `85.7` for AMR2.0 and `84.1` for AMR3.0 by introducing Smatch-based ensemble distillation.
+
+### Action Pointer
+
+Checkout the `action-pointer` branch (derived from version `0.4.2`) for the `Action Pointer Transformer` model [(Zhou et al 2021)](https://www.aclweb.org/anthology/2021.naacl-main.443) from NAACL2021. As the stack-Transformer, APT encodes the parser state in dedicated attention heads. APT uses however actions creating nodes to represent them. This decouples token and node representations yielding much shorter sequences than previous oracles with higher coverage. APT achieves `81.8` Smatch (`83.4` with silver data and partial ensemble) on AMR2.0 test using RoBERTa embeddings and has an efficient shallow decoder. Due to aligner implementation improvements this code reaches `82.1` on AMR2.0 test, better that what is reported in the paper.
+
+### Stack-Transformer
+
+Checkout the `stack-transformer` branch (derived from version `0.3.4`) for the `stack-Transformer` model [(Fernandez Astudillo et al 2020)](https://www.aclweb.org/anthology/2020.findings-emnlp.89) from EMNLP findings 2020. The stack-Transformer masks dedicated cross attention heads to encode the parser state represented by stack and buffer. It yields `80.2` Smatch (`81.3` with self-learning) on AMR2.0 test (this code reaches `80.5` due to the aligner implementation). Stack-Transformer can be used to reproduce our works on self-learning and cycle consistency in AMR parsing [(Lee et al 2020)](https://www.aclweb.org/anthology/2020.findings-emnlp.288/) from EMNLP findings 2020, alignment-based multi-lingual AMR parsing [(Sheth et al 2021)](https://www.aclweb.org/anthology/2021.eacl-main.30/) from EACL 2021 and Knowledge Base Question Answering [(Kapanipathi et al 2021)](https://arxiv.org/abs/2012.01707) from ACL findings 2021.
+
+The code also contains an implementation of the AMR aligner from [(Naseem et al 2019)](https://www.aclweb.org/anthology/P19-1451/) with the forced-alignment introduced in [(Fernandez Astudillo et al 2020)](https://www.aclweb.org/anthology/2020.findings-emnlp.89).
+
+Aside from listed [contributors](https://github.com/IBM/transition-amr-parser/graphs/contributors), the initial commit was developed by Miguel Ballesteros and Austin Blodgett while at IBM.
+
+
+## IBM Internal Features
+
+IBM-ers please look [here](https://github.ibm.com/mnlp/transition-amr-parser/wiki) for available parsing web-services, CCC installers/trainers, trained models, etc. 
+
+## Evaluating Trained checkpoints
+
+We offer some trained checkpoints on demand, and their evalution score measured in Smatch is below:
+
+|  paper                                                          |  config(.zip)                                         | beam    | Smatch  |
+|:---------------------------------------------------------------:|:------------------------------------------------------:|:-------:|:-------:|
+| [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464) MAP    | amr2.0-structured-bart-large-neur-al-seed42            |   10    |   84.0  |
+| [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464) MAP    | amr3.0-structured-bart-large-neur-al-seed42            |   10    |   82.6  |
+| [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464) PR     | amr3.0-structured-bart-large-neur-al-sampling5-seed42  |   1     |   82.9  |
+| [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | amr2joint_ontowiki2_g2g-structured-bart-large          |   10    |   85.9  |  
+| [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | amr3joint_ontowiki2_g2g-structured-bart-large          |   10    |   84.4  |  
+
+we also provide the trained `ibm-neural-aligner` under names `AMR2.0_ibm_neural_aligner.zip` and `AMR3.0_ibm_neural_aligner.zip`. For the ensemble we provide the three seeds. Following fairseq conventions, to run the ensemble just give the three checkpoint paths joined by `:` to the normal checkpoint argument `-c`. Note that the checkpoints were trained with the `v0.5.1` tokenizer, this reduces performance by `0.1` on `v0.5.2` tokenized data.
+
+Note that we allways report average of three seeds in papers while these are individual models. A fast way to test models standalone is
+
+    bash tests/standalone.sh configs/<config>.sh
```

### Comparing `transition_neural_parser-0.5.3/setup.py` & `transition_neural_parser-0.5.3.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.5.3'
+VERSION = '0.5.3.1'
 
 install_requires = [
     "torch==1.13.1",
     'numpy<=1.23.5',
-    'ipython<=8.12', # python 3.8 vs ipython 8.13 incompatibility
     'tqdm>=4.55.0',
-    'fairseq==0.10.2', # seems to not work on python 3.9 for some platforms
+    'fairseq==0.10.2',
     'packaging>=20.8',
     'requests>=2.25.1',
     # for data (ELMO embeddings)
     'h5py>=3.0.0',
     'python-dateutil>=2.8.1',
     # for scoringy
     'penman>=1.1.0',
     # needs tools to be importable > 1.0.4
     'smatch>=1.0.3.2',
     # for debugging
-    'ipdb',
+    'ipdb>=0.13.0',
     'line_profiler>=4.0.2',
     'pyinstrument>=4.4.0',
     # for aws download
     'boto3>=1.26.1',
     'progressbar',
+    # 'torch-scatter @ https://data.pyg.org/whl/torch-1.13.0%2Bcu117/torch_scatter-2.1.0%2Bpt113cu117-cp38-cp38-linux_x86_64.whl',
 ]
 
 if __name__ == '__main__':
     setup(
         name='transition_amr_parser',
         version=VERSION,
         description="Trasition-based neural parser",
```

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_reform/o10_action_reformer_subtok.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_reform/o10_action_reformer_subtok.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_bartsv.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize_bartsv.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize_graphmp.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize_graphmp_amr1.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize_graphmp_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_graphmp.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_graphmp_amr1.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_graphmp_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/old_action_info.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/old_action_info.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/old_action_info_binarize.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/old_action_info_binarize.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/average_checkpoints.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/average_checkpoints.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/binarize.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/binarize.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/criterions/__init__.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/__init__.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer_alignment.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer_alignment.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_bartsv_dataset.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_bartsv_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_dataset.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_goldamr_dataset.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_goldamr_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_graphmp_dataset.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_graphmp_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_bpe.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_bpe.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/data_utils.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/indexed_dataset.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/language_pair_dataset.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/language_pair_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/binarize_encodings.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/binarize_encodings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/composite_embeddings.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/composite_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/mapavg_embeddings.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/mapavg_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/sentence_encoding.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/sentence_encoding.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/generate.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/generate.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/generate_sliding.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/generate_sliding.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/__init__.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/__init__.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/attention_masks.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/attention_masks.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/graph_attention_masks.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/graph_attention_masks.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/graphmp_attention_masks.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/graphmp_attention_masks.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bart.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bart.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bart_sattn.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bart_sattn.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bartsv.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bartsv_sattn.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bartsv_sattn.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_graph.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_graph.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_graphmp.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/modules/factored_embeddings.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/factored_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/modules/multihead_attention.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/modules/multihead_attention_old.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/multihead_attention_old.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/modules/transformer_layer.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/transformer_layer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/modules/transformer_layer_old.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/transformer_layer_old.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/options.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/options.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/options_train.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/options_train.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/preprocess.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/preprocess_bart.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess_bart.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/preprocess_bartsv.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/preprocess_graphmp.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/roberta/binarize_embeddings.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/binarize_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/roberta/pretrained_embeddings.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/pretrained_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/roberta/pretrained_embeddings_bert.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/pretrained_embeddings_bert.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator_bartsv.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator_graph.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator_graph.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator_graphmp.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/__init__.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_bart.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_bart.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_bart_dyo.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_bart_dyo.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_bartsv.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_graphmp.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_graphmp_amr1.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_graphmp_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/train.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     task = tasks.setup_task(args)
 
     # Load valid dataset (we load training data below, based on the latest checkpoint)
     valid_sub_splits = args.valid_subset.split(",")
     potential_sub_split =  glob(args.data+"/valid_?.*.en")
     if len(potential_sub_split):
         valid_sub_splits = [sub_split.split("/")[-1].split(".")[0] for sub_split in potential_sub_split]
-
+        
     for valid_sub_split in valid_sub_splits:
         task.load_dataset(valid_sub_split, combine=False, epoch=1)
 
     # Build model and criterion
     model = task.build_model(args)
     criterion = task.build_criterion(args)
     logger.info(model)
@@ -246,15 +246,15 @@
                     model.decoder.output_projection.weight.copy_(composite_embed.embedding_weight)
             else:
                 # initialize both the decoder input and output embeddings
                 with torch.no_grad():
                     model.decoder.embed_tokens.weight.copy_(composite_embed.embedding_weight)
                     model.decoder.output_projection.weight.copy_(composite_embed.embedding_weight)
 
-    elif 'apt2_mini' in args.arch:
+    elif 'apt2_mini' in args.arch: 
         if args.initialize_with_bart:
             logger.info('-' * 10 + ' initializing model parameters with pretrained BART model ' + '-' * 10)
 
             new_state_dict = copy.deepcopy(task.bart.model.state_dict())
             if not args.bart_emb_decoder:
                 logger.info('-' * 10 + ' build a separate decoder dictionary embedding ' + '-' * 10)
                 if not args.bart_emb_decoder_input:
```

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/utils.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/utils_font.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/utils_font.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/utils_import.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/utils_import.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/README.md` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/README.md`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/align_leamr.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/align_leamr.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/align_utils.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/align_utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/alignment_decoder.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/alignment_decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         len_a = y_a.shape[-1]
         device = x_t.device
 
         for i_b in range(batch_size):
 
             # variables
 
-            indexa = torch.arange(len_a).to(device)
-            indext = torch.arange(len_t).to(device)
+            indexa = torch.arange(len_a)
+            indext = torch.arange(len_t)
 
             # select
 
             b_x_t = x_t[i_b]
             b_y_a_mask = y_a_mask[i_b].view(-1)
             b_align = align[i_b]
```

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/amr_utils.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/amr_utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/ccc.launch_many_jobs.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/ccc.launch_many_jobs.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/ccc.summarize.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/ccc.summarize.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/dummy_align.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/dummy_align.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/evaluation.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/evaluation.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/formatter.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/formatter.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/gcn.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/gcn.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/lexicon.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/lexicon.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/main.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/main.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/make_splits.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/make_splits.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/metric_utils.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/metric_utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/pretrained_embeddings.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/pretrained_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/resolve_manual_alignments.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/resolve_manual_alignments.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_detailed_eval.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/run_detailed_eval.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_eval.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/run_eval.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_model_selection.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/run_model_selection.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_sampler.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/run_sampler.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/standalone_elmo.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/standalone_elmo.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/tokenize_amr.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/tokenize_amr.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/transformer_lm.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/tree_lstm.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/tree_lstm.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/tree_rnn.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/tree_rnn.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/view_manual_alignments.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/view_manual_alignments.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/vocab.py` & `transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/vocab.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/__init__.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/amr_parser.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/amr_parser.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_data_oracle.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_data_oracle.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_fake_parse.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_fake_parse.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine_amr1.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine_reformer.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine_reformer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine_reformer_amr1.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine_reformer_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/parse.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/parse.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/roberta_utils.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/roberta_utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/add_id_to_amr.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/add_id_to_amr.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/add_sentence_amrs_to_file.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/add_sentence_amrs_to_file.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/amr.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/amr_aligner.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_aligner.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/amr_constituents.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_constituents.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/amr_latex.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_latex.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/amr_machine.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_machine.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/clbar.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/clbar.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/force_overlap_actions.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/force_overlap_actions.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/gold_subgraph_align.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/gold_subgraph_align.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/io.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/io.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/make_sliding_splits.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/make_sliding_splits.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/merge_sliding_splits.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/merge_sliding_splits.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/parse.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,52 +299,52 @@
             checkpoint_file='model.pt'
         )
     roberta.eval()
     if roberta_use_gpu:
         roberta.cuda()
     return roberta
 
-
 def read_doc_text(in_file):
     sents = []
     docs = []
     for line in open(in_file, 'r').readlines():
         if line == '\n':
             docs.append(sents)
             sents = []
         else:
             sents.append(line.strip('\n'))
     if len(sents) > 0:
         docs.append(sents)
 
     return docs
 
-
 def get_force_actions(docs, sen_ends=None):
 
     force_actions_set = []
     return_docs = []
-
+    
+    
     for idx, docsen in enumerate(docs):
 
         offset = 0
         if sen_ends is None:
             ends = []
             doc_toks = []
             for sen in docsen:
-
+                
                 ends.append(offset+len(sen)-1)
                 offset += len(sen)
                 doc_toks.extend(sen)
 
             force_actions = make_eos_force_actions(doc_toks, ends)
         else:
             force_actions = make_eos_force_actions(doc_toks, sen_ends[idx])
         force_actions_set.append(force_actions)
         return_docs.append(doc_toks)
+        
 
     return force_actions_set, return_docs
 
 
 def get_sliding_windows(tok_sentences, window_size, window_overlap,
                         force_actions=None):
     windowed_tok_sentences = []
@@ -884,15 +884,16 @@
             target_tokens = None
 
             sample_predictions = []
             for j, hypo in enumerate(hypos[i][:self.args.nbest]):
                 # args.nbest is default 1, i.e. saving only the top predictions
                 if 'bartsv' in self.model_args.arch:
                     # shared vocabulary BART
-
+                    print(yellow_font(
+                        'WARNING: If force actions have been provided, they will not be used since this model is a joint vocab model and does not support force actions yet . '))
                     actions_nopos, actions_pos, actions = \
                         post_process_action_pointer_prediction_bartsv(
                             hypo, self.tgt_dict
                         )
 
                     # FIXME: hypo['state_machine'].machine.action_history !=
                     # actions
@@ -946,19 +947,14 @@
 
         Args:
             batch (List[List[str]]): list of tokenized sentences.
             batch_size (int, optional): batch size. Defaults to 128.
             roberta_batch_size (int, optional): RoBerta batch size. Defaults to
             10.
         """
-        # check if model is bartsv and force_actions are given
-        if 'bartsv' in self.model_args.arch and force_actions is not None:
-            raise Exception(
-                "The given model is a joint vocabulary model (bartsv) and does not support force actions. Please provide a different model or remove force actions")
-
         # max batch_size
         if len(batch) < batch_size:
             batch_size = len(batch)
         print("Running on batch size: " + str(batch_size))
 
         sentences = []
         # The model expects <ROOT> token at the end of the input sentence
@@ -1014,24 +1010,23 @@
                     for m in machine_nbest
                 )
                 machines.append(machine_nbest)
 
         return annotations, machines
 
     def parse_docs(self, tok_sentences, **kwargs):
-
+        
         init_force_actions, doc_sen = get_force_actions(tok_sentences)
 
+            
         force_actions = [fac+[[]] for fac in init_force_actions]
 
-        annotations, decoding_data = get_sliding_output(
-            tok_sentences=doc_sen, parser=self, force_actions=force_actions, **kwargs)
-
-        return annotations, decoding_data
+        annotations, decoding_data = get_sliding_output(tok_sentences=doc_sen,parser=self,force_actions=force_actions,**kwargs)
 
+        return annotations,decoding_data
 
 def simple_inspector(machine):
     '''
     print the first machine
     '''
     os.system('clear')
     print(machine)
@@ -1262,14 +1257,17 @@
 
                     if args.tokenize:
                         tok_sen.append(protected_tokenizer(newsen.rstrip())[0])
                     else:
                         tok_sen.append(newsen.split())
                 tok_sentences.append(tok_sen)
 
+
+
+
         else:
             if args.tokenize:
                 # TODO: have tokenized as default
                 # jamr-like tokenization
                 with open(args.in_tokenized_sentences) as fid:
                     tok_sentences = [
                         protected_tokenizer(sentence.rstrip())[0]
@@ -1279,21 +1277,23 @@
                 tok_sentences = read_tokenized_sentences(
                     args.in_tokenized_sentences
                 )
 
     # check for empty sentences
     assert all(s != [''] for s in tok_sentences), "Empty sentences!"
 
+    
     # sampling needs copy of sentences N times
     if args.num_samples is not None:
         tok_sentences = [
             tsent
             for tsent in tok_sentences
             for _ in range(args.num_samples)
         ]
+        
 
     return tok_sentences, gold_amrs
 
 
 def save_data(args, annotations, machines):
 
     num_sent = len(machines)
@@ -1355,16 +1355,16 @@
         force_actions = None
 
         # read constrained decoding forced actions if provided
         if args.in_actions:
             with open(args.in_actions) as fact:
                 force_actions = [eval(line.strip()) + [[]] for line in fact]
             assert len(tok_sentences) == len(
-                force_actions), "Number of force actions doesn't match the number of sentences"
-
+            force_actions), "Number of force actions doesn't match the number of sentences"
+        
             # sampling needs copy of force actions N times
             if args.num_samples is not None:
                 force_actions = [
                     a
                     for a in force_actions
                     for _ in range(args.num_samples)
                 ]
@@ -1372,23 +1372,24 @@
         # TODO: max batch sizes could be computed from max sentence length
 
         num_sent = len(tok_sentences)
         print(f'Parsing {num_sent} sentences')
         start = time.time()
 
         if args.in_doc:
-            annotations, machines = parser.parse_docs(tok_sentences,
-                                                      gold_amrs=gold_amrs,
-                                                      window_size=args.window_size,
-                                                      window_overlap=args.window_overlap,
-                                                      batch_size=args.batch_size,
-                                                      roberta_batch_size=args.roberta_batch_size,
-                                                      beam=args.beam,
-                                                      jamr=args.jamr,
-                                                      no_isi=args.no_isi)
+            annotations, machines = parser.parse_docs(tok_sentences, 
+                gold_amrs=gold_amrs,
+                window_size=args.window_size,
+                window_overlap=args.window_overlap,
+                batch_size=args.batch_size,
+                roberta_batch_size=args.roberta_batch_size,
+                beam=args.beam,
+                jamr=args.jamr,
+                no_isi=args.no_isi)
+    
 
         else:
 
             # normal parsing
             annotations, machines = parser.parse_sentences(
                 tok_sentences,
                 batch_size=args.batch_size,
```

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/plots.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/plots.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/SOURCES.txt` & `transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

