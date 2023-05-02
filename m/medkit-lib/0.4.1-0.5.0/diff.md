# Comparing `tmp/medkit_lib-0.4.1.tar.gz` & `tmp/medkit_lib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medkit_lib-0.4.1.tar", max compression
+gzip compressed data, was "medkit_lib-0.5.0.tar", max compression
```

## Comparing `medkit_lib-0.4.1.tar` & `medkit_lib-0.5.0.tar`

### file list

```diff
@@ -1,114 +1,121 @@
--rw-r--r--   0        0        0     1077 2023-03-23 15:19:08.254089 medkit_lib-0.4.1/LICENSE
--rw-r--r--   0        0        0     1098 2023-03-23 15:19:08.254089 medkit_lib-0.4.1/README.md
--rw-r--r--   0        0        0       63 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/__init__.py
--rw-r--r--   0        0        0       61 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/audio/__init__.py
--rw-r--r--   0        0        0      328 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/audio/preprocessing/__init__.py
--rw-r--r--   0        0        0     2236 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/audio/preprocessing/downmixer.py
--rw-r--r--   0        0        0     2460 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/audio/preprocessing/power_normalizer.py
--rw-r--r--   0        0        0     2332 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/audio/preprocessing/resampler.py
--rw-r--r--   0        0        0      446 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/audio/segmentation/__init__.py
--rw-r--r--   0        0        0     6370 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/audio/segmentation/pa_speaker_detector.py
--rw-r--r--   0        0        0     7254 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/audio/segmentation/webrtc_voice_detector.py
--rw-r--r--   0        0        0      762 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/audio/transcription/__init__.py
--rw-r--r--   0        0        0     7168 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/audio/transcription/doc_transcriber.py
--rw-r--r--   0        0        0     3657 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/audio/transcription/hf_transcriber_function.py
--rw-r--r--   0        0        0     4398 2023-03-23 15:19:08.258090 medkit_lib-0.4.1/medkit/audio/transcription/sb_transcriber_function.py
--rw-r--r--   0        0        0     4776 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/audio/transcription/transcribed_document.py
--rw-r--r--   0        0        0     1489 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/__init__.py
--rw-r--r--   0        0        0     9449 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/_prov_graph.py
--rw-r--r--   0        0        0     1200 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/annotation.py
--rw-r--r--   0        0        0     4523 2023-03-26 11:17:15.663942 medkit_lib-0.4.1/medkit/core/annotation_container.py
--rw-r--r--   0        0        0     2684 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/attribute.py
--rw-r--r--   0        0        0     2907 2023-03-26 11:17:15.663942 medkit_lib-0.4.1/medkit/core/attribute_container.py
--rw-r--r--   0        0        0      514 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/audio/__init__.py
--rw-r--r--   0        0        0     3718 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/audio/annotation.py
--rw-r--r--   0        0        0     1534 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/audio/annotation_container.py
--rw-r--r--   0        0        0    10898 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/audio/audio_buffer.py
--rw-r--r--   0        0        0     4016 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/audio/document.py
--rw-r--r--   0        0        0      963 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/audio/operation.py
--rw-r--r--   0        0        0      973 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/audio/span.py
--rw-r--r--   0        0        0     1750 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/collection.py
--rw-r--r--   0        0        0      575 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/conversion.py
--rw-r--r--   0        0        0      475 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/data_item.py
--rw-r--r--   0        0        0     4719 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/dict_conv.py
--rw-r--r--   0        0        0     3951 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/doc_pipeline.py
--rw-r--r--   0        0        0      825 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/document.py
--rw-r--r--   0        0        0       96 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/id.py
--rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/operation.py
--rw-r--r--   0        0        0     1042 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/operation_desc.py
--rw-r--r--   0        0        0    13044 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/pipeline.py
--rw-r--r--   0        0        0     1470 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/prov_store.py
--rw-r--r--   0        0        0    10886 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/prov_tracer.py
--rw-r--r--   0        0        0     2396 2023-03-23 15:19:08.262090 medkit_lib-0.4.1/medkit/core/store.py
--rw-r--r--   0        0        0      883 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/core/text/__init__.py
--rw-r--r--   0        0        0     8691 2023-03-26 11:17:15.663942 medkit_lib-0.4.1/medkit/core/text/annotation.py
--rw-r--r--   0        0        0     5316 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/core/text/annotation_container.py
--rw-r--r--   0        0        0     4854 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/core/text/document.py
--rw-r--r--   0        0        0     1334 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/core/text/entity_attribute_container.py
--rw-r--r--   0        0        0     3235 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/core/text/entity_norm_attribute.py
--rw-r--r--   0        0        0     6471 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/core/text/operation.py
--rw-r--r--   0        0        0     3147 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/core/text/span.py
--rw-r--r--   0        0        0    18208 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/core/text/span_utils.py
--rw-r--r--   0        0        0    11691 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/core/text/utils.py
--rw-r--r--   0        0        0     1462 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/core/utils.py
--rw-r--r--   0        0        0      566 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/io/__init__.py
--rw-r--r--   0        0        0    16195 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/io/_brat_utils.py
--rw-r--r--   0        0        0    21158 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/io/brat.py
--rw-r--r--   0        0        0      649 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/io/medkit_json/__init__.py
--rw-r--r--   0        0        0     1235 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/io/medkit_json/_common.py
--rw-r--r--   0        0        0     5506 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/io/medkit_json/audio.py
--rw-r--r--   0        0        0     5496 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/io/medkit_json/text.py
--rw-r--r--   0        0        0    12123 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/io/rttm.py
--rw-r--r--   0        0        0     7603 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/io/spacy.py
--rw-r--r--   0        0        0      152 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/text/__init__.py
--rw-r--r--   0        0        0      590 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/text/context/__init__.py
--rw-r--r--   0        0        0     8982 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/text/context/family_detector.py
--rw-r--r--   0        0        0      790 2023-03-23 15:19:08.266090 medkit_lib-0.4.1/medkit/text/context/family_detector_default_rules.yml
--rw-r--r--   0        0        0    13939 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/context/hypothesis_detector.py
--rw-r--r--   0        0        0      905 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/context/hypothesis_detector_example_rules.yml
--rw-r--r--   0        0        0   307270 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/context/hypothesis_detector_example_verbs.yml
--rw-r--r--   0        0        0     8988 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/context/negation_detector.py
--rw-r--r--   0        0        0     4101 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/context/negation_detector_default_rules.yml
--rw-r--r--   0        0        0     1231 2023-03-28 14:12:23.614288 medkit_lib-0.4.1/medkit/text/ner/__init__.py
--rw-r--r--   0        0        0     5501 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/ner/duckling_matcher.py
--rw-r--r--   0        0        0     5568 2023-03-28 14:12:23.618289 medkit_lib-0.4.1/medkit/text/ner/hf_entity_matcher.py
--rw-r--r--   0        0        0    12758 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/ner/quick_umls_matcher.py
--rw-r--r--   0        0        0    12642 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/ner/regexp_matcher.py
--rw-r--r--   0        0        0    22942 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/ner/regexp_matcher_default_rules.yml
--rw-r--r--   0        0        0    16917 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/ner/umls_coder_normalizer.py
--rw-r--r--   0        0        0     2744 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/ner/umls_norm_attribute.py
--rw-r--r--   0        0        0     5468 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/ner/umls_semgroups_v04.txt
--rw-r--r--   0        0        0     4365 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/ner/umls_utils.py
--rw-r--r--   0        0        0       89 2023-03-23 15:19:08.270090 medkit_lib-0.4.1/medkit/text/postprocessing/__init__.py
--rw-r--r--   0        0        0     3302 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/postprocessing/attribute_duplicator.py
--rw-r--r--   0        0        0     2953 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/preprocessing/__init__.py
--rw-r--r--   0        0        0     5393 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/preprocessing/eds_cleaner.py
--rw-r--r--   0        0        0     3157 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/preprocessing/normalizer.py
--rw-r--r--   0        0        0      476 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/relations/__init__.py
--rw-r--r--   0        0        0     9469 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/relations/syntactic_relation_extractor.py
--rw-r--r--   0        0        0      667 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/segmentation/__init__.py
--rw-r--r--   0        0        0    13452 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/segmentation/default_section_definition.yml
--rw-r--r--   0        0        0      389 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/segmentation/default_syntagma_definition.yml
--rw-r--r--   0        0        0     3567 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/segmentation/rush_sentence_tokenizer.py
--rw-r--r--   0        0        0    23436 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv
--rw-r--r--   0        0        0     6557 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/segmentation/section_tokenizer.py
--rw-r--r--   0        0        0     4687 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/segmentation/sentence_tokenizer.py
--rw-r--r--   0        0        0     4655 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/segmentation/syntagma_tokenizer.py
--rw-r--r--   0        0        0      454 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/spacy/__init__.py
--rw-r--r--   0        0        0     4203 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/spacy/displacy_utils.py
--rw-r--r--   0        0        0     5142 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/spacy/doc_pipeline.py
--rw-r--r--   0        0        0     4518 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/spacy/pipeline.py
--rw-r--r--   0        0        0    16971 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/spacy/spacy_utils.py
--rw-r--r--   0        0        0      434 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/translation/__init__.py
--rw-r--r--   0        0        0    15325 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/text/translation/hf_translator.py
--rw-r--r--   0        0        0      312 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/tools/__init__.py
--rw-r--r--   0        0        0     1049 2023-03-23 15:19:08.274090 medkit_lib-0.4.1/medkit/tools/hf_utils.py
--rw-r--r--   0        0        0     5443 2023-03-23 15:19:08.278091 medkit_lib-0.4.1/medkit/tools/save_prov_to_dot.py
--rw-r--r--   0        0        0      615 2023-03-28 14:12:23.618289 medkit_lib-0.4.1/medkit/training/__init__.py
--rw-r--r--   0        0        0     3822 2023-03-23 15:19:08.278091 medkit_lib-0.4.1/medkit/training/callbacks.py
--rw-r--r--   0        0        0     2598 2023-03-28 14:12:23.618289 medkit_lib-0.4.1/medkit/training/trainable_operation.py
--rw-r--r--   0        0        0    11650 2023-03-28 14:12:23.618289 medkit_lib-0.4.1/medkit/training/trainer.py
--rw-r--r--   0        0        0      755 2023-03-23 15:19:08.278091 medkit_lib-0.4.1/medkit/training/trainer_config.py
--rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.278091 medkit_lib-0.4.1/medkit/training/utils.py
--rw-r--r--   0        0        0     3562 2023-03-28 14:40:23.151807 medkit_lib-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4638 1970-01-01 00:00:00.000000 medkit_lib-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-23 15:19:08.254089 medkit_lib-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1098 2023-03-23 15:19:08.254089 medkit_lib-0.5.0/README.md
+-rw-r--r--   0        0        0      173 2023-04-04 06:31:49.436370 medkit_lib-0.5.0/medkit/__init__.py
+-rw-r--r--   0        0        0       61 2023-03-23 15:19:08.258090 medkit_lib-0.5.0/medkit/audio/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-04 06:31:49.436370 medkit_lib-0.5.0/medkit/audio/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2236 2023-03-23 15:19:08.258090 medkit_lib-0.5.0/medkit/audio/preprocessing/downmixer.py
+-rw-r--r--   0        0        0     2460 2023-03-23 15:19:08.258090 medkit_lib-0.5.0/medkit/audio/preprocessing/power_normalizer.py
+-rw-r--r--   0        0        0     2482 2023-04-21 12:33:02.946744 medkit_lib-0.5.0/medkit/audio/preprocessing/resampler.py
+-rw-r--r--   0        0        0      250 2023-04-04 06:31:49.440370 medkit_lib-0.5.0/medkit/audio/segmentation/__init__.py
+-rw-r--r--   0        0        0     6530 2023-04-21 12:33:02.946744 medkit_lib-0.5.0/medkit/audio/segmentation/pa_speaker_detector.py
+-rw-r--r--   0        0        0     7416 2023-04-21 12:33:02.946744 medkit_lib-0.5.0/medkit/audio/segmentation/webrtc_voice_detector.py
+-rw-r--r--   0        0        0      554 2023-04-04 06:31:49.460371 medkit_lib-0.5.0/medkit/audio/transcription/__init__.py
+-rw-r--r--   0        0        0     7168 2023-03-23 15:19:08.258090 medkit_lib-0.5.0/medkit/audio/transcription/doc_transcriber.py
+-rw-r--r--   0        0        0     3821 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/audio/transcription/hf_transcriber_function.py
+-rw-r--r--   0        0        0     4562 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/audio/transcription/sb_transcriber_function.py
+-rw-r--r--   0        0        0     4776 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/audio/transcription/transcribed_document.py
+-rw-r--r--   0        0        0     1489 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/__init__.py
+-rw-r--r--   0        0        0     7827 2023-04-20 16:18:05.215523 medkit_lib-0.5.0/medkit/core/_prov_graph.py
+-rw-r--r--   0        0        0     1200 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/annotation.py
+-rw-r--r--   0        0        0     4665 2023-03-28 15:25:00.537196 medkit_lib-0.5.0/medkit/core/annotation_container.py
+-rw-r--r--   0        0        0     2969 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/core/attribute.py
+-rw-r--r--   0        0        0     3052 2023-03-28 15:25:00.537196 medkit_lib-0.5.0/medkit/core/attribute_container.py
+-rw-r--r--   0        0        0      514 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/__init__.py
+-rw-r--r--   0        0        0     3718 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/annotation.py
+-rw-r--r--   0        0        0     1534 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/annotation_container.py
+-rw-r--r--   0        0        0    10898 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/audio_buffer.py
+-rw-r--r--   0        0        0     4016 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/document.py
+-rw-r--r--   0        0        0      963 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/operation.py
+-rw-r--r--   0        0        0      973 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/audio/span.py
+-rw-r--r--   0        0        0     1750 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/collection.py
+-rw-r--r--   0        0        0      575 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/conversion.py
+-rw-r--r--   0        0        0      475 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/data_item.py
+-rw-r--r--   0        0        0     4719 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/dict_conv.py
+-rw-r--r--   0        0        0     3951 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/doc_pipeline.py
+-rw-r--r--   0        0        0      825 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/document.py
+-rw-r--r--   0        0        0       96 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/id.py
+-rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/operation.py
+-rw-r--r--   0        0        0     1042 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/operation_desc.py
+-rw-r--r--   0        0        0    13044 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/pipeline.py
+-rw-r--r--   0        0        0     1470 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/prov_store.py
+-rw-r--r--   0        0        0    10886 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/prov_tracer.py
+-rw-r--r--   0        0        0     2396 2023-03-23 15:19:08.262090 medkit_lib-0.5.0/medkit/core/store.py
+-rw-r--r--   0        0        0      883 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/__init__.py
+-rw-r--r--   0        0        0     8728 2023-04-04 06:31:49.484372 medkit_lib-0.5.0/medkit/core/text/annotation.py
+-rw-r--r--   0        0        0     5316 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/annotation_container.py
+-rw-r--r--   0        0        0     4854 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/document.py
+-rw-r--r--   0        0        0     1334 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/entity_attribute_container.py
+-rw-r--r--   0        0        0     3244 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/core/text/entity_norm_attribute.py
+-rw-r--r--   0        0        0     6471 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/operation.py
+-rw-r--r--   0        0        0     3147 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/span.py
+-rw-r--r--   0        0        0    18208 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/span_utils.py
+-rw-r--r--   0        0        0    11691 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/text/utils.py
+-rw-r--r--   0        0        0     1462 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/core/utils.py
+-rw-r--r--   0        0        0      401 2023-04-04 06:31:49.484372 medkit_lib-0.5.0/medkit/io/__init__.py
+-rw-r--r--   0        0        0    16195 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/io/_brat_utils.py
+-rw-r--r--   0        0        0    21166 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/io/brat.py
+-rw-r--r--   0        0        0      649 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/io/medkit_json/__init__.py
+-rw-r--r--   0        0        0     1235 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/io/medkit_json/_common.py
+-rw-r--r--   0        0        0     5506 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/io/medkit_json/audio.py
+-rw-r--r--   0        0        0     5496 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/io/medkit_json/text.py
+-rw-r--r--   0        0        0    12123 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/io/rttm.py
+-rw-r--r--   0        0        0     7750 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/io/spacy.py
+-rw-r--r--   0        0        0      152 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/text/__init__.py
+-rw-r--r--   0        0        0      590 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/text/context/__init__.py
+-rw-r--r--   0        0        0     9128 2023-04-20 16:18:05.219523 medkit_lib-0.5.0/medkit/text/context/family_detector.py
+-rw-r--r--   0        0        0      790 2023-03-23 15:19:08.266090 medkit_lib-0.5.0/medkit/text/context/family_detector_default_rules.yml
+-rw-r--r--   0        0        0    14243 2023-04-20 16:18:05.219523 medkit_lib-0.5.0/medkit/text/context/hypothesis_detector.py
+-rw-r--r--   0        0        0      905 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/context/hypothesis_detector_example_rules.yml
+-rw-r--r--   0        0        0   307270 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/context/hypothesis_detector_example_verbs.yml
+-rw-r--r--   0        0        0     9134 2023-04-20 16:18:05.219523 medkit_lib-0.5.0/medkit/text/context/negation_detector.py
+-rw-r--r--   0        0        0     4101 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/context/negation_detector_default_rules.yml
+-rw-r--r--   0        0        0     1320 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/ner/__init__.py
+-rw-r--r--   0        0        0     3795 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/ner/adicap_norm_attribute.py
+-rw-r--r--   0        0        0    11470 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/ner/date_attribute.py
+-rw-r--r--   0        0        0     5527 2023-04-20 16:18:05.219523 medkit_lib-0.5.0/medkit/text/ner/duckling_matcher.py
+-rw-r--r--   0        0        0     6534 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/ner/hf_entity_matcher.py
+-rw-r--r--   0        0        0     8109 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/ner/hf_entity_matcher_trainable.py
+-rw-r--r--   0        0        0     6396 2023-04-20 16:18:05.219523 medkit_lib-0.5.0/medkit/text/ner/hf_tokenization_utils.py
+-rw-r--r--   0        0        0     5215 2023-04-04 06:31:49.488372 medkit_lib-0.5.0/medkit/text/ner/iamsystem_matcher.py
+-rw-r--r--   0        0        0    12917 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/ner/quick_umls_matcher.py
+-rw-r--r--   0        0        0    12788 2023-04-20 16:18:05.219523 medkit_lib-0.5.0/medkit/text/ner/regexp_matcher.py
+-rw-r--r--   0        0        0    22942 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/ner/regexp_matcher_default_rules.yml
+-rw-r--r--   0        0        0     5154 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/ner/tnm_attribute.py
+-rw-r--r--   0        0        0    17079 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/ner/umls_coder_normalizer.py
+-rw-r--r--   0        0        0     2791 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/ner/umls_norm_attribute.py
+-rw-r--r--   0        0        0     5468 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/ner/umls_semgroups_v04.txt
+-rw-r--r--   0        0        0     4365 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/ner/umls_utils.py
+-rw-r--r--   0        0        0       89 2023-03-23 15:19:08.270090 medkit_lib-0.5.0/medkit/text/postprocessing/__init__.py
+-rw-r--r--   0        0        0     3302 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/postprocessing/attribute_duplicator.py
+-rw-r--r--   0        0        0     2953 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/preprocessing/__init__.py
+-rw-r--r--   0        0        0     5393 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/preprocessing/eds_cleaner.py
+-rw-r--r--   0        0        0     3157 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/preprocessing/normalizer.py
+-rw-r--r--   0        0        0      202 2023-04-04 06:31:49.492373 medkit_lib-0.5.0/medkit/text/relations/__init__.py
+-rw-r--r--   0        0        0     9639 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/relations/syntactic_relation_extractor.py
+-rw-r--r--   0        0        0      404 2023-04-04 06:31:49.496373 medkit_lib-0.5.0/medkit/text/segmentation/__init__.py
+-rw-r--r--   0        0        0    13452 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/segmentation/default_section_definition.yml
+-rw-r--r--   0        0        0      389 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/segmentation/default_syntagma_definition.yml
+-rw-r--r--   0        0        0     3731 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/segmentation/rush_sentence_tokenizer.py
+-rw-r--r--   0        0        0    23436 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv
+-rw-r--r--   0        0        0     6800 2023-04-20 16:18:05.223523 medkit_lib-0.5.0/medkit/text/segmentation/section_tokenizer.py
+-rw-r--r--   0        0        0     4765 2023-04-05 07:40:19.924515 medkit_lib-0.5.0/medkit/text/segmentation/sentence_tokenizer.py
+-rw-r--r--   0        0        0     4876 2023-04-20 16:18:05.223523 medkit_lib-0.5.0/medkit/text/segmentation/syntagma_tokenizer.py
+-rw-r--r--   0        0        0      669 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/spacy/__init__.py
+-rw-r--r--   0        0        0     4203 2023-03-23 15:19:08.274090 medkit_lib-0.5.0/medkit/text/spacy/displacy_utils.py
+-rw-r--r--   0        0        0     5765 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/spacy/doc_pipeline.py
+-rw-r--r--   0        0        0    15636 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/spacy/edsnlp.py
+-rw-r--r--   0        0        0     5136 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/spacy/pipeline.py
+-rw-r--r--   0        0        0    18167 2023-04-21 08:20:44.049464 medkit_lib-0.5.0/medkit/text/spacy/spacy_utils.py
+-rw-r--r--   0        0        0      180 2023-04-04 06:31:49.500373 medkit_lib-0.5.0/medkit/text/translation/__init__.py
+-rw-r--r--   0        0        0    15478 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/text/translation/hf_translator.py
+-rw-r--r--   0        0        0      204 2023-04-04 06:31:49.552376 medkit_lib-0.5.0/medkit/tools/__init__.py
+-rw-r--r--   0        0        0     1198 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/tools/hf_utils.py
+-rw-r--r--   0        0        0     5443 2023-03-23 15:19:08.278091 medkit_lib-0.5.0/medkit/tools/save_prov_to_dot.py
+-rw-r--r--   0        0        0      765 2023-04-21 12:33:02.950744 medkit_lib-0.5.0/medkit/training/__init__.py
+-rw-r--r--   0        0        0     3822 2023-03-23 15:19:08.278091 medkit_lib-0.5.0/medkit/training/callbacks.py
+-rw-r--r--   0        0        0     1987 2023-04-20 16:18:05.231523 medkit_lib-0.5.0/medkit/training/trainable_component.py
+-rw-r--r--   0        0        0    11628 2023-04-20 16:18:05.231523 medkit_lib-0.5.0/medkit/training/trainer.py
+-rw-r--r--   0        0        0      755 2023-03-23 15:19:08.278091 medkit_lib-0.5.0/medkit/training/trainer_config.py
+-rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.278091 medkit_lib-0.5.0/medkit/training/utils.py
+-rw-r--r--   0        0        0     3764 2023-05-02 15:41:31.551957 medkit_lib-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4879 1970-01-01 00:00:00.000000 medkit_lib-0.5.0/PKG-INFO
```

### Comparing `medkit_lib-0.4.1/LICENSE` & `medkit_lib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/README.md` & `medkit_lib-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/audio/preprocessing/downmixer.py` & `medkit_lib-0.5.0/medkit/audio/preprocessing/downmixer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/audio/preprocessing/power_normalizer.py` & `medkit_lib-0.5.0/medkit/audio/preprocessing/power_normalizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/audio/preprocessing/resampler.py` & `medkit_lib-0.5.0/medkit/audio/preprocessing/resampler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[resampler]`.
+"""
+
 __all__ = ["Resampler"]
 
 from typing import List, Optional
 
 import resampy
 
 from medkit.core.audio import PreprocessingOperation, Segment, MemoryAudioBuffer
```

