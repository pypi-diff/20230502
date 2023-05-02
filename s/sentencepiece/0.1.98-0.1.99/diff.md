# Comparing `tmp/sentencepiece-0.1.98.tar.gz` & `tmp/sentencepiece-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentencepiece-0.1.98.tar", last modified: Wed Apr 12 09:04:54 2023, max compression
+gzip compressed data, was "sentencepiece-0.1.99.tar", last modified: Tue May  2 03:42:19 2023, max compression
```

## Comparing `sentencepiece-0.1.98.tar` & `sentencepiece-0.1.99.tar`

### file list

```diff
@@ -1,240 +1,240 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:54.054038 sentencepiece-0.1.98/
--rw-r--r--   0 runner     (501) staff       (20)      148 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     7684 2023-04-12 09:04:54.054310 sentencepiece-0.1.98/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6965 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/README.md
--rwxr-xr-x   0 runner     (501) staff       (20)      625 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/build_bundled.sh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.824650 sentencepiece-0.1.98/sentencepiece/
--rw-r--r--   0 runner     (501) staff       (20)     5795 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    11358 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)    16899 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/README.md
--rw-r--r--   0 runner     (501) staff       (20)        7 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/VERSION.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.825949 sentencepiece-0.1.98/sentencepiece/cmake/
--rw-r--r--   0 runner     (501) staff       (20)    46672 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/cmake/ios.toolchain.cmake
--rw-r--r--   0 runner     (501) staff       (20)      169 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/config.h.in
--rw-r--r--   0 runner     (501) staff       (20)      387 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/sentencepiece.pc.in
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.930409 sentencepiece-0.1.98/sentencepiece/src/
--rw-r--r--   0 runner     (501) staff       (20)    13029 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     6596 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/bpe_model.cc
--rw-r--r--   0 runner     (501) staff       (20)     1748 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/bpe_model.h
--rw-r--r--   0 runner     (501) staff       (20)     9294 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/bpe_model_test.cc
--rw-r--r--   0 runner     (501) staff       (20)    11226 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/bpe_model_trainer.cc
--rw-r--r--   0 runner     (501) staff       (20)     4521 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/bpe_model_trainer.h
--rw-r--r--   0 runner     (501) staff       (20)     4850 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/bpe_model_trainer_test.cc
--rw-r--r--   0 runner     (501) staff       (20)    18686 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/builder.cc
--rw-r--r--   0 runner     (501) staff       (20)     5203 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/builder.h
--rw-r--r--   0 runner     (501) staff       (20)     7354 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/builder_test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.935438 sentencepiece-0.1.98/sentencepiece/src/builtin_pb/
--rw-r--r--   0 runner     (501) staff       (20)    35154 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
--rw-r--r--   0 runner     (501) staff       (20)    40648 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/builtin_pb/sentencepiece.pb.h
--rw-r--r--   0 runner     (501) staff       (20)   136631 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
--rw-r--r--   0 runner     (501) staff       (20)   200094 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
--rw-r--r--   0 runner     (501) staff       (20)     1304 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/char_model.cc
--rw-r--r--   0 runner     (501) staff       (20)     1061 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/char_model.h
--rw-r--r--   0 runner     (501) staff       (20)     3525 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/char_model_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1782 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/char_model_trainer.cc
--rw-r--r--   0 runner     (501) staff       (20)     1265 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/char_model_trainer.h
--rw-r--r--   0 runner     (501) staff       (20)     2506 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/char_model_trainer_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     5168 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/common.h
--rw-r--r--   0 runner     (501) staff       (20)     5936 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/compile_charsmap_main.cc
--rw-r--r--   0 runner     (501) staff       (20)     4103 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/error.cc
--rw-r--r--   0 runner     (501) staff       (20)     3563 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/filesystem.cc
--rw-r--r--   0 runner     (501) staff       (20)     1852 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/filesystem.h
--rw-r--r--   0 runner     (501) staff       (20)     1577 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/filesystem_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     2605 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/freelist.h
--rw-r--r--   0 runner     (501) staff       (20)     1280 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/freelist_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1770 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/init.h
--rw-r--r--   0 runner     (501) staff       (20)     5359 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/init_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1644 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/model_factory.cc
--rw-r--r--   0 runner     (501) staff       (20)      972 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/model_factory.h
--rw-r--r--   0 runner     (501) staff       (20)     1743 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/model_factory_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     6609 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/model_interface.cc
--rw-r--r--   0 runner     (501) staff       (20)     8751 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/model_interface.h
--rw-r--r--   0 runner     (501) staff       (20)    15351 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/model_interface_test.cc
--rw-r--r--   0 runner     (501) staff       (20)  7198605 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/normalization_rule.h
--rw-r--r--   0 runner     (501) staff       (20)    11583 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/normalizer.cc
--rw-r--r--   0 runner     (501) staff       (20)     5817 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/normalizer.h
--rw-r--r--   0 runner     (501) staff       (20)    16156 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/normalizer_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     2132 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/pretokenizer_for_training.cc
--rw-r--r--   0 runner     (501) staff       (20)     2152 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/pretokenizer_for_training.h
--rw-r--r--   0 runner     (501) staff       (20)     2892 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/pretokenizer_for_training_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     2523 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/sentencepiece.proto
--rw-r--r--   0 runner     (501) staff       (20)    13845 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/sentencepiece_model.proto
--rw-r--r--   0 runner     (501) staff       (20)    37639 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/sentencepiece_processor.cc
--rw-r--r--   0 runner     (501) staff       (20)    27254 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/sentencepiece_processor.h
--rw-r--r--   0 runner     (501) staff       (20)    54189 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/sentencepiece_processor_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     9966 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/sentencepiece_trainer.cc
--rw-r--r--   0 runner     (501) staff       (20)     6523 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/sentencepiece_trainer.h
--rw-r--r--   0 runner     (501) staff       (20)    13402 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/sentencepiece_trainer_test.cc
--rw-r--r--   0 runner     (501) staff       (20)    10925 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/spec_parser.h
--rw-r--r--   0 runner     (501) staff       (20)     4037 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/spm_decode_main.cc
--rw-r--r--   0 runner     (501) staff       (20)     6597 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/spm_encode_main.cc
--rw-r--r--   0 runner     (501) staff       (20)     2083 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/spm_export_vocab_main.cc
--rw-r--r--   0 runner     (501) staff       (20)     4214 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/spm_normalize_main.cc
--rw-r--r--   0 runner     (501) staff       (20)    13036 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/spm_train_main.cc
--rw-r--r--   0 runner     (501) staff       (20)     1077 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/test_main.cc
--rw-r--r--   0 runner     (501) staff       (20)     1899 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/testharness.cc
--rw-r--r--   0 runner     (501) staff       (20)     8718 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/testharness.h
--rw-r--r--   0 runner     (501) staff       (20)     2103 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/trainer_factory.cc
--rw-r--r--   0 runner     (501) staff       (20)     1104 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/trainer_factory.h
--rw-r--r--   0 runner     (501) staff       (20)     1656 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/trainer_factory_test.cc
--rw-r--r--   0 runner     (501) staff       (20)    28978 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/trainer_interface.cc
--rw-r--r--   0 runner     (501) staff       (20)     5727 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/trainer_interface.h
--rw-r--r--   0 runner     (501) staff       (20)    20727 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/trainer_interface_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1239 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/unicode_script.cc
--rw-r--r--   0 runner     (501) staff       (20)     2817 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/unicode_script.h
--rw-r--r--   0 runner     (501) staff       (20)   106446 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/unicode_script_map.h
--rw-r--r--   0 runner     (501) staff       (20)     1525 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/unicode_script_test.cc
--rw-r--r--   0 runner     (501) staff       (20)    34126 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/unigram_model.cc
--rw-r--r--   0 runner     (501) staff       (20)     7324 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/unigram_model.h
--rw-r--r--   0 runner     (501) staff       (20)    32283 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/unigram_model_test.cc
--rw-r--r--   0 runner     (501) staff       (20)    22266 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/unigram_model_trainer.cc
--rw-r--r--   0 runner     (501) staff       (20)     4053 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/unigram_model_trainer.h
--rw-r--r--   0 runner     (501) staff       (20)     6752 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/unigram_model_trainer_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     7393 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/util.cc
--rw-r--r--   0 runner     (501) staff       (20)    10907 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/util.h
--rw-r--r--   0 runner     (501) staff       (20)    12866 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/util_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1124 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/word_model.cc
--rw-r--r--   0 runner     (501) staff       (20)     1045 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/word_model.h
--rw-r--r--   0 runner     (501) staff       (20)     2639 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/src/word_model_test.cc
--rw-r--r--   0 runner     (501) staff       (20)     2101 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/word_model_trainer.cc
--rw-r--r--   0 runner     (501) staff       (20)     1372 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/word_model_trainer.h
--rw-r--r--   0 runner     (501) staff       (20)     2464 2023-04-12 09:04:52.000000 sentencepiece-0.1.98/sentencepiece/src/word_model_trainer_test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.937204 sentencepiece-0.1.98/sentencepiece/third_party/
--rw-r--r--   0 runner     (501) staff       (20)       69 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.937752 sentencepiece-0.1.98/sentencepiece/third_party/absl/
--rw-r--r--   0 runner     (501) staff       (20)    11365 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.939224 sentencepiece-0.1.98/sentencepiece/third_party/absl/container/
--rw-r--r--   0 runner     (501) staff       (20)     1001 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/container/flat_hash_map.h
--rw-r--r--   0 runner     (501) staff       (20)      966 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/container/flat_hash_set.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.940927 sentencepiece-0.1.98/sentencepiece/third_party/absl/flags/
--rw-r--r--   0 runner     (501) staff       (20)     5857 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/flags/flag.cc
--rw-r--r--   0 runner     (501) staff       (20)     1745 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/flags/flag.h
--rw-r--r--   0 runner     (501) staff       (20)      799 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/flags/parse.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.941772 sentencepiece-0.1.98/sentencepiece/third_party/absl/memory/
--rw-r--r--   0 runner     (501) staff       (20)     2592 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/memory/memory.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.943054 sentencepiece-0.1.98/sentencepiece/third_party/absl/random/
--rw-r--r--   0 runner     (501) staff       (20)      959 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/random/distributions.h
--rw-r--r--   0 runner     (501) staff       (20)      926 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/random/random.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.948962 sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/
--rw-r--r--   0 runner     (501) staff       (20)     1309 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/ascii.h
--rw-r--r--   0 runner     (501) staff       (20)     1308 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/match.h
--rw-r--r--   0 runner     (501) staff       (20)     1012 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/numbers.h
--rw-r--r--   0 runner     (501) staff       (20)     1447 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/str_cat.h
--rw-r--r--   0 runner     (501) staff       (20)     1088 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/str_format.h
--rw-r--r--   0 runner     (501) staff       (20)     2413 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/str_join.h
--rw-r--r--   0 runner     (501) staff       (20)     2127 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/str_replace.h
--rw-r--r--   0 runner     (501) staff       (20)     2669 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/str_split.h
--rw-r--r--   0 runner     (501) staff       (20)     2106 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/string_view.h
--rw-r--r--   0 runner     (501) staff       (20)      991 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/strip.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.950085 sentencepiece-0.1.98/sentencepiece/third_party/darts_clone/
--rw-r--r--   0 runner     (501) staff       (20)     1481 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/darts_clone/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)    51750 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/darts_clone/darts.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.952403 sentencepiece-0.1.98/sentencepiece/third_party/esaxx/
--rw-r--r--   0 runner     (501) staff       (20)     1112 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/esaxx/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     4224 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/esaxx/esa.hxx
--rw-r--r--   0 runner     (501) staff       (20)    12385 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/esaxx/sais.hxx
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.971628 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/
--rw-r--r--   0 runner     (501) staff       (20)     1732 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)    15726 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/arena.cc
--rw-r--r--   0 runner     (501) staff       (20)     8985 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/arenastring.cc
--rw-r--r--   0 runner     (501) staff       (20)     5975 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/bytestream.cc
--rw-r--r--   0 runner     (501) staff       (20)    30847 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/coded_stream.cc
--rw-r--r--   0 runner     (501) staff       (20)    10999 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/common.cc
--rw-r--r--   0 runner     (501) staff       (20)    82338 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/extension_set.cc
--rw-r--r--   0 runner     (501) staff       (20)     3573 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
--rw-r--r--   0 runner     (501) staff       (20)     4441 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
--rw-r--r--   0 runner     (501) staff       (20)    30000 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.814825 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.995036 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/
--rw-r--r--   0 runner     (501) staff       (20)     6215 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
--rw-r--r--   0 runner     (501) staff       (20)    29756 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
--rw-r--r--   0 runner     (501) staff       (20)    18092 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
--rw-r--r--   0 runner     (501) staff       (20)    15918 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
--rw-r--r--   0 runner     (501) staff       (20)    96637 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
--rw-r--r--   0 runner     (501) staff       (20)    78585 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
--rw-r--r--   0 runner     (501) staff       (20)    12437 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
--rw-r--r--   0 runner     (501) staff       (20)     3993 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
--rw-r--r--   0 runner     (501) staff       (20)     3266 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
--rw-r--r--   0 runner     (501) staff       (20)    12532 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
--rw-r--r--   0 runner     (501) staff       (20)    31313 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
--rw-r--r--   0 runner     (501) staff       (20)    10023 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
--rw-r--r--   0 runner     (501) staff       (20)     3542 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
--rw-r--r--   0 runner     (501) staff       (20)     7024 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:54.000175 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
--rw-r--r--   0 runner     (501) staff       (20)    69376 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
--rw-r--r--   0 runner     (501) staff       (20)     5384 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
--rw-r--r--   0 runner     (501) staff       (20)    10258 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
--rw-r--r--   0 runner     (501) staff       (20)    12750 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
--rw-r--r--   0 runner     (501) staff       (20)    16950 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
--rw-r--r--   0 runner     (501) staff       (20)    48107 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
--rw-r--r--   0 runner     (501) staff       (20)    24921 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
--rw-r--r--   0 runner     (501) staff       (20)     7104 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
--rw-r--r--   0 runner     (501) staff       (20)    31973 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
--rw-r--r--   0 runner     (501) staff       (20)    27172 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
--rw-r--r--   0 runner     (501) staff       (20)     8270 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
--rw-r--r--   0 runner     (501) staff       (20)    32754 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
--rw-r--r--   0 runner     (501) staff       (20)     2050 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
--rw-r--r--   0 runner     (501) staff       (20)    20834 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
--rw-r--r--   0 runner     (501) staff       (20)     4209 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
--rw-r--r--   0 runner     (501) staff       (20)   101600 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:54.015279 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
--rw-r--r--   0 runner     (501) staff       (20)    11769 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
--rw-r--r--   0 runner     (501) staff       (20)    17098 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
--rw-r--r--   0 runner     (501) staff       (20)     5733 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
--rw-r--r--   0 runner     (501) staff       (20)     7283 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
--rw-r--r--   0 runner     (501) staff       (20)     3911 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
--rw-r--r--   0 runner     (501) staff       (20)    11971 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
--rw-r--r--   0 runner     (501) staff       (20)     8915 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
--rw-r--r--   0 runner     (501) staff       (20)     4903 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
--rw-r--r--   0 runner     (501) staff       (20)    31213 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
--rw-r--r--   0 runner     (501) staff       (20)     6157 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
--rw-r--r--   0 runner     (501) staff       (20)     2184 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
--rw-r--r--   0 runner     (501) staff       (20)     5108 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
--rw-r--r--   0 runner     (501) staff       (20)    12765 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
--rw-r--r--   0 runner     (501) staff       (20)     3949 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
--rw-r--r--   0 runner     (501) staff       (20)     8558 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
--rw-r--r--   0 runner     (501) staff       (20)     3293 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
--rw-r--r--   0 runner     (501) staff       (20)    17861 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
--rw-r--r--   0 runner     (501) staff       (20)     3615 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
--rw-r--r--   0 runner     (501) staff       (20)    39629 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
--rw-r--r--   0 runner     (501) staff       (20)     3356 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
--rw-r--r--   0 runner     (501) staff       (20)    14401 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
--rw-r--r--   0 runner     (501) staff       (20)    83648 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
--rw-r--r--   0 runner     (501) staff       (20)     2756 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
--rw-r--r--   0 runner     (501) staff       (20)     6587 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/int128.cc
--rw-r--r--   0 runner     (501) staff       (20)    13526 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/io_win32.cc
--rw-r--r--   0 runner     (501) staff       (20)    20751 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/message_lite.cc
--rw-r--r--   0 runner     (501) staff       (20)    20703 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/parse_context.cc
--rw-r--r--   0 runner     (501) staff       (20)     5500 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/repeated_field.cc
--rw-r--r--   0 runner     (501) staff       (20)     4197 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/status.cc
--rw-r--r--   0 runner     (501) staff       (20)     2096 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/statusor.cc
--rw-r--r--   0 runner     (501) staff       (20)     9193 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/stringpiece.cc
--rw-r--r--   0 runner     (501) staff       (20)     6283 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/stringprintf.cc
--rw-r--r--   0 runner     (501) staff       (20)    26415 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
--rw-r--r--   0 runner     (501) staff       (20)    88575 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/strutil.cc
--rw-r--r--   0 runner     (501) staff       (20)    10168 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/time.cc
--rw-r--r--   0 runner     (501) staff       (20)    27892 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
--rw-r--r--   0 runner     (501) staff       (20)     2392 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
--rw-r--r--   0 runner     (501) staff       (20)    11345 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
--rw-r--r--   0 runner     (501) staff       (20)    13255 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
--rw-r--r--   0 runner     (501) staff       (20)       79 2023-04-12 09:04:54.056766 sentencepiece-0.1.98/setup.cfg
--rwxr-xr-x   0 runner     (501) staff       (20)     6173 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:53.816236 sentencepiece-0.1.98/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:54.021653 sentencepiece-0.1.98/src/sentencepiece/
--rw-r--r--   0 runner     (501) staff       (20)    43910 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/src/sentencepiece/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       23 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/src/sentencepiece/_version.py
--rw-r--r--   0 runner     (501) staff       (20)    65033 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/src/sentencepiece/sentencepiece.i
--rw-r--r--   0 runner     (501) staff       (20)    40692 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/src/sentencepiece/sentencepiece_model_pb2.py
--rw-r--r--   0 runner     (501) staff       (20)     8128 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/src/sentencepiece/sentencepiece_pb2.py
--rw-r--r--   0 runner     (501) staff       (20)   334356 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/src/sentencepiece/sentencepiece_wrap.cxx
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:54.029268 sentencepiece-0.1.98/src/sentencepiece.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     7684 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/src/sentencepiece.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    10504 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/src/sentencepiece.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/src/sentencepiece.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      130 2023-04-12 09:04:53.000000 sentencepiece-0.1.98/src/sentencepiece.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 09:04:54.049376 sentencepiece-0.1.98/test/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/test/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)   278779 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/test/botchan.txt
--rwxr-xr-x   0 runner     (501) staff       (20)    26434 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/test/sentencepiece_test.py
--rw-r--r--   0 runner     (501) staff       (20)   352301 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/test/test_ja_model.model
--rw-r--r--   0 runner     (501) staff       (20)   253165 2023-04-12 08:48:03.000000 sentencepiece-0.1.98/test/test_model.model
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.601746 sentencepiece-0.1.99/
+-rw-r--r--   0 runner     (501) staff       (20)      148 2023-05-02 03:22:17.000000 sentencepiece-0.1.99/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     7684 2023-05-02 03:42:19.601973 sentencepiece-0.1.99/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     6965 2023-05-02 03:22:17.000000 sentencepiece-0.1.99/README.md
+-rwxr-xr-x   0 runner     (501) staff       (20)      625 2023-05-02 03:22:18.000000 sentencepiece-0.1.99/build_bundled.sh
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.268261 sentencepiece-0.1.99/sentencepiece/
+-rw-r--r--   0 runner     (501) staff       (20)     5795 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    11358 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    16899 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/README.md
+-rw-r--r--   0 runner     (501) staff       (20)        7 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/VERSION.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.268835 sentencepiece-0.1.99/sentencepiece/cmake/
+-rw-r--r--   0 runner     (501) staff       (20)    46672 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/cmake/ios.toolchain.cmake
+-rw-r--r--   0 runner     (501) staff       (20)      169 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/config.h.in
+-rw-r--r--   0 runner     (501) staff       (20)      387 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/sentencepiece.pc.in
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.511757 sentencepiece-0.1.99/sentencepiece/src/
+-rw-r--r--   0 runner     (501) staff       (20)    13029 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     6596 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/bpe_model.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1748 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/bpe_model.h
+-rw-r--r--   0 runner     (501) staff       (20)     9294 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/bpe_model_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    10624 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/bpe_model_trainer.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4521 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/bpe_model_trainer.h
+-rw-r--r--   0 runner     (501) staff       (20)     4850 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/bpe_model_trainer_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    18686 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/builder.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5203 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/builder.h
+-rw-r--r--   0 runner     (501) staff       (20)     7354 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/builder_test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.516491 sentencepiece-0.1.99/sentencepiece/src/builtin_pb/
+-rw-r--r--   0 runner     (501) staff       (20)    35154 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
+-rw-r--r--   0 runner     (501) staff       (20)    40648 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/builtin_pb/sentencepiece.pb.h
+-rw-r--r--   0 runner     (501) staff       (20)   136631 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
+-rw-r--r--   0 runner     (501) staff       (20)   200094 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
+-rw-r--r--   0 runner     (501) staff       (20)     1304 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/char_model.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1061 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/char_model.h
+-rw-r--r--   0 runner     (501) staff       (20)     3525 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/char_model_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1782 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/char_model_trainer.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1265 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/char_model_trainer.h
+-rw-r--r--   0 runner     (501) staff       (20)     2506 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/char_model_trainer_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5168 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     5936 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/compile_charsmap_main.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4103 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/error.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3563 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/filesystem.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1852 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/filesystem.h
+-rw-r--r--   0 runner     (501) staff       (20)     1577 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/filesystem_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2605 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/freelist.h
+-rw-r--r--   0 runner     (501) staff       (20)     1280 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/freelist_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1770 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/init.h
+-rw-r--r--   0 runner     (501) staff       (20)     5359 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/init_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1644 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/model_factory.cc
+-rw-r--r--   0 runner     (501) staff       (20)      972 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/model_factory.h
+-rw-r--r--   0 runner     (501) staff       (20)     1743 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/model_factory_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6609 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/model_interface.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8751 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/model_interface.h
+-rw-r--r--   0 runner     (501) staff       (20)    15351 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/model_interface_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)  7198605 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/normalization_rule.h
+-rw-r--r--   0 runner     (501) staff       (20)    11583 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/normalizer.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5817 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/normalizer.h
+-rw-r--r--   0 runner     (501) staff       (20)    16156 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/normalizer_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2132 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/pretokenizer_for_training.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2152 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/pretokenizer_for_training.h
+-rw-r--r--   0 runner     (501) staff       (20)     2892 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/pretokenizer_for_training_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2523 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/sentencepiece.proto
+-rw-r--r--   0 runner     (501) staff       (20)    13845 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/sentencepiece_model.proto
+-rw-r--r--   0 runner     (501) staff       (20)    37639 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/sentencepiece_processor.cc
+-rw-r--r--   0 runner     (501) staff       (20)    27254 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/sentencepiece_processor.h
+-rw-r--r--   0 runner     (501) staff       (20)    54189 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/sentencepiece_processor_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     9966 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/sentencepiece_trainer.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6523 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/sentencepiece_trainer.h
+-rw-r--r--   0 runner     (501) staff       (20)    13402 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/sentencepiece_trainer_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    10925 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/spec_parser.h
+-rw-r--r--   0 runner     (501) staff       (20)     4037 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/spm_decode_main.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6597 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/spm_encode_main.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2083 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/spm_export_vocab_main.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4214 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/spm_normalize_main.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13036 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/spm_train_main.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1077 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/test_main.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1899 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/testharness.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8718 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/testharness.h
+-rw-r--r--   0 runner     (501) staff       (20)     2103 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/trainer_factory.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1104 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/trainer_factory.h
+-rw-r--r--   0 runner     (501) staff       (20)     1656 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/trainer_factory_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    28979 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/trainer_interface.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5727 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/trainer_interface.h
+-rw-r--r--   0 runner     (501) staff       (20)    20727 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/trainer_interface_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1239 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/unicode_script.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2817 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/unicode_script.h
+-rw-r--r--   0 runner     (501) staff       (20)   106446 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/unicode_script_map.h
+-rw-r--r--   0 runner     (501) staff       (20)     1525 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/unicode_script_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    34126 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/unigram_model.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7324 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/unigram_model.h
+-rw-r--r--   0 runner     (501) staff       (20)    32283 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/unigram_model_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    20993 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/unigram_model_trainer.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3939 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/unigram_model_trainer.h
+-rw-r--r--   0 runner     (501) staff       (20)     6862 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/unigram_model_trainer_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7393 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/util.cc
+-rw-r--r--   0 runner     (501) staff       (20)    10907 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/util.h
+-rw-r--r--   0 runner     (501) staff       (20)    12866 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/util_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1124 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/word_model.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1045 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/word_model.h
+-rw-r--r--   0 runner     (501) staff       (20)     2639 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/word_model_test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2101 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/word_model_trainer.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1372 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/word_model_trainer.h
+-rw-r--r--   0 runner     (501) staff       (20)     2464 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/src/word_model_trainer_test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.517652 sentencepiece-0.1.99/sentencepiece/third_party/
+-rw-r--r--   0 runner     (501) staff       (20)       69 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.518216 sentencepiece-0.1.99/sentencepiece/third_party/absl/
+-rw-r--r--   0 runner     (501) staff       (20)    11365 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.520072 sentencepiece-0.1.99/sentencepiece/third_party/absl/container/
+-rw-r--r--   0 runner     (501) staff       (20)     1001 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/container/flat_hash_map.h
+-rw-r--r--   0 runner     (501) staff       (20)      966 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/container/flat_hash_set.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.521814 sentencepiece-0.1.99/sentencepiece/third_party/absl/flags/
+-rw-r--r--   0 runner     (501) staff       (20)     5857 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/flags/flag.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1745 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/flags/flag.h
+-rw-r--r--   0 runner     (501) staff       (20)      799 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/flags/parse.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.522511 sentencepiece-0.1.99/sentencepiece/third_party/absl/memory/
+-rw-r--r--   0 runner     (501) staff       (20)     2592 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/memory/memory.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.523669 sentencepiece-0.1.99/sentencepiece/third_party/absl/random/
+-rw-r--r--   0 runner     (501) staff       (20)      959 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/random/distributions.h
+-rw-r--r--   0 runner     (501) staff       (20)      926 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/random/random.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.529532 sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/
+-rw-r--r--   0 runner     (501) staff       (20)     1309 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/ascii.h
+-rw-r--r--   0 runner     (501) staff       (20)     1308 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/match.h
+-rw-r--r--   0 runner     (501) staff       (20)     1012 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/numbers.h
+-rw-r--r--   0 runner     (501) staff       (20)     1447 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/str_cat.h
+-rw-r--r--   0 runner     (501) staff       (20)     1088 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/str_format.h
+-rw-r--r--   0 runner     (501) staff       (20)     2413 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/str_join.h
+-rw-r--r--   0 runner     (501) staff       (20)     2127 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/str_replace.h
+-rw-r--r--   0 runner     (501) staff       (20)     2669 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/str_split.h
+-rw-r--r--   0 runner     (501) staff       (20)     2106 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/string_view.h
+-rw-r--r--   0 runner     (501) staff       (20)      991 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/strip.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.531063 sentencepiece-0.1.99/sentencepiece/third_party/darts_clone/
+-rw-r--r--   0 runner     (501) staff       (20)     1481 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/darts_clone/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    51750 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/darts_clone/darts.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.533323 sentencepiece-0.1.99/sentencepiece/third_party/esaxx/
+-rw-r--r--   0 runner     (501) staff       (20)     1112 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/esaxx/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     4224 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/esaxx/esa.hxx
+-rw-r--r--   0 runner     (501) staff       (20)    12385 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/esaxx/sais.hxx
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.550459 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/
+-rw-r--r--   0 runner     (501) staff       (20)     1732 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    15726 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/arena.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8985 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/arenastring.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5975 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/bytestream.cc
+-rw-r--r--   0 runner     (501) staff       (20)    30847 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/coded_stream.cc
+-rw-r--r--   0 runner     (501) staff       (20)    10999 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/common.cc
+-rw-r--r--   0 runner     (501) staff       (20)    82338 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/extension_set.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3573 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4441 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
+-rw-r--r--   0 runner     (501) staff       (20)    30000 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.259810 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.568707 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/
+-rw-r--r--   0 runner     (501) staff       (20)     6215 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
+-rw-r--r--   0 runner     (501) staff       (20)    29756 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
+-rw-r--r--   0 runner     (501) staff       (20)    18092 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)    15918 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
+-rw-r--r--   0 runner     (501) staff       (20)    96637 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
+-rw-r--r--   0 runner     (501) staff       (20)    78585 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
+-rw-r--r--   0 runner     (501) staff       (20)    12437 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
+-rw-r--r--   0 runner     (501) staff       (20)     3993 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
+-rw-r--r--   0 runner     (501) staff       (20)     3266 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
+-rw-r--r--   0 runner     (501) staff       (20)    12532 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
+-rw-r--r--   0 runner     (501) staff       (20)    31313 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
+-rw-r--r--   0 runner     (501) staff       (20)    10023 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
+-rw-r--r--   0 runner     (501) staff       (20)     3542 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
+-rw-r--r--   0 runner     (501) staff       (20)     7024 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.572461 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
+-rw-r--r--   0 runner     (501) staff       (20)    69376 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
+-rw-r--r--   0 runner     (501) staff       (20)     5384 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
+-rw-r--r--   0 runner     (501) staff       (20)    10258 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
+-rw-r--r--   0 runner     (501) staff       (20)    12750 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)    16950 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
+-rw-r--r--   0 runner     (501) staff       (20)    48107 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
+-rw-r--r--   0 runner     (501) staff       (20)    24921 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
+-rw-r--r--   0 runner     (501) staff       (20)     7104 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
+-rw-r--r--   0 runner     (501) staff       (20)    31973 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
+-rw-r--r--   0 runner     (501) staff       (20)    27172 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
+-rw-r--r--   0 runner     (501) staff       (20)     8270 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
+-rw-r--r--   0 runner     (501) staff       (20)    32754 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
+-rw-r--r--   0 runner     (501) staff       (20)     2050 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
+-rw-r--r--   0 runner     (501) staff       (20)    20834 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
+-rw-r--r--   0 runner     (501) staff       (20)     4209 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
+-rw-r--r--   0 runner     (501) staff       (20)   101600 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.585795 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
+-rw-r--r--   0 runner     (501) staff       (20)    11769 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
+-rw-r--r--   0 runner     (501) staff       (20)    17098 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
+-rw-r--r--   0 runner     (501) staff       (20)     5733 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
+-rw-r--r--   0 runner     (501) staff       (20)     7283 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     3911 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
+-rw-r--r--   0 runner     (501) staff       (20)    11971 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
+-rw-r--r--   0 runner     (501) staff       (20)     8915 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
+-rw-r--r--   0 runner     (501) staff       (20)     4903 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
+-rw-r--r--   0 runner     (501) staff       (20)    31213 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
+-rw-r--r--   0 runner     (501) staff       (20)     6157 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
+-rw-r--r--   0 runner     (501) staff       (20)     2184 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
+-rw-r--r--   0 runner     (501) staff       (20)     5108 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
+-rw-r--r--   0 runner     (501) staff       (20)    12765 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
+-rw-r--r--   0 runner     (501) staff       (20)     3949 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
+-rw-r--r--   0 runner     (501) staff       (20)     8558 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
+-rw-r--r--   0 runner     (501) staff       (20)     3293 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
+-rw-r--r--   0 runner     (501) staff       (20)    17861 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
+-rw-r--r--   0 runner     (501) staff       (20)     3615 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
+-rw-r--r--   0 runner     (501) staff       (20)    39629 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
+-rw-r--r--   0 runner     (501) staff       (20)     3356 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
+-rw-r--r--   0 runner     (501) staff       (20)    14401 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
+-rw-r--r--   0 runner     (501) staff       (20)    83648 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
+-rw-r--r--   0 runner     (501) staff       (20)     2756 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6587 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/int128.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13526 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/io_win32.cc
+-rw-r--r--   0 runner     (501) staff       (20)    20751 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/message_lite.cc
+-rw-r--r--   0 runner     (501) staff       (20)    20703 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/parse_context.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5500 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/repeated_field.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4197 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/status.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2096 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/statusor.cc
+-rw-r--r--   0 runner     (501) staff       (20)     9193 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/stringpiece.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6283 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/stringprintf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    26415 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
+-rw-r--r--   0 runner     (501) staff       (20)    88575 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/strutil.cc
+-rw-r--r--   0 runner     (501) staff       (20)    10168 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/time.cc
+-rw-r--r--   0 runner     (501) staff       (20)    27892 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2392 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
+-rw-r--r--   0 runner     (501) staff       (20)    11345 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13255 2023-05-02 03:42:18.000000 sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
+-rw-r--r--   0 runner     (501) staff       (20)       79 2023-05-02 03:42:19.602911 sentencepiece-0.1.99/setup.cfg
+-rwxr-xr-x   0 runner     (501) staff       (20)     6173 2023-05-02 03:22:18.000000 sentencepiece-0.1.99/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.261219 sentencepiece-0.1.99/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.591676 sentencepiece-0.1.99/src/sentencepiece/
+-rw-r--r--   0 runner     (501) staff       (20)    43910 2023-05-02 03:22:18.000000 sentencepiece-0.1.99/src/sentencepiece/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       23 2023-05-02 03:22:18.000000 sentencepiece-0.1.99/src/sentencepiece/_version.py
+-rw-r--r--   0 runner     (501) staff       (20)    65033 2023-05-02 03:22:18.000000 sentencepiece-0.1.99/src/sentencepiece/sentencepiece.i
+-rw-r--r--   0 runner     (501) staff       (20)    40692 2023-05-02 03:22:18.000000 sentencepiece-0.1.99/src/sentencepiece/sentencepiece_model_pb2.py
+-rw-r--r--   0 runner     (501) staff       (20)     8128 2023-05-02 03:22:18.000000 sentencepiece-0.1.99/src/sentencepiece/sentencepiece_pb2.py
+-rw-r--r--   0 runner     (501) staff       (20)   334356 2023-05-02 03:22:18.000000 sentencepiece-0.1.99/src/sentencepiece/sentencepiece_wrap.cxx
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.595220 sentencepiece-0.1.99/src/sentencepiece.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     7684 2023-05-02 03:42:19.000000 sentencepiece-0.1.99/src/sentencepiece.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    10504 2023-05-02 03:42:19.000000 sentencepiece-0.1.99/src/sentencepiece.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-05-02 03:42:19.000000 sentencepiece-0.1.99/src/sentencepiece.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      130 2023-05-02 03:42:19.000000 sentencepiece-0.1.99/src/sentencepiece.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 03:42:19.600407 sentencepiece-0.1.99/test/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-02 03:22:18.000000 sentencepiece-0.1.99/test/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)   278779 2023-05-02 03:22:15.000000 sentencepiece-0.1.99/test/botchan.txt
+-rwxr-xr-x   0 runner     (501) staff       (20)    26434 2023-05-02 03:22:18.000000 sentencepiece-0.1.99/test/sentencepiece_test.py
+-rw-r--r--   0 runner     (501) staff       (20)   352301 2023-05-02 03:22:18.000000 sentencepiece-0.1.99/test/test_ja_model.model
+-rw-r--r--   0 runner     (501) staff       (20)   253165 2023-05-02 03:22:19.000000 sentencepiece-0.1.99/test/test_model.model
```

### Comparing `sentencepiece-0.1.98/PKG-INFO` & `sentencepiece-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentencepiece
-Version: 0.1.98
+Version: 0.1.99
 Summary: SentencePiece python wrapper
 Home-page: https://github.com/google/sentencepiece
 Author: Taku Kudo
 Author-email: taku@google.com
 License: Apache
 Platform: Unix
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sentencepiece-0.1.98/README.md` & `sentencepiece-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/build_bundled.sh` & `sentencepiece-0.1.99/build_bundled.sh`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/CMakeLists.txt` & `sentencepiece-0.1.99/sentencepiece/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/LICENSE` & `sentencepiece-0.1.99/sentencepiece/LICENSE`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/README.md` & `sentencepiece-0.1.99/sentencepiece/README.md`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/cmake/ios.toolchain.cmake` & `sentencepiece-0.1.99/sentencepiece/cmake/ios.toolchain.cmake`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/CMakeLists.txt` & `sentencepiece-0.1.99/sentencepiece/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/bpe_model.cc` & `sentencepiece-0.1.99/sentencepiece/src/bpe_model.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/bpe_model.h` & `sentencepiece-0.1.99/sentencepiece/src/bpe_model.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/bpe_model_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/bpe_model_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/bpe_model_trainer.cc` & `sentencepiece-0.1.99/sentencepiece/src/bpe_model_trainer.cc`

 * *Files 3% similar despite different names*

```diff
@@ -82,36 +82,24 @@
   return s;
 }
 
 void Trainer::ComputeFreq(Symbol *symbol) const {
   if (symbol->freq > 0) {  // if freq == 0, re-computation is required.
     return;
   }
-  // Avoids double-count. ("AAA" => only count the first "AA").
-  Position prev_pos = {-1, 0};
   CHECK_EQ(0, symbol->freq);
   for (auto it = symbol->positions.begin(); it != symbol->positions.end();) {
     const Position pos = DecodePos(*it);
-    // There are two same bigrams in "AAA", [AA] [AA], and we want to
-    // remove the second one to avoid double counts.
-    // If the right symbol in the first bigram and the left symbol in the
-    // second bigram have the same position, (pos.left == prev_pos.right),
-    // duplicated bigram exisit.
-    // Also, symbols_[sid][left] and symbols_[sid]right] must store
+    // symbols_[sid][left] and symbols_[sid]right] must store
     // the same symbols in symbol->left and symbols->right.
-    if ((pos.sid == prev_pos.sid && pos.left == prev_pos.right) ||
-        symbol->left != symbols_[pos.sid][pos.left] ||
+    if (symbol->left != symbols_[pos.sid][pos.left] ||
         symbol->right != symbols_[pos.sid][pos.right]) {
       it = symbol->positions.erase(it);
-      // Initializes prev_pos.
-      // In "AAAA", the last "AA" can be counted.
-      prev_pos = {-1, 0};
     } else {
       symbol->freq += sentences_[pos.sid].second;
-      prev_pos = pos;
       ++it;
     }
   }
 }
 
 int Trainer::GetNextIndex(int sid, int index) const {
   for (size_t i = index + 1; i < symbols_[sid].size(); ++i) {
```

### Comparing `sentencepiece-0.1.98/sentencepiece/src/bpe_model_trainer.h` & `sentencepiece-0.1.99/sentencepiece/src/bpe_model_trainer.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/bpe_model_trainer_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/bpe_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/builder.cc` & `sentencepiece-0.1.99/sentencepiece/src/builder.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/builder.h` & `sentencepiece-0.1.99/sentencepiece/src/builder.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/builder_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/builder_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/builtin_pb/sentencepiece.pb.cc` & `sentencepiece-0.1.99/sentencepiece/src/builtin_pb/sentencepiece.pb.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/builtin_pb/sentencepiece.pb.h` & `sentencepiece-0.1.99/sentencepiece/src/builtin_pb/sentencepiece.pb.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc` & `sentencepiece-0.1.99/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h` & `sentencepiece-0.1.99/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/char_model.cc` & `sentencepiece-0.1.99/sentencepiece/src/char_model.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/char_model.h` & `sentencepiece-0.1.99/sentencepiece/src/char_model.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/char_model_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/char_model_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/char_model_trainer.cc` & `sentencepiece-0.1.99/sentencepiece/src/char_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/char_model_trainer.h` & `sentencepiece-0.1.99/sentencepiece/src/char_model_trainer.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/char_model_trainer_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/char_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/common.h` & `sentencepiece-0.1.99/sentencepiece/src/common.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/compile_charsmap_main.cc` & `sentencepiece-0.1.99/sentencepiece/src/compile_charsmap_main.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/error.cc` & `sentencepiece-0.1.99/sentencepiece/src/error.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/filesystem.cc` & `sentencepiece-0.1.99/sentencepiece/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/filesystem.h` & `sentencepiece-0.1.99/sentencepiece/src/filesystem.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/filesystem_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/filesystem_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/freelist.h` & `sentencepiece-0.1.99/sentencepiece/src/freelist.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/freelist_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/freelist_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/init.h` & `sentencepiece-0.1.99/sentencepiece/src/init.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/init_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/init_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/model_factory.cc` & `sentencepiece-0.1.99/sentencepiece/src/model_factory.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/model_factory.h` & `sentencepiece-0.1.99/sentencepiece/src/model_factory.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/model_factory_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/model_factory_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/model_interface.cc` & `sentencepiece-0.1.99/sentencepiece/src/model_interface.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/model_interface.h` & `sentencepiece-0.1.99/sentencepiece/src/model_interface.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/model_interface_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/model_interface_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/normalization_rule.h` & `sentencepiece-0.1.99/sentencepiece/src/normalization_rule.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/normalizer.cc` & `sentencepiece-0.1.99/sentencepiece/src/normalizer.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/normalizer.h` & `sentencepiece-0.1.99/sentencepiece/src/normalizer.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/normalizer_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/normalizer_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/pretokenizer_for_training.cc` & `sentencepiece-0.1.99/sentencepiece/src/pretokenizer_for_training.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/pretokenizer_for_training.h` & `sentencepiece-0.1.99/sentencepiece/src/pretokenizer_for_training.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/pretokenizer_for_training_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/pretokenizer_for_training_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/sentencepiece.proto` & `sentencepiece-0.1.99/sentencepiece/src/sentencepiece.proto`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/sentencepiece_model.proto` & `sentencepiece-0.1.99/sentencepiece/src/sentencepiece_model.proto`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/sentencepiece_processor.cc` & `sentencepiece-0.1.99/sentencepiece/src/sentencepiece_processor.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/sentencepiece_processor.h` & `sentencepiece-0.1.99/sentencepiece/src/sentencepiece_processor.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/sentencepiece_processor_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/sentencepiece_processor_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/sentencepiece_trainer.cc` & `sentencepiece-0.1.99/sentencepiece/src/sentencepiece_trainer.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/sentencepiece_trainer.h` & `sentencepiece-0.1.99/sentencepiece/src/sentencepiece_trainer.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/sentencepiece_trainer_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/sentencepiece_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/spec_parser.h` & `sentencepiece-0.1.99/sentencepiece/src/spec_parser.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/spm_decode_main.cc` & `sentencepiece-0.1.99/sentencepiece/src/spm_decode_main.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/spm_encode_main.cc` & `sentencepiece-0.1.99/sentencepiece/src/spm_encode_main.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/spm_export_vocab_main.cc` & `sentencepiece-0.1.99/sentencepiece/src/spm_export_vocab_main.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/spm_normalize_main.cc` & `sentencepiece-0.1.99/sentencepiece/src/spm_normalize_main.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/spm_train_main.cc` & `sentencepiece-0.1.99/sentencepiece/src/spm_train_main.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/test_main.cc` & `sentencepiece-0.1.99/sentencepiece/src/test_main.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/testharness.cc` & `sentencepiece-0.1.99/sentencepiece/src/testharness.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/testharness.h` & `sentencepiece-0.1.99/sentencepiece/src/testharness.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/trainer_factory.cc` & `sentencepiece-0.1.99/sentencepiece/src/trainer_factory.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/trainer_factory.h` & `sentencepiece-0.1.99/sentencepiece/src/trainer_factory.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/trainer_factory_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/trainer_factory_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/trainer_interface.cc` & `sentencepiece-0.1.99/sentencepiece/src/trainer_interface.cc`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 #define CHECK_RANGE(variable, minval, maxval) \
   CHECK_OR_RETURN(variable >= minval && variable <= maxval)
 
   CHECK_RANGE(trainer_spec.character_coverage(), 0.98, 1.0);
   CHECK_RANGE(trainer_spec.max_sentencepiece_length(), 1, 512);
   CHECK_RANGE(trainer_spec.num_sub_iterations(), 1, 10);
-  CHECK_RANGE(trainer_spec.num_threads(), 1, 128);
+  CHECK_RANGE(trainer_spec.num_threads(), 1, 1024);
   CHECK_RANGE(trainer_spec.self_test_sample_size(), 0, 1000);
   CHECK_RANGE(trainer_spec.shrinking_factor(), 0.5, 0.95);
   CHECK_RANGE(trainer_spec.max_sentence_length(), 10, 1073741824);
 #undef CHECK_RANGE
 
   CHECK_OR_RETURN(trainer_spec.input_sentence_size() <= 0 ||
                   trainer_spec.input_sentence_size() > 100);
```

### Comparing `sentencepiece-0.1.98/sentencepiece/src/trainer_interface.h` & `sentencepiece-0.1.99/sentencepiece/src/trainer_interface.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/trainer_interface_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/trainer_interface_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/unicode_script.cc` & `sentencepiece-0.1.99/sentencepiece/src/unicode_script.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/unicode_script.h` & `sentencepiece-0.1.99/sentencepiece/src/unicode_script.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/unicode_script_map.h` & `sentencepiece-0.1.99/sentencepiece/src/unicode_script_map.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/unicode_script_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/unicode_script_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/unigram_model.cc` & `sentencepiece-0.1.99/sentencepiece/src/unigram_model.cc`

 * *Files 0% similar despite different names*

```diff
@@ -457,15 +457,15 @@
       hyp->node = lnode;
       if (sample) {
         hyp->gx = probs[i];
         hyp->fx = adjusted_probs[i];
       } else {
         hyp->gx = lnode->score + top->gx;  // just adds node->score
         hyp->fx =
-            lnode->backtrace_score + hyp->gx;  // backtrace_score is h(node).
+            lnode->backtrace_score + top->gx;  // backtrace_score is h(node).
       }
       hyp->next = top;
       agenda.push(hyp);
     }
 
     static constexpr int kOneBillion = 1000000000;  // 10^9.
     if (hypothesis_allocator.size() >= kOneBillion) {
```

### Comparing `sentencepiece-0.1.98/sentencepiece/src/unigram_model.h` & `sentencepiece-0.1.99/sentencepiece/src/unigram_model.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/unigram_model_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/unigram_model_test.cc`

 * *Files 0% similar despite different names*

```diff
@@ -602,15 +602,15 @@
           (num_samples == 1 ? probs : inclusion_probs);
 
       for (const auto &it : scores) Z += it.second;
       for (const auto &it : probs_to_use) {
         EXPECT_NEAR(it.second, 1.0 * counts[it.first] / (kTrials * num_samples),
                     0.02);
         // The expectation is quite loose, use a higher tolerance
-        EXPECT_NEAR(1.0, scores[it.first] / kTrials, 0.20);
+        EXPECT_NEAR(1.0, scores[it.first] / kTrials, 0.30);
       }
     }
   }
 }
 
 TEST_P(UnigramModelTest, PieceToIdTest) {
   ModelProto model_proto = MakeBaseModelProto();
```

### Comparing `sentencepiece-0.1.98/sentencepiece/src/unigram_model_trainer.cc` & `sentencepiece-0.1.99/sentencepiece/src/unigram_model_trainer.cc`

 * *Files 10% similar despite different names*

```diff
@@ -24,28 +24,26 @@
 #include <utility>
 #include <vector>
 
 #include "normalizer.h"
 #include "pretokenizer_for_training.h"
 #include "sentencepiece_trainer.h"
 #include "third_party/absl/container/flat_hash_map.h"
-#include "third_party/absl/container/flat_hash_set.h"
 #include "third_party/absl/memory/memory.h"
 #include "third_party/absl/strings/str_replace.h"
 #include "third_party/absl/strings/str_split.h"
 #include "third_party/esaxx/esa.hxx"  // Suffix array library.
 #include "unicode_script.h"
 #include "util.h"
 
 namespace sentencepiece {
 namespace unigram {
 namespace {
 
 constexpr char32 kSentenceBoundary = 0x0000;
-constexpr char32 kWsMarker = 0x2581;
 
 double Digamma(double x) {
   double result = 0.0;
   for (; x < 7; ++x) result -= 1 / x;
   x -= 1.0 / 2.0;
   const double xx = 1.0 / x;
   const double xx2 = xx * xx;
@@ -63,66 +61,43 @@
   }
   float logsum = std::log(static_cast<double>(sum));
   for (auto it = begin; it != end; ++it) {
     it->second = std::log(static_cast<double>(it->second)) - logsum;
   }
 }
 
-template <typename T>
-std::vector<std::pair<const T *, const T *>> SplitBySentenceBoundary(
-    const T *begin, const T *end) {
-  std::vector<std::pair<const T *, const T *>> result;
-
-  while (begin < end) {
-    const auto *p = std::find(begin, end, static_cast<T>(kSentenceBoundary));
-    if (p != end) {
-      result.emplace_back(begin, p);
-      begin = p + 1;
-    } else {
-      result.emplace_back(begin, end);
-      break;
-    }
-  }
-
-  return result;
-}
-
 template <class T>
 class BoundedPriorityQueue {
  public:
   explicit BoundedPriorityQueue(size_t size) : size_(size) {}
   ~BoundedPriorityQueue() = default;
 
-  void push(const T &elem, int64 score) {
+  void push(T elem, int64 score) {
     if (queue_.size() > 4 * size_) resize();
-    if (queue_.size() >= size_ && queue_[size_ - 1].second > score) return;
+    if (sorted && queue_.size() >= size_ && queue_[size_ - 1].second > score)
+      return;
     queue_.emplace_back(elem, score);
   }
 
   const std::vector<std::pair<T, int64>> &get() {
     resize();
     return queue_;
   }
 
  private:
   void resize() {
     std::sort(queue_.begin(), queue_.end(), [](const auto &p1, const auto &p2) {
       return (p1.second > p2.second ||
               (p1.second == p2.second && p1.first < p2.first));
     });
-
-    absl::flat_hash_set<absl::string_view> dup;
-    std::vector<std::pair<T, int64>> new_queue;
-    for (auto &p : queue_) {
-      if (dup.insert(p.first).second) new_queue.emplace_back(std::move(p));
-      if (new_queue.size() == size_) break;
-    }
-    queue_ = std::move(new_queue);
+    sorted = true;
+    if (queue_.size() > size_) queue_.resize(size_);
   }
 
+  bool sorted = false;
   size_t size_ = 0;
   std::vector<std::pair<T, int64>> queue_;
 };
 
 }  // namespace
 
 TrainerModel::TrainerModel(const TrainerSpec &trainer_spec,
@@ -245,59 +220,57 @@
   constexpr node_int_type kAlphabetSize = 0x110000;  // All UCS4 range.
   node_int_type node_num = 0;
   LOG(INFO) << "Making suffix array...";
   CHECK_EQ(0, esaxx(array.begin(), SA.begin(), L.begin(), R.begin(), D.begin(),
                     n, kAlphabetSize, node_num));
 
   LOG(INFO) << "Extracting frequent sub strings... node_num=" << node_num;
-
-  BoundedPriorityQueue<std::string> queue(
+  BoundedPriorityQueue<node_int_type> queue(
       static_cast<size_t>(trainer_spec_.seed_sentencepiece_size()));
 
   for (node_int_type i = 0; i < node_num; ++i) {
     const node_int_type offset = SA[L[i]];
     const node_int_type len = D[i];
     if (len <= 1) {
       continue;
     }
-
-    for (const auto &p :
-         SplitBySentenceBoundary(&array[offset], &array[offset + len])) {
-      if (p.first == p.second) continue;
-      const auto [begin, end] = NormalizeRange(p.first, p.second);
-
-      const UnicodeText uw(begin, end);
-      if (uw.size() <= 1 || !IsValidSentencePiece(uw)) {
-        continue;
-      }
-
-      // character-wise coverage is the default score.
-      const node_int_type freq = R[i] - L[i];
-      const node_int_type score = freq * freq;
-
-      const auto w = string_util::UnicodeTextToUTF8(uw);
-      queue.push(w, score);
-
-      const auto subpieces =
-          SplitIntoWords(w, trainer_spec_.treat_whitespace_as_suffix(),
-                         trainer_spec_.allow_whitespace_only_pieces());
-      if (subpieces.size() > 1) {
-        for (const auto &s : subpieces) queue.push(std::string(s), score);
-      }
+    const char32 *begin = &array[offset];
+    const char32 *end = &array[offset + len];
+    // Skips if a substring contains a sentence boundary.
+    if (std::find(begin, end, kSentenceBoundary) != end) {
+      continue;
     }
+    const UnicodeText uw(begin, end);
+    if (!IsValidSentencePiece(uw)) {
+      continue;
+    }
+
+    // character-wise coverage is the default score.
+    const node_int_type freq = R[i] - L[i];
+    const node_int_type score = freq * len;
+    queue.push(i, score);
   }
 
   // all_chars must be included in the seed sentencepieces.
   TrainerModel::SentencePieces seed_sentencepieces;
   for (const auto &it : Sorted(all_chars)) {
     seed_sentencepieces.emplace_back(it);
   }
 
   for (const auto &p : queue.get()) {
-    seed_sentencepieces.emplace_back(p);
+    const node_int_type offset = SA[L[p.first]];
+    const node_int_type len = D[p.first];
+    CHECK_GT(len, 0);
+    const char32 *begin = &array[offset];
+    const char32 *end = &array[offset + len];
+    const UnicodeText uw(begin, end);
+    const std::string w = string_util::UnicodeTextToUTF8(uw);
+    CHECK(IsValidSentencePiece(uw));  // just in case.
+    CHECK(!port::ContainsKey(all_chars, w));
+    seed_sentencepieces.emplace_back(w, p.second);
   }
 
   ToLogProb(seed_sentencepieces.begin(), seed_sentencepieces.end());
 
   LOG(INFO) << "Initialized " << seed_sentencepieces.size()
             << " seed sentencepieces";
 
@@ -492,18 +465,18 @@
       F /= vsum;  // normalizes by all sentence frequency.
 
       // The logprob with the sentencepiece[i].
       const float logprob_sp = std::log(static_cast<double>(freq[i])) - logsum;
 
       // After removing the sentencepiece[i], its frequency freq[i] is
       // re-assigned to alternatives.
-      // new_sum = current_sum - freq[i] + freq[i] * alternatives.size()
-      //         = current_sum + freq[i] (alternatives - 1)
+      // new_sum = current_sum - freq[i] + freq[i] * alternatives[i].size()
+      //         = current_sum + freq[i] * (alternatives[i] - 1)
       const float logsum_alt = std::log(
-          static_cast<double>(sum + freq[i] * (alternatives.size() - 1)));
+          static_cast<double>(sum + freq[i] * (alternatives[i].size() - 1)));
 
       // The frequencies of altenatives are increased by freq[i].
       float logprob_alt = 0.0;
       for (const int n : alternatives[i]) {
         logprob_alt +=
             (std::log(static_cast<double>(freq[n] + freq[i])) - logsum_alt);
       }
@@ -526,30 +499,14 @@
     }
     new_sentencepieces.emplace_back(sentencepieces[w.first]);
   }
 
   return new_sentencepieces;
 }
 
-std::pair<const char32 *, const char32 *> Trainer::NormalizeRange(
-    const char32 *begin, const char32 *end) const {
-  if (trainer_spec_.treat_whitespace_as_suffix()) {
-    while ((*begin == kSentenceBoundary || *begin == kWsMarker) &&
-           begin + 1 < end)
-      ++begin;
-    while (*(end - 1) == kSentenceBoundary && begin + 1 < end) --end;
-  } else {
-    while (*begin == kSentenceBoundary && begin + 1 < end) ++begin;
-    while ((*(end - 1) == kSentenceBoundary || *(end - 1) == kWsMarker) &&
-           begin + 1 < end)
-      --end;
-  }
-  return std::make_pair(begin, end);
-}
-
 TrainerModel::SentencePieces Trainer::FinalizeSentencePieces(
     const TrainerModel &model) const {
   const auto &sentencepieces = model.GetSentencePieces();
   absl::flat_hash_map<std::string, float> final_sentencepieces;
   absl::flat_hash_map<std::string, float> sp(sentencepieces.begin(),
                                              sentencepieces.end());
```

### Comparing `sentencepiece-0.1.98/sentencepiece/src/unigram_model_trainer.h` & `sentencepiece-0.1.99/sentencepiece/src/unigram_model_trainer.h`

 * *Files 8% similar despite different names*

```diff
@@ -101,17 +101,14 @@
       const TrainerModel &model) const;
 
   // Makes the final sentence pieces by incorporating the required characters
   // and control/user defined symbols.
   TrainerModel::SentencePieces FinalizeSentencePieces(
       const TrainerModel &model) const;
 
-  std::pair<const char32 *, const char32 *> NormalizeRange(
-      const char32 *begin, const char32 *end) const;
-
   // When the size of SentencePieces becomes less than desired_vocab_size_,
   // break the main training loop. desired_vocab_size_ = 1.1 * vocab_size_
   // for now.
   int desired_vocab_size_;
 };
 }  // namespace unigram
 }  // namespace sentencepiece
```

### Comparing `sentencepiece-0.1.98/sentencepiece/src/unigram_model_trainer_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/unigram_model_trainer_test.cc`

 * *Files 3% similar despite different names*

```diff
@@ -113,32 +113,33 @@
 TEST(UnigramTrainerTest, BasicTest) {
   const auto& res = RunTrainer(
       {"magnanimity \t 5", "Pineapple \t 6", "i have an apple and a pen \t 1",
        "Overly \t 6", "Available \t 3"},
       30);
 
   // Check seed pieces.
-  EXPECT_EQ(63, res.seed_pieces_and_probs.size());
+  EXPECT_EQ(27, res.seed_pieces_and_probs.size());
+
+  LOG(INFO) << "[" << res.sentence_pieces << "]";
 
   // Check final pieces.
-  EXPECT_EQ(
-      "Overly Pineapple magnanimity Available ▁an a ▁ b A t g r P O v m y p n "
-      "l d e h i",
-      res.sentence_pieces);
+  EXPECT_EQ("i a n y m l e apple ve O P r g t an v ▁ b A le ▁an p d h",
+            res.sentence_pieces);
 }
 
 TEST(UnigramTrainerTest, BasicDPTest) {
   // no noise, clipping.
   {
     const auto& res = RunTrainer(
         {"magnanimity \t 5", "Pineapple \t 6", "i have an apple and a pen \t 1",
          "Overly \t 6", "Available \t 5"},
         22, true /*use_dp*/, 0 /*dp_noise*/, 4 /*dp_clipping*/);
 
-    EXPECT_EQ(49, res.seed_pieces_and_probs.size());
+    // Got 16 instead of 27 seeds.
+    EXPECT_EQ(16, res.seed_pieces_and_probs.size());
 
     // And they are equiv to if the last sentence was not there.
     const auto& res_nodp = RunTrainer(
         {"magnanimity \t 5", "Pineapple \t 6", "Overly \t 6", "Available \t 5"},
         22);
 
     EXPECT_EQ(res.seed_pieces_and_probs, res_nodp.seed_pieces_and_probs);
@@ -188,19 +189,20 @@
                         "何でも薄暗いじめじめした所でニャーニャー泣いていた事だ"
                         "けは記憶している"
                         "。",
                         &tok)
                   .ok());
   // TODO(taku): Temporally disable this test on Windows.
 #ifndef OS_WIN
+  LOG(INFO) << "[" << absl::StrJoin(tok, " ") << std::endl;
   EXPECT_EQ(
       WS
-      " 吾輩 《 わ が は い 》 は猫である 。 名前は まだ 無 い 。 どこ で 生れ "
-      "た か とん と 見当 《 けん とう 》 が つか ぬ 。 何でも 薄 暗 い じめ "
-      "じめ した 所で ニャーニャー 泣 い ていた 事 だけ は記憶している 。",
+      " 吾輩 《 わが はい 》 は猫である 。 名前はまだ 無 い 。 どこ で 生 れた "
+      "か とん と 見当 《 けん とう 》 が つか ぬ 。 何でも 薄 暗 い じめ じめ "
+      "した 所で ニャーニャー 泣 い ていた 事 だけは 記憶 している 。",
       absl::StrJoin(tok, " "));
 #endif
 }
 
 }  // namespace
 }  // namespace unigram
 }  // namespace sentencepiece
```

### Comparing `sentencepiece-0.1.98/sentencepiece/src/util.cc` & `sentencepiece-0.1.99/sentencepiece/src/util.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/util.h` & `sentencepiece-0.1.99/sentencepiece/src/util.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/util_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/util_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/word_model.cc` & `sentencepiece-0.1.99/sentencepiece/src/word_model.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/word_model.h` & `sentencepiece-0.1.99/sentencepiece/src/word_model.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/word_model_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/word_model_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/word_model_trainer.cc` & `sentencepiece-0.1.99/sentencepiece/src/word_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/word_model_trainer.h` & `sentencepiece-0.1.99/sentencepiece/src/word_model_trainer.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/src/word_model_trainer_test.cc` & `sentencepiece-0.1.99/sentencepiece/src/word_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/LICENSE` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/LICENSE`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/container/flat_hash_map.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/container/flat_hash_map.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/container/flat_hash_set.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/container/flat_hash_set.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/flags/flag.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/flags/flag.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/flags/flag.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/flags/flag.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/flags/parse.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/flags/parse.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/memory/memory.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/memory/memory.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/random/distributions.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/random/distributions.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/random/random.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/random/random.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/ascii.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/ascii.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/match.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/match.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/numbers.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/numbers.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/str_cat.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/str_cat.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/str_format.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/str_format.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/str_join.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/str_join.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/str_replace.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/str_replace.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/str_split.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/str_split.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/string_view.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/string_view.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/absl/strings/strip.h` & `sentencepiece-0.1.99/sentencepiece/third_party/absl/strings/strip.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/darts_clone/LICENSE` & `sentencepiece-0.1.99/sentencepiece/third_party/darts_clone/LICENSE`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/darts_clone/darts.h` & `sentencepiece-0.1.99/sentencepiece/third_party/darts_clone/darts.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/esaxx/LICENSE` & `sentencepiece-0.1.99/sentencepiece/third_party/esaxx/LICENSE`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/esaxx/esa.hxx` & `sentencepiece-0.1.99/sentencepiece/third_party/esaxx/esa.hxx`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/esaxx/sais.hxx` & `sentencepiece-0.1.99/sentencepiece/third_party/esaxx/sais.hxx`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/LICENSE` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/LICENSE`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/arena.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/arena.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/arenastring.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/arenastring.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/bytestream.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/bytestream.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/coded_stream.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/coded_stream.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/common.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/common.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/extension_set.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/extension_set.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/generated_message_util.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/generated_message_util.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/int128.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/int128.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/io_win32.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/io_win32.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/message_lite.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/message_lite.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/parse_context.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/parse_context.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/repeated_field.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/repeated_field.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/status.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/status.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/statusor.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/statusor.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/stringpiece.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/stringprintf.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/stringprintf.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/structurally_valid.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/structurally_valid.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/strutil.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/strutil.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/time.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/time.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc` & `sentencepiece-0.1.99/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/setup.py` & `sentencepiece-0.1.99/setup.py`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/src/sentencepiece/__init__.py` & `sentencepiece-0.1.99/src/sentencepiece/__init__.py`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/src/sentencepiece/sentencepiece.i` & `sentencepiece-0.1.99/src/sentencepiece/sentencepiece.i`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/src/sentencepiece/sentencepiece_model_pb2.py` & `sentencepiece-0.1.99/src/sentencepiece/sentencepiece_model_pb2.py`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/src/sentencepiece/sentencepiece_pb2.py` & `sentencepiece-0.1.99/src/sentencepiece/sentencepiece_pb2.py`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/src/sentencepiece/sentencepiece_wrap.cxx` & `sentencepiece-0.1.99/src/sentencepiece/sentencepiece_wrap.cxx`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/src/sentencepiece.egg-info/PKG-INFO` & `sentencepiece-0.1.99/src/sentencepiece.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentencepiece
-Version: 0.1.98
+Version: 0.1.99
 Summary: SentencePiece python wrapper
 Home-page: https://github.com/google/sentencepiece
 Author: Taku Kudo
 Author-email: taku@google.com
 License: Apache
 Platform: Unix
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sentencepiece-0.1.98/src/sentencepiece.egg-info/SOURCES.txt` & `sentencepiece-0.1.99/src/sentencepiece.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/test/botchan.txt` & `sentencepiece-0.1.99/test/botchan.txt`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/test/sentencepiece_test.py` & `sentencepiece-0.1.99/test/sentencepiece_test.py`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/test/test_ja_model.model` & `sentencepiece-0.1.99/test/test_ja_model.model`

 * *Files identical despite different names*

### Comparing `sentencepiece-0.1.98/test/test_model.model` & `sentencepiece-0.1.99/test/test_model.model`

 * *Files identical despite different names*

