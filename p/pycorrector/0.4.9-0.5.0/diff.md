# Comparing `tmp/pycorrector-0.4.9.tar.gz` & `tmp/pycorrector-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycorrector-0.4.9.tar", last modified: Fri Mar 31 09:42:25 2023, max compression
+gzip compressed data, was "pycorrector-0.5.0.tar", last modified: Tue May  2 13:53:41 2023, max compression
```

## Comparing `pycorrector-0.4.9.tar` & `pycorrector-0.5.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.506798 pycorrector-0.4.9/
--rw-r--r--   0 xuming     (501) staff       (20)    43134 2023-03-31 09:42:25.506225 pycorrector-0.4.9/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    35894 2023-03-28 03:18:33.000000 pycorrector-0.4.9/README.md
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.352644 pycorrector-0.4.9/pycorrector/
--rw-r--r--   0 xuming     (501) staff       (20)     1249 2022-11-09 13:02:53.000000 pycorrector-0.4.9/pycorrector/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1915 2022-03-21 13:34:34.000000 pycorrector-0.4.9/pycorrector/__main__.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.361265 pycorrector-0.4.9/pycorrector/bert/
--rw-r--r--   0 xuming     (501) staff       (20)        0 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/bert/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3484 2022-06-17 08:37:20.000000 pycorrector-0.4.9/pycorrector/bert/bert_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)     3144 2022-06-26 13:51:34.000000 pycorrector-0.4.9/pycorrector/bert/bert_generate.py
--rw-r--r--   0 xuming     (501) staff       (20)     1145 2021-11-23 05:01:44.000000 pycorrector-0.4.9/pycorrector/bert/predict_mask.py
--rw-r--r--   0 xuming     (501) staff       (20)     2592 2022-07-22 13:00:06.000000 pycorrector-0.4.9/pycorrector/config.py
--rw-r--r--   0 xuming     (501) staff       (20)     2292 2022-11-09 13:39:32.000000 pycorrector-0.4.9/pycorrector/confusion_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)    12185 2022-09-17 04:51:17.000000 pycorrector-0.4.9/pycorrector/corrector.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.385160 pycorrector-0.4.9/pycorrector/data/
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.340876 pycorrector-0.4.9/pycorrector/data/cn/
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.411354 pycorrector-0.4.9/pycorrector/data/cn/sighan_2015/
--rwxr-xr-x   0 xuming     (501) staff       (20)   204700 2021-12-03 04:52:34.000000 pycorrector-0.4.9/pycorrector/data/cn/sighan_2015/test.tsv
--rw-r--r--   0 xuming     (501) staff       (20)    14008 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/data/common_char_set.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.412100 pycorrector-0.4.9/pycorrector/data/en/
--rw-r--r--   0 xuming     (501) staff       (20)   588917 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/data/en/en.json.gz
--rw-r--r--   0 xuming     (501) staff       (20)   214642 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/data/eval_corpus.json
--rw-r--r--   0 xuming     (501) staff       (20)      559 2022-03-21 08:04:01.000000 pycorrector-0.4.9/pycorrector/data/get_confusion_pair.py
--rw-r--r--   0 xuming     (501) staff       (20)   163162 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/data/person_name.txt
--rw-r--r--   0 xuming     (501) staff       (20)   640666 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/data/place_name.txt
--rw-r--r--   0 xuming     (501) staff       (20)     1195 2022-03-22 08:30:08.000000 pycorrector-0.4.9/pycorrector/data/proper_name.txt
--rw-r--r--   0 xuming     (501) staff       (20)   197815 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/data/same_pinyin.txt
--rw-r--r--   0 xuming     (501) staff       (20)    14636 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/data/same_stroke.txt
--rw-r--r--   0 xuming     (501) staff       (20)     9136 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/data/stopwords.txt
--rw-r--r--   0 xuming     (501) staff       (20)   202746 2022-11-22 07:22:06.000000 pycorrector-0.4.9/pycorrector/data/stroke.txt
--rwxr-xr-x   0 xuming     (501) staff       (20)  8583143 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/data/word_freq.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.425185 pycorrector-0.4.9/pycorrector/deepcontext/
--rw-r--r--   0 xuming     (501) staff       (20)        0 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/deepcontext/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1165 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/deepcontext/config.py
--rw-r--r--   0 xuming     (501) staff       (20)     3912 2021-12-02 13:25:35.000000 pycorrector-0.4.9/pycorrector/deepcontext/data_reader.py
--rw-r--r--   0 xuming     (501) staff       (20)     2075 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/deepcontext/dataset.py
--rw-r--r--   0 xuming     (501) staff       (20)     5568 2022-06-17 08:37:20.000000 pycorrector-0.4.9/pycorrector/deepcontext/infer.py
--rw-r--r--   0 xuming     (501) staff       (20)     2941 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/deepcontext/loss.py
--rw-r--r--   0 xuming     (501) staff       (20)     6726 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/deepcontext/model.py
--rw-r--r--   0 xuming     (501) staff       (20)     2078 2021-12-02 13:20:56.000000 pycorrector-0.4.9/pycorrector/deepcontext/preprocess.py
--rw-r--r--   0 xuming     (501) staff       (20)     5050 2021-10-18 07:02:32.000000 pycorrector-0.4.9/pycorrector/deepcontext/train.py
--rw-r--r--   0 xuming     (501) staff       (20)    17711 2022-09-17 04:51:17.000000 pycorrector-0.4.9/pycorrector/detector.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.427549 pycorrector-0.4.9/pycorrector/electra/
--rw-r--r--   0 xuming     (501) staff       (20)        0 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/electra/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     4264 2022-06-17 08:37:19.000000 pycorrector-0.4.9/pycorrector/electra/electra_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)     1459 2021-11-23 05:08:54.000000 pycorrector-0.4.9/pycorrector/electra/predict_mask.py
--rw-r--r--   0 xuming     (501) staff       (20)     5830 2022-10-12 02:22:38.000000 pycorrector-0.4.9/pycorrector/en_spell.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.435623 pycorrector-0.4.9/pycorrector/ernie/
--rw-r--r--   0 xuming     (501) staff       (20)       81 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/ernie/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     5866 2022-06-17 08:37:20.000000 pycorrector-0.4.9/pycorrector/ernie/ernie_corrector.py
--rwxr-xr-x   0 xuming     (501) staff       (20)     3062 2022-10-27 09:34:47.000000 pycorrector-0.4.9/pycorrector/ernie/file_utils.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    30612 2022-06-17 08:37:20.000000 pycorrector-0.4.9/pycorrector/ernie/modeling_ernie.py
--rwxr-xr-x   0 xuming     (501) staff       (20)     7650 2022-06-17 08:37:20.000000 pycorrector-0.4.9/pycorrector/ernie/optimization.py
--rw-r--r--   0 xuming     (501) staff       (20)     3349 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/ernie/predict_mask.py
--rwxr-xr-x   0 xuming     (501) staff       (20)     9238 2022-06-17 08:37:20.000000 pycorrector-0.4.9/pycorrector/ernie/tokenizing_ernie.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.446792 pycorrector-0.4.9/pycorrector/ernie_csc/
--rw-r--r--   0 xuming     (501) staff       (20)       81 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/ernie_csc/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1448 2022-01-06 09:00:22.000000 pycorrector-0.4.9/pycorrector/ernie_csc/change_sgml_to_txt.py
--rw-r--r--   0 xuming     (501) staff       (20)     1150 2022-01-06 09:00:22.000000 pycorrector-0.4.9/pycorrector/ernie_csc/download.py
--rw-r--r--   0 xuming     (501) staff       (20)     1135 2022-01-06 09:04:42.000000 pycorrector-0.4.9/pycorrector/ernie_csc/ernie_csc_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)     2255 2022-01-06 09:00:22.000000 pycorrector-0.4.9/pycorrector/ernie_csc/export_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6253 2022-01-06 09:00:22.000000 pycorrector-0.4.9/pycorrector/ernie_csc/model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6371 2022-01-06 09:00:22.000000 pycorrector-0.4.9/pycorrector/ernie_csc/predict.py
--rw-r--r--   0 xuming     (501) staff       (20)     5874 2022-01-06 09:00:22.000000 pycorrector-0.4.9/pycorrector/ernie_csc/predict_sighan.py
--rw-r--r--   0 xuming     (501) staff       (20)     4662 2022-01-06 09:00:22.000000 pycorrector-0.4.9/pycorrector/ernie_csc/sighan_evaluate.py
--rw-r--r--   0 xuming     (501) staff       (20)    11027 2022-01-06 09:00:22.000000 pycorrector-0.4.9/pycorrector/ernie_csc/train.py
--rw-r--r--   0 xuming     (501) staff       (20)     5147 2022-01-06 09:00:22.000000 pycorrector-0.4.9/pycorrector/ernie_csc/utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.463684 pycorrector-0.4.9/pycorrector/macbert/
--rw-r--r--   0 xuming     (501) staff       (20)        0 2021-11-22 13:24:05.000000 pycorrector-0.4.9/pycorrector/macbert/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     7246 2022-06-17 08:37:20.000000 pycorrector-0.4.9/pycorrector/macbert/base_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     1097 2021-11-15 09:52:07.000000 pycorrector-0.4.9/pycorrector/macbert/correct_demo.py
--rw-r--r--   0 xuming     (501) staff       (20)     3565 2021-10-31 04:24:05.000000 pycorrector-0.4.9/pycorrector/macbert/defaults.py
--rw-r--r--   0 xuming     (501) staff       (20)     9013 2021-11-05 06:19:17.000000 pycorrector-0.4.9/pycorrector/macbert/evaluate_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     4952 2022-10-17 03:25:37.000000 pycorrector-0.4.9/pycorrector/macbert/infer.py
--rw-r--r--   0 xuming     (501) staff       (20)     6636 2021-10-31 04:24:05.000000 pycorrector-0.4.9/pycorrector/macbert/lr_scheduler.py
--rw-r--r--   0 xuming     (501) staff       (20)     2101 2021-12-28 03:36:23.000000 pycorrector-0.4.9/pycorrector/macbert/macbert4csc.py
--rw-r--r--   0 xuming     (501) staff       (20)     7881 2023-01-17 12:09:19.000000 pycorrector-0.4.9/pycorrector/macbert/macbert_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)     7635 2022-09-05 06:59:51.000000 pycorrector-0.4.9/pycorrector/macbert/preprocess.py
--rw-r--r--   0 xuming     (501) staff       (20)     2652 2022-10-17 03:25:37.000000 pycorrector-0.4.9/pycorrector/macbert/reader.py
--rw-r--r--   0 xuming     (501) staff       (20)     6375 2021-11-22 11:54:21.000000 pycorrector-0.4.9/pycorrector/macbert/softmaskedbert4csc.py
--rw-r--r--   0 xuming     (501) staff       (20)     5241 2022-10-19 06:49:39.000000 pycorrector-0.4.9/pycorrector/macbert/train.py
--rw-r--r--   0 xuming     (501) staff       (20)     8533 2022-11-22 07:22:06.000000 pycorrector-0.4.9/pycorrector/proper_corrector.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.479666 pycorrector-0.4.9/pycorrector/seq2seq/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/seq2seq/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    12173 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/seq2seq/convseq2seq.py
--rw-r--r--   0 xuming     (501) staff       (20)     5527 2022-06-17 08:37:19.000000 pycorrector-0.4.9/pycorrector/seq2seq/data_reader.py
--rw-r--r--   0 xuming     (501) staff       (20)     8405 2022-06-17 09:02:07.000000 pycorrector-0.4.9/pycorrector/seq2seq/infer.py
--rw-r--r--   0 xuming     (501) staff       (20)     6719 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/seq2seq/model_args.py
--rw-r--r--   0 xuming     (501) staff       (20)     2468 2022-06-14 06:14:52.000000 pycorrector-0.4.9/pycorrector/seq2seq/preprocess.py
--rw-r--r--   0 xuming     (501) staff       (20)     7745 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/seq2seq/seq2seq.py
--rw-r--r--   0 xuming     (501) staff       (20)     3865 2022-06-17 09:02:07.000000 pycorrector-0.4.9/pycorrector/seq2seq/seq2seq_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)    50354 2022-06-17 08:37:20.000000 pycorrector-0.4.9/pycorrector/seq2seq/seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     4640 2022-06-17 08:37:19.000000 pycorrector-0.4.9/pycorrector/seq2seq/seq2seq_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    16239 2022-06-17 08:37:20.000000 pycorrector-0.4.9/pycorrector/seq2seq/train.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.485902 pycorrector-0.4.9/pycorrector/t5/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2022-06-11 01:43:17.000000 pycorrector-0.4.9/pycorrector/t5/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     8551 2022-07-25 03:19:38.000000 pycorrector-0.4.9/pycorrector/t5/copyt5_corrector_bak.py
--rw-r--r--   0 xuming     (501) staff       (20)     3201 2022-09-20 06:39:49.000000 pycorrector-0.4.9/pycorrector/t5/infer.py
--rw-r--r--   0 xuming     (501) staff       (20)     7378 2022-07-25 03:14:23.000000 pycorrector-0.4.9/pycorrector/t5/t5_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)    11266 2023-01-03 06:21:45.000000 pycorrector-0.4.9/pycorrector/t5/train.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.489811 pycorrector-0.4.9/pycorrector/transformer/
--rw-r--r--   0 xuming     (501) staff       (20)       81 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/transformer/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1580 2021-12-02 13:25:35.000000 pycorrector-0.4.9/pycorrector/transformer/config.py
--rw-r--r--   0 xuming     (501) staff       (20)     3132 2021-12-02 13:20:56.000000 pycorrector-0.4.9/pycorrector/transformer/preprocess.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.501150 pycorrector-0.4.9/pycorrector/utils/
--rw-r--r--   0 xuming     (501) staff       (20)        0 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/utils/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    13747 2022-09-28 05:07:31.000000 pycorrector-0.4.9/pycorrector/utils/eval.py
--rw-r--r--   0 xuming     (501) staff       (20)    12583 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/utils/get_file.py
--rw-r--r--   0 xuming     (501) staff       (20)     1132 2021-12-02 13:22:02.000000 pycorrector-0.4.9/pycorrector/utils/io_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     8081 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/utils/langconv.py
--rw-r--r--   0 xuming     (501) staff       (20)     3214 2022-03-22 06:45:40.000000 pycorrector-0.4.9/pycorrector/utils/math_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     6242 2022-03-21 14:22:12.000000 pycorrector-0.4.9/pycorrector/utils/ngram_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     4884 2022-08-29 01:01:15.000000 pycorrector-0.4.9/pycorrector/utils/text_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     6086 2022-06-17 08:37:20.000000 pycorrector-0.4.9/pycorrector/utils/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)   143019 2021-08-04 13:23:48.000000 pycorrector-0.4.9/pycorrector/utils/zh_wiki.py
--rw-r--r--   0 xuming     (501) staff       (20)       22 2023-03-31 02:47:28.000000 pycorrector-0.4.9/pycorrector/version.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-03-31 09:42:25.357107 pycorrector-0.4.9/pycorrector.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    43134 2023-03-31 09:42:24.000000 pycorrector-0.4.9/pycorrector.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     3467 2023-03-31 09:42:25.000000 pycorrector-0.4.9/pycorrector.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-03-31 09:42:24.000000 pycorrector-0.4.9/pycorrector.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2022-06-17 09:04:59.000000 pycorrector-0.4.9/pycorrector.egg-info/not-zip-safe
--rw-r--r--   0 xuming     (501) staff       (20)       38 2023-03-31 09:42:24.000000 pycorrector-0.4.9/pycorrector.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)       12 2023-03-31 09:42:24.000000 pycorrector-0.4.9/pycorrector.egg-info/top_level.txt
--rw-r--r--   0 xuming     (501) staff       (20)       38 2023-03-31 09:42:25.507028 pycorrector-0.4.9/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1635 2023-03-31 02:47:28.000000 pycorrector-0.4.9/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.938971 pycorrector-0.5.0/
+-rw-r--r--   0 xuming     (501) staff       (20)    43134 2023-05-02 13:53:41.938444 pycorrector-0.5.0/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    35894 2023-03-28 03:18:33.000000 pycorrector-0.5.0/README.md
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.752274 pycorrector-0.5.0/pycorrector/
+-rw-r--r--   0 xuming     (501) staff       (20)     1249 2022-11-09 13:02:53.000000 pycorrector-0.5.0/pycorrector/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1915 2022-03-21 13:34:34.000000 pycorrector-0.5.0/pycorrector/__main__.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.760646 pycorrector-0.5.0/pycorrector/bert/
+-rw-r--r--   0 xuming     (501) staff       (20)        0 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/bert/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3484 2022-06-17 08:37:20.000000 pycorrector-0.5.0/pycorrector/bert/bert_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3144 2022-06-26 13:51:34.000000 pycorrector-0.5.0/pycorrector/bert/bert_generate.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1145 2021-11-23 05:01:44.000000 pycorrector-0.5.0/pycorrector/bert/predict_mask.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2592 2022-07-22 13:00:06.000000 pycorrector-0.5.0/pycorrector/config.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2292 2022-11-09 13:39:32.000000 pycorrector-0.5.0/pycorrector/confusion_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)    12185 2022-09-17 04:51:17.000000 pycorrector-0.5.0/pycorrector/corrector.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.787595 pycorrector-0.5.0/pycorrector/data/
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.736548 pycorrector-0.5.0/pycorrector/data/cn/
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.829528 pycorrector-0.5.0/pycorrector/data/cn/sighan_2015/
+-rwxr-xr-x   0 xuming     (501) staff       (20)   204700 2021-12-03 04:52:34.000000 pycorrector-0.5.0/pycorrector/data/cn/sighan_2015/test.tsv
+-rw-r--r--   0 xuming     (501) staff       (20)    14008 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/data/common_char_set.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.834560 pycorrector-0.5.0/pycorrector/data/en/
+-rw-r--r--   0 xuming     (501) staff       (20)   588917 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/data/en/en.json.gz
+-rw-r--r--   0 xuming     (501) staff       (20)   214642 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/data/eval_corpus.json
+-rw-r--r--   0 xuming     (501) staff       (20)      559 2022-03-21 08:04:01.000000 pycorrector-0.5.0/pycorrector/data/get_confusion_pair.py
+-rw-r--r--   0 xuming     (501) staff       (20)   163162 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/data/person_name.txt
+-rw-r--r--   0 xuming     (501) staff       (20)   640666 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/data/place_name.txt
+-rw-r--r--   0 xuming     (501) staff       (20)     1195 2022-03-22 08:30:08.000000 pycorrector-0.5.0/pycorrector/data/proper_name.txt
+-rw-r--r--   0 xuming     (501) staff       (20)   197815 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/data/same_pinyin.txt
+-rw-r--r--   0 xuming     (501) staff       (20)    14636 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/data/same_stroke.txt
+-rw-r--r--   0 xuming     (501) staff       (20)     9136 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/data/stopwords.txt
+-rw-r--r--   0 xuming     (501) staff       (20)   202746 2022-11-22 07:22:06.000000 pycorrector-0.5.0/pycorrector/data/stroke.txt
+-rwxr-xr-x   0 xuming     (501) staff       (20)  8583143 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/data/word_freq.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.853380 pycorrector-0.5.0/pycorrector/deepcontext/
+-rw-r--r--   0 xuming     (501) staff       (20)        0 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/deepcontext/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1165 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/deepcontext/config.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3912 2021-12-02 13:25:35.000000 pycorrector-0.5.0/pycorrector/deepcontext/data_reader.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2075 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/deepcontext/dataset.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5568 2022-06-17 08:37:20.000000 pycorrector-0.5.0/pycorrector/deepcontext/infer.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2941 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/deepcontext/loss.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6726 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/deepcontext/model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2078 2021-12-02 13:20:56.000000 pycorrector-0.5.0/pycorrector/deepcontext/preprocess.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5050 2021-10-18 07:02:32.000000 pycorrector-0.5.0/pycorrector/deepcontext/train.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17711 2022-09-17 04:51:17.000000 pycorrector-0.5.0/pycorrector/detector.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.855789 pycorrector-0.5.0/pycorrector/electra/
+-rw-r--r--   0 xuming     (501) staff       (20)        0 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/electra/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4264 2022-06-17 08:37:19.000000 pycorrector-0.5.0/pycorrector/electra/electra_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1459 2021-11-23 05:08:54.000000 pycorrector-0.5.0/pycorrector/electra/predict_mask.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5830 2022-10-12 02:22:38.000000 pycorrector-0.5.0/pycorrector/en_spell.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.865351 pycorrector-0.5.0/pycorrector/ernie/
+-rw-r--r--   0 xuming     (501) staff       (20)       81 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/ernie/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5866 2022-06-17 08:37:20.000000 pycorrector-0.5.0/pycorrector/ernie/ernie_corrector.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)     3062 2022-10-27 09:34:47.000000 pycorrector-0.5.0/pycorrector/ernie/file_utils.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    30612 2022-06-17 08:37:20.000000 pycorrector-0.5.0/pycorrector/ernie/modeling_ernie.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)     7650 2022-06-17 08:37:20.000000 pycorrector-0.5.0/pycorrector/ernie/optimization.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3349 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/ernie/predict_mask.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)     9238 2022-06-17 08:37:20.000000 pycorrector-0.5.0/pycorrector/ernie/tokenizing_ernie.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.880103 pycorrector-0.5.0/pycorrector/ernie_csc/
+-rw-r--r--   0 xuming     (501) staff       (20)       81 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/ernie_csc/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1448 2022-01-06 09:00:22.000000 pycorrector-0.5.0/pycorrector/ernie_csc/change_sgml_to_txt.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1150 2022-01-06 09:00:22.000000 pycorrector-0.5.0/pycorrector/ernie_csc/download.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1135 2022-01-06 09:04:42.000000 pycorrector-0.5.0/pycorrector/ernie_csc/ernie_csc_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2255 2022-01-06 09:00:22.000000 pycorrector-0.5.0/pycorrector/ernie_csc/export_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6253 2022-01-06 09:00:22.000000 pycorrector-0.5.0/pycorrector/ernie_csc/model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6371 2022-01-06 09:00:22.000000 pycorrector-0.5.0/pycorrector/ernie_csc/predict.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5874 2022-01-06 09:00:22.000000 pycorrector-0.5.0/pycorrector/ernie_csc/predict_sighan.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4662 2022-01-06 09:00:22.000000 pycorrector-0.5.0/pycorrector/ernie_csc/sighan_evaluate.py
+-rw-r--r--   0 xuming     (501) staff       (20)    11027 2022-01-06 09:00:22.000000 pycorrector-0.5.0/pycorrector/ernie_csc/train.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5147 2022-01-06 09:00:22.000000 pycorrector-0.5.0/pycorrector/ernie_csc/utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.897185 pycorrector-0.5.0/pycorrector/macbert/
+-rw-r--r--   0 xuming     (501) staff       (20)        0 2021-11-22 13:24:05.000000 pycorrector-0.5.0/pycorrector/macbert/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7246 2022-06-17 08:37:20.000000 pycorrector-0.5.0/pycorrector/macbert/base_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1097 2021-11-15 09:52:07.000000 pycorrector-0.5.0/pycorrector/macbert/correct_demo.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3565 2021-10-31 04:24:05.000000 pycorrector-0.5.0/pycorrector/macbert/defaults.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9013 2021-11-05 06:19:17.000000 pycorrector-0.5.0/pycorrector/macbert/evaluate_util.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4952 2022-10-17 03:25:37.000000 pycorrector-0.5.0/pycorrector/macbert/infer.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6636 2021-10-31 04:24:05.000000 pycorrector-0.5.0/pycorrector/macbert/lr_scheduler.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2101 2021-12-28 03:36:23.000000 pycorrector-0.5.0/pycorrector/macbert/macbert4csc.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7922 2023-05-02 13:44:00.000000 pycorrector-0.5.0/pycorrector/macbert/macbert_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7635 2022-09-05 06:59:51.000000 pycorrector-0.5.0/pycorrector/macbert/preprocess.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2652 2022-10-17 03:25:37.000000 pycorrector-0.5.0/pycorrector/macbert/reader.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6375 2021-11-22 11:54:21.000000 pycorrector-0.5.0/pycorrector/macbert/softmaskedbert4csc.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5241 2022-10-19 06:49:39.000000 pycorrector-0.5.0/pycorrector/macbert/train.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8533 2022-11-22 07:22:06.000000 pycorrector-0.5.0/pycorrector/proper_corrector.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.912498 pycorrector-0.5.0/pycorrector/seq2seq/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/seq2seq/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    12173 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/seq2seq/convseq2seq.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5527 2022-06-17 08:37:19.000000 pycorrector-0.5.0/pycorrector/seq2seq/data_reader.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8405 2022-06-17 09:02:07.000000 pycorrector-0.5.0/pycorrector/seq2seq/infer.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6719 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/seq2seq/model_args.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2468 2022-06-14 06:14:52.000000 pycorrector-0.5.0/pycorrector/seq2seq/preprocess.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7745 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/seq2seq/seq2seq.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3865 2022-06-17 09:02:07.000000 pycorrector-0.5.0/pycorrector/seq2seq/seq2seq_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50354 2022-06-17 08:37:20.000000 pycorrector-0.5.0/pycorrector/seq2seq/seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4640 2022-06-17 08:37:19.000000 pycorrector-0.5.0/pycorrector/seq2seq/seq2seq_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    16239 2022-06-17 08:37:20.000000 pycorrector-0.5.0/pycorrector/seq2seq/train.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.918863 pycorrector-0.5.0/pycorrector/t5/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2022-06-11 01:43:17.000000 pycorrector-0.5.0/pycorrector/t5/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8551 2022-07-25 03:19:38.000000 pycorrector-0.5.0/pycorrector/t5/copyt5_corrector_bak.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3201 2022-09-20 06:39:49.000000 pycorrector-0.5.0/pycorrector/t5/infer.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7378 2022-07-25 03:14:23.000000 pycorrector-0.5.0/pycorrector/t5/t5_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)    11266 2023-01-03 06:21:45.000000 pycorrector-0.5.0/pycorrector/t5/train.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.922916 pycorrector-0.5.0/pycorrector/transformer/
+-rw-r--r--   0 xuming     (501) staff       (20)       81 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/transformer/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1580 2021-12-02 13:25:35.000000 pycorrector-0.5.0/pycorrector/transformer/config.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3132 2021-12-02 13:20:56.000000 pycorrector-0.5.0/pycorrector/transformer/preprocess.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.934770 pycorrector-0.5.0/pycorrector/utils/
+-rw-r--r--   0 xuming     (501) staff       (20)        0 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/utils/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13747 2022-09-28 05:07:31.000000 pycorrector-0.5.0/pycorrector/utils/eval.py
+-rw-r--r--   0 xuming     (501) staff       (20)    12583 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/utils/get_file.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1132 2021-12-02 13:22:02.000000 pycorrector-0.5.0/pycorrector/utils/io_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8081 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/utils/langconv.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3214 2022-03-22 06:45:40.000000 pycorrector-0.5.0/pycorrector/utils/math_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6242 2022-03-21 14:22:12.000000 pycorrector-0.5.0/pycorrector/utils/ngram_util.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4884 2022-08-29 01:01:15.000000 pycorrector-0.5.0/pycorrector/utils/text_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6086 2022-06-17 08:37:20.000000 pycorrector-0.5.0/pycorrector/utils/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)   143019 2021-08-04 13:23:48.000000 pycorrector-0.5.0/pycorrector/utils/zh_wiki.py
+-rw-r--r--   0 xuming     (501) staff       (20)       22 2023-05-02 13:49:52.000000 pycorrector-0.5.0/pycorrector/version.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-02 13:53:41.757192 pycorrector-0.5.0/pycorrector.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    43134 2023-05-02 13:53:41.000000 pycorrector-0.5.0/pycorrector.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     3467 2023-05-02 13:53:41.000000 pycorrector-0.5.0/pycorrector.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-05-02 13:53:41.000000 pycorrector-0.5.0/pycorrector.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2022-06-17 09:04:59.000000 pycorrector-0.5.0/pycorrector.egg-info/not-zip-safe
+-rw-r--r--   0 xuming     (501) staff       (20)       38 2023-05-02 13:53:41.000000 pycorrector-0.5.0/pycorrector.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       12 2023-05-02 13:53:41.000000 pycorrector-0.5.0/pycorrector.egg-info/top_level.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       38 2023-05-02 13:53:41.939419 pycorrector-0.5.0/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1635 2023-03-31 02:47:28.000000 pycorrector-0.5.0/setup.py
```

### Comparing `pycorrector-0.4.9/PKG-INFO` & `pycorrector-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycorrector
-Version: 0.4.9
+Version: 0.5.0
 Summary: Chinese Text Error Corrector
 Home-page: https://github.com/shibing624/pycorrector
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: ![alt text](docs/pycorrector.png)
```

### Comparing `pycorrector-0.4.9/README.md` & `pycorrector-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/__init__.py` & `pycorrector-0.5.0/pycorrector/__init__.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/__main__.py` & `pycorrector-0.5.0/pycorrector/__main__.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/bert/bert_corrector.py` & `pycorrector-0.5.0/pycorrector/bert/bert_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/bert/bert_generate.py` & `pycorrector-0.5.0/pycorrector/bert/bert_generate.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/bert/predict_mask.py` & `pycorrector-0.5.0/pycorrector/bert/predict_mask.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/config.py` & `pycorrector-0.5.0/pycorrector/config.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/confusion_corrector.py` & `pycorrector-0.5.0/pycorrector/confusion_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/corrector.py` & `pycorrector-0.5.0/pycorrector/corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/cn/sighan_2015/test.tsv` & `pycorrector-0.5.0/pycorrector/data/cn/sighan_2015/test.tsv`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/common_char_set.txt` & `pycorrector-0.5.0/pycorrector/data/common_char_set.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/en/en.json.gz` & `pycorrector-0.5.0/pycorrector/data/en/en.json.gz`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/eval_corpus.json` & `pycorrector-0.5.0/pycorrector/data/eval_corpus.json`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/get_confusion_pair.py` & `pycorrector-0.5.0/pycorrector/data/get_confusion_pair.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/person_name.txt` & `pycorrector-0.5.0/pycorrector/data/person_name.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/place_name.txt` & `pycorrector-0.5.0/pycorrector/data/place_name.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/proper_name.txt` & `pycorrector-0.5.0/pycorrector/data/proper_name.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/same_pinyin.txt` & `pycorrector-0.5.0/pycorrector/data/same_pinyin.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/same_stroke.txt` & `pycorrector-0.5.0/pycorrector/data/same_stroke.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/stopwords.txt` & `pycorrector-0.5.0/pycorrector/data/stopwords.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/stroke.txt` & `pycorrector-0.5.0/pycorrector/data/stroke.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/data/word_freq.txt` & `pycorrector-0.5.0/pycorrector/data/word_freq.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/deepcontext/config.py` & `pycorrector-0.5.0/pycorrector/deepcontext/config.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/deepcontext/data_reader.py` & `pycorrector-0.5.0/pycorrector/deepcontext/data_reader.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/deepcontext/dataset.py` & `pycorrector-0.5.0/pycorrector/deepcontext/dataset.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/deepcontext/infer.py` & `pycorrector-0.5.0/pycorrector/deepcontext/infer.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/deepcontext/loss.py` & `pycorrector-0.5.0/pycorrector/deepcontext/loss.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/deepcontext/model.py` & `pycorrector-0.5.0/pycorrector/deepcontext/model.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/deepcontext/preprocess.py` & `pycorrector-0.5.0/pycorrector/deepcontext/preprocess.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/deepcontext/train.py` & `pycorrector-0.5.0/pycorrector/deepcontext/train.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/detector.py` & `pycorrector-0.5.0/pycorrector/detector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/electra/electra_corrector.py` & `pycorrector-0.5.0/pycorrector/electra/electra_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/electra/predict_mask.py` & `pycorrector-0.5.0/pycorrector/electra/predict_mask.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/en_spell.py` & `pycorrector-0.5.0/pycorrector/en_spell.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie/ernie_corrector.py` & `pycorrector-0.5.0/pycorrector/ernie/ernie_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie/file_utils.py` & `pycorrector-0.5.0/pycorrector/ernie/file_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie/modeling_ernie.py` & `pycorrector-0.5.0/pycorrector/ernie/modeling_ernie.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie/optimization.py` & `pycorrector-0.5.0/pycorrector/ernie/optimization.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie/predict_mask.py` & `pycorrector-0.5.0/pycorrector/ernie/predict_mask.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie/tokenizing_ernie.py` & `pycorrector-0.5.0/pycorrector/ernie/tokenizing_ernie.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie_csc/change_sgml_to_txt.py` & `pycorrector-0.5.0/pycorrector/ernie_csc/change_sgml_to_txt.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie_csc/download.py` & `pycorrector-0.5.0/pycorrector/ernie_csc/download.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie_csc/ernie_csc_corrector.py` & `pycorrector-0.5.0/pycorrector/ernie_csc/ernie_csc_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie_csc/export_model.py` & `pycorrector-0.5.0/pycorrector/ernie_csc/export_model.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie_csc/model.py` & `pycorrector-0.5.0/pycorrector/ernie_csc/model.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie_csc/predict.py` & `pycorrector-0.5.0/pycorrector/ernie_csc/predict.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie_csc/predict_sighan.py` & `pycorrector-0.5.0/pycorrector/ernie_csc/predict_sighan.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie_csc/sighan_evaluate.py` & `pycorrector-0.5.0/pycorrector/ernie_csc/sighan_evaluate.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie_csc/train.py` & `pycorrector-0.5.0/pycorrector/ernie_csc/train.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/ernie_csc/utils.py` & `pycorrector-0.5.0/pycorrector/ernie_csc/utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/macbert/base_model.py` & `pycorrector-0.5.0/pycorrector/macbert/base_model.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/macbert/correct_demo.py` & `pycorrector-0.5.0/pycorrector/macbert/correct_demo.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/macbert/defaults.py` & `pycorrector-0.5.0/pycorrector/macbert/defaults.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/macbert/evaluate_util.py` & `pycorrector-0.5.0/pycorrector/macbert/evaluate_util.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/macbert/infer.py` & `pycorrector-0.5.0/pycorrector/macbert/infer.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/macbert/lr_scheduler.py` & `pycorrector-0.5.0/pycorrector/macbert/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/macbert/macbert4csc.py` & `pycorrector-0.5.0/pycorrector/macbert/macbert4csc.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/macbert/macbert_corrector.py` & `pycorrector-0.5.0/pycorrector/macbert/macbert_corrector.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,34 +51,34 @@
 
         self.tokenizer = BertTokenizerFast.from_pretrained(model_dir)
         self.model = BertForMaskedLM.from_pretrained(model_dir)
         self.model.to(device)
         logger.debug("Use device: {}".format(device))
         logger.debug('Loaded macbert4csc model: %s, spend: %.3f s.' % (model_dir, time.time() - t1))
 
-    def macbert_correct(self, text, threshold=0.7, verbose=False):
+    def macbert_correct(self, text, threshold=0.7, verbose=False, maxlen=128):
         """
         句子纠错
         :param text: 句子文本
         :param threshold: 阈值
         :param verbose: 是否打印详细信息
         :return: corrected_text, list[list], [error_word, correct_word, begin_pos, end_pos]
         """
         text_new = ''
         details = []
         # 长句切分为短句
-        blocks = split_text_by_maxlen(text, maxlen=128)
+        blocks = split_text_by_maxlen(text, maxlen=maxlen)
         block_texts = [block[0] for block in blocks]
         inputs = self.tokenizer(block_texts, padding=True, return_tensors='pt').to(device)
         with torch.no_grad():
             outputs = self.model(**inputs)
 
-        for ids, (text, idx) in zip(outputs.logits, blocks):
+        for id, (ids, (text, idx)) in enumerate(zip(outputs.logits, blocks)):
             decode_tokens_new = self.tokenizer.decode(torch.argmax(ids, dim=-1), skip_special_tokens=True).split(' ')
-            decode_tokens_old = self.tokenizer.decode(inputs['input_ids'][idx], skip_special_tokens=True).split(' ')
+            decode_tokens_old = self.tokenizer.decode(inputs['input_ids'][id], skip_special_tokens=True).split(' ')
             if len(decode_tokens_new) != len(decode_tokens_old):
                 continue
             probs = torch.max(torch.softmax(ids, dim=-1), dim=-1)[0].cpu().numpy()
             decode_tokens = ''
             for i in range(len(decode_tokens_old)):
                 if probs[i + 1] >= threshold:
                     if verbose:
@@ -152,15 +152,15 @@
         '	部分优先权：',
         '实施其专利的行为（生产经营≠营利≠商业经营）',
         '实施,i can speak chinese, can i spea english. ? hello.',
         "我不唉“看 琅擤琊榜”",
     ]
     t1 = time.time()
     for sent in error_sentences:
-        corrected_sent, err = m.macbert_correct(sent, 0.6)
+        corrected_sent, err = m.macbert_correct(sent, 0.6, maxlen=8)
         print("original sentence:{} => {} err:{}".format(sent, corrected_sent, err))
     print('[single]spend time:', time.time() - t1)
     t2 = time.time()
     res = m.batch_macbert_correct(error_sentences)
     for sent, r in zip(error_sentences, res):
         print("original sentence:{} => {} err:{}".format(sent, r[0], r[1]))
     print('[batch]spend time:', time.time() - t2)
```