### Comparing `medkit_lib-0.4.1/medkit/audio/segmentation/pa_speaker_detector.py` & `medkit_lib-0.5.0/medkit/audio/segmentation/pa_speaker_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[pa-speaker-detector]`.
+"""
+
 __all__ = ["PASpeakerDetector"]
 
 from pathlib import Path
 from typing import Dict, Iterator, List, Optional, Union
 from typing_extensions import Literal
 
 # When pyannote and spacy are both installed, a conflict might occur between the
```

### Comparing `medkit_lib-0.4.1/medkit/audio/segmentation/webrtc_voice_detector.py` & `medkit_lib-0.5.0/medkit/audio/segmentation/webrtc_voice_detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[webrtc-voice-detector]`.
+"""
+
 __all__ = ["WebRTCVoiceDetector"]
 
 import collections
 from typing import Iterator, List, Optional
 from typing_extensions import Literal
 
 import numpy as np
```

### Comparing `medkit_lib-0.4.1/medkit/audio/transcription/__init__.py` & `medkit_lib-0.5.0/medkit/audio/transcription/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,11 @@
     DocTranscriber,
     TranscriberFunction,
     TranscriberFunctionDescription,
 )
 from .transcribed_document import TranscribedDocument
 
 if modules_are_available(["torchaudio", "transformers"]):
-    # fmt: off
-    from .hf_transcriber_function import HFTranscriberFunction  # noqa: F401
-    __all__.append("HFTranscriberFunction")
-    # fmt: on
+    __all__.append("hf_transcriber_function")
 
 if modules_are_available(["torch", "speechbrain"]):
-    # fmt: off
-    from .sb_transcriber_function import SBTranscriberFunction  # noqa: F401
-    __all__.append("SBTranscriberFunction")
-    # fmt: on
+    __all__.append("sb_transcriber_function")
```

### Comparing `medkit_lib-0.4.1/medkit/audio/transcription/doc_transcriber.py` & `medkit_lib-0.5.0/medkit/audio/transcription/doc_transcriber.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/audio/transcription/hf_transcriber_function.py` & `medkit_lib-0.5.0/medkit/audio/transcription/hf_transcriber_function.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[hf-transcriber_function]`.
+"""
+
 __all__ = ["HFTranscriberFunction"]
 
 from pathlib import Path
 from typing import List, Optional, Union
 
 import transformers
 from transformers import AutomaticSpeechRecognitionPipeline
```

### Comparing `medkit_lib-0.4.1/medkit/audio/transcription/sb_transcriber_function.py` & `medkit_lib-0.5.0/medkit/audio/transcription/sb_transcriber_function.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[sb-transcriber_function]`.
+"""
+
 __all__ = ["SBTranscriberFunction"]
 
 from pathlib import Path
 from typing import List, Optional, Union
 
 import speechbrain as sb
```

### Comparing `medkit_lib-0.4.1/medkit/audio/transcription/transcribed_document.py` & `medkit_lib-0.5.0/medkit/audio/transcription/transcribed_document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/__init__.py` & `medkit_lib-0.5.0/medkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/_prov_graph.py` & `medkit_lib-0.5.0/medkit/core/_prov_graph.py`

 * *Files 20% similar despite different names*

```diff
@@ -140,58 +140,14 @@
         }
         merged_prov_graph._sub_graphs_by_op_id = {
             **self._sub_graphs_by_op_id,
             **other_graph._sub_graphs_by_op_id,
         }
         return merged_prov_graph
 
-    def flatten(self) -> ProvGraph:
-        flattened_graph = ProvGraph()
-
-        for node in self._nodes_by_id.values():
-            if node.operation_id not in self._sub_graphs_by_op_id:
-                flattened_graph._nodes_by_id[node.data_item_id] = node
-
-        for sub_graph in self._sub_graphs_by_op_id.values():
-            flattened_sub_graph = sub_graph.flatten()
-            flattened_graph._nodes_by_id.update(flattened_sub_graph._nodes_by_id)
-
-        return flattened_graph
-
-    # def prune(
-    #     self,
-    #     data_item_ids: List[str],
-    # ) -> ProvGraph:
-    #     assert all(uid in self._nodes_by_id for uid in data_item_ids)
-
-    #     ids_to_keep = []
-
-    #     queue = collections.deque(data_item_ids)
-    #     seen = set()
-    #     while queue:
-    #         data_item_id = queue.popleft()
-    #         seen.add(data_item_id)
-    #         node = self._nodes_by_id[data_item_id]
-    #         ids_to_keep.append(data_item_id)
-    #         queue.extend(uid for uid in node.source_ids if uid not in seen)
-
-    #     kept_nodes_by_id = []
-    #     for data_item_id in ids_to_keep:
-    #         node = self._nodes_by_id[data_item_id]
-    #         source_ids = [uid for uid in node.source_ids if uid in ids_to_keep]
-    #         # derived_ids = [uid for uid in node.derived_ids if uid in ids_to_keep]
-    #         pruned_node = dataclasses.replace(
-    #             node, source_ids=source_ids  # derived_ids=derived_ids
-    #         )
-    #         kept_nodes_by_id[data_item_id] = pruned_node
-
-    #     # TODO what about subgraphs?
-
-    #     return ProvGraph(kept_nodes_by_id)
-
     def check_sanity(self):
         for node_id, node in self._nodes_by_id.items():
             if node.source_ids and node.operation_id is None:
                 raise Exception(
                     f"Node with identifier {node_id} has source ids but no operation"
                 )
             for source_id in node.source_ids:
```

### Comparing `medkit_lib-0.4.1/medkit/core/annotation.py` & `medkit_lib-0.5.0/medkit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/annotation_container.py` & `medkit_lib-0.5.0/medkit/core/annotation_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,7 +145,11 @@
         ann = self._store.get_data_item(uid)
         return typing.cast(AnnotationType, ann)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, self.__class__):
             return False
         return self.get() == other.get()
+
+    def __repr__(self) -> str:
+        anns = self.get()
+        return f"{self.__class__.__name__}(doc_id={self._doc_id!r}, anns={anns!r})"
```

### Comparing `medkit_lib-0.4.1/medkit/core/attribute.py` & `medkit_lib-0.5.0/medkit/core/attribute.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,28 @@
             label=self.label,
             value=self.value,
             metadata=self.metadata,
         )
         dict_conv.add_class_name_to_data_dict(self, attribute_dict)
         return attribute_dict
 
+    def to_brat(self) -> Optional[Any]:
+        """
+        Return a value compatible with the brat format
+        """
+
+        return self.value
+
+    def to_spacy(self) -> Optional[Any]:
+        """
+        Return a value compatible with spaCy
+        """
+
+        return self.value
+
     def copy(self) -> Attribute:
         """
         Create a new attribute that is a copy of the current instance, but
         with a new identifier
 
         This is used when we want to duplicate an existing attribute onto a
         different annotation.
```

### Comparing `medkit_lib-0.4.1/medkit/core/attribute_container.py` & `medkit_lib-0.5.0/medkit/core/attribute_container.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,7 +88,11 @@
         attr = self._store.get_data_item(uid)
         return typing.cast(Attribute, attr)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, self.__class__):
             return False
         return self.get() == other.get()
+
+    def __repr__(self) -> str:
+        attrs = self.get()
+        return f"{self.__class__.__name__}(ann_id={self._ann_id!r}, attrs={attrs!r})"
```

### Comparing `medkit_lib-0.4.1/medkit/core/audio/__init__.py` & `medkit_lib-0.5.0/medkit/core/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/audio/annotation.py` & `medkit_lib-0.5.0/medkit/core/audio/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/audio/annotation_container.py` & `medkit_lib-0.5.0/medkit/core/audio/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/audio/audio_buffer.py` & `medkit_lib-0.5.0/medkit/core/audio/audio_buffer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/audio/document.py` & `medkit_lib-0.5.0/medkit/core/audio/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/audio/operation.py` & `medkit_lib-0.5.0/medkit/core/audio/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/audio/span.py` & `medkit_lib-0.5.0/medkit/core/audio/span.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/collection.py` & `medkit_lib-0.5.0/medkit/core/collection.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/conversion.py` & `medkit_lib-0.5.0/medkit/core/conversion.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/dict_conv.py` & `medkit_lib-0.5.0/medkit/core/dict_conv.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/doc_pipeline.py` & `medkit_lib-0.5.0/medkit/core/doc_pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/document.py` & `medkit_lib-0.5.0/medkit/core/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/operation.py` & `medkit_lib-0.5.0/medkit/core/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/operation_desc.py` & `medkit_lib-0.5.0/medkit/core/operation_desc.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/pipeline.py` & `medkit_lib-0.5.0/medkit/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/prov_store.py` & `medkit_lib-0.5.0/medkit/core/prov_store.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/prov_tracer.py` & `medkit_lib-0.5.0/medkit/core/prov_tracer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/store.py` & `medkit_lib-0.5.0/medkit/core/store.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/text/__init__.py` & `medkit_lib-0.5.0/medkit/core/text/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/text/annotation.py` & `medkit_lib-0.5.0/medkit/core/text/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     def to_dict(self) -> Dict[str, Any]:
         raise NotImplementedError()
 
 
 @dataclasses.dataclass(init=False)
 class Segment(TextAnnotation):
     """
-    Text segment referencing part of an {class}`~medkit.core.text.TextDocument`.
+    Text segment referencing part of an :class:`~medkit.core.text.TextDocument`.
 
     Attributes
     ----------
     uid:
         The segment identifier.
     label:
         The label for this segment (e.g., SENTENCE)
@@ -180,15 +180,15 @@
             metadata=segment_dict["metadata"],
         )
 
 
 @dataclasses.dataclass(init=False)
 class Entity(Segment):
     """