### Comparing `pycorrector-0.4.9/pycorrector/macbert/preprocess.py` & `pycorrector-0.5.0/pycorrector/macbert/preprocess.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/macbert/reader.py` & `pycorrector-0.5.0/pycorrector/macbert/reader.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/macbert/softmaskedbert4csc.py` & `pycorrector-0.5.0/pycorrector/macbert/softmaskedbert4csc.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/macbert/train.py` & `pycorrector-0.5.0/pycorrector/macbert/train.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/proper_corrector.py` & `pycorrector-0.5.0/pycorrector/proper_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/seq2seq/convseq2seq.py` & `pycorrector-0.5.0/pycorrector/seq2seq/convseq2seq.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/seq2seq/data_reader.py` & `pycorrector-0.5.0/pycorrector/seq2seq/data_reader.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/seq2seq/infer.py` & `pycorrector-0.5.0/pycorrector/seq2seq/infer.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/seq2seq/model_args.py` & `pycorrector-0.5.0/pycorrector/seq2seq/model_args.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/seq2seq/preprocess.py` & `pycorrector-0.5.0/pycorrector/seq2seq/preprocess.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/seq2seq/seq2seq.py` & `pycorrector-0.5.0/pycorrector/seq2seq/seq2seq.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/seq2seq/seq2seq_corrector.py` & `pycorrector-0.5.0/pycorrector/seq2seq/seq2seq_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/seq2seq/seq2seq_model.py` & `pycorrector-0.5.0/pycorrector/seq2seq/seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/seq2seq/seq2seq_utils.py` & `pycorrector-0.5.0/pycorrector/seq2seq/seq2seq_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/seq2seq/train.py` & `pycorrector-0.5.0/pycorrector/seq2seq/train.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/t5/copyt5_corrector_bak.py` & `pycorrector-0.5.0/pycorrector/t5/copyt5_corrector_bak.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/t5/infer.py` & `pycorrector-0.5.0/pycorrector/t5/infer.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/t5/t5_corrector.py` & `pycorrector-0.5.0/pycorrector/t5/t5_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/t5/train.py` & `pycorrector-0.5.0/pycorrector/t5/train.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/transformer/config.py` & `pycorrector-0.5.0/pycorrector/transformer/config.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/transformer/preprocess.py` & `pycorrector-0.5.0/pycorrector/transformer/preprocess.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/utils/eval.py` & `pycorrector-0.5.0/pycorrector/utils/eval.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/utils/get_file.py` & `pycorrector-0.5.0/pycorrector/utils/get_file.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/utils/io_utils.py` & `pycorrector-0.5.0/pycorrector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/utils/langconv.py` & `pycorrector-0.5.0/pycorrector/utils/langconv.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/utils/math_utils.py` & `pycorrector-0.5.0/pycorrector/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/utils/ngram_util.py` & `pycorrector-0.5.0/pycorrector/utils/ngram_util.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/utils/text_utils.py` & `pycorrector-0.5.0/pycorrector/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/utils/tokenizer.py` & `pycorrector-0.5.0/pycorrector/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector/utils/zh_wiki.py` & `pycorrector-0.5.0/pycorrector/utils/zh_wiki.py`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/pycorrector.egg-info/PKG-INFO` & `pycorrector-0.5.0/pycorrector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycorrector
-Version: 0.4.9
+Version: 0.5.0
 Summary: Chinese Text Error Corrector
 Home-page: https://github.com/shibing624/pycorrector
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: ![alt text](docs/pycorrector.png)
```

### Comparing `pycorrector-0.4.9/pycorrector.egg-info/SOURCES.txt` & `pycorrector-0.5.0/pycorrector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-0.4.9/setup.py` & `pycorrector-0.5.0/setup.py`

 * *Files identical despite different names*