-    Text entity referencing part of an {class}`~medkit.core.text.TextDocument`.
+    Text entity referencing part of an :class:`~medkit.core.text.TextDocument`.
 
     Attributes
     ----------
     uid:
         The entity identifier.
     label:
         The label for this entity (e.g., DISEASE)
@@ -203,14 +203,16 @@
         init.
     metadata:
         The metadata of the entity
     keys:
         Pipeline output keys to which the entity belongs to.
     """
 
+    attrs: EntityAttributeContainer
+
     def __init__(
         self,
         label: str,
         text: str,
         spans: List[AnySpan],
         attrs: Optional[List[Attribute]] = None,
         metadata: Optional[Dict[str, Any]] = None,
```

### Comparing `medkit_lib-0.4.1/medkit/core/text/annotation_container.py` & `medkit_lib-0.5.0/medkit/core/text/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/text/document.py` & `medkit_lib-0.5.0/medkit/core/text/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/text/entity_attribute_container.py` & `medkit_lib-0.5.0/medkit/core/text/entity_attribute_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/text/entity_norm_attribute.py` & `medkit_lib-0.5.0/medkit/text/ner/umls_norm_attribute.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,101 @@
 from __future__ import annotations
 
-__all__ = ["EntityNormAttribute"]
+__all__ = ["UMLSNormAttribute"]
 
 import dataclasses
-from typing import Any, ClassVar, Dict, Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Self
 
 from medkit.core import dict_conv
-from medkit.core.attribute import Attribute
+from medkit.core.text import EntityNormAttribute
 
 
 @dataclasses.dataclass(init=False)
-class EntityNormAttribute(Attribute):
+class UMLSNormAttribute(EntityNormAttribute):
     """
-    Normalization attribute linking an entity to an ID in a knowledge base
+    Normalization attribute linking an entity to a CUI in the UMLS knowledge base
 
     Attributes
     ----------
     uid:
         Identifier of the attribute
     label:
-        The attribute label, always set to :attr:`EntityNormAttribute.LABEL`
+        The attribute label, always set to :attr:`EntityNormAttribute.LABEL
+        <.core.text.EntityNormAttribute.LABEL>`
     value:
-        Value of the attribute. Built by concatenating `kb_name` with `kb_id` when
-        available, otherwise `term` is used.
+        Value of the attribute, built by prefixing the cui with "umls:"
     kb_name:
-        Name of the knowledge base (ex: "icd"). Should always be provided except
-        in special cases when we just want to store a normalized term.
+        Name of the knowledge base. Always "umls"
     kb_id:
-        ID in the knowledge base to which the annotation should be linked.
-        Should always be provided except in special cases when we just want to
-        store a normalized term.
+        CUI (Concept Unique Identifier) to which the annotation should be linked
+    cui:
+        Convenience alias of `kb_id`
     kb_version:
-        Optional version of the knowledge base.
+        Version of the UMLS database (ex: "202AB")
+    umls_version:
+        Convenience alias of `kb_version`
     term:
-        Optional normalized version of the entity text.
+        Optional normalized version of the entity text
     score:
-        Optional score reflecting confidence of this link.
+        Optional score reflecting confidence of this link
+    sem_types:
+        Optional IDs of semantic types of the CUI (ex: ["T047"])
     metadata:
         Metadata of the attribute
     """
 
-    kb_name: Optional[str]
-    kb_id: Optional[Any]
-    kb_version: Optional[str]
-    term: Optional[str]
-    score: Optional[float]
-
-    LABEL: ClassVar[str] = "NORMALIZATION"
-    """
-    Label used for all normalization attributes
-    """
+    sem_types: Optional[List[str]] = None
 
     def __init__(
         self,
-        kb_name: Optional[str],
-        kb_id: Optional[Any],
-        kb_version: Optional[str] = None,
+        cui: str,
+        umls_version: str,
         term: Optional[str] = None,
         score: Optional[float] = None,
+        sem_types: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         uid: Optional[str] = None,
     ):
-        if kb_id is None and term is None:
-            raise ValueError("Must provide at least kb_id or term")
+        super().__init__(
+            kb_name="umls",
+            kb_id=cui,
+            kb_version=umls_version,
+            term=term,
+            score=score,
+            metadata=metadata,
+            uid=uid,
+        )
+        self.sem_types = sem_types
 
-        if kb_id is not None:
-            if kb_name is not None:
-                value = f"{kb_name}:{kb_id}"
-            else:
-                value = kb_id
-        else:
-            value = str(term)
-
-        super().__init__(label=self.LABEL, value=value, metadata=metadata, uid=uid)
-
-        self.kb_name = kb_name
-        self.kb_id = kb_id
-        self.kb_version = kb_version
-        self.term = term
-        self.score = score
+    @property
+    def cui(self):
+        return self.kb_id
+
+    @property
+    def umls_version(self):
+        return self.kb_version
 
     def to_dict(self) -> Dict[str, Any]:
         norm_dict = dict(
             uid=self.uid,
-            label=self.label,
-            kb_name=self.kb_name,
-            kb_id=self.kb_id,
-            kb_version=self.kb_version,
+            cui=self.cui,
+            umls_version=self.umls_version,
             term=self.term,
             score=self.score,
+            sem_types=self.sem_types,
             metadata=self.metadata,
         )
         dict_conv.add_class_name_to_data_dict(self, norm_dict)
         return norm_dict
 
     @classmethod
-    def from_dict(cls, data_dict: Dict[str, Any]) -> Self:
+    def from_dict(cls, data: Dict[str, Any]) -> Self:
         return cls(
-            uid=data_dict["uid"],
-            kb_name=data_dict["kb_name"],
-            kb_id=data_dict["kb_id"],
-            kb_version=data_dict["kb_version"],
-            term=data_dict["term"],
-            score=data_dict["score"],
-            metadata=data_dict["metadata"],
+            uid=data["uid"],
+            cui=data["cui"],
+            umls_version=data["umls_version"],
+            term=data["term"],
+            score=data["score"],
+            sem_types=data["sem_types"],
+            metadata=data["metadata"],
         )
```

### Comparing `medkit_lib-0.4.1/medkit/core/text/operation.py` & `medkit_lib-0.5.0/medkit/core/text/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/text/span.py` & `medkit_lib-0.5.0/medkit/core/text/span.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/text/span_utils.py` & `medkit_lib-0.5.0/medkit/core/text/span_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/text/utils.py` & `medkit_lib-0.5.0/medkit/core/text/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/core/utils.py` & `medkit_lib-0.5.0/medkit/core/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/io/_brat_utils.py` & `medkit_lib-0.5.0/medkit/io/_brat_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/io/brat.py` & `medkit_lib-0.5.0/medkit/io/brat.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,15 +414,15 @@
             else:
                 attrs = [
                     a
                     for label in self.attrs
                     for a in medkit_segment.attrs.get(label=label)
                 ]
             for attr in attrs:
-                value = attr.value
+                value = attr.to_brat()
 
                 if isinstance(value, bool) and not value:
                     # in brat 'False' means the attributes does not exist
                     continue
 
                 try:
                     brat_attr, attr_config = self._convert_attribute_to_brat(
@@ -458,15 +458,15 @@
             else:
                 attrs = [
                     a
                     for label in self.attrs
                     for a in medkit_relation.attrs.get(label=label)
                 ]
             for attr in attrs:
-                value = attr.value
+                value = attr.to_brat()
 
                 if isinstance(value, bool) and not value:
                     continue
 
                 try:
                     brat_attr, attr_config = self._convert_attribute_to_brat(
                         label=attr.label,
```

### Comparing `medkit_lib-0.4.1/medkit/io/medkit_json/__init__.py` & `medkit_lib-0.5.0/medkit/io/medkit_json/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/io/medkit_json/_common.py` & `medkit_lib-0.5.0/medkit/io/medkit_json/_common.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/io/medkit_json/audio.py` & `medkit_lib-0.5.0/medkit/io/medkit_json/audio.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/io/medkit_json/text.py` & `medkit_lib-0.5.0/medkit/io/medkit_json/text.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/io/rttm.py` & `medkit_lib-0.5.0/medkit/io/rttm.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/io/spacy.py` & `medkit_lib-0.5.0/medkit/io/spacy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[spacy]`.
+"""
+
+
 __all__ = ["SpacyInputConverter", "SpacyOutputConverter"]
 
 from typing import List, Optional
 
 from spacy import Language
 from spacy.tokens import Doc
```

### Comparing `medkit_lib-0.4.1/medkit/text/context/__init__.py` & `medkit_lib-0.5.0/medkit/text/context/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/context/family_detector.py` & `medkit_lib-0.5.0/medkit/text/context/family_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         """
         # Pass all arguments to super (remove self)
         init_args = locals()
         init_args.pop("self")
         super().__init__(**init_args)
 
         if rules is None:
-            rules = self.load_rules(_PATH_TO_DEFAULT_RULES)
+            rules = self.load_rules(_PATH_TO_DEFAULT_RULES, encoding="utf-8")
 
         self.check_rules_sanity(rules)
 
         self.output_label = output_label
         self.rules = rules
 
         # pre-compile patterns
@@ -210,32 +210,36 @@
                     # return the rule id or the rule index if no id has been set
                     rule_id = rule.id if rule.id is not None else rule_index
                     return rule_id
 
         return None
 
     @staticmethod
-    def load_rules(path_to_rules) -> List[FamilyDetectorRule]:
+    def load_rules(
+        path_to_rules: Path, encoding: Optional[str] = None
+    ) -> List[FamilyDetectorRule]:
         """
         Load all rules stored in a yml file
 
         Parameters
         ----------
-        path_to_rules:
+        path_to_rules
             Path to a yml file containing a list of mappings
             with the same structure as `FamilyDetectorRule`
+        encoding
+            Encoding of the file to open
 
         Returns
         -------
         List[FamilyDetectorRule]
             List of all the rules in `path_to_rules`,
             can be used to init a `FamilyDetector`
         """
 
-        with open(path_to_rules, mode="r") as f:
+        with open(path_to_rules, mode="r", encoding=encoding) as f:
             rules_data = yaml.safe_load(f)
         rules = [FamilyDetectorRule(**d) for d in rules_data]
         return rules
 
     @staticmethod
     def check_rules_sanity(rules: List[FamilyDetectorRule]):
         """Check consistency of a set of rules"""
```

### Comparing `medkit_lib-0.4.1/medkit/text/context/family_detector_default_rules.yml` & `medkit_lib-0.5.0/medkit/text/context/family_detector_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/context/hypothesis_detector.py` & `medkit_lib-0.5.0/medkit/text/context/hypothesis_detector.py`

 * *Files 5% similar despite different names*

```diff
@@ -300,66 +300,74 @@
                     # return the rule uid or the rule index if no uid has been set
                     rule_id = rule.id if rule.id is not None else rule_index
                     return rule_id
 
         return None
 
     @staticmethod
-    def load_verbs(path_to_verbs) -> Dict[str, Dict[str, Dict[str, List[str]]]]:
+    def load_verbs(
+        path_to_verbs: Path, encoding: Optional[str] = None
+    ) -> Dict[str, Dict[str, Dict[str, List[str]]]]:
         """
         Load all conjugated verb forms stored in a yml file.
         Conjugated verb forms at a specific mode and tense must be stored in nested mappings
         with the 1st key being the verb root, the 2d key the mode and the 3d key the tense.
 
         Parameters
         ----------
-        path_to_verbs:
+        path_to_verbs
             Path to a yml file containing a list of verbs form,
             arranged by mode and tense.
+        encoding:
+            Encoding on the file to open
 
         Returns
         -------
         List[Dict[str, Dict[str, List[str]]]]
             List of verb forms in `path_to_verbs`,
             can be used to init an `HypothesisDetector`
         """
-        with open(path_to_verbs) as f:
+        with open(path_to_verbs, mode="r", encoding=encoding) as f:
             verbs = yaml.safe_load(f)
         return verbs
 
     @staticmethod
-    def load_rules(path_to_rules) -> List[HypothesisDetectorRule]:
+    def load_rules(
+        path_to_rules: Path, encoding: Optional[str] = None
+    ) -> List[HypothesisDetectorRule]:
         """
         Load all rules stored in a yml file
 
         Parameters
         ----------
         path_to_rules:
             Path to a yml file containing a list of mappings
             with the same structure as `HypothesisDetectorRule`
+        encoding
+            Encoding of the file to open
 
         Returns
         -------
         List[HypothesisDetectorRule]
             List of all the rules in `path_to_rules`,
             can be used to init an `HypothesisDetector`
         """
 
-        with open(path_to_rules, mode="r") as f:
+        with open(path_to_rules, mode="r", encoding=encoding) as f:
             rules_data = yaml.safe_load(f)
         rules = [HypothesisDetectorRule(**d) for d in rules_data]
         return rules
 
     @classmethod
     def get_example(cls) -> HypothesisDetector:
         """Instantiate an HypothesisDetector with example rules and verbs,
         designed for usage with EDS documents
         """
-        rules = cls.load_rules(_PATH_TO_EXAMPLE_RULES)
-        verbs = cls.load_verbs(_PATH_TO_EXAMPLE_VERBS)
+        rules = cls.load_rules(_PATH_TO_EXAMPLE_RULES, encoding="utf-8")
+        verbs = cls.load_verbs(_PATH_TO_EXAMPLE_VERBS, encoding="utf-8")
         modes_and_tenses = [
             ("conditionnel", "présent"),
             ("indicatif", "futur simple"),
         ]
         return cls(rules=rules, verbs=verbs, modes_and_tenses=modes_and_tenses)
 
     @staticmethod
```

### Comparing `medkit_lib-0.4.1/medkit/text/context/hypothesis_detector_example_rules.yml` & `medkit_lib-0.5.0/medkit/text/context/hypothesis_detector_example_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/context/hypothesis_detector_example_verbs.yml` & `medkit_lib-0.5.0/medkit/text/context/hypothesis_detector_example_verbs.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/context/negation_detector.py` & `medkit_lib-0.5.0/medkit/text/context/negation_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         """
         # Pass all arguments to super (remove self)
         init_args = locals()
         init_args.pop("self")
         super().__init__(**init_args)
 
         if rules is None:
-            rules = self.load_rules(_PATH_TO_DEFAULT_RULES)
+            rules = self.load_rules(_PATH_TO_DEFAULT_RULES, encoding="utf-8")
 
         self.check_rules_sanity(rules)
 
         self.output_label = output_label
         self.rules = rules
 
         # pre-compile patterns
@@ -211,32 +211,36 @@
                     # return the rule uid or the rule index if no uid has been set
                     rule_id = rule.id if rule.id is not None else rule_index
                     return rule_id
 
         return None
 
     @staticmethod
-    def load_rules(path_to_rules) -> List[NegationDetectorRule]:
+    def load_rules(
+        path_to_rules: Path, encoding: Optional[str] = None
+    ) -> List[NegationDetectorRule]:
         """
         Load all rules stored in a yml file
 
         Parameters
         ----------
-        path_to_rules:
+        path_to_rules
             Path to a yml file containing a list of mappings
             with the same structure as `NegationDetectorRule`
+        encoding
+            Encoding of the file to open
 
         Returns
         -------
         List[NegationDetectorRule]
             List of all the rules in `path_to_rules`,
             can be used to init a `NegationDetector`
         """
 
-        with open(path_to_rules, mode="r") as f:
+        with open(path_to_rules, mode="r", encoding=encoding) as f:
             rules_data = yaml.safe_load(f)
         rules = [NegationDetectorRule(**d) for d in rules_data]
         return rules
 
     @staticmethod
     def check_rules_sanity(rules: List[NegationDetectorRule]):
         """Check consistency of a set of rules"""
```

### Comparing `medkit_lib-0.4.1/medkit/text/context/negation_detector_default_rules.yml` & `medkit_lib-0.5.0/medkit/text/context/negation_detector_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/ner/duckling_matcher.py` & `medkit_lib-0.5.0/medkit/text/ner/duckling_matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         if api_result.status_code != 200:
             raise ConnectionError(
                 "Request response not correct : status code {res.status_code}"
             )
 
         matches = api_result.json()
         for match in matches:
-            if match["dim"] not in self.dims:
+            if self.dims is not None and match["dim"] not in self.dims:
                 warnings.warn("Dims are not properly filtered by duckling API call")
                 continue
 
             text, spans = span_utils.extract(
                 segment.text, segment.spans, [(match["start"], match["end"])]
             )
```

### Comparing `medkit_lib-0.4.1/medkit/text/ner/hf_entity_matcher.py` & `medkit_lib-0.5.0/medkit/text/ner/hf_entity_matcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-__all__ = ["HFEntityMatcher"]
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[hf-entity-matcher]`.
+"""
 
+__all__ = ["HFEntityMatcher"]
 from pathlib import Path
 from typing import Dict, Iterator, List, Optional, Union
 from typing_extensions import Literal
 
 import transformers
 from transformers import TokenClassificationPipeline
 
 from medkit.core import Attribute
 from medkit.core.text import NEROperation, Segment, span_utils, Entity
+from medkit.text.ner.hf_entity_matcher_trainable import HFEntityMatcherTrainable
 from medkit.tools import hf_utils
 
 
 class HFEntityMatcher(NEROperation):
     """
     Entity matcher based on HuggingFace transformers model
 
@@ -67,24 +72,24 @@
 
         if attrs_to_copy is None:
             attrs_to_copy = []
 
         self.model = model
         self.attrs_to_copy = attrs_to_copy
 
-        if isinstance(self.model, str):
-            valid_model = hf_utils.check_model_for_task_HF(
-                self.model, "token-classification"
+        valid_model = hf_utils.check_model_for_task_HF(
+            self.model, "token-classification"
+        )
+
+        if not valid_model:
+            raise ValueError(
+                f"Model {self.model} is not associated to a"
+                " token-classification/ner task and cannot be used with"
+                " HFEntityMatcher"
             )
-            if not valid_model:
-                raise ValueError(
-                    f"Model {self.model} is not associated to a"
-                    " token-classification/ner task and cannot be used with"
-                    " HFEntityMatcher"
-                )
 
         self._pipeline = transformers.pipeline(
             task="token-classification",
             model=self.model,
             aggregation_strategy=aggregation_strategy,
             pipeline_class=TokenClassificationPipeline,
             device=device,
@@ -150,7 +155,30 @@
                     entity, self.description, source_data_items=[segment]
                 )
                 self._prov_tracer.add_prov(
                     score_attr, self.description, source_data_items=[segment]
                 )
 
             yield entity
+
+    @staticmethod
+    def make_trainable(
+        model_name_or_path: Union[str, Path],
+        labels: List[str],
+        tagging_scheme: Literal["bilou", "iob2"],
+        tag_subtokens: bool = False,
+        tokenizer_max_length: Optional[int] = None,
+        device: int = -1,
+    ):
+        """
+        Return the trainable component of the operation.
+        This component can be trained using :class:`~medkit.training.Trainer`, and then
+        used in a new `HFEntityMatcher` operation.
+        """
+        return HFEntityMatcherTrainable(
+            model_name_or_path=model_name_or_path,
+            labels=labels,
+            tagging_scheme=tagging_scheme,
+            tokenizer_max_length=tokenizer_max_length,
+            tag_subtokens=tag_subtokens,
+            device=device,
+        )
```

### Comparing `medkit_lib-0.4.1/medkit/text/ner/quick_umls_matcher.py` & `medkit_lib-0.5.0/medkit/text/ner/quick_umls_matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[quick-umls-matcher]`.
+"""
+
 __all__ = ["QuickUMLSMatcher"]
 
 from pathlib import Path
 from packaging.version import parse as parse_version
 from typing import Dict, Iterator, List, NamedTuple, Optional, Union
 from typing_extensions import Literal
```

### Comparing `medkit_lib-0.4.1/medkit/text/ner/regexp_matcher.py` & `medkit_lib-0.5.0/medkit/text/ner/regexp_matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         """
         # Pass all arguments to super (remove self)
         init_args = locals()
         init_args.pop("self")
         super().__init__(**init_args)
 
         if rules is None:
-            rules = self.load_rules(_PATH_TO_DEFAULT_RULES)
+            rules = self.load_rules(_PATH_TO_DEFAULT_RULES, encoding="utf-8")
         if attrs_to_copy is None:
             attrs_to_copy = []
 
         self.check_rules_sanity(rules)
 
         self.rules = rules
         self.attrs_to_copy = attrs_to_copy
@@ -312,23 +312,27 @@
         else:
             norm_attr = EntityNormAttribute(
                 kb_name=norm.kb_name, kb_id=norm.id, kb_version=norm.kb_version
             )
         return norm_attr
 
     @staticmethod
-    def load_rules(path_to_rules) -> List[RegexpMatcherRule]:
+    def load_rules(
+        path_to_rules: Path, encoding: Optional[str] = None
+    ) -> List[RegexpMatcherRule]:
         """
         Load all rules stored in a yml file
 
         Parameters
         ----------
-        path_to_rules:
+        path_to_rules
             Path to a yml file containing a list of mappings
             with the same structure as `RegexpMatcherRule`
+        encoding
+            Encoding of the file to open
 
         Returns
         -------
         List[RegexpMatcherRule]
             List of all the rules in `path_to_rules`,
             can be used to init a `RegexpMatcher`
         """
@@ -343,15 +347,15 @@
             else:
                 return RegexpMatcherRule(**data)
 
         Loader.add_constructor(
             yaml.resolver.BaseResolver.DEFAULT_MAPPING_TAG, construct_mapping
         )
 
-        with open(path_to_rules, mode="r") as f:
+        with open(path_to_rules, mode="r", encoding=encoding) as f:
             rules = yaml.load(f, Loader=Loader)
         return rules
 
     @staticmethod
     def check_rules_sanity(rules: List[RegexpMatcherRule]):
         """Check consistency of a set of rules"""
```

### Comparing `medkit_lib-0.4.1/medkit/text/ner/regexp_matcher_default_rules.yml` & `medkit_lib-0.5.0/medkit/text/ner/regexp_matcher_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/ner/umls_coder_normalizer.py` & `medkit_lib-0.5.0/medkit/text/ner/umls_coder_normalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[umls-coder-normalizer]`.
+"""
+
 __all__ = ["UMLSCoderNormalizer"]
 
 from typing import Any, Dict, List, NamedTuple, Optional, Tuple, Union
 from typing_extensions import Literal
 from pathlib import Path
 
 import pandas as pd
```

### Comparing `medkit_lib-0.4.1/medkit/text/ner/umls_semgroups_v04.txt` & `medkit_lib-0.5.0/medkit/text/ner/umls_semgroups_v04.txt`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/ner/umls_utils.py` & `medkit_lib-0.5.0/medkit/text/ner/umls_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/postprocessing/attribute_duplicator.py` & `medkit_lib-0.5.0/medkit/text/postprocessing/attribute_duplicator.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/preprocessing/__init__.py` & `medkit_lib-0.5.0/medkit/text/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/preprocessing/eds_cleaner.py` & `medkit_lib-0.5.0/medkit/text/preprocessing/eds_cleaner.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/preprocessing/normalizer.py` & `medkit_lib-0.5.0/medkit/text/preprocessing/normalizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/relations/syntactic_relation_extractor.py` & `medkit_lib-0.5.0/medkit/text/relations/syntactic_relation_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[syntactic-relation-extractor]`.
+"""
+
+
 __all__ = ["SyntacticRelationExtractor"]
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 import spacy
```

### Comparing `medkit_lib-0.4.1/medkit/text/segmentation/default_section_definition.yml` & `medkit_lib-0.5.0/medkit/text/segmentation/default_section_definition.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/segmentation/rush_sentence_tokenizer.py` & `medkit_lib-0.5.0/medkit/text/segmentation/rush_sentence_tokenizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[rush-sentence-tokenizer]`.
+"""
+
 from __future__ import annotations
 
 __all__ = ["RushSentenceTokenizer"]
 
 import dataclasses
 from pathlib import Path
 import re
```

### Comparing `medkit_lib-0.4.1/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv` & `medkit_lib-0.5.0/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/segmentation/section_tokenizer.py` & `medkit_lib-0.5.0/medkit/text/segmentation/section_tokenizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 import yaml
 
 from flashtext import KeywordProcessor
 
 from medkit.core.text import Segment, SegmentationOperation, span_utils
 
 
+_DEFAULT_SECTION_DEFINITION_RULES = (
+    pathlib.Path(__file__).parent / "default_section_definition.yml"
+)
+
+
 @dataclasses.dataclass(frozen=True)
 class DefaultConfig:
     output_label: str = "SECTION"
 
 
 @dataclasses.dataclass
 class SectionModificationRule:
@@ -148,45 +153,49 @@
                         map_index_new_name[candidate_index] = rule.new_section_name
                     candidate_sections.clear()
 
         return map_index_new_name
 
     @classmethod
     def get_example(cls):
-        config_path = pathlib.Path(__file__).parent / "default_section_definition.yml"
-        section_dict, section_rules = cls.load_section_definition(config_path)
+        config_path = _DEFAULT_SECTION_DEFINITION_RULES
+        section_dict, section_rules = cls.load_section_definition(
+            config_path, encoding="utf-8"
+        )
         section_tokenizer = cls(
             section_dict=section_dict,
             section_rules=section_rules,
         )
         return section_tokenizer
 
     @staticmethod
     def load_section_definition(
-        filepath,
+        filepath: pathlib.Path, encoding: Optional[str] = None
     ) -> Tuple[Dict[str, List[str]], Tuple[SectionModificationRule]]:
         """
         Load the sections definition stored in a yml file
 
         Parameters
         ----------
         filepath:
             Path to a yml file containing the sections(name + mappings) and rules
+        encoding:
+            Encoding of the file to open
 
         Returns
         -------
         Tuple[Dict[str, List[str]], Tuple[SectionModificationRule]]
             Tuple containing:
             - the dictionary where key is the section name and value is the list of all
             equivalent strings.
             - the list of section modification rules.
             These rules allow to rename some sections according their order
         """
 
-        with open(filepath, mode="r") as f:
+        with open(filepath, mode="r", encoding=encoding) as f:
             config = yaml.safe_load(f)
 
         section_dict = config["sections"]
         section_rules = tuple(
             SectionModificationRule(**rule) for rule in config["rules"]
         )
```

### Comparing `medkit_lib-0.4.1/medkit/text/segmentation/sentence_tokenizer.py` & `medkit_lib-0.5.0/medkit/text/segmentation/sentence_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,20 +103,21 @@
             for start, end in self._split_text(
                 segment.text, self._punct_pattern, keep_separator=self.keep_punct
             ):
                 yield self._build_sentence(segment, range=(start, end))
 
     @staticmethod
     def _split_text(
-        text: str, pattern: re.Match, keep_separator: bool
+        text: str, pattern: re.Pattern, keep_separator: bool
     ) -> Iterator[Tuple[int, int]]:
         for match in pattern.finditer(text):
             start = match.start("content")
             end = match.end("separator") if keep_separator else match.end("content")
-            if end > start:
+            has_letters = re.search(r"\w", text[start:end])
+            if end > start and has_letters:
                 yield start, end
 
     def _build_sentence(
         self, source_segment: Segment, range: Tuple[int, int]
     ) -> Segment:
         text, spans = span_utils.extract(
             text=source_segment.text,
```

### Comparing `medkit_lib-0.4.1/medkit/text/segmentation/syntagma_tokenizer.py` & `medkit_lib-0.5.0/medkit/text/segmentation/syntagma_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 import re
 from typing import Iterator, List, Optional, Tuple
 
 import yaml
 
 from medkit.core.text import Segment, SegmentationOperation, span_utils
 
+_DEFAULT_SYNTAGMA_DEFINITION_RULES = (
+    pathlib.Path(__file__).parent / "default_syntagma_definition.yml"
+)
+
 
 @dataclasses.dataclass
 class DefaultConfig:
     output_label = "SYNTAGMA"
     keep_separator = True
 
 
@@ -118,36 +122,38 @@
                     syntagma, self.description, source_data_items=[segment]
                 )
 
             yield syntagma
 
     @classmethod
     def get_example(cls, keep_separator=True):
-        config_path = pathlib.Path(__file__).parent / "default_syntagma_definition.yml"
-        separators = cls.load_syntagma_definition(config_path)
+        config_path = _DEFAULT_SYNTAGMA_DEFINITION_RULES
+        separators = cls.load_syntagma_definition(config_path, encoding="utf-8")
         syntagma_tokenizer = cls(separators=separators, keep_separator=keep_separator)
         return syntagma_tokenizer
 
     @staticmethod
     def load_syntagma_definition(
-        filepath,
+        filepath: pathlib.Path, encoding: Optional[str] = None
     ) -> Tuple[str, ...]:
         """
         Load the syntagma definition stored in yml file
 
         Parameters
         ----------
         filepath:
             Path to a yml file containing the syntagma separators
+        encoding
+            Encoding of the file to open
 
         Returns
         -------
         Tuple[str, ...]:
             Tuple containing the separators
         """
 
-        with open(filepath, mode="r") as f:
+        with open(filepath, mode="r", encoding=encoding) as f:
             config = yaml.safe_load(f)
 
         syntagma_seps = tuple(str(sep) for sep in config["syntagmas"]["separators"])
 
         return syntagma_seps
```

### Comparing `medkit_lib-0.4.1/medkit/text/spacy/displacy_utils.py` & `medkit_lib-0.5.0/medkit/text/spacy/displacy_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/text/spacy/doc_pipeline.py` & `medkit_lib-0.5.0/medkit/text/spacy/doc_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __all__ = ["SpacyDocPipeline"]
 
-from typing import List, Optional
+from typing import Callable, Dict, List, Optional
 
 from spacy import Language
+from spacy.tokens import Span as SpacySpan
 
-from medkit.core import DocOperation
+from medkit.core import DocOperation, Attribute
 from medkit.core.text import TextDocument
 from medkit.text.spacy import spacy_utils
 
 
 class SpacyDocPipeline(DocOperation):
     """DocPipeline to obtain annotations created using spacy"""
 
@@ -16,14 +17,17 @@
         self,
         nlp: Language,
         medkit_labels_anns: Optional[List[str]] = None,
         medkit_attrs: Optional[List[str]] = None,
         spacy_entities: Optional[List[str]] = None,
         spacy_span_groups: Optional[List[str]] = None,
         spacy_attrs: Optional[List[str]] = None,
+        medkit_attribute_factories: Optional[
+            Dict[str, Callable[[SpacySpan, str], Attribute]]
+        ] = None,
         name: Optional[str] = None,
         uid: Optional[str] = None,
     ):
         """Initialize the pipeline
 
         Parameters
         ----------
@@ -44,14 +48,19 @@
             Name of new spacy span groups (`doc.spans`) to convert into medkit segments.
             If `None` (default) new spacy span groups will be converted and added into
             its origin medkit document.
         spacy_attrs:
             Name of span extensions to convert into medkit attributes.
             If `None` (default) all non-None extensions will be added for each annotation with
             a medkit ID.
+        medkit_attribute_factories:
+            Mapping of factories in charge of converting spacy attributes to
+            medkit attributes. Factories will receive a spacy span and an an
+            attribute label when called. The key in the mapping is the attribute
+            label.
         name:
             Name describing the pipeline (defaults to the class name).
         uid:
             Identifier of the pipeline
 
         """
         # Pass all arguments to super (remove self)
@@ -61,14 +70,15 @@
 
         self.nlp = nlp
         self.medkit_labels_anns = medkit_labels_anns
         self.medkit_attrs = medkit_attrs
         self.spacy_entities = spacy_entities
         self.spacy_span_groups = spacy_span_groups
         self.spacy_attrs = spacy_attrs
+        self.medkit_attribute_factories = medkit_attribute_factories
 
     def run(self, medkit_docs: List[TextDocument]) -> None:
         """Run a spacy pipeline on a list of medkit documents.
         Each medkit document is converted to spacy document (Doc object),
         with the selected annotations and attributes. Then, the spacy pipeline
         is executed and finally, the new annotations and attributes are
         converted into medkit annotations.
@@ -96,14 +106,15 @@
 
             anns, attrs_by_ann_id = spacy_utils.extract_anns_and_attrs_from_spacy_doc(
                 spacy_doc=spacy_doc,
                 medkit_source_ann=raw_segment,
                 entities=self.spacy_entities,
                 span_groups=self.spacy_span_groups,
                 attrs=self.spacy_attrs,
+                attribute_factories=self.medkit_attribute_factories,
                 rebuild_medkit_anns_and_attrs=False,
             )
             # annotate
             # add new annotations
             for ann in anns:
                 medkit_doc.anns.add(ann)
                 if self._prov_tracer is not None:
```

### Comparing `medkit_lib-0.4.1/medkit/text/spacy/spacy_utils.py` & `medkit_lib-0.5.0/medkit/text/spacy/spacy_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = [
     "extract_anns_and_attrs_from_spacy_doc",
     "build_spacy_doc_from_medkit_doc",
     "build_spacy_doc_from_medkit_segment",
 ]
 import warnings
-from typing import Dict, List, Optional, Tuple
+from typing import Callable, Dict, List, Optional, Tuple
 
 from spacy import Language
 from spacy.tokens import Doc
 from spacy.tokens import Span as SpacySpan
 from spacy.tokens.underscore import Underscore
 from spacy.util import filter_spans
 
@@ -28,14 +28,17 @@
 
 def extract_anns_and_attrs_from_spacy_doc(
     spacy_doc: Doc,
     medkit_source_ann: Optional[Segment] = None,
     entities: Optional[List[str]] = None,
     span_groups: Optional[List[str]] = None,
     attrs: Optional[List[str]] = None,
+    attribute_factories: Optional[
+        Dict[str, Callable[[SpacySpan, str], Attribute]]
+    ] = None,
     rebuild_medkit_anns_and_attrs: bool = False,
 ) -> Tuple[List[Segment], Dict[str, List[Attribute]]]:
     """Given a spacy document, convert selected entities or spans into Segments.
     Extract attributes for each annotation in the document.
 
     Parameters
     ----------
@@ -48,14 +51,18 @@
         If `None` (default) all new entities will be extracted as annotations
     span_groups:
         Name of span groups to be extracted
         If `None` (default) all new spans will be extracted as annotations
     attrs:
         Name of custom attributes to extract from the annotations that will be included.
         If `None` (default) all the custom attributes will be extracted
+    attribute_factories:
+        Mapping of factories in charge of converting spacy attributes to medkit
+        attributes. Factories will receive a spacy span and an attribute label
+        when called. The key in the mapping is the attribute label.
     rebuild_medkit_anns_and_attrs:
         If True the annotations and attributes with medkit ids will become
         new annotations/attributes with new ids.
         If False (default) the annotations and attributes with medkit ids are not
         rebuilt, only new annotations and attributes are returned
 
     Returns
@@ -67,14 +74,17 @@
 
     Raises
     ------
     ValueError
         Raises when the given medkit source and the spacy doc do not have the same medkit uid
     """
 
+    if attribute_factories is None:
+        attribute_factories = {}
+
     # extensions to indicate the medkit origin
     _define_default_extensions()
     spacy_doc_medkit_id = spacy_doc._.get(_ATTR_MEDKIT_ID)
     if spacy_doc_medkit_id is not None:
         if (
             medkit_source_ann is not None
             and medkit_source_ann.uid != spacy_doc_medkit_id
@@ -107,26 +117,38 @@
 
             entity = Entity(label=label, spans=spans, text=text)
             medkit_id = entity.uid
             annotations.append(entity)
 
         # for each spacy extension having a value other than None,
         # a medkit Attribute is created
-        attributes = [
-            Attribute(label=attr, value=entity_spacy._.get(attr))
-            for attr in spacy_attrs
-            if entity_spacy._.get(attr) is not None
-        ]
+        attributes = []
+        for attr_label in spacy_attrs:
+            value = entity_spacy._.get(attr_label)
+            if value is None:
+                continue
+            factory = attribute_factories.get(attr_label)
+            if factory is not None:
+                attribute = factory(entity_spacy, attr_label)
+            else:
+                attribute = Attribute(attr_label, value)
+            attributes.append(attribute)
 
         if attributes:
             attributes_by_ann[medkit_id] = attributes
 
     # convert spacy span groups
     for label, spans in spacy_spans.items():
         for span_spacy in spans:
+            # ignore spans that have a corresponding entity
+            # (some matchers, for instance in EDS-NLP create both an entity and
+            # a span for each match)
+            if span_spacy in spacy_entities:
+                continue
+
             medkit_id = span_spacy._.get(_ATTR_MEDKIT_ID)
 
             if medkit_id is None or rebuild_medkit_anns_and_attrs:
                 # create new segment annotation
                 text, spans = _get_text_and_spans_from_span_spacy(
                     span_spacy=span_spacy, medkit_source_ann=medkit_source_ann
                 )
@@ -140,19 +162,25 @@
                 # 'label' represents 'span_key' from spacy
                 # 'name' in metadata represents the original label of the span in spacy
                 medkit_id = segment.uid
                 annotations.append(segment)
 
             # for each spacy extension having a value other than None,
             # a medkit Attribute is created
-            attributes = [
-                Attribute(label=attr, value=span_spacy._.get(attr))
-                for attr in spacy_attrs
-                if span_spacy._.get(attr) is not None
-            ]
+            attributes = []
+            for attr_label in spacy_attrs:
+                value = span_spacy._.get(attr_label)
+                if value is None:
+                    continue
+                factory = attribute_factories.get(attr_label)
+                if factory is not None:
+                    attribute = factory(span_spacy, attr_label)
+                else:
+                    attribute = Attribute(attr_label, value)
+                attributes.append(attribute)
 
             if attributes:
                 attributes_by_ann[medkit_id] = attributes
 
     return annotations, attributes_by_ann
 
 
@@ -432,20 +460,19 @@
     span = spacy_doc_target.char_span(start, end, alignment_mode="expand", label=label)
 
     if include_medkit_info:
         span._.set(_ATTR_MEDKIT_ID, medkit_segment.uid)
 
     for label in attrs:
         for attr in medkit_segment.attrs.get(label=label):
-            if attr.value is None:
+            value = attr.to_spacy()
+            if value is None:
                 # in medkit having an attribute, indicates that the attribute exists
                 # for the given annotation, we force True as value
                 value = True
-            else:
-                value = attr.value
             # set attributes as extensions
             span._.set(attr.label, value)
             if include_medkit_info:
                 span._.set(f"{attr.label}_{_ATTR_MEDKIT_ID}", attr.uid)
 
     return span
```

### Comparing `medkit_lib-0.4.1/medkit/text/translation/hf_translator.py` & `medkit_lib-0.5.0/medkit/text/translation/hf_translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[hf-translator]`.
+"""
 from __future__ import annotations
 
 __all__ = ["HFTranslator"]
 
 from collections import defaultdict
 import dataclasses
 from pathlib import Path
```

### Comparing `medkit_lib-0.4.1/medkit/tools/hf_utils.py` & `medkit_lib-0.5.0/medkit/tools/hf_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module needs extra-dependencies not installed as core dependencies of medkit.
+To install them, use `pip install medkit-lib[hf-utils]`.
+"""
+
 __all__ = ["check_model_for_task_HF"]
 
 from pathlib import Path
 from typing import Union
 import transformers
```

### Comparing `medkit_lib-0.4.1/medkit/tools/save_prov_to_dot.py` & `medkit_lib-0.5.0/medkit/tools/save_prov_to_dot.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/training/callbacks.py` & `medkit_lib-0.5.0/medkit/training/callbacks.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/training/trainable_operation.py` & `medkit_lib-0.5.0/medkit/training/trainable_component.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 from __future__ import annotations
 
-__all__ = ["TrainableOperation"]
+__all__ = ["TrainableComponent"]
 
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Protocol, runtime_checkable
 
 import torch
 
-from medkit.core import IdentifiableDataItem
-
 from medkit.training.utils import BatchData
 
 
 @runtime_checkable
-class TrainableOperation(Protocol):
-    """A TrainableOperation is the base protocol for an operation to be trainable"""
+class TrainableComponent(Protocol):
+    """TrainableComponent is the base protocol to be trainable in medkit"""
 
     @property
     def device(self) -> torch.device:
         pass
 
     def configure_optimizer(self, lr: float) -> torch.optim.Optimizer:
         """Create optimizer using the learning rate"""
         pass
 
-    def preprocess(
-        self,
-        data_item: Union[IdentifiableDataItem, List[IdentifiableDataItem]],
-        inference_mode: bool,
-    ) -> Dict[str, Any]:
+    def preprocess(self, data_item: Any) -> Dict[str, Any]:
         """
         Preprocess the input data item and return a dictionary with
         everything needed for the forward pass.
 
         This method is intended to preprocess an input, `self.collate` must be
         used to generate batches for `self.forward` to run properly.
-
-        `inference_mode` indicates the phase of the call. If `inference_mode` is False,
-        the call is made in a training context, so preprocess must generate labels to
-        compute a loss. If `inference_mode` is True, the call is made in an inference context,
-        the input has no label to preprocess.
+        Preprocess should include `labels` to compute a loss.
         """
         pass
 
     def collate(self, batch: List[Dict[str, Any]]) -> BatchData:
         """Collate a list of data processed by `preprocess` to form a batch"""
         pass
 
@@ -59,20 +49,14 @@
 
         Before forwarding the model, this method must set the model to training
         or evaluation mode depending on `eval_mode`. In PyTorch models there are
         two methods to set the mode `model.train()` and `model.eval()`
         """
         pass
 
-    def postprocess(
-        self, model_output: BatchData
-    ) -> Union[IdentifiableDataItem, List[IdentifiableDataItem]]:
-        """Create a medkit annotation for model output"""
-        pass
-
     def save(self, path: Union[str, Path]):
         """Save model to disk"""
         pass
 
     def load(self, path: Union[str, Path]):
         """Load weights from disk"""
         # model.from_pretrained or torch load
```

### Comparing `medkit_lib-0.4.1/medkit/training/trainer.py` & `medkit_lib-0.5.0/medkit/training/trainer.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import numpy as np
 import torch
 import yaml
 from medkit.training.trainer_config import TrainerConfig
 from torch.optim.lr_scheduler import ReduceLROnPlateau
 from torch.utils.data import DataLoader, Dataset
 
-from medkit.training.trainable_operation import TrainableOperation
+from medkit.training.trainable_component import TrainableComponent
 from medkit.training.callbacks import DefaultPrinterCallback, TrainerCallback
 from medkit.training.utils import BatchData, MetricsComputer
 
 # checkpoint constants
 OPTIMIZER_NAME = "optimizer.pt"
 SCHEDULER_NAME = "scheduler.pt"
 CONFIG_NAME = "config.yml"
@@ -31,51 +31,51 @@
     """Set seed to keep deterministic operations"""
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
 
 
 class _TrainerDataset(Dataset):
-    """A Dataset that preprocesses data using the 'preprocess' defined in a trainable operation.
+    """A Dataset that preprocesses data using the 'preprocess' defined in a trainable component.
     This class is inspired from the ``PipelineDataset`` class from hugginface transformers library.
     """
 
-    def __init__(self, dataset, operation: TrainableOperation):
+    def __init__(self, dataset, component: TrainableComponent):
         self.dataset = dataset
-        self.operation = operation
+        self.component = component
 
     def __len__(self):
         return len(self.dataset)
 
     def __getitem__(self, i):
         item = self.dataset[i]
-        processed = self.operation.preprocess(item, inference_mode=False)
+        processed = self.component.preprocess(item)
         return processed
 
 
 class Trainer:
-    """A trainer is a base training/eval loop for a TrainableOperation that uses PyTorch models
+    """A trainer is a base training/eval loop for a TrainableComponent that uses PyTorch models
     to create medkit annotations
     """
 
     def __init__(
         self,
-        operation: TrainableOperation,
+        component: TrainableComponent,
         config: TrainerConfig,
         train_data: Any,
         eval_data: Any,
         metrics_computer: Optional[MetricsComputer] = None,
         lr_scheduler_builder: Optional[Callable[[torch.optim.Optimizer], Any]] = None,
         callback: Optional[TrainerCallback] = None,
     ):
         """
         Parameters
         ----------
-        operation:
-            The operation to train, the operation must implement the `TrainableOperation` protocol.
+        component:
+            The component to train, the component must implement the `TrainableComponent` protocol.
         config:
             A `TrainerConfig` with the parameters for training, the parameter `output_dir` define the
             path of the checkpoints
         train_data:
             The data to use for training. This should be a corpus of medkit objects. The data could be,
             for instance, a `torch.utils.data.Dataset` that returns medkit objects for training.
         eval_data:
@@ -94,45 +94,45 @@
         # enable deterministic operation
         if config.seed is not None:
             set_seed(config.seed)
 
         self.output_dir = Path(config.output_dir)
         os.makedirs(self.output_dir, exist_ok=True)
 
-        self.operation = operation
+        self.component = component
         self.batch_size = config.batch_size
         self.dataloader_drop_last = False
         self.dataloader_nb_workers = config.dataloader_nb_workers
         self.dataloader_pin_memory = False
 
-        self.device = self.operation.device
+        self.device = self.component.device
 
         self.train_dataloader = self.get_dataloader(train_data, shuffle=True)
         self.eval_dataloader = self.get_dataloader(eval_data, shuffle=False)
         self.nb_training_epochs = config.nb_training_epochs
 
         self.config = config
 
-        self.optimizer = operation.configure_optimizer(self.config.learning_rate)
+        self.optimizer = component.configure_optimizer(self.config.learning_rate)
         self.lr_scheduler = (
             None
             if lr_scheduler_builder is None
             else lr_scheduler_builder(self.optimizer)
         )
 
         self.metrics_computer = metrics_computer
 
         if callback is None:
             self.callback = DefaultPrinterCallback()
 
     def get_dataloader(self, data: any, shuffle: bool) -> DataLoader:
         """Return a DataLoader with transformations defined
-        in the operation to train"""
-        dataset = _TrainerDataset(data, self.operation)
-        collate_fn = self.operation.collate
+        in the component to train"""
+        dataset = _TrainerDataset(data, self.component)
+        collate_fn = self.component.collate
         return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=shuffle,
             collate_fn=collate_fn,
             drop_last=self.dataloader_drop_last,
             num_workers=self.dataloader_nb_workers,
@@ -224,22 +224,22 @@
         if self.metrics_computer is not None:
             metrics.update(self.metrics_computer.compute(dict(data_for_metrics)))
         return metrics
 
     def make_forward_pass(
         self, inputs: BatchData, eval_mode: bool
     ) -> Tuple[BatchData, torch.Tensor]:
-        """Run forward safely, same device as the operation"""
+        """Run forward safely, same device as the component"""
         inputs = inputs.to_device(self.device)
-        model_output, loss = self.operation.forward(
+        model_output, loss = self.component.forward(
             inputs, return_loss=True, eval_mode=eval_mode
         )
 
         if loss is None:
-            raise ValueError("The operation did not return a 'loss' from the input.")
+            raise ValueError("The component did not return a 'loss' from the input.")
 
         return model_output, loss
 
     def update_learning_rate(self, eval_metrics: Dict[str, float]):
         """Call the learning rate scheduler if defined"""
         if self.lr_scheduler is None:
             return
@@ -317,8 +317,8 @@
 
         if self.lr_scheduler is not None:
             torch.save(
                 self.lr_scheduler.state_dict(),
                 os.path.join(checkpoint_dir, SCHEDULER_NAME),
             )
 
-        self.operation.save(checkpoint_dir)
+        self.component.save(checkpoint_dir)
```

### Comparing `medkit_lib-0.4.1/medkit/training/trainer_config.py` & `medkit_lib-0.5.0/medkit/training/trainer_config.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/medkit/training/utils.py` & `medkit_lib-0.5.0/medkit/training/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.4.1/pyproject.toml` & `medkit_lib-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "medkit-lib"
-version = "0.4.1"
+version = "0.5.0"
 description = "A Python library for a learning health system"
 readme = "README.md"
 repository = "https://gitlab.inria.fr/heka/medkit/"
 documentation = "https://heka.gitlabpages.inria.fr/medkit/"
 authors = ["HeKA Research Team"]
 maintainers = [
     "medkit-maintainers <medkit-maintainers@inria.fr>"
@@ -32,16 +32,18 @@
 smart-open = "*"
 soundfile = "*"
 tqdm = "*"
 typing-extensions = "*"
 Unidecode = "*"
 intervaltree = "*"
 wheel = "*"
+iamsystem = ">=0.3"
 
 # optional
+edsnlp = {version = "^0.7", optional = true}
 feather-format = {version = "^0.4", optional = true}
 packaging = {version = "*", optional = true}
 pandas = [
     {version = "~1.3", python = ">=3.7.1, <3.8", optional = true},
     {version = "^1.4", python = ">=3.8, <4.0", optional = true},
 ]
 pyannote-audio = {version = "^2.1", optional = true}
@@ -72,29 +74,32 @@
 spacy = "^3.4"
 sphinx = ">=4.3.3"
 sphinxcontrib-mermaid = ">=0.8"
 sphinx-toolbox = "*"
 
 [tool.poetry.extras]
 
+# Dependencies related to optional medkit modules
+edsnlp = ["edsnlp"]
 hf-entity-matcher = [
     "torch",
     "transformers",
 ]
 hf-transcriber-function = [
     "torchaudio",
     "transformers"
 ]
 hf-translator = [
     "sacremoses",  # needed by default model "Helsinki-NLP/opus-mt-fr-en"
     "sentencepiece",
     "torch",
     "transformers"
 ]
-pa-speaker-translator = [
+hf-utils = ["transformers"]
+pa-speaker-detector = [
     "torch",
     "pyannote-audio",
 ]
 quick-umls = [
     "packaging",  # needed to check quickumls version
     "quickumls",
 ]
@@ -102,14 +107,15 @@
 rush-sentence-tokenizer = ["PyRush"]
 sb-transcriber-function = [
     "speechbrain",
     "torch",
     "transformers",
 ]
 spacy = ["spacy"]
+syntactic-relation-extractor = ["spacy"]
 training = ["torch"]
 umls-coder-normalizer = [
     "feather-format",
     "pandas",
     "torch",
     "transformers",
 ]
```

### Comparing `medkit_lib-0.4.1/PKG-INFO` & `medkit_lib-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medkit-lib
-Version: 0.4.1
+Version: 0.5.0
 Summary: A Python library for a learning health system
 Home-page: https://gitlab.inria.fr/heka/medkit/
 License: MIT
 Author: HeKA Research Team
 Maintainer: medkit-maintainers
 Maintainer-email: medkit-maintainers@inria.fr
 Requires-Python: >=3.7.1,<4.0
@@ -15,51 +15,56 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Provides-Extra: edsnlp
 Provides-Extra: hf-entity-matcher
 Provides-Extra: hf-transcriber-function
 Provides-Extra: hf-translator
+Provides-Extra: hf-utils
 Provides-Extra: optional
-Provides-Extra: pa-speaker-translator
+Provides-Extra: pa-speaker-detector
 Provides-Extra: quick-umls
 Provides-Extra: resampler
 Provides-Extra: rush-sentence-tokenizer
 Provides-Extra: sb-transcriber-function
 Provides-Extra: spacy
+Provides-Extra: syntactic-relation-extractor
 Provides-Extra: training
 Provides-Extra: umls-coder-normalizer
 Provides-Extra: webrtc-voice-detector
 Requires-Dist: PyRuSH (>=1.0,<2.0) ; extra == "rush-sentence-tokenizer" or extra == "optional"
 Requires-Dist: Unidecode
+Requires-Dist: edsnlp (>=0.7,<0.8) ; extra == "edsnlp"
 Requires-Dist: feather-format (>=0.4,<0.5) ; extra == "umls-coder-normalizer" or extra == "optional"
 Requires-Dist: flashtext
+Requires-Dist: iamsystem (>=0.3)
 Requires-Dist: intervaltree
 Requires-Dist: numpy
 Requires-Dist: packaging ; extra == "quick-umls" or extra == "optional"
 Requires-Dist: pandas (>=1.3,<1.4) ; (python_full_version >= "3.7.1" and python_version < "3.8") and (extra == "umls-coder-normalizer" or extra == "optional")
 Requires-Dist: pandas (>=1.4,<2.0) ; (python_version >= "3.8" and python_version < "4.0") and (extra == "umls-coder-normalizer" or extra == "optional")
 Requires-Dist: pyaml
-Requires-Dist: pyannote-audio (>=2.1,<3.0) ; extra == "pa-speaker-translator"
+Requires-Dist: pyannote-audio (>=2.1,<3.0) ; extra == "pa-speaker-detector"
 Requires-Dist: quickumls (>=1.4,<2.0) ; extra == "quick-umls" or extra == "optional"
 Requires-Dist: requests
 Requires-Dist: resampy (>=0.4,<0.5) ; extra == "resampler" or extra == "optional"
 Requires-Dist: sacremoses ; extra == "hf-translator" or extra == "optional"
 Requires-Dist: sentencepiece ; extra == "hf-translator" or extra == "optional"
 Requires-Dist: smart-open
 Requires-Dist: soundfile
-Requires-Dist: spacy (>=3.4,<4.0) ; extra == "spacy" or extra == "optional"
+Requires-Dist: spacy (>=3.4,<4.0) ; extra == "spacy" or extra == "syntactic-relation-extractor" or extra == "optional"
 Requires-Dist: speechbrain (>=0.5,<0.6) ; extra == "sb-transcriber-function"
-Requires-Dist: torch (>=1.0,<2.0) ; extra == "hf-entity-matcher" or extra == "hf-translator" or extra == "pa-speaker-translator" or extra == "sb-transcriber-function" or extra == "training" or extra == "umls-coder-normalizer" or extra == "optional"
+Requires-Dist: torch (>=1.0,<2.0) ; extra == "hf-entity-matcher" or extra == "hf-translator" or extra == "pa-speaker-detector" or extra == "sb-transcriber-function" or extra == "training" or extra == "umls-coder-normalizer" or extra == "optional"
 Requires-Dist: torchaudio (>=0.12,<0.13) ; extra == "hf-transcriber-function" or extra == "optional"
 Requires-Dist: tqdm
-Requires-Dist: transformers (>=4.21,<5.0) ; extra == "hf-entity-matcher" or extra == "hf-transcriber-function" or extra == "hf-translator" or extra == "sb-transcriber-function" or extra == "umls-coder-normalizer" or extra == "optional"
+Requires-Dist: transformers (>=4.21,<5.0) ; extra == "hf-entity-matcher" or extra == "hf-transcriber-function" or extra == "hf-translator" or extra == "hf-utils" or extra == "sb-transcriber-function" or extra == "umls-coder-normalizer" or extra == "optional"
 Requires-Dist: typing-extensions
 Requires-Dist: webrtcvad (>=2.0,<3.0) ; extra == "webrtc-voice-detector" or extra == "optional"
 Requires-Dist: wheel
 Project-URL: Documentation, https://heka.gitlabpages.inria.fr/medkit/
 Project-URL: Repository, https://gitlab.inria.fr/heka/medkit/
 Description-Content-Type: text/markdown
```

