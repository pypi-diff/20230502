# Comparing `tmp/keyword_explorer-0.4a0.tar.gz` & `tmp/keyword_explorer-0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\keyword_explorer-0.4a0.tar", last modified: Mon Jan 16 21:25:26 2023, max compression
+gzip compressed data, was "dist\keyword_explorer-0.5a0.tar", last modified: Tue May  2 13:38:22 2023, max compression
```

## Comparing `keyword_explorer-0.4a0.tar` & `keyword_explorer-0.5a0.tar`

### file list

```diff
@@ -1,65 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-01-16 21:25:26.000000 keyword_explorer-0.4a0/
--rw-rw-rw-   0        0        0     1115 2022-03-09 16:58:07.000000 keyword_explorer-0.4a0/LICENSE
--rw-rw-rw-   0        0        0     1627 2023-01-16 21:25:26.000000 keyword_explorer-0.4a0/PKG-INFO
--rw-rw-rw-   0        0        0      577 2022-08-03 13:33:36.000000 keyword_explorer-0.4a0/README
-drwxrwxrwx   0        0        0        0 2023-01-16 21:25:26.000000 keyword_explorer-0.4a0/keyword_explorer/
-drwxrwxrwx   0        0        0        0 2023-01-16 21:25:26.000000 keyword_explorer-0.4a0/keyword_explorer/Apps/
--rw-rw-rw-   0        0        0     7381 2022-11-15 13:04:51.000000 keyword_explorer-0.4a0/keyword_explorer/Apps/AppBase.py
--rw-rw-rw-   0        0        0     4014 2022-08-02 14:17:54.000000 keyword_explorer-0.4a0/keyword_explorer/Apps/GoogleExplorer.py
--rw-rw-rw-   0        0        0    16712 2022-12-11 13:01:48.000000 keyword_explorer-0.4a0/keyword_explorer/Apps/KeywordExplorer.py
--rw-rw-rw-   0        0        0    15476 2022-12-11 17:55:33.000000 keyword_explorer-0.4a0/keyword_explorer/Apps/ModelExplorer.py
--rw-rw-rw-   0        0        0    10146 2022-12-07 20:46:12.000000 keyword_explorer-0.4a0/keyword_explorer/Apps/TweetCountExplorer.py
--rw-rw-rw-   0        0        0    26465 2022-11-13 11:54:47.000000 keyword_explorer-0.4a0/keyword_explorer/Apps/TweetDownloader.py
--rw-rw-rw-   0        0        0    27439 2022-11-08 23:09:16.000000 keyword_explorer-0.4a0/keyword_explorer/Apps/TweetEmbedExplorer.py
--rw-rw-rw-   0        0        0    10867 2022-10-13 12:52:51.000000 keyword_explorer-0.4a0/keyword_explorer/Apps/WikiPageviewExplorer.py
--rw-rw-rw-   0        0        0        0 2022-03-02 13:40:13.000000 keyword_explorer-0.4a0/keyword_explorer/Apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-16 21:25:26.000000 keyword_explorer-0.4a0/keyword_explorer/OpenAI/
--rw-rw-rw-   0        0        0     4655 2022-12-15 21:08:16.000000 keyword_explorer-0.4a0/keyword_explorer/OpenAI/OpenAIComms.py
-drwxrwxrwx   0        0        0        0 2023-01-16 21:25:26.000000 keyword_explorer-0.4a0/keyword_explorer/TwitterV2/
--rw-rw-rw-   0        0        0    19367 2023-01-13 20:15:17.000000 keyword_explorer-0.4a0/keyword_explorer/TwitterV2/TweetKeywords.py
--rw-rw-rw-   0        0        0     4693 2022-09-07 17:20:53.000000 keyword_explorer-0.4a0/keyword_explorer/TwitterV2/TwitterV2Base.py
--rw-rw-rw-   0        0        0     8853 2022-12-05 20:54:31.000000 keyword_explorer-0.4a0/keyword_explorer/TwitterV2/TwitterV2Counts.py
--rw-rw-rw-   0        0        0        0 2022-02-01 19:48:49.000000 keyword_explorer-0.4a0/keyword_explorer/TwitterV2/__init__.py
--rw-rw-rw-   0        0        0     8625 2022-12-18 12:34:08.000000 keyword_explorer-0.4a0/keyword_explorer/TwitterV2/tweet_lookup.py
--rw-rw-rw-   0        0        0        0 2022-03-02 13:40:28.000000 keyword_explorer-0.4a0/keyword_explorer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-16 21:25:26.000000 keyword_explorer-0.4a0/keyword_explorer/mastodon/
--rw-rw-rw-   0        0        0        0 2022-12-02 14:15:20.000000 keyword_explorer-0.4a0/keyword_explorer/mastodon/__init__.py
--rw-rw-rw-   0        0        0     1418 2023-01-13 15:06:40.000000 keyword_explorer-0.4a0/keyword_explorer/mastodon/post_lookup.py
-drwxrwxrwx   0        0        0        0 2023-01-16 21:25:26.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/
--rw-rw-rw-   0        0        0     1159 2022-09-26 17:43:47.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/Buttons.py
--rw-rw-rw-   0        0        0      458 2021-09-20 14:28:52.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/CanvasData.py
--rw-rw-rw-   0        0        0    13329 2022-08-30 14:28:42.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/CanvasFrame.py
--rw-rw-rw-   0        0        0     2325 2022-11-08 23:04:03.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/Checkboxes.py
--rw-rw-rw-   0        0        0     1967 2022-09-30 13:29:58.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/ConsoleDprint.py
--rw-rw-rw-   0        0        0     2667 2022-06-15 13:06:41.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/DataField.py
--rw-rw-rw-   0        0        0     1728 2022-08-17 14:36:57.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/DateEntryField.py
--rw-rw-rw-   0        0        0     1823 2022-09-23 19:53:54.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/LabeledParam.py
--rw-rw-rw-   0        0        0     4785 2022-02-25 16:17:14.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/ListField.py
--rw-rw-rw-   0        0        0     6046 2022-09-26 14:56:22.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/MoveableNode.py
--rw-rw-rw-   0        0        0     7019 2022-03-01 16:44:28.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/TextComparePopup.py
--rw-rw-rw-   0        0        0     4981 2022-03-07 21:15:51.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/TextField.py
--rw-rw-rw-   0        0        0     7912 2022-03-01 16:46:29.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/TkCanvasBase.py
--rw-rw-rw-   0        0        0     1163 2022-08-01 14:40:36.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/ToolTip.py
--rw-rw-rw-   0        0        0     4145 2022-09-07 17:40:13.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/TopicCombo.py
--rw-rw-rw-   0        0        0     3748 2022-09-08 18:13:11.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/TopicComboExt.py
--rw-rw-rw-   0        0        0        0 2021-09-24 12:22:20.000000 keyword_explorer-0.4a0/keyword_explorer/tkUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-16 21:25:26.000000 keyword_explorer-0.4a0/keyword_explorer/utils/
--rw-rw-rw-   0        0        0     6872 2022-10-13 19:07:46.000000 keyword_explorer-0.4a0/keyword_explorer/utils/CorporaGenerator.py
--rw-rw-rw-   0        0        0    31002 2022-09-30 13:29:58.000000 keyword_explorer-0.4a0/keyword_explorer/utils/ManifoldReduction.py
--rw-rw-rw-   0        0        0     3568 2022-10-14 12:47:24.000000 keyword_explorer-0.4a0/keyword_explorer/utils/MySqlInterface.py
--rw-rw-rw-   0        0        0     1386 2022-03-07 17:02:10.000000 keyword_explorer-0.4a0/keyword_explorer/utils/SharedObjects.py
--rw-rw-rw-   0        0        0     8686 2022-01-21 15:29:51.000000 keyword_explorer-0.4a0/keyword_explorer/utils/TextSimilarity.py
--rw-rw-rw-   0        0        0       67 2022-08-18 21:37:11.000000 keyword_explorer-0.4a0/keyword_explorer/utils/app_test.py
--rw-rw-rw-   0        0        0      408 2022-01-14 14:47:24.000000 keyword_explorer-0.4a0/keyword_explorer/utils/excel_to_latex.py
--rw-rw-rw-   0        0        0      483 2021-03-22 11:48:23.000000 keyword_explorer-0.4a0/keyword_explorer/utils/find_transformer_models.py
--rw-rw-rw-   0        0        0     2214 2022-05-24 19:24:37.000000 keyword_explorer-0.4a0/keyword_explorer/utils/google_search.py
--rw-rw-rw-   0        0        0     4090 2022-03-04 20:54:01.000000 keyword_explorer-0.4a0/keyword_explorer/utils/wikipedia_search.py
-drwxrwxrwx   0        0        0        0 2023-01-16 21:25:26.000000 keyword_explorer-0.4a0/keyword_explorer.egg-info/
--rw-rw-rw-   0        0        0     1627 2023-01-16 21:25:25.000000 keyword_explorer-0.4a0/keyword_explorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2065 2023-01-16 21:25:25.000000 keyword_explorer-0.4a0/keyword_explorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-16 21:25:25.000000 keyword_explorer-0.4a0/keyword_explorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      202 2023-01-16 21:25:25.000000 keyword_explorer-0.4a0/keyword_explorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-01-16 21:25:25.000000 keyword_explorer-0.4a0/keyword_explorer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-03-29 19:08:22.000000 keyword_explorer-0.4a0/pyproject.toml
--rw-rw-rw-   0        0        0      111 2023-01-16 21:25:26.000000 keyword_explorer-0.4a0/setup.cfg
--rw-rw-rw-   0        0        0     2735 2023-01-16 21:20:45.000000 keyword_explorer-0.4a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/
+-rw-rw-rw-   0        0        0     1115 2022-03-09 16:58:07.000000 keyword_explorer-0.5a0/LICENSE
+-rw-rw-rw-   0        0        0     2014 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2022-08-03 13:33:36.000000 keyword_explorer-0.5a0/README
+drwxrwxrwx   0        0        0        0 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer/
+drwxrwxrwx   0        0        0        0 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/
+-rw-rw-rw-   0        0        0     7854 2023-02-22 22:28:46.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/AppBase.py
+-rw-rw-rw-   0        0        0    26285 2023-04-24 17:14:48.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/ContextExplorer.py
+-rw-rw-rw-   0        0        0     4113 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/GoogleExplorer.py
+-rw-rw-rw-   0        0        0    17258 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/KeywordExplorer.py
+-rw-rw-rw-   0        0        0    15540 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/ModelExplorer.py
+-rw-rw-rw-   0        0        0    37366 2023-03-15 14:09:02.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/NarrativeExplorer.py
+-rw-rw-rw-   0        0        0    29399 2023-04-12 13:32:31.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/NarrativeExplorer2.py
+-rw-rw-rw-   0        0        0    16372 2023-03-17 19:53:40.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/TerrainFromGML.py
+-rw-rw-rw-   0        0        0    10386 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/TweetCountExplorer.py
+-rw-rw-rw-   0        0        0    27254 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/TweetDownloader.py
+-rw-rw-rw-   0        0        0    40960 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/TweetEmbedExplorer.py
+-rw-rw-rw-   0        0        0    11243 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/WikiPageviewExplorer.py
+-rw-rw-rw-   0        0        0        0 2022-03-02 13:40:13.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer/OpenAI/
+-rw-rw-rw-   0        0        0    17090 2023-04-25 20:28:22.000000 keyword_explorer-0.5a0/keyword_explorer/OpenAI/OpenAIComms.py
+-rw-rw-rw-   0        0        0    23382 2023-04-18 22:38:59.000000 keyword_explorer-0.5a0/keyword_explorer/OpenAI/OpenAIEmbeddings.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/
+-rw-rw-rw-   0        0        0     8404 2022-01-04 13:05:33.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/DefinedColors.py
+-rw-rw-rw-   0        0        0     8055 2020-09-18 13:05:26.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/DefinedColors_GOES.py
+-rw-rw-rw-   0        0        0     1825 2023-03-17 19:53:40.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/ExampleHand.py
+-rw-rw-rw-   0        0        0     3078 2019-10-16 17:42:36.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/HelloWorld.py
+-rw-rw-rw-   0        0        0     3354 2023-03-17 19:54:27.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/LinePrimitives.py
+-rw-rw-rw-   0        0        0     1405 2019-10-16 17:42:36.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/MouseEventHandler.py
+-rw-rw-rw-   0        0        0     5866 2023-03-17 19:53:40.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/Pandas_main.py
+-rw-rw-rw-   0        0        0     5078 2021-12-29 16:05:04.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/Primitives.py
+-rw-rw-rw-   0        0        0     6339 2019-10-16 17:42:36.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/ProceduralCube.py
+-rw-rw-rw-   0        0        0    14012 2023-03-17 19:54:41.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/ShapePrimitives.py
+-rw-rw-rw-   0        0        0        0 2019-07-10 17:34:16.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/keyword_explorer/TwitterV2/
+-rw-rw-rw-   0        0        0    19367 2023-01-13 20:15:17.000000 keyword_explorer-0.5a0/keyword_explorer/TwitterV2/TweetKeywords.py
+-rw-rw-rw-   0        0        0     4693 2022-09-07 17:20:53.000000 keyword_explorer-0.5a0/keyword_explorer/TwitterV2/TwitterV2Base.py
+-rw-rw-rw-   0        0        0     8853 2022-12-05 20:54:31.000000 keyword_explorer-0.5a0/keyword_explorer/TwitterV2/TwitterV2Counts.py
+-rw-rw-rw-   0        0        0        0 2022-02-01 19:48:49.000000 keyword_explorer-0.5a0/keyword_explorer/TwitterV2/__init__.py
+-rw-rw-rw-   0        0        0     8625 2022-12-18 12:34:08.000000 keyword_explorer-0.5a0/keyword_explorer/TwitterV2/tweet_lookup.py
+-rw-rw-rw-   0        0        0        0 2022-03-02 13:40:28.000000 keyword_explorer-0.5a0/keyword_explorer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/
+-rw-rw-rw-   0        0        0     3932 2022-10-27 13:43:22.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/HFaceGPT.py
+-rw-rw-rw-   0        0        0     6158 2022-10-25 15:59:55.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/PatternCounter.py
+-rw-rw-rw-   0        0        0        0 2022-10-14 11:54:53.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/__init__.py
+-rw-rw-rw-   0        0        0     5070 2022-10-13 19:45:32.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/test1.py
+-rw-rw-rw-   0        0        0     2069 2021-04-15 17:58:09.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/test2.py
+-rw-rw-rw-   0        0        0     3090 2021-04-21 13:27:35.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/test3.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/keyword_explorer/mastodon/
+-rw-rw-rw-   0        0        0        0 2022-12-02 14:15:20.000000 keyword_explorer-0.5a0/keyword_explorer/mastodon/__init__.py
+-rw-rw-rw-   0        0        0     1418 2023-01-13 15:06:40.000000 keyword_explorer-0.5a0/keyword_explorer/mastodon/post_lookup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/
+-rw-rw-rw-   0        0        0     1633 2023-04-13 19:13:26.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/Buttons.py
+-rw-rw-rw-   0        0        0      458 2021-09-20 14:28:52.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/CanvasData.py
+-rw-rw-rw-   0        0        0    13329 2022-08-30 14:28:42.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/CanvasFrame.py
+-rw-rw-rw-   0        0        0     2356 2023-02-23 21:54:28.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/Checkboxes.py
+-rw-rw-rw-   0        0        0     1967 2022-09-30 13:29:58.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/ConsoleDprint.py
+-rw-rw-rw-   0        0        0     2667 2022-06-15 13:06:41.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/DataField.py
+-rw-rw-rw-   0        0        0     1728 2022-08-17 14:36:57.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/DateEntryField.py
+-rw-rw-rw-   0        0        0     9542 2023-03-15 17:03:25.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/GPT3EmbeddingFrame.py
+-rw-rw-rw-   0        0        0    12835 2023-03-22 14:00:45.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/GPT3GeneratorFrame.py
+-rw-rw-rw-   0        0        0     1823 2022-09-23 19:53:54.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/LabeledParam.py
+-rw-rw-rw-   0        0        0     5269 2023-04-20 18:56:29.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/ListField.py
+-rw-rw-rw-   0        0        0     6046 2022-09-26 14:56:22.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/MoveableNode.py
+-rw-rw-rw-   0        0        0      613 2023-03-21 22:11:34.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/SelectParam.py
+-rw-rw-rw-   0        0        0     7019 2022-03-01 16:44:28.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/TextComparePopup.py
+-rw-rw-rw-   0        0        0     5144 2023-01-31 13:58:52.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/TextField.py
+-rw-rw-rw-   0        0        0     7912 2022-03-01 16:46:29.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/TkCanvasBase.py
+-rw-rw-rw-   0        0        0     1163 2022-08-01 14:40:36.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/ToolTip.py
+-rw-rw-rw-   0        0        0     4145 2022-09-07 17:40:13.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/TopicCombo.py
+-rw-rw-rw-   0        0        0     3954 2023-04-20 18:44:25.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/TopicComboExt.py
+-rw-rw-rw-   0        0        0        0 2021-09-24 12:22:20.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtilsExt/
+-rw-rw-rw-   0        0        0    22026 2023-04-26 15:26:09.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtilsExt/GPTContextFrame.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 15:04:56.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtilsExt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/keyword_explorer/utils/
+-rw-rw-rw-   0        0        0     6872 2022-10-13 19:07:46.000000 keyword_explorer-0.5a0/keyword_explorer/utils/CorporaGenerator.py
+-rw-rw-rw-   0        0        0    34486 2023-03-15 22:25:18.000000 keyword_explorer-0.5a0/keyword_explorer/utils/ManifoldReduction.py
+-rw-rw-rw-   0        0        0     3568 2022-10-14 12:47:24.000000 keyword_explorer-0.5a0/keyword_explorer/utils/MySqlInterface.py
+-rw-rw-rw-   0        0        0    16560 2023-03-16 15:23:45.000000 keyword_explorer-0.5a0/keyword_explorer/utils/NetworkxGraphing.py
+-rw-rw-rw-   0        0        0     1609 2023-03-14 20:38:59.000000 keyword_explorer-0.5a0/keyword_explorer/utils/SharedObjects.py
+-rw-rw-rw-   0        0        0     8686 2022-01-21 15:29:51.000000 keyword_explorer-0.5a0/keyword_explorer/utils/TextSimilarity.py
+-rw-rw-rw-   0        0        0       67 2022-08-18 21:37:11.000000 keyword_explorer-0.5a0/keyword_explorer/utils/app_test.py
+-rw-rw-rw-   0        0        0      408 2022-01-14 14:47:24.000000 keyword_explorer-0.5a0/keyword_explorer/utils/excel_to_latex.py
+-rw-rw-rw-   0        0        0      483 2021-03-22 11:48:23.000000 keyword_explorer-0.5a0/keyword_explorer/utils/find_transformer_models.py
+-rw-rw-rw-   0        0        0     4670 2023-03-06 13:15:31.000000 keyword_explorer-0.5a0/keyword_explorer/utils/google_search.py
+-rw-rw-rw-   0        0        0     4090 2022-03-04 20:54:01.000000 keyword_explorer-0.5a0/keyword_explorer/utils/wikipedia_search.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer.egg-info/
+-rw-rw-rw-   0        0        0     2014 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3244 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      168 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-03-29 19:08:22.000000 keyword_explorer-0.5a0/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/setup.cfg
+-rw-rw-rw-   0        0        0     3272 2023-05-02 13:37:07.000000 keyword_explorer-0.5a0/setup.py
```

### Comparing `keyword_explorer-0.4a0/LICENSE` & `keyword_explorer-0.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/PKG-INFO` & `keyword_explorer-0.5a0/keyword_explorer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
-Name: keyword_explorer
-Version: 0.4a0
+Name: keyword-explorer
+Version: 0.5a0
 Summary: A set of tools for producing and exploring keywords on Twitter and the Wikipedia
 Home-page: https://github.com/pgfeldman/KeywordExplorer
 Author: Philip Feldman
 Author-email: phil@philfeldman.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 
 Explorer Apps
 ====================================
-There are four applications in this project, _KeywordExplorer_, _TweetsCountExplorer_, _TweetDownloader_, and _WikiPageviewExplorer_. They, and the classes that support them, can be installed with pip:
+There are six applications in this project: KeywordExplorer, TweetsCountExplorer, TweetDownloader, WikiPageviewExplorer, TweetEmbedExplorer, and ModelExplorer. They, and the classes that support them, can be installed with pip:
 
     pip install keyword-explorer
 
 **KeywordExplorer** is a Python desktop app that lets you use the GPT-3 to search for keywords and Twitter to see if those keywords are any good.
 
 **TweetCountsExplorer** is a Python desktop app that lets you explore the quantity of tweets containing keywords over days, weeks or months.
 
 **TweetDownloader** is a Python desktop app that lets you select and download tweets containing keywords into a database. The number of Tweets can be adjusted so that they are the same for each day or proportional. Users can apply daily and overall limits for each keyword corpora.
 
 **WikiPageviewExplorer**  is a Python desktop app that lets you explore keywords that appear as articles in the Wikipedia, and chart their relative page views.
 
+**TweetEmbedExplorer** is a Python desktop app for analyzing, filtering, and augmenting tweet information. Augmented information can them be used to create a train/test corpus for finetuning language models such as the GPT-2.
+
+**ModelExplorer** is a Python desktop app that lets a user interact with a finetuned GPT-2 model trained using EmbeddingExplorer
+
 Full documentation is available at https://github.com/pgfeldman/KeywordExplorer#readme
```

### Comparing `keyword_explorer-0.4a0/README` & `keyword_explorer-0.5a0/README`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/Apps/AppBase.py` & `keyword_explorer-0.5a0/keyword_explorer/Apps/AppBase.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,25 @@
         menu_file = tk.Menu(menubar)
         menubar.add_cascade(menu=menu_file, label='File')
         menu_file.add_command(label='Load experiment', command=self.load_experiment_callback)
         menu_file.add_command(label='Save experiment', command=self.save_experiment_callback)
         menu_file.add_command(label='Load IDs', command=self.load_ids_callback)
         menu_file.add_command(label='Exit', command=self.terminate)
 
+    def load_json(self, key_dict:Dict) -> Dict:
+        so = SharedObjects()
+        result = filedialog.askopenfile(filetypes=(("JSON files", "*.json"),("All Files", "*.*")), title="Load json ID file")
+        if result:
+            so.load_from_file(result.name)
+            for key in key_dict.keys():
+                val = so.get_object(key)
+                if val != None:
+                    key_dict[key] = val
+        return key_dict
+
     def load_ids_callback(self):
         result = filedialog.askopenfile(filetypes=(("JSON files", "*.json"),("All Files", "*.*")), title="Load json ID file")
         if result:
             self.so.load_from_file(result.name)
             self.tvc.bearer_token = self.so.get_object('BEARER_TOKEN_2')
             #print("bearer_token = {}".format(self.tvc.bearer_token))
 
@@ -128,15 +139,15 @@
         if result:
             filename = result.name
             print("AppBase.save_experiment_json() Saving to {}".format(filename))
             with open (filename, 'w') as f:
                 json.dump(d, f, indent=4)
 
     def safe_dict_read(self, d:Dict, key:str, default:Any) -> Any:
-        if key in d:
+        if key in d and d[key] != None:
             return d[key]
         return default
 
     def clean_text(self, s:str) -> str:
         char_list = [s[j] for j in range(len(s)) if ord(s[j]) in range(65536)]
         s=''
         for j in char_list:
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/Apps/GoogleExplorer.py` & `keyword_explorer-0.5a0/keyword_explorer/Apps/GoogleExplorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,23 @@
 html_end = html_str = '''
         </body>
     </html>'''
 
 class GoogleExplorer(AppBase):
     search_field:DataField
     search_frame:HtmlFrame
+    action_buttons:Buttons
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         print("GoogleExplorer")
 
     def setup_app(self):
         self.app_name = "GoogleExplorer"
-        self.app_version = "3.14.22"
+        self.app_version = "4.11.2023"
         self.geom = (850, 850)
         if not gs.key_exists():
             message.showwarning("Key Error", "Could not find Environment key 'GOOGLE_CSE_KEY'")
 
     def build_app_view(self, row:int, text_width:int, label_width:int) -> int:
         row += 1
         lf = tk.LabelFrame(self, text="Search")
@@ -56,17 +57,17 @@
 
     def build_search(self, parent:tk.LabelFrame, text_width:int, label_width:int):
         row = 0
         self.search_field = DataField(parent, row, "Search:", text_width, label_width=label_width)
         ToolTip(self.search_field.tk_entry, "Type your search term or phrase here")
         row = self.search_field.get_next_row()
 
-        buttons = Buttons(parent, row, "Actions:", label_width)
-        buttons.add_button("Search", self.search_callback)
-        row = buttons.get_next_row()
+        self.action_buttons = Buttons(parent, row, "Actions:", label_width)
+        self.action_buttons.add_button("Search", self.search_callback)
+        row = self.action_buttons.get_next_row()
 
 
         self.search_frame = HtmlFrame(parent) #create HTML browser
         self.search_frame.load_html(html_str)
         self.search_frame.on_link_click(self.load_new_page)
         self.search_frame.grid(row = row, column=0, columnspan = 2, sticky="nsew", padx=5, pady=2)
         ToolTip(self.search_frame, "Search results are here\nLinks open tabs in your default browser")
@@ -78,18 +79,18 @@
         if key == None:
             key = self.so.get_object("GOOGLE_CSE_KEY")
         if key == None:
             message.showwarning("Key Error", "Could not find Environment key 'GOOGLE_CSE_KEY. Please load from ids.json file'")
             return
 
         self.log_action("search", {"query":query})
-        l = gs.get_search_results_list(query, engine, key)
+        results_list, info_list = gs.get_search_results_list(query, engine, key)
         s = html_begin
         g:gs.GoogleCSEResult
-        for g in l:
+        for g in results_list:
             s += g.to_html()
             # print("\n{}".format(g.to_string()))
         s += html_end
         self.search_frame.load_html(s)
 
     def load_new_page(self, url):
         print(url)
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/Apps/KeywordExplorer.py` & `keyword_explorer-0.5a0/keyword_explorer/Apps/KeywordExplorer.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,22 +29,24 @@
     end_date_field:DateEntryField
     regex_field:DataField
     max_chars_field:DataField
     token_list:ListField
     engine_list:ListField
     sample_list:ListField
     query_options_field:DataField
+    action_buttons:Buttons
+    action_buttons2:Buttons
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         print("KeywordExplorer")
 
     def setup_app(self):
         self.app_name = "KeywordExplorer"
-        self.app_version = "12.11.22"
+        self.app_version = "3.17.2023"
         self.geom = (850, 790)
         self.oai = OpenAIComms()
         self.tvc = TwitterV2Counts()
 
         if not self.oai.key_exists():
             message.showwarning("Key Error", "Could not find Environment key 'OPENAI_KEY'")
         if not self.tvc.key_exists():
@@ -93,33 +95,35 @@
         row = self.max_chars_field.get_next_row()
 
         self.regex_field = DataField(lf, row, 'Parse regex', text_width, label_width=label_width)
         self.regex_field.set_text(r"\n[0-9]+\)|\n[0-9]+|[0-9]+\)")
         ToolTip(self.regex_field.tk_entry, "The regex used to parse the GPT response. Editable")
         row = self.regex_field.get_next_row()
 
-        buttons = Buttons(lf, row, "Actions", label_width=label_width)
-        b = buttons.add_button("New prompt", self.new_prompt_callback, width=-1)
+        self.action_buttons = Buttons(lf, row, "Actions", label_width=label_width)
+        b = self.action_buttons.add_button("New prompt", self.new_prompt_callback, width=-1)
         ToolTip(b, "Sends the prompt to the GPT-3")
-        b = buttons.add_button("Extend prompt", self.extend_prompt_callback, width=-1)
+        b = self.action_buttons.add_button("Extend prompt", self.extend_prompt_callback, width=-1)
         ToolTip(b, "Uses the previous prompt and response as the new prompt")
-        b = buttons.add_button("Parse response", self.parse_response_callback, width=-1)
+        b = self.action_buttons.add_button("Parse response", self.parse_response_callback, width=-1)
         ToolTip(b, "Applies the regex in the 'Parse Regex' field to each line in the resonse text \nthat is longer than Max Chars and places the parsed results in the 'Test Keyords' area below")
-        row = buttons.get_next_row()
+        row = self.action_buttons.get_next_row()
 
     def build_gpt_params(self, lf:tk.LabelFrame, text_width:int, label_width:int):
         row = 0
         self.token_list = ListField(lf, row, "Tokens", width=text_width, label_width=label_width, static_list=True)
         self.token_list.set_text(text='32, 64, 128, 256')
         self.token_list.set_callback(self.set_tokens_callback)
         ToolTip(self.token_list.tk_list, "Sets the maxumum number of tokens that the GPT can use in a response")
         row = self.token_list.get_next_row()
 
+        engine_list = self.oai.list_models(exclude_list = [":", "ada", "embed", "similarity", "code", "edit", "search", "audio", "instruct", "2020", "if", "insert", "whisper"])
+        engine_list = sorted(engine_list, reverse=True)
         self.engine_list = ListField(lf, row, "Engines", width=text_width, label_width=label_width, static_list=True)
-        self.engine_list.set_text(list=self.oai.engines)
+        self.engine_list.set_text(list=engine_list)
         self.engine_list.set_callback(self.set_engine_callback)
         ToolTip(self.engine_list.tk_list, "Sets the GPT engine. Includes the original and most recent engines")
         row = self.engine_list.get_next_row()
         #
         # lbl = tk.Label(lf, text="Tokens", width=label_width, bg="red")
         # lbl.grid(row=row, column=0, sticky="w", padx=2, pady=2)
 
@@ -130,26 +134,26 @@
                 "List of terms to search.\nTerms can have spaces or be combined with OR:\nNorth Korea\nSouth Korea\nNorth Korea OR South Korea")
         row = self.keyword_text_field.get_next_row()
 
         self.start_date_field = DateEntryField(lf, row, 'Start Date', text_width, label_width=label_width)
         row = self.start_date_field.get_next_row()
         self.end_date_field = DateEntryField(lf, row, 'End Date', text_width, label_width=label_width)
         row = self.end_date_field.get_next_row()
-        buttons = Buttons(lf, row, "Actions", label_width=label_width)
-        b = buttons.add_button("Clear", self.clear_counts_callbacks, width=-1)
+        self.action_buttons2 = Buttons(lf, row, "Actions", label_width=label_width)
+        b = self.action_buttons2.add_button("Clear", self.clear_counts_callbacks, width=-1)
         ToolTip(b, "Clears any old data from the plot")
-        b = buttons.add_button("Test Keyword", self.test_keyword_callback, width=-1)
+        b = self.action_buttons2.add_button("Test Keyword", self.test_keyword_callback, width=-1)
         ToolTip(b, "Query Twitter for each keyword and plot")
-        b = buttons.add_button("Plot", self.plot_counts_callback, width=-1)
+        b = self.action_buttons2.add_button("Plot", self.plot_counts_callback, width=-1)
         ToolTip(b, "Plot the current data")
-        b = buttons.add_button("Save", self.save_callback, width=-1)
+        b = self.action_buttons2.add_button("Save", self.save_callback, width=-1)
         ToolTip(b, "Save the results as an xlsx file")
-        b = buttons.add_button("Launch Twitter", self.launch_twitter_callback, width=-1)
+        b = self.action_buttons2.add_button("Launch Twitter", self.launch_twitter_callback, width=-1)
         ToolTip(b, "Open tabs in the default browser for each term over the time period")
-        row = buttons.get_next_row()
+        row = self.action_buttons2.get_next_row()
 
     def build_twitter_params(self, lf:tk.LabelFrame, text_width:int, label_width:int):
         row = 0
         self.sample_list = ListField(lf, row, "Sample", width=text_width, label_width=label_width, static_list=True)
         self.sample_list.set_text(text='day, week, month')
         self.sample_list.set_callback(self.set_time_sample_callback)
         self.set_time_sample_callback()
@@ -171,15 +175,16 @@
     def save_experiment_text(self, filename:str):
         s = self.prompt_text_field.get_text()
         with open(filename, mode="w", encoding="utf8") as f:
             f.write(s)
 
     def set_engine_callback(self, event:tk.Event = None):
         engine_str = self.engine_list.get_selected()
-        self.engine_list.set_label("Engines\n({})".format(engine_str))
+        self.oai.engine = engine_str
+        self.engine_list.set_label("Engines\n{}".format(engine_str))
 
     def set_tokens_callback(self, event:tk.Event = None):
         token_str = self.token_list.get_selected()
         self.token_list.set_label("Tokens\n({})".format(token_str))
 
     def set_time_sample_callback(self, event:tk.Event = None):
         sample_str = self.sample_list.get_selected()
@@ -215,24 +220,27 @@
             #s = '\n'.join(response_list)
             self.keyword_text_field.set_text(s.strip())
         else:
             message.showwarning("Parse Error",
                                 "Could not parse [{}]".format(self.response_text_field.get_text()))
 
     def test_keyword_callback(self):
-        key_list = self.keyword_text_field.get_list("\n")
-        print(key_list)
+        l = self.keyword_text_field.get_list("\n")
+        print(l)
         start_dt = self.start_date_field.get_date()
         end_dt = self.end_date_field.get_date()
 
-        for keyword in key_list:
-            if len(keyword) < 3:
-                message.showwarning("Keyword too short",
-                                    "Please enter something longer than [{}] text area".format(keyword))
-                return
+        key_list = []
+        for keyword in l:
+            if len(keyword) > 2:
+                key_list.append(keyword)
+        if len(key_list) == 0:
+            message.showwarning("Keyword too short",
+                                "Please enter something longer than [{}] in the text area".format(keyword))
+            return
 
         tweet_options = self.query_options_field.get_text()
         granularity = self.sample_list.get_selected()
         log_dict = {"granularity":granularity, "twitter_start": start_dt.strftime("%Y-%m-%d"), "twitter_end":end_dt.strftime("%Y-%m-%d")}
         for keyword in key_list:
             if granularity == 'day':
                 self.tvc.get_counts(keyword, start_dt, end_time=end_dt, granularity=granularity, tweet_options=tweet_options)
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/Apps/ModelExplorer.py` & `keyword_explorer-0.5a0/keyword_explorer/Apps/ModelExplorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     twenty_percent:LabeledParam
     thirty_percent:LabeledParam
     forty_percent:LabeledParam
     flag_checkboxes:Checkboxes
     spreadsheet_checkbox:Checkbox
     seed_checkbox:Checkbox
     db_checkbox:Checkbox
+    action_buttons:Buttons
     msi: MySqlInterface
     sequence_regex:Pattern
     element_regex:Pattern
     pattern_counters:PatternCounters
     hgpt:HFaceGPT
     reuse_seed:bool
     db_flag:bool
@@ -103,17 +104,17 @@
         row = self.flag_checkboxes.get_next_row()
 
         self.probe_field = DataField(parent, row, "Probe:", text_width, label_width=label_width)
         ToolTip(self.probe_field.tk_entry, "Type your comma-separated search\n terms or phrase here")
         self.probe_field.set_text(']][[text: ')
         row = self.probe_field.get_next_row()
 
-        buttons = Buttons(parent, row, "Actions:", label_width)
-        buttons.add_button("Run", self.run_probe_callback)
-        row = buttons.get_next_row()
+        self.action_buttons = Buttons(parent, row, "Actions:", label_width)
+        self.action_buttons.add_button("Run", self.run_probe_callback)
+        row = self.action_buttons.get_next_row()
 
         self.gpt_response_frame = tk.Text(parent)
         self.gpt_response_frame.grid(row = row, column=0, columnspan = 2, sticky="nsew", padx=5, pady=2)
         text_scrollbar = ttk.Scrollbar(parent, orient=tk.VERTICAL, command=self.gpt_response_frame.yview)
         self.gpt_response_frame['yscrollcommand'] = text_scrollbar.set
         text_scrollbar.grid(column=2, row=row, rowspan=1, sticky=(tk.N, tk.S))
         ToolTip(self.gpt_response_frame, "Parsed responses from GPT are here")
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/Apps/TweetCountExplorer.py` & `keyword_explorer-0.5a0/keyword_explorer/Apps/TweetCountExplorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     keyword_text_field:TextField
     start_date_field:DateEntryField
     end_date_field:DateEntryField
     token_list:ListField
     engine_list:ListField
     sample_list:ListField
     query_options_field:DataField
+    action_buttons:Buttons
 
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.totals_dict = {}
         print("TweetCountExplorer")
 
@@ -67,26 +68,26 @@
         ToolTip(self.keyword_text_field.tk_text,
             "List of terms to search.\nTerms can have spaces or be combined with OR:\nNorth Korea\nSouth Korea\nNorth Korea OR South Korea")
         row = self.keyword_text_field.get_next_row()
         self.start_date_field = DateEntryField(lf, row, 'Start Date', text_width, label_width=label_width)
         row = self.start_date_field.get_next_row()
         self.end_date_field = DateEntryField(lf, row, 'End Date', text_width, label_width=label_width)
         row = self.end_date_field.get_next_row()
-        buttons = Buttons(lf, row, "Actions", label_width=label_width)
-        b = buttons.add_button("Clear", self.clear_counts_callbacks, width=-1)
+        self.action_buttons = Buttons(lf, row, "Actions", label_width=label_width)
+        b = self.action_buttons.add_button("Clear", self.clear_counts_callbacks, width=-1)
         ToolTip(b, "Clears any old data from the plot")
-        b = buttons.add_button("Test Keyword", self.test_keyword_callback, width=-1)
+        b = self.action_buttons.add_button("Test Keyword", self.test_keyword_callback, width=-1)
         ToolTip(b, "Query Twitter for each keyword and plot")
-        b = buttons.add_button("Plot", self.plot_counts_callback, width=-1)
+        b = self.action_buttons.add_button("Plot", self.plot_counts_callback, width=-1)
         ToolTip(b, "Plot the current data")
-        b = buttons.add_button("Save", self.save_callback, width=-1)
+        b = self.action_buttons.add_button("Save", self.save_callback, width=-1)
         ToolTip(b, "Save the results as an xlsx file")
-        b = buttons.add_button("Launch Twitter", self.launch_twitter_callback, width=-1)
+        b = self.action_buttons.add_button("Launch Twitter", self.launch_twitter_callback, width=-1)
         ToolTip(b, "Open tabs in the default browser for each term over the time period")
-        row = buttons.get_next_row()
+        row = self.action_buttons.get_next_row()
 
     def build_twitter_params(self, lf:tk.LabelFrame, text_width:int, label_width:int):
         row = 0
         self.sample_list = ListField(lf, row, "Sample", width=text_width, label_width=label_width, static_list=True)
         self.sample_list.set_text(text='day, week, month')
         self.sample_list.set_callback(self.set_time_sample_callback)
         ToolTip(self.sample_list.tk_list, "The sampling period\nWeek and month are subsamples")
@@ -114,23 +115,28 @@
 
     def test_keyword_callback(self):
         key_list = self.keyword_text_field.get_list("\n")
         print(key_list)
         start_dt = self.start_date_field.get_date()
         end_dt = self.end_date_field.get_date()
 
+        clean_list = []
+        keyword:str
         for keyword in key_list:
-            if len(keyword) < 3:
-                message.showwarning("Keyword too short",
-                                    "Please enter something longer than [{}] text area".format(keyword))
-                return
+            if len(keyword) > 2:
+                clean_list.append(keyword.strip())
+
+        if len(clean_list) == 0:
+            message.showwarning("Keyword(s) too short",
+                                "Please enter something longer than [{}] text area".format(key_list))
+            return
         tweet_options = self.query_options_field.get_text()
         granularity = self.sample_list.get_selected()
         log_dict = {"granularity":granularity, "twitter_start": start_dt.strftime("%Y-%m-%d"), "twitter_end":end_dt.strftime("%Y-%m-%d")}
-        for keyword in key_list:
+        for keyword in clean_list:
             if granularity == 'day':
                 self.tvc.get_counts(keyword, start_dt, end_time=end_dt, granularity=granularity, tweet_options=tweet_options)
                 print("testing keyword {} between {} and {} - granularity = {}".format(keyword, start_dt, end_dt, granularity))
             elif granularity == 'week':
                 self.tvc.get_sampled_counts(keyword, start_dt, end_time=end_dt, skip_days=7, tweet_options=tweet_options)
                 print("testing keyword {} between {} and {} - skip_days = {}".format(keyword, start_dt, end_dt, 7))
             elif granularity == 'month':
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/Apps/TweetDownloader.py` & `keyword_explorer-0.5a0/keyword_explorer/Apps/TweetDownloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     samples_field:DataField
     clamp_field:DataField
     corpus_size_field:DataField
     lowest_count_field:DataField
     highest_count_field:DataField
     percent_field:DataField
     query_options_field:DataField
+    collect_buttons:Buttons
+    analytics_buttons:Buttons
     # option_checkboxes:Checkboxes
     experiment_combo: TopicComboExt
     db_option_checkboxes: Checkboxes
     db_write_cb: Checkbox
     keyword_data_list:List
     randomize:bool
     hour_offset:int
@@ -67,15 +69,15 @@
         self.randomize = False
         self.hour_offset = 0 # offset from zulu
         self.set_experiment_id(-1)
         print("TweetDownloader.init()")
 
     def setup_app(self):
         self.app_name = "TweetDownloader"
-        self.app_version = "11.14.22"
+        self.app_version = "03.24.2023"
         self.geom = (1000, 560)
         self.console_lines = 10
         self.text_width = 70
 
         self.tkws = TweetKeywords()
         self.msi = MySqlInterface(user_name ="root", db_name ="twitter_v2")
         if not self.tkws.key_exists():
@@ -114,30 +116,29 @@
         self.duration_field = DataField(lf, row, 'Duration:', int(text_width/2), label_width=label_width)
         ToolTip(self.duration_field.tk_entry, "How many days in the pull\nCalculted from the start and stop dates")
         b = self.duration_field.add_button("set start", self.set_start_callback)
         ToolTip(b, "Reset the start date based on the end date and duration")
         b = self.duration_field.add_button("set end", self.set_end_callback)
         ToolTip(b, "Reset the end date based on the start date and duration")
         row = self.duration_field.get_next_row()
-        buttons = Buttons(lf, row, "Collect:", label_width=label_width)
-        b = buttons.add_button("Balanced", self.collect_balanced_callback)
+        self.collect_buttons = Buttons(lf, row, "Collect:", label_width=label_width)
+        b = self.collect_buttons.add_button("Balanced", self.collect_balanced_callback)
         ToolTip(b, "Collect the same number (Samples/Clamp) of tweets per day for each item\nUses each day's smallest count")
-        b = buttons.add_button("Percent", self.collect_percent_callback)
+        b = self.collect_buttons.add_button("Percent", self.collect_percent_callback)
         ToolTip(b, "Collect a proportional (Percent) sample with\nan upper clamp (Samples/Clamp) per day for all terms\nMinimum of 10 samples per day")
-        row = buttons.get_next_row()
-        b = buttons.add_button("Threads", self.collect_thread_callback)
+        b = self.collect_buttons.add_button("Threads", self.collect_thread_callback)
         ToolTip(b, "Collect all the treads that are associated with the downloaded tweets. \nReliably works for the past 7 days but *may also* work over longer times")
-        row = buttons.get_next_row()
+        row = self.collect_buttons.get_next_row()
 
-        buttons = Buttons(lf, row, "Analytics:", label_width=label_width)
-        b = buttons.add_button("Calc rates", self.calc_rates_callback)
+        self.analytics_buttons = Buttons(lf, row, "Analytics:", label_width=label_width)
+        b = self.analytics_buttons.add_button("Calc rates", self.calc_rates_callback)
         ToolTip(b, "Gets the rough number of tweets per day per term\n and prints to the Console window")
-        b = buttons.add_button("Browser", self.launch_twitter_callback)
+        b = self.analytics_buttons.add_button("Browser", self.launch_twitter_callback)
         ToolTip(b, "Open tabs in the default browser for each term over the time period")
-        row = buttons.get_next_row()
+        row = self.analytics_buttons.get_next_row()
 
     def build_twitter_params(self, lf:tk.LabelFrame, text_width:int, label_width:int):
         row = 0
         self.samples_field = DataField(lf, row, 'Sample (10-500):', text_width, label_width=label_width)
         self.samples_field.set_text(TweetKeywords.max_tweets_per_sample)
         ToolTip(self.samples_field.tk_entry, "The sample size (10 - 500)")
         row = self.samples_field.get_next_row()
@@ -266,14 +267,26 @@
 
     def set_end_callback(self):
         duration = int(self.duration_field.get_text())
         start_dt = self.start_date_field.get_date()
         end_dt = start_dt + timedelta(days = duration)
         self.end_date_field.set_date(end_dt)
 
+    def clean_key_list(self, key_list) -> List:
+        clean_list = []
+        keyword:str
+        for keyword in key_list:
+            if len(keyword) > 2:
+                clean_list.append(keyword.strip())
+
+        if len(clean_list) == 0:
+            message.showwarning("Keyword(s) too short",
+                                "Please enter something longer than [{}] text area".format(key_list))
+        return clean_list
+
     def collect_thread_callback(self):
         row_dict:Dict
         tk:TweetKeyword
         tk_list = []
         tweets_to_download = self.thread_length.get_as_int()
         self.tkws.set_query_params(self.query_options_field.get_text())
 
@@ -305,14 +318,15 @@
     def collect_percent_callback(self):
         self.tkws.set_query_params(self.query_options_field.get_text())
         date_fmt = "%B %d, %Y (%H:%M:%S)"
         percent = self.percent_field.get_as_int()
         clamp = self.clamp_field.get_as_int()
         # get the keywords
         key_list = self.keyword_text_field.get_list("\n")
+        key_list = self.clean_key_list(key_list)
         # set up the counters for corpus size
         corpus_size_dict = {}
         for s in key_list:
             corpus_size_dict[s] = KeywordData(s)
 
         # get the entire date range
         cur_dt = self.start_date_field.get_date()
@@ -381,14 +395,15 @@
         # get the max number of samples that we want to get per day
         clamp = self.clamp_field.get_as_int()
         # get the sample size
         tweets_per_sample = self.samples_field.get_as_int()
 
         # get the keywords
         key_list = self.keyword_text_field.get_list("\n")
+        key_list = self.clean_key_list(key_list)
         # set up the counters for corpus size
         corpus_size_dict = {}
         for s in key_list:
             corpus_size_dict[s] = KeywordData(s)
 
         # get the entire date range
         cur_dt = self.start_date_field.get_date()
@@ -452,14 +467,15 @@
 
         print("collect_individual_callback(): done")
 
 
     def calc_rates_callback(self):
         corpus_size = int(self.corpus_size_field.get_text())
         key_list = self.keyword_text_field.get_list("\n")
+        key_list = self.clean_key_list(key_list)
         start_dt = self.start_date_field.get_date()
         i = 0
         highest = KeywordData("unset", 0)
         lowest = KeywordData("unset", 0)
         self.dp.clear()
         self.keyword_data_list = []
         for s in key_list:
@@ -487,14 +503,15 @@
         self.keyword_data_list.sort(key=lambda kd:kd.num_tweets)
         for kd in self.keyword_data_list:
             print(kd.to_string())
 
     def launch_twitter_callback(self):
         # single word
         key_list = self.keyword_text_field.get_list("\n")
+        key_list = self.clean_key_list(key_list)
         start_dt = self.start_date_field.get_date()
         end_dt = self.end_date_field.get_date()
         self.log_action("Launch_twitter", {"twitter_start": start_dt.strftime("%Y-%m-%d"), "twitter_end":end_dt.strftime("%Y-%m-%d"), "terms":" ".join(key_list)})
         self.tkws.launch_twitter(key_list, start_dt, end_dt)
         # webbrowser.open('https://twitter.com/search?q=chinavirus%20until%3A2020-02-01%20since%3A2019-12-01&src=typed_query')
         # webbrowser.open('https://twitter.com/search?q=%22china%20virus%22%20until%3A2020-02-01%20since%3A2019-12-01&src=typed_query')
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/Apps/TweetEmbedExplorer.py` & `keyword_explorer-0.5a0/keyword_explorer/Apps/NarrativeExplorer2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,532 +1,605 @@
+'''
+Load - Loads an existing experiment
+Model Selection - Various models of the GPT-3 or a local model
+Prompt - "Once upon a time there was." or potentially much longer, paragraph-sized so lots of room. Also UTF-8 to handle other languages
+Parameters - number of tokens, etc.
+Run - sends the prompt to the GPT and gets the text response. A checkbox indicates if there should be automatic embedding
+Clear embeddings
+Get Embeddings
+Extend - uses the existing prompt and response as a prompt
+Cluster - happens on line boundaries. There should be an editable regex for that. Same sort of PCA/T-SNE as embedding explorer, which means there needs to be parameter tweaking. Clustering will have to be re-run multiple times, though I hope the embedding step is run once. To avoid the complexity of the interactive plotting, I think I'll just label the clusters (https://stackoverflow.com/questions/44998205/labeling-points-in-matplotlib-scatterplot)
+Query - 1) Run cluster queries on the DB. Select the cluster ID and the number of responses. 2) Get the number of responses per cluster
+Save - stores the text on a sentence-by sentence bases with clustering info
+Generate Graph - runs through each narrative in an experiment to produce a directed graph of nodes. The output is all the narratives threaded together. Used as an input to Gephi
+'''
+import os
 import re
-import tkinter.messagebox as message
+import getpass
+import math
+import numpy as np
 import tkinter as tk
 from tkinter import ttk
+import tkinter.messagebox as message
+from datetime import datetime
+from tkinter import filedialog
 from matplotlib import pyplot as plt
 import matplotlib.colors as mcolors
 
+import pandas as pd
+
 from keyword_explorer.Apps.AppBase import AppBase
-from keyword_explorer.OpenAI.OpenAIComms import OpenAIComms
-from keyword_explorer.TwitterV2.TweetKeywords import TweetKeywords
-from keyword_explorer.tkUtils.CanvasFrame import CanvasFrame
-from keyword_explorer.tkUtils.TopicComboExt import TopicComboExt
-from keyword_explorer.tkUtils.DataField import DataField
-from keyword_explorer.tkUtils.LabeledParam import LabeledParam
 from keyword_explorer.tkUtils.Buttons import Buttons
 from keyword_explorer.tkUtils.ToolTip import ToolTip
-from keyword_explorer.tkUtils.MoveableNode import MovableNode
-from keyword_explorer.tkUtils.Checkboxes import Checkboxes, DIR
+from keyword_explorer.tkUtils.GPT3GeneratorFrame import GPT3GeneratorSettings, GPT3GeneratorFrame
+from keyword_explorer.tkUtils.GPT3EmbeddingFrame import GPT3EmbeddingSettings, GPT3EmbeddingFrame
+from keyword_explorer.tkUtils.ListField import ListField
+from keyword_explorer.tkUtils.TextField import TextField
+from keyword_explorer.tkUtils.DataField import DataField
+from keyword_explorer.tkUtils.TopicComboExt import TopicComboExt
+from keyword_explorer.tkUtils.LabeledParam import LabeledParam
+from keyword_explorer.OpenAI.OpenAIComms import OpenAIComms
 from keyword_explorer.utils.MySqlInterface import MySqlInterface
-from keyword_explorer.utils.ManifoldReduction import ManifoldReduction, EmbeddedText
-from keyword_explorer.utils.CorporaGenerator import CorporaGenerator
+from keyword_explorer.utils.ManifoldReduction import ManifoldReduction, EmbeddedText, ClusterInfo
+from keyword_explorer.utils.SharedObjects import SharedObjects
+from keyword_explorer.utils.NetworkxGraphing import NetworkxGraphing
 
-from typing import Dict, List, Any
+from typing import List, Dict
 
-# General TODO:
-# Move "selected experiment" and "keyword" out of the tabs
-# Add a "Create Corpora" tab
-# Implement calls to GPT embeddings and verify on small dataset. I could even try Aaron's Wikipedia cats vs computers idea but use tweets
-class EmbeddingsExplorer(AppBase):
+class NarrativeExplorer2(AppBase):
     oai: OpenAIComms
     msi: MySqlInterface
     mr: ManifoldReduction
-    cg: CorporaGenerator
-    canvas_frame: CanvasFrame
-    engine_combo: TopicComboExt
-    keyword_combo: TopicComboExt
-    graph_keyword_combo: TopicComboExt
+    so:SharedObjects
+    generator_frame: GPT3GeneratorFrame
+    embedding_frame: GPT3EmbeddingFrame
     experiment_combo: TopicComboExt
-    keyword_count_field: DataField
-    exclude_cluster_field: DataField
-    pca_dim_param: LabeledParam
-    eps_param: LabeledParam
-    min_samples_param: LabeledParam
-    perplexity_param: LabeledParam
-    rows_param: LabeledParam
-    tweet_option_checkboxes:Checkboxes
-    author_option_checkboxes:Checkboxes
-    generation_options:Checkboxes
-    experiment_id: int
+    recurse_depth_list:ListField
+    style_list:ListField
+    new_experiment_button:Buttons
+    embed_state_text_field:TextField
+    embedded_field:DataField
+    reduced_field:DataField
+    experiment_id:int
+    run_id:int
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        print("EmbeddingsExplorer")
+        print("NarrativeExplorer")
+        self.text_width = 60
+        self.label_width = 15
+
+        dt = datetime.now()
+        experiment_str = "{}_{}_{}".format(self.app_name, getpass.getuser(), dt.strftime("%H:%M:%S"))
+        self.experiment_field.set_text(experiment_str)
+        self.load_experiment_list()
+
+        self.so.add_object("experiment_field", self.experiment_field, DataField)
+        self.so.add_object("clusters_field", self.clusters_field, DataField)
+        self.so.add_object("reduced_field", self.reduced_field, DataField)
+        self.so.print_contents()
+        # self.test_data_callback()
 
     def setup_app(self):
-        self.app_name = "EmbeddingsExplorer"
-        self.app_version = "11.8.22"
-        self.geom = (600, 620)
+        self.app_name = "NarrativeExplorer2"
+        self.app_version = "3.30.2023"
+        self.geom = (870, 670)
         self.oai = OpenAIComms()
-        self.tkws = TweetKeywords()
-        self.msi = MySqlInterface(user_name="root", db_name="twitter_v2")
+        self.msi = MySqlInterface(user_name="root", db_name="narrative_maps")
         self.mr = ManifoldReduction()
-        self.cg = CorporaGenerator(self.msi)
+        self.so = SharedObjects()
 
         if not self.oai.key_exists():
             message.showwarning("Key Error", "Could not find Environment key 'OPENAI_KEY'")
 
-        if not self.tkws.key_exists():
-            message.showwarning("Key Error", "Could not find Environment key 'BEARER_TOKEN_2'")
         self.experiment_id = -1
-
+        self.run_id = -1
 
     def build_app_view(self, row: int, text_width: int, label_width: int) -> int:
-        experiments = ["exp_1", "exp_2", "exp_3"]
-        keywords = ["foo", "bar", "bas"]
         print("build_app_view")
+        self.generator_frame = GPT3GeneratorFrame(self.oai, self.dp, self.so)
+        self.embedding_frame = GPT3EmbeddingFrame(self.oai, self.mr, self.dp, self.so)
+        lf = tk.LabelFrame(self, text="GPT")
+        lf.grid(row=row, column=0, columnspan = 2, sticky="nsew", padx=5, pady=2)
+        self.build_gpt(lf, text_width, label_width)
+
+        lf = tk.LabelFrame(self, text="Params")
+        lf.grid(row=row, column=2, sticky="nsew", padx=5, pady=2)
+        self.build_params(lf, int(text_width/3), int(label_width*.75))
 
-        self.experiment_combo = TopicComboExt(self, row, "Experiment:", self.dp, entry_width=20, combo_width=20)
+        return row + 1
+
+    def build_menus(self):
+        print("building menus")
+        self.option_add('*tearOff', tk.FALSE)
+        menubar = tk.Menu(self)
+        self['menu'] = menubar
+        menu_file = tk.Menu(menubar)
+        menubar.add_cascade(menu=menu_file, label='File')
+        menu_file.add_command(label='Load params', command=self.load_params_callback)
+        menu_file.add_command(label='Save params', command=self.save_params_callback)
+        menu_file.add_command(label='Load IDs', command=self.load_ids_callback)
+        menu_file.add_command(label='Test data', command=self.generator_frame.test_data_callback)
+        menu_file.add_command(label='Exit', command=self.terminate)
+
+    def load_experiment_list(self):
+        experiments = []
+        results = self.msi.read_data("select name from table_experiment")
+        for r in results:
+            experiments.append(r['name'])
         self.experiment_combo.set_combo_list(experiments)
-        self.experiment_combo.set_callback(self.keyword_callback)
+
+    def build_gpt(self, lf:tk.LabelFrame, text_width:int, label_width:int):
+        row = 0
+        self.experiment_combo = TopicComboExt(lf, row, "Saved Experiments:", self.dp, entry_width=20, combo_width=20)
+        self.experiment_combo.set_callback(self.load_experiment_callback)
         row = self.experiment_combo.get_next_row()
-        ToolTip(self.experiment_combo.tk_combo, "Select the experiment you want to explore here")
-        self.keyword_combo = TopicComboExt(self, row, "Keyword:", self.dp, entry_width=20, combo_width=20)
-        self.keyword_combo.set_combo_list(keywords)
-        ToolTip(self.keyword_combo.tk_combo, "Select the keyword for the experiment. 'all_keywords' gets everything")
-        b = self.keyword_combo.add_button("Num Entries:", command=lambda: self.get_keyword_entries_callback(
-            self.keyword_combo.get_text()))
-        ToolTip(b, "Query the DB to see how many entries there are\nResults go in 'Num Rows:'")
-        row = self.keyword_combo.get_next_row()
+        self.new_experiment_button = Buttons(lf, row, "Experiments")
+        b = self.new_experiment_button.add_button("Create", self.create_experiment_callback)
+        ToolTip(b, "Create a new, named experiment")
+        b = self.new_experiment_button.add_button("Load", self.load_experiment_callback)
+        ToolTip(b, "Load an existing experiment")
+        b = self.new_experiment_button.add_button("Update", self.update_experiment_callback)
+        ToolTip(b, "Update an existing experiment")
+        row = self.new_experiment_button.get_next_row()
 
         s = ttk.Style()
         s.configure('TNotebook.Tab', font=self.default_font)
 
         # Add the tabs
-        tab_control = ttk.Notebook(self)
+        tab_control = ttk.Notebook(lf)
         tab_control.grid(column=0, row=row, columnspan=2, sticky="nsew")
-        get_store_tab = ttk.Frame(tab_control)
-        tab_control.add(get_store_tab, text='Get/Store')
-        self.build_get_store_tab(get_store_tab)
-
-        canvas_tab = ttk.Frame(tab_control)
-        tab_control.add(canvas_tab, text='Canvas')
-        self.build_graph_tab(canvas_tab)
-
-        corpora_tab = ttk.Frame(tab_control)
-        tab_control.add(corpora_tab, text='Corpora')
-        self.build_create_corpora_tab(corpora_tab)
-        row += 1
+        gpt_tab = ttk.Frame(tab_control)
+        tab_control.add(gpt_tab, text='Generate')
+        self.build_generator_tab(gpt_tab, text_width, label_width)
+
+        embed_tab = ttk.Frame(tab_control)
+        tab_control.add(embed_tab, text='Embedding')
+        self.build_embed_tab(embed_tab, text_width, label_width)
 
+        row += 1
         return row
 
-    def build_create_corpora_tab(self, tab: ttk.Frame):
-        label_width = 20
-        row = 0
-        self.tweet_option_checkboxes = Checkboxes(tab, row, "Tweet meta wrapping:", label_width=label_width, border=True)
-        # cb = self.tweet_option_checkboxes.add_checkbox("Randomize", self.randomize_callback, dir=DIR.ROW)
-        # ToolTip(cb, "Randomly select the starting time for each day so that a full pull won't go into tomorrow")
-        cb = self.tweet_option_checkboxes.add_checkbox("Created at", lambda : self.set_corpora_flag_callback("tweet_created_at_flag"), dir=DIR.ROW)
-        ToolTip(cb.cb, "Adds the date and time the tweet was created to the tweet meta-wrapping")
-        cb = self.tweet_option_checkboxes.add_checkbox("Language", lambda: self.set_corpora_flag_callback("language_flag"), dir=DIR.ROW)
-        ToolTip(cb.cb, "Adds the tweet language to the tweet meta-wrapping")
-        cb = self.tweet_option_checkboxes.add_checkbox("Keyword", lambda: self.set_corpora_flag_callback("keyword_flag"), dir=DIR.ROW)
-        ToolTip(cb.cb, "Adds the keyword to the tweet meta-wrapping")
-        cb = self.tweet_option_checkboxes.add_checkbox("Exclude threaded tweets", lambda: self.set_corpora_flag_callback("exclude_thread_flag"), dir=DIR.ROW)
-        ToolTip(cb.cb, "Excludes tweets that are in threads connected\nto a tweet containing the keyword")
-        row = self.tweet_option_checkboxes.get_next_row()
-        self.author_option_checkboxes = Checkboxes(tab, row, "Author meta wrapping:", label_width=label_width, border=True)
-        cb = self.author_option_checkboxes.add_checkbox("Name", lambda: self.set_corpora_flag_callback("name_flag"), dir=DIR.ROW)
-        ToolTip(cb.cb, "Adds the tweet author's name to the tweet meta-wrapping")
-        cb = self.author_option_checkboxes.add_checkbox("Username", lambda: self.set_corpora_flag_callback("username_flag"), dir=DIR.ROW)
-        ToolTip(cb.cb, "Adds the tweet author's username to the tweet meta-wrapping")
-        cb = self.author_option_checkboxes.add_checkbox("Location", lambda: self.set_corpora_flag_callback("location_flag"), dir=DIR.ROW)
-        ToolTip(cb.cb, "Adds the tweet author's location to the tweet meta-wrapping")
-        cb = self.author_option_checkboxes.add_checkbox("Description", lambda: self.set_corpora_flag_callback("description_flag"), dir=DIR.ROW)
-        ToolTip(cb.cb, "Adds the tweet author's self-description to the tweet meta-wrapping")
-        row = self.author_option_checkboxes.get_next_row()
-        self.generation_options = Checkboxes(tab, row, "Corpora Generation:", label_width=label_width, border=True)
-        cb = self.generation_options.add_checkbox("Wrapping before text (default is after)", lambda: self.set_corpora_flag_callback("wrap_after_text_flag"), dir=DIR.ROW)
-        ToolTip(cb.cb, "Check to place the meta-wrapping before the tweet text")
-        cb = self.generation_options.add_checkbox("Single file (default is separate)", lambda: self.set_corpora_flag_callback("single_file_flag"), dir=DIR.ROW)
-        ToolTip(cb.cb, "Generate a single test/train set with all keywords in it\nrather than a separate test/trin file for each keyword")
-        cb = self.generation_options.add_checkbox("Percent OFF (default is ON)", lambda: self.set_corpora_flag_callback("percent_on_flag"), dir=DIR.ROW)
-        ToolTip(cb.cb, "Disable the generation of percent values in the meta-wrapping to determine learning accuracy (10%, 20%, 30%, 40%")
-        cb = self.generation_options.add_checkbox("Include excluded clusters", lambda: self.set_corpora_flag_callback("excluded_culsters_flag"), dir=DIR.ROW)
-        ToolTip(cb.cb, "Include all clusters that were flagged for exclusion")
-        row = self.generation_options.get_next_row()
-        buttons = Buttons(tab, row, "Corpora")
-        b = buttons.add_button("Set folder", self.cg.set_folder)
-        ToolTip(b, "Set the folder for all test/train files to be written to")
-        b = buttons.add_button("Generate", lambda: self.cg.write_files(self.experiment_id, self.keyword_combo.get_text()))
-        ToolTip(b, "Write all test/train files to the selected directory")
-
-
-    def build_get_store_tab(self, tab: ttk.Frame):
-        engine_list = ['text-similarity-ada-001',
-                       'text-similarity-babbage-001',
-                       'text-similarity-curie-001',
-                       'text-similarity-davinci-001']
+    def build_params(self, lf:tk.LabelFrame, text_width:int, label_width:int):
         row = 0
-        self.engine_combo = TopicComboExt(tab, row, "Engine:", self.dp, entry_width=20, combo_width=20)
-        self.engine_combo.set_combo_list(engine_list)
-        self.engine_combo.set_text(engine_list[0])
-        self.engine_combo.tk_combo.current(0)
-        row = self.engine_combo.get_next_row()
-        ToolTip(self.engine_combo.tk_combo, "Select the embedding engine.\nAda is the cheapest, Davinci is the best")
-        self.keyword_count_field = DataField(tab, row, "Num rows")
-        b = self.keyword_count_field.add_button("Get Embeddings", self.get_oai_embeddings_callback)
-        row = self.keyword_count_field.get_next_row()
-        ToolTip(b, "Get embeddings for each tweet using the\nselected engine and store them with the\ntweets in the DB")
-        buttons = Buttons(tab, row, "Update DB")
-        b = buttons.add_button("Reduced+Clusters", self.store_reduced_and_clustering_callback, -1)
-        ToolTip(b, "Add cluster ids and reduced embeddings (from the Canvas tab)\n to the db along with each tweet")
-        b = buttons.add_button("Clusters", self.store_clustering_callback, -1)
-        ToolTip(b, "Add just the cluster ids (from the Canvas tab)\n to the db along with each tweet")
-        b = buttons.add_button("Topic Names", self.implement_me, -1)
-        ToolTip(b, "Not implemented. Will guess at topic names using GPT-3")
-        b = buttons.add_button("Users", self.store_user_callback, -1)
-        ToolTip(b, "Fora each tweet's user id, create an\nentry in the db for that user using\n the twitter API")
-        row = buttons.get_next_row()
+        self.runs_field = DataField(lf, row, 'Runs:', text_width, label_width=label_width)
+        row = self.runs_field.get_next_row()
+        self.parsed_field = DataField(lf, row, 'Parsed:', text_width, label_width=label_width)
+        row = self.parsed_field.get_next_row()
+        self.embedded_field = DataField(lf, row, 'Embeds:', text_width, label_width=label_width)
+        row = self.embedded_field.get_next_row()
+        self.reduced_field = DataField(lf, row, 'Reduced:', text_width, label_width=label_width)
+        row = self.reduced_field.get_next_row()
+        self.clusters_field = DataField(lf, row, 'Clusters:', text_width, label_width=label_width)
+        row = self.clusters_field.get_next_row()
+        self.style_list = ListField(lf, row, "Style", width=text_width, label_width=label_width, static_list=True)
+        self.style_list.set_text(text='Story, List, Sequence')
+        self.style_list.set_callback(self.set_style_callback)
+        ToolTip(self.style_list.tk_list, "Creates a narrative or recursive context for generation - Not implemented")
+        row = self.style_list.get_next_row()
+        self.recurse_depth_list = ListField(lf, row, "Depth\n(2)", width=text_width, label_width=label_width, static_list=True)
+        self.recurse_depth_list.set_text(text='2, 3, 4, 5')
+        self.recurse_depth_list.set_callback(self.set_recurse_depth_callback)
+        ToolTip(self.recurse_depth_list.tk_list, "The  recursion depth for lists - Not implemented")
+        row = self.recurse_depth_list.get_next_row()
+
+    def build_generator_tab(self, tab: ttk.Frame, text_width:int, label_width:int):
+        self.generator_frame.build_frame(tab, text_width, label_width)
+        self.generator_frame.add_button("Save", self.save_text_list_callback, "Manually saves the result to the database")
+        self.generator_frame.add_button("Automate", self.automate_callback, "Automatically runs probes, parses, and stores the results\n the number of times in the 'Run Count' field")
+
+    def build_embed_tab(self, tab: ttk.Frame, text_width:int, label_width:int):
+        self.embedding_frame.build_frame(tab, text_width, label_width)
+        self.embedding_frame.add_button("GPT embed", self.get_oai_embeddings_callback, "Get source embeddings from the GPT")
+        self.embedding_frame.add_button("Retreive", self.get_db_embeddings_callback, "Get the high-dimensional embeddings from the DB")
+        self.embedding_frame.add_button("Export", self.export_network_callback, "Plot and Export the graph to GML")
 
-    def build_param_row(self, parent:tk.Frame, row:int) -> int:
+    def build_embed_params(self, parent:tk.Frame, row:int) -> int:
         f = tk.Frame(parent)
         f.grid(row=row, column=0, columnspan=2, sticky="nsew", padx=1, pady=1)
         self.pca_dim_param = LabeledParam(f, 0, "PCA Dim:")
         self.pca_dim_param.set_text('10')
         ToolTip(self.pca_dim_param.tk_entry, "The number of dimensions that the PCA\nwill reduce the original vectors to")
         self.eps_param = LabeledParam(f, 2, "EPS:")
         self.eps_param.set_text('8')
         ToolTip(self.eps_param.tk_entry, "DBSCAN: Specifies how close points should be to each other to be considered a part of a \ncluster. It means that if the distance between two points is lower or equal to \nthis value (eps), these points are considered neighbors.")
         self.min_samples_param = LabeledParam(f, 4, "Min Samples:")
         self.min_samples_param.set_text('5')
         ToolTip(self.min_samples_param.tk_entry, "DBSCAN: The minimum number of points to form a dense region. For \nexample, if we set the minPoints parameter as 5, then we need at least 5 points \nto form a dense region.")
         self.perplexity_param = LabeledParam(f, 6, "Perplex:")
         self.perplexity_param.set_text('80')
         ToolTip(self.perplexity_param.tk_entry, "T-SNE: The size of the neighborhood around each point that \nthe embedding attempts to preserve")
-        self.rows_param = LabeledParam(f, 8, "Limit:")
-        self.rows_param.set_text('1000')
-        ToolTip(self.rows_param.tk_entry, "The number of rows that the full list will be subsampled down to\nfor performance")
         return row + 1
 
-    def build_graph_tab(self, tab: ttk.Frame):
-        row = 0
-        row = self.build_param_row(tab, row)
-        f = tk.Frame(tab)
-        # add "select clusters" field and "export corpus" button
-        buttons = Buttons(tab, row, "Commands", label_width=10)
-        b = buttons.add_button("Retreive", self.retreive_tweet_data_callback, -1)
-        ToolTip(b, "Get the high-dimensional embeddings from the DB")
-        b = buttons.add_button("Reduce", self.reduce_dimensions_callback, -1)
-        ToolTip(b, "Reduce to 2 dimensions with PCS and TSNE")
-        b = buttons.add_button("Cluster", self.cluster_callback, -1)
-        ToolTip(b, "Compute clusters on reduced data")
-        b = buttons.add_button("Plot", self.plot_callback, -1)
-        ToolTip(b, "Plot the clustered points using PyPlot")
-        b = buttons.add_button("Explore", self.explore_callback, -1)
-        ToolTip(b, "Interactive graph of a subsample of points")
-        b = buttons.add_button("Topics", self.label_clusters_callback, -1)
-        ToolTip(b, "Use GPT to guess at topic names for clusters\n(not implemented)")
-        row = buttons.get_next_row()
+    def count_parsed(self, experiment_id):
+        sql = "select * from parsed_view where experiment_id = %s"
+        vals = (experiment_id,)
+        results = self.msi.read_data(sql, vals)
+        run_set = set()
+        parsed_set = set()
+        embed_set = set()
+        reduced_set = set()
+        clusters_set = set()
+        d:Dict
+        for d in results:
+            if d['run_index'] != None:
+                run_set.add(d['run_index'])
+            if d['embedding'] != None:
+                embed_set.add(d['embedding'])
+            if d['parsed_text'] != None:
+                parsed_set.add(d['parsed_text'])
+            if d['mapped'] != None:
+                reduced_set.add(d['mapped'])
+            if d['cluster_id'] != None:
+                clusters_set.add(d['cluster_id'])
+
+        self.runs_field.set_text(len(run_set))
+        self.parsed_field.set_text(len(parsed_set))
+        self.embedded_field.set_text(len(embed_set))
+        self.reduced_field.set_text(len(reduced_set))
+        self.clusters_field.set_text(len(clusters_set))
+
+    def get_list(self, to_parse:str, regex_str:str = ",") -> List:
+        rlist = re.split(regex_str, to_parse)
+        to_return = []
+        for t in rlist:
+            if t != None:
+                to_return.append(t.strip())
+        to_return = [x for x in to_return if x] # filter out the blanks
+        return to_return
+
+    def set_style_callback(self, event:tk.Event = None):
+        style_str = self.style_list.get_selected()
+        self.style_list.set_label("Style\n({})".format(style_str))
+        if style_str == "Story":
+            print("Set story regex")
+        elif style_str == "List":
+            print("Set list regex")
+        elif style_str == "Sequence":
+            print("Set Sequence regex")
+
+    def set_recurse_depth_callback(self, event:tk.Event = None):
+        depth_str = self.recurse_depth_list.get_selected()
+        self.recurse_depth_list.set_label("Depth\n({})".format(depth_str))
+
+    def create_experiment_callback(self):
+        print("create_experiment_callback")
+        cur_date = datetime.now()
+        experiment_name = self.experiment_field.get_text()
+
+        if self.app_name in experiment_name:
+            result = tk.messagebox.askyesno("Warning!", "You are about to creat an experiment\nwith the default name{}\nProceed?".format(experiment_name))
+            print("result = {}".format(result))
+            if not result:
+                return
+        if "experiment" in experiment_name:
+            tk.messagebox.showwarning("Duplicate Experiment", "{} exists in db".format(experiment_name))
+            return
 
-        f = tk.Frame(tab)
-        f.grid(row=row, column=0, columnspan=2, sticky="nsew", padx=1, pady=1)
-        self.canvas_frame = CanvasFrame(f, 0, "Interactive embedding explorer (Mouse wheel to zoom)", self.dp, width=550, height=250)
-        self.canvas_frame.set_select_callback_fn(self.selected_node_callback)
+        sql = "insert into table_experiment (name, date) values (%s, %s)"
+        vals = (experiment_name, cur_date)
+        self.experiment_id = self.msi.write_sql_values_get_row(sql, vals)
+        self.load_experiment_list()
+        self.experiment_combo.clear()
+        self.experiment_combo.set_text(experiment_name)
 
-        row += 1
-        self.exclude_cluster_field = DataField(tab, row, "Exclude Cluster:")
-        b = self.exclude_cluster_field.add_button("Exclude", self.exclude_cluster_callback)
-        ToolTip(b, "Add cluster ID to the exclude table for this experiment")
-        row = self.exclude_cluster_field.get_next_row()
-
-    def color_excluded_clusters(self):
-        keyword = self.keyword_combo.get_text()
-        sql = "select * from table_exclude where experiment_id = %s and keyword = %s"
-        vals = (self.experiment_id, keyword)
-        if keyword == 'all_keywords':
-            sql = "select * from table_exclude where experiment_id = %s"
-            vals = (self.experiment_id, )
-        result = self.msi.read_data(sql, vals)
-        cluster_list = []
+    def load_experiment_callback(self, event = None):
+        print("load_experiment_callback")
+        s = self.experiment_combo.tk_combo.get()
+        self.experiment_combo.clear()
+        self.experiment_combo.set_text(s)
+        results = self.msi.read_data("select id from table_experiment where name = %s", (s,))
+        if len(results) > 0:
+            self.experiment_id = results[0]['id']
+            self.experiment_field.set_text(" experiment {}: {}".format(self.experiment_id, s))
+        print("experiment_callback: experiment_id = {}".format(self.experiment_id))
+        if self.experiment_id != -1:
+            sql = "select MAX(run_id) as max from table_run where experiment_id = %s"
+            vals = (self.experiment_id,)
+            results = self.msi.read_data(sql, vals)
+            print(results)
+            self.generator_frame.set_prompt("No prompt available in database")
+            self.runs_field.set_text('0')
+            self.count_parsed(self.experiment_id)
+            if results[0]['max'] != None:
+                run_id = results[0]['max']
+                #self.runs_field.set_text(run_id)
+                sql = "select * from run_params_view where run_id = %s and experiment_id = %s"
+                vals = (run_id, self.experiment_id)
+                results = self.msi.read_data(sql, vals)
+                d = results[0]
+
+                ggs = GPT3GeneratorSettings()
+                ggs.from_dict(d)
+                self.generator_frame.set_params(ggs)
+
+                ges = GPT3EmbeddingSettings()
+                ges.from_dict(d)
+                self.embedding_frame.set_params(ges)
+
+
+    def update_experiment_callback(self):
+        print("update_experiment_callback()")
+        if self.experiment_id == -1:
+            result = tk.messagebox.showwarning("Warning!", "Please create or select a database first")
+            return
+        params = self.get_current_params()
+        # update the table_embedding_params for this experiment/runs
+        sql = "select distinct emb_id from index_view where experiment_id = %s"
+        vals = (self.experiment_id,)
+        results = self.msi.read_data(sql, vals)
         d:Dict
-        for d in result:
-            cluster_list.append(d['cluster_id'])
+        for d in results:
+            embed_id = d['emb_id']
+            sql = "update table_embedding_params set model = %s, PCA_dim = %s, EPS = %s, min_samples = %s, perplexity = %s where id = %s"
+            vals = (params['embedding_model'], params['PCA_dimensions'], params['EPS'], params['min_samples'], params['perplexity'], embed_id)
+            self.msi.write_sql_values_get_row(sql, vals)
 
-        et:EmbeddedText
+        # update table_parsed_text with the reduced/mapped data
+        et: EmbeddedText
         for et in self.mr.embedding_list:
-            if et.cluster_id in cluster_list and et.mnode != None:
-                et.mnode.set_color("black")
+            reduced_s = np.array(et.reduced).dumps()
+            sql = "update table_parsed_text set mapped = %s, cluster_id = %s, cluster_name = %s where id = %s"
+            vals = (reduced_s, int(et.cluster_id), et.cluster_name, int(et.row_id))
+            self.msi.write_sql_values_get_row(sql, vals)
 
-    def safe_dict(self, d:Dict, name:str, default:Any) -> Any:
-        if name in d:
-            return d[name]
-        return default
-
-    def set_corpora_flag_callback(self, var_name:str):
-        print("set_corpora_flag_callback({})".format(var_name))
-        val = self.cg.set_by_name(var_name)
+        self.count_parsed(self.experiment_id)
 
-    def store_reduced_and_clustering_callback(self):
-        print("store_reduced_and_clustering_callback")
-        et:EmbeddedText
-        rows = 0
-        for et in self.mr.embedding_list:
-            sql = "update table_tweet set cluster_id = %s, cluster_name = %s, reduced = %s where row_id = %s;"
-            vals = (int(et.cluster_id), et.cluster_name, "{}".format(et.reduced), int(et.row_id))
-            print("store_reduced_and_clustering_callback\n\t{}\n\t{}".format(sql, vals))
-            self.msi.write_sql_values_get_row(sql, vals)
-            rows += 1
-        message.showinfo("DB Write", "Wrote {} rows of reduced and cluster data".format(rows))
 
-    def store_clustering_callback(self):
-        print("store_clustering_callback")
-        et:EmbeddedText
-        rows = 0
-        for et in self.mr.embedding_list:
-            sql = "update table_tweet set cluster_id = %s, cluster_name = %s where row_id = %s;"
-            vals = (et.cluster_id, et.cluster_name, et.row_id)
-            self.msi.write_sql_values_get_row(sql, vals)
-            rows += 1
-        message.showinfo("DB Write", "Wrote {} rows of cluster data".format(rows))
+    def save_text_list_callback(self):
+        print("NarrativeExplorer2.save_text_list_callback()")
+
+        if self.experiment_id == -1:
+            result = tk.messagebox.showwarning("Warning!", "Please create or select a database first")
+            return
+        gf = self.generator_frame
+        ef = self.embedding_frame
+        print("\tSaving {} lines".format(len(gf.parsed_full_text_list)))
+        if len(gf.parsed_full_text_list) > 0:
+            # create the run
+            run_id = 1
+            sql = "select MAX(run_id) as max from table_run where experiment_id = %s"
+            vals = (self.experiment_id,)
+            results = self.msi.read_data(sql, vals)
+            print(results)
+            if results[0]['max'] != None:
+                run_id = results[0]['max'] + 1
+            # get the language model params entry
+            gs = gf.get_settings()
+            sql = "insert into table_generate_params (tokens, temp, presence_penalty, frequency_penalty, model, automated_runs) values (%s, %s, %s, %s, %s, %s)"
+            vals = (gs.tokens, gs.temperature, gs.presence_penalty, gs.frequency_penalty, gs.model, gs.auto_runs)
+            lang_param_id = self.msi.write_sql_values_get_row(sql, vals)
+
+            # get the embedding model entry
+            es = ef.get_settings()
+            sql = "insert into table_embedding_params (model, PCA_dim, EPS, min_samples, perplexity) values (%s, %s, %s, %s, %s)"
+            vals = (es.model, es.pca_dim, es.eps, es.min_samples, es.perplexity)
+            embed_param_id = self.msi.write_sql_values_get_row(sql, vals)
+
+            sql = "insert into table_run (experiment_id, run_id, prompt, response, generator_params, embedding_params) values (%s, %s, %s, %s, %s, %s)"
+            vals = (self.experiment_id, run_id, gf.saved_prompt_text,
+                    gf.saved_response_text, lang_param_id, embed_param_id)
+            run_index = self.msi.write_sql_values_get_row(sql, vals)
+
+            # store the text
+            s:str
+            for s in gf.parsed_full_text_list:
+                sql = "insert into table_parsed_text (run_index, parsed_text) values (%s, %s)"
+                vals = (run_index, s)
+                self.msi.write_sql_values_get_row(sql, vals)
+        else:
+            result = tk.messagebox.showwarning("Warning!", "There are no parsed lines")
+            return
 
-    def store_user_callback(self):
-        keyword = self.keyword_combo.get_text()
+        #reset the list
+        gf.parsed_full_text_list = []
 
-        if self.experiment_id == -1 or len(keyword) < 2:
-            message.showwarning("DB Error", "get_db_embeddings_callback(): Please set database and/or keyword")
+    def automate_callback(self):
+        print("automate_callback():")
+        if self.experiment_id == -1:
+            result = tk.messagebox.showwarning("Warning!", "Please create or select a database first")
             return
 
-        sql = "select distinct author_id from keyword_tweet_view where experiment_id = %s order by author_id"
+        gf = self.generator_frame
+        num_runs = gf.auto_field.get_as_int()
+        parsed_lines = 0
+        for i in range(num_runs):
+            prompt = gf.prompt_text_field.get_text()
+            print("{}: prompting: ...{}".format(i, prompt[-80:]))
+            gf.new_prompt_callback()
+            response = gf.response_text_field.get_text()
+            print("\tgetting response: {}...".format(response[:80]))
+            print("\tparsing response")
+            gf.parse_response_callback()
+            parsed_lines += len(gf.parsed_full_text_list)
+            print("\tstoring data")
+            self.save_text_list_callback()
+            print("\tresetting")
+            gf.parsed_full_text_list = []
+            gf.response_text_field.clear()
+            self.runs_field.set_text(str(i+1))
+            self.parsed_field.set_text(str(parsed_lines))
+        print("done")
+        tk.messagebox.showinfo("Automate", "Finished processing {} rows".format(parsed_lines))
+
+    def get_oai_embeddings_callback(self):
+        print("get_oai_embeddings_callback")
+        if self.experiment_id == -1:
+            tk.messagebox.showwarning("Warning!", "Please create or select a database first")
+            return
+        # get all the embeddings for text that we don't have yet
+        sql = "select experiment_id, id, parsed_text, embedding_model from parsed_view where experiment_id = %s and embedding IS NULL"
         vals = (self.experiment_id,)
-        if keyword != 'all_keywords':
-            sql = "select distinct author_id from keyword_tweet_view where experiment_id = %s and keyword = %s order by author_id"
-            vals = (self.experiment_id, keyword)
         results = self.msi.read_data(sql, vals)
         d:Dict
-        count = 0
-        l = []
+        # create a list of text
+        s_list = []
         for d in results:
-            l.append(d['author_id'])
-            count += 1
-            if count == 99:
-                self.tkws.run_user_query(l, self.msi)
-                s = ",".join(map(str, l))
-                print("[{}]: {}".format(len(l), s))
-                count = 0
-                l = []
-        if len(l) > 0:
-            self.tkws.run_user_query(l, self.msi)
-            s = ",".join(map(str, l))
-            print("[{}]: {}".format(len(l), s))
+            s_list.append(d['parsed_text'])
 
-        # self.tkws.run_user_query([155,22186596,758514997995589632,1289933022901370880], self.msi)
-        print("store_user_callback(): complete")
+        # send that list to get embeddings
+        engine = results[0]['embedding_model']
+        d_list = self.oai.get_embedding_list(s_list, engine)
+
+        # store embeddings
+        for i in range(len(results)):
+            rd = results[i]
+            id = rd['id']
+            d = d_list[i]
+            embedding = d['embedding']
+            text = d['text']
+            embd_s = np.array(embedding)
+            sql = "update table_parsed_text set embedding = %s where id = %s"
+            vals = (embd_s.dumps(), id)
+            self.msi.write_sql_values_get_row(sql, vals)
 
-    def retreive_tweet_data_callback(self):
-        print("get_db_embeddings_callback")
-        keyword = self.keyword_combo.get_text()
+            print("[{}]: {} [{}]".format(id, text, embd_s))
 
-        if self.experiment_id == -1 or len(keyword) < 2:
-            message.showwarning("DB Error", "get_db_embeddings_callback(): Please set database and/or keyword")
-            return
+        tk.messagebox.showinfo("get_oai_embeddings_callback", "Finished embedding {} rows".format(len(results)))
 
-        print("\t Loading from DB")
-        query = 'select tweet_row, tweet_id, embedding, cluster_id, cluster_name, reduced from keyword_tweet_view where experiment_id = %s'
-        values = (self.experiment_id,)
-        if keyword != 'all_keywords':
-            query = 'select tweet_row, tweet_id, text, embedding, cluster_id, cluster_name, reduced from keyword_tweet_view where experiment_id = %s and keyword = %s'
-            values = (self.experiment_id, keyword)
-        result = self.msi.read_data(query, values, True)
-        row_dict:Dict
 
+    def get_db_embeddings_callback(self):
+        print("get_db_embeddings_callback")
+        if self.experiment_id == -1:
+            message.showwarning("DB Error", "get_db_embeddings_callback(): Please set database")
+            return
+
+        print("Loading from DB")
         print("\tClearing ManifoldReduction")
         self.mr.clear()
-        self.canvas_frame.clear_Nodes()
-        self.dp.dprint("\tLoading {} rows".format(len(result)))
-        count = 0
+        sql = "select * from parsed_view where experiment_id = %s"
+        vals = (self.experiment_id,)
+        results = self.msi.read_data(sql, vals)
+        d:Dict
         et:EmbeddedText
-        for row_dict in result:
-            et = self.mr.load_row(row_dict['tweet_row'], row_dict['embedding'])
-            et.text = self.safe_dict(row_dict, 'text', "unset")
-            reduced = self.safe_dict(row_dict, 'reduced', None)
-            cluster_id = self.safe_dict(row_dict, 'cluster_id', None)
-            cluster_name = self.safe_dict(row_dict, 'cluster_name', None)
-            et.set_optional(reduced, cluster_id, cluster_name)
-            if count % 1000 == 0:
-                self.dp.dprint("loaded {} of {} records".format(count, len(result)))
-            count += 1
-
-        self.mr.calc_xy_range()
-
-
-        for i in range(10):
-            et = self.mr.embedding_list[i]
+        for d in results:
+            embed_s = d['embedding']
+            id = d['id']
+            et = self.mr.load_row(id, embed_s, None, None)
+            et.text = self.safe_dict_read(d, 'parsed_text', 'unset')
+            mapped = self.safe_dict_read(d, 'mapped', None)
+            cluster_id = self.safe_dict_read(d, 'cluster_id', None)
+            cluster_name = self.safe_dict_read(d, 'cluster_name', "clstr_{}".format(cluster_id))
+            run_id = self.safe_dict_read(d, 'run_id', None)
+            et.set_optional(mapped, cluster_id, cluster_name, run_id)
             print(et.to_string())
+        self.mr.calc_clusters()
+        message.showinfo("get_db_embeddings_callback", "Loaded ({:,}) embeddings".format(len(results)))
 
-        message.showinfo("get_db_embeddings_callback", "Finished loading {} rows".format(len(self.mr.embedding_list)))
-
-        print("\tFinished loading")
-
-    def reduce_dimensions_callback(self):
-        pca_dim = self.pca_dim_param.get_as_int()
-        perplexity = self.perplexity_param.get_as_int()
-        self.dp.dprint("Reducing: PCA dim = {}  perplexity = {}".format(pca_dim, perplexity))
-        self.mr.calc_embeding(perplexity=perplexity, pca_components=pca_dim)
-        print("\tFinished dimension reduction")
-        message.showinfo("reduce_dimensions_callback", "Reduced to {} dimensions".format(pca_dim))
-
-    def cluster_callback(self):
-        print("Clustering")
-        eps = self.eps_param.get_as_float()
-        min_samples = self.min_samples_param.get_as_int()
-        self.mr.dbscan(eps=eps, min_samples=min_samples)
-        self.dp.dprint("Finished clustering")
-
-    def plot_callback(self):
-        print("Plotting")
-        keyword = self.keyword_combo.get_text()
-        perplexity = self.perplexity_param.get_as_int()
-        eps = self.eps_param.get_as_int()
-        min_samples = self.min_samples_param.get_as_int()
-        pca_dim = self.pca_dim_param.get_as_int()
-        self.mr.plot("{}\ndim: {}, eps: {}, min_sample: {}, perplex = {}".format(
-            keyword, pca_dim, eps, min_samples, perplexity))
-        plt.show()
-
-    def explore_callback(self):
-        print("Exploring")
-        et:EmbeddedText
-        n:MovableNode
-        color_list = list(mcolors.TABLEAU_COLORS.values())
-        num_nodes = len(self.mr.embedding_list)
-        self.dp.dprint("Explore: num_nodes = {}".format(num_nodes))
-        if num_nodes == 0:
+    def get_current_params(self) -> Dict:
+        generator_settings = self.generator_frame.get_settings()
+        embed_settings = self.embedding_frame.get_settings()
+        d = {
+            "probe_str": generator_settings.prompt,
+            "name": self.experiment_field.get_text(),
+            "automated_runs": generator_settings.auto_runs,
+            "generate_model": generator_settings.model,
+            "tokens": generator_settings.tokens,
+            "temp": generator_settings.temperature,
+            "presence_penalty": generator_settings.presence_penalty,
+            "frequency_penalty": generator_settings.frequency_penalty,
+            "embedding_model": embed_settings.model,
+            "PCA_dimensions": embed_settings.pca_dim,
+            "EPS": embed_settings.eps,
+            "min_samples": embed_settings.min_samples,
+            "perplexity": embed_settings.perplexity
+        }
+        return d
+
+    def load_params_callback(self):
+        defaults = self.get_current_params()
+
+        param_dict = self.load_json(defaults)
+        # print(param_dict)
+        gs = GPT3GeneratorSettings()
+        gs.from_dict(param_dict)
+        self.generator_frame.set_params(gs)
+
+        gs = GPT3EmbeddingSettings(defaults)
+        gs.from_dict(param_dict)
+        self.embedding_frame.set_params(gs)
+
+        self.experiment_field.clear()
+
+        if 'name' in param_dict:
+            self.experiment_field.set_text(param_dict['name'])
+
+    def save_params_callback(self):
+        params = self.get_current_params()
+        self.save_experiment_json(params)
+
+    def export_network_callback(self):
+        print("NarrativeExplorer2.export_network_callback()")
+        if self.experiment_id == -1:
+            message.showwarning("DB Error", "get_db_embeddings_callback(): Please set database")
             return
-        step = int(num_nodes / self.rows_param.get_as_int())
-        print("\tstep = {}".format(step))
-        #calculate the x, y scalar
-        x_dist = self.mr.max_x - self.mr.min_x
-        y_dist = self.mr.max_y - self.mr.min_y
-        x_scale = self.canvas_frame.virtual_canvas_size / x_dist
-        y_scale = self.canvas_frame.virtual_canvas_size / y_dist
-        for i in range(0, num_nodes, step):
-            et = self.mr.embedding_list[i]
-            c = self.mr.get_cluster_color(et.cluster_id, color_list)
-            x = et.reduced[0] * x_scale
-            y = et.reduced[1] * y_scale
-            if et.mnode == None:
-                n = self.canvas_frame.create_MoveableNode(et.text, x=x, y=y, color=c, size = 2, show_name=False)
-                et.mnode = n
-            else:
-                et.mnode.set_color(c)
-        self.color_excluded_clusters()
-        self.dp.dprint("Finished creating points")
+        user = os.getlogin()
+        ng = NetworkxGraphing(name=self.experiment_field.get_text(), creator=user)
 
-    def selected_node_callback(self, node_id:int, msg:str):
-        print("node_id = {}, msg = {}".format(node_id, msg))
-        et:EmbeddedText
-        for et in self.mr.embedding_list:
-            if et.mnode != None:
-                mn = et.mnode
-                if mn.id == node_id:
-                    self.exclude_cluster_field.clear()
-                    self.exclude_cluster_field.set_text(str(et.cluster_id))
-                    break
-
-    def exclude_cluster_callback(self):
-        print("exclude_cluster_callback")
-        to_exclude = self.exclude_cluster_field.get_text()
-        if to_exclude.isdigit():
-            cluster_id = int(to_exclude)
-            keyword = self.keyword_combo.get_text()
-            experiment_id = self.experiment_id
-            sql = "SELECT COUNT(*) FROM table_exclude where experiment_id = %s and cluster_id = %s and keyword = %s"
-            vals = (experiment_id, cluster_id, keyword)
-            result = self.msi.read_data(sql, vals)
-            d:Dict = result[0]
-            print(d)
-            if d['COUNT(*)'] == 0:
-                sql = "INSERT INTO table_exclude (experiment_id, cluster_id, keyword) VALUES (%s, %s, %s)"
-                self.msi.write_sql_values_get_row(sql, vals, True)
-                self.color_excluded_clusters()
+        sql = "select id, experiment_id, run_id from table_run where experiment_id = %s"
+        vals = (self.experiment_id,)
 
+        runs_response = self.msi.read_data(sql, vals)
+        runs_d:Dict
+        parsed_d1:Dict
+        parsed_d2:Dict
+        weight_dict = {}
+        for runs_d in runs_response:
+            run_index = int(runs_d['id'])
+            sql = "select id, cluster_name, parsed_text from table_parsed_text where run_index = %s order by id"
+            vals = (run_index,)
+            parsed_response = self.msi.read_data(sql, vals)
+            for i in range(len(parsed_response) - 1):
+                parsed_d1 = parsed_response[i]
+                parsed_d2 = parsed_response[i+1]
+                cl = str(parsed_d1['cluster_name']).split("\n")
+                cl = [x.strip() for x in cl]
+                source = "-".join(cl).strip()
+                cl = str(parsed_d2['cluster_name']).split("\n")
+                cl = [x.strip() for x in cl]
+                target = "-".join(cl).strip()
+                if source != target:
+                    if source in weight_dict:
+                        weight_dict[source] += 1
+                    else:
+                        weight_dict[source] = 1
+                    if target in weight_dict:
+                        weight_dict[target] += 1
+                    else:
+                        weight_dict[target] = 1
+
+        for key, val in weight_dict.items():
+            print("{} = {}".format(key, val))
+
+        for runs_d in runs_response:
+            run_index = int(runs_d['id'])
+            sql = "select id, cluster_name, parsed_text from table_parsed_text where run_index = %s order by id"
+            vals = (run_index,)
+            parsed_response = self.msi.read_data(sql, vals)
+            for i in range(len(parsed_response) - 1):
+                parsed_d1 = parsed_response[i]
+                parsed_d2 = parsed_response[i+1]
+                cl = str(parsed_d1['cluster_name']).split("\n")
+                cl = [x.strip() for x in cl]
+                source = "-".join(cl).strip()
+                cl = str(parsed_d2['cluster_name']).split("\n")
+                cl = [x.strip() for x in cl]
+                target = "-".join(cl).strip()
+                if source != target:
+                    # print("[{}] source: {}, target: {}".format(runs_d['run_id'], source, target))
+                    ng.add_weighted_nodes(source, weight_dict[source], target, weight_dict[target])
+        #ng.draw(self.experiment_field.get_text(), draw_legend=False, do_show=True, scalar=2.0)
+        result = filedialog.asksaveasfile(filetypes=(("gml files", "*.gml"),("All Files", "*.*")), title="Save/Update network", initialfile = "{}.gml".format(self.experiment_field.get_text()))
+        if result:
+            filename = result.name
+            ng.to_gml(filename, graph_creator=user, node_attributes=['weight'])
+            self.dp.dprint("Saved network to {}".format(filename))
 
-    def label_clusters_callback(self):
-        pass
 
-    def get_oai_embeddings_callback(self):
-        print("get_oai_embeddings_callback")
-        keyword = self.keyword_combo.get_text()
-
-        if self.experiment_id == -1 or len(keyword) < 2:
-            message.showwarning("DB Error", "get_oai_embeddings_callback(): Please set database and/or keyword")
-            return
-
-        query = "select tweet_id, text from keyword_tweet_view where experiment_id = %s and embedding is NULL"
-        values = (self.experiment_id,)
-        if keyword != 'all_keywords':
-            query = "select tweet_id, text from keyword_tweet_view where experiment_id = %s and keyword = %s and embedding is NULL"
-            values = (self.experiment_id, keyword)
-
-        engine = self.engine_combo.get_text()
-        print("get_embeddings_callback() Experiment id = {}, Keyword = {}, Engine = {}".format(self.experiment_id, keyword, engine))
-        result = self.msi.read_data(query, values)
-        self.dp.dprint("Getting embeddings for {} rows".format(len(result)))
-        count = 0
-        row_dict:Dict
-        for row_dict in result:
-            id = row_dict['tweet_id']
-            tweet = row_dict['text']
-            embd = self.oai.get_embedding(tweet, engine)
-            print("id: {} text: {} embed: {}".format(id, tweet, embd))
-            query = "update table_tweet set embedding = %s where id = %s"
-            values = ("{}:{}".format(engine, embd), id)
-            self.msi.write_sql_values_get_row(query, values)
-            if count % 1000 == 0:
-                self.dp.dprint("Embedded {} of {} records".format(count, len(result)))
-            count += 1
-
-
-    def get_keyword_entries_callback(self, keyword: str):
-        print("get_keyword_entries: keyword = {}, experiment_id = {}".format(keyword, self.experiment_id))
-        query = "select count(*) from keyword_tweet_view where experiment_id = %s"
-        values = (self.experiment_id)
-        if keyword != 'all_keywords':
-            query = "select count(*) from keyword_tweet_view where experiment_id = %s and keyword = %s"
-            values = (self.experiment_id, keyword)
-        result:Dict = self.msi.read_data(query, values)[0]
-        count = result['count(*)']
-
-        self.keyword_count_field.set_text(count)
-        self.rows_param.set_text(count)
-
-    def keyword_callback(self, event:tk.Event):
-        print("keyword_callback: event = {}".format(event))
-        num_regex = re.compile(r"\d+")
-        s = self.experiment_combo.tk_combo.get()
-        self.experiment_combo.set_text(s)
-        self.experiment_id = num_regex.findall(s)[0]
-        print("keyword_callback: experiment_id = {}".format(self.experiment_id))
-        query = "select distinct keyword from table_query where experiment_id = %s"
-        values = (self.experiment_id,)
-        result = self.msi.read_data(query, values)
-        l = ['all_keywords']
-        row_dict:Dict
-        for row_dict in result:
-            l.append(row_dict['keyword'])
-        self.keyword_combo.set_combo_list(l)
-
-
-    def setup(self):
-        # set up the canvas
-        self.canvas_frame.setup(debug=False, show_names=False)
-
-        # set up the selections that come from the db
-        l = []
-        row_dict:Dict
-        query = "select * from table_experiment"
-        result = self.msi.read_data(query)
-        for row_dict in result:
-            s = "{}: {}".format(row_dict['id'], row_dict['keywords'])
-            l.append(s)
-        self.experiment_combo.set_combo_list(l)
 
 
 def main():
-    app = EmbeddingsExplorer()
-    app.setup()
+    app = NarrativeExplorer2()
     app.mainloop()
 
-
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/Apps/WikiPageviewExplorer.py` & `keyword_explorer-0.5a0/keyword_explorer/Apps/WikiPageviewExplorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     topic_text_field:TextField
     response_text_field:TextField
     wiki_pages_text_field:TextField
     start_date_field:DateEntryField
     end_date_field:DateEntryField
     sample_list:ListField
     multi_count_list:List
+    topic_action_buttons:Buttons
+    views_action_buttons:Buttons
     totals_dict:dict
     user_agent:str
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         print("WikiPageviewExplorer.md")
 
@@ -74,42 +76,42 @@
         self.topic_text_field = TextField(lf, row, "Topic", text_width, height=5, label_width=label_width)
         self.topic_text_field.set_text("simpson characters\npinky and the brain")
         ToolTip(self.topic_text_field.tk_text, "List of possible Wikipedia topics")
         row = self.topic_text_field.get_next_row()
         self.response_text_field = TextField(lf, row, 'Response', text_width, height=10, label_width=label_width)
         ToolTip(self.response_text_field.tk_text, "List of best matches in English Wikipedia\nSelect the desired results to examine and\nclick 'Copy Selected'")
         row = self.response_text_field.get_next_row()
-        buttons = Buttons(lf, row, "Actions", label_width=label_width)
-        b = buttons.add_button("Search", self.search_wiki_callback, width=-1)
+        self.topic_action_buttons = Buttons(lf, row, "Actions", label_width=label_width)
+        b = self.topic_action_buttons.add_button("Search", self.search_wiki_callback, width=-1)
         ToolTip(b, "Search for best matches in English Wikipedia")
-        b = buttons.add_button("Copy Selected", self.copy_selected_callback, width=-1)
+        b = self.topic_action_buttons.add_button("Copy Selected", self.copy_selected_callback, width=-1)
         ToolTip(b, "Copy selected responses to 'Pages' below for views")
-        row = buttons.get_next_row()
+        row = self.topic_action_buttons.get_next_row()
 
     def build_page_views(self, lf:tk.LabelFrame, text_width:int, label_width:int):
         row = 0
         self.wiki_pages_text_field = TextField(lf, row, 'Pages', text_width, height=7, label_width=label_width)
         ToolTip(self.wiki_pages_text_field.tk_text, "The list of topics to get page views for")
         row = self.wiki_pages_text_field.get_next_row()
         self.start_date_field = DateEntryField(lf, row, 'Start Date', text_width, label_width=label_width)
         row = self.start_date_field.get_next_row()
         self.end_date_field = DateEntryField(lf, row, 'End Date', text_width, label_width=label_width)
         row = self.end_date_field.get_next_row()
-        buttons = Buttons(lf, row, "Actions", label_width=label_width)
-        b = buttons.add_button("Clear", self.clear_pageviews_callback)
+        self.views_action_buttons = Buttons(lf, row, "Actions", label_width=label_width)
+        b = self.views_action_buttons.add_button("Clear", self.clear_pageviews_callback)
         ToolTip(b, "Clears the topics from the Views text area")
-        b = buttons.add_button("Test Pages", self.test_pages_callback, width=-1)
+        b = self.views_action_buttons.add_button("Test Pages", self.test_pages_callback, width=-1)
         ToolTip(b, "Query page views between Start Date and End Date and plot results")
-        b = buttons.add_button("Plot", self.plot_callback, width=-1)
+        b = self.views_action_buttons.add_button("Plot", self.plot_callback, width=-1)
         ToolTip(b, "Plot page views")
-        b = buttons.add_button("Save", self.save_callback, width=-1)
+        b = self.views_action_buttons.add_button("Save", self.save_callback, width=-1)
         ToolTip(b, "Save page views to Excel file")
-        b = buttons.add_button("Show Pages", self.show_pages_callback, width=-1)
+        b = self.views_action_buttons.add_button("Show Pages", self.show_pages_callback, width=-1)
         ToolTip(b, "Launch each Wikipedia page as a separate tab in the default browser")
-        row = buttons.get_next_row()
+        row = self.views_action_buttons.get_next_row()
 
     def build_page_view_params(self, lf:tk.LabelFrame, text_width:int, label_width:int):
         row = 0
         self.sample_list = ListField(lf, row, "Sample", width=text_width, label_width=label_width, static_list=True)
         self.sample_list.set_text(text='daily, monthly')
         self.sample_list.set_callback(self.set_time_sample_callback)
         self.set_time_sample_callback()
@@ -136,39 +138,41 @@
     def clear_pageviews_callback(self):
         self.wiki_pages_text_field.clear()
 
     def search_wiki_callback(self):
         key_list = self.topic_text_field.get_list("\n")
         result_list = []
         for keyword in key_list:
-            page_list = ws.get_closet_wiki_page_list(keyword, n=7, cutoff=0.4)
-            s = " | ".join(page_list)
-            self.log_action("search term", {keyword: s.replace(",", " ")})
-            result_list.extend(page_list)
+            if len(keyword) > 2:
+                page_list = ws.get_closet_wiki_page_list(keyword, n=7, cutoff=0.4)
+                s = " | ".join(page_list)
+                self.log_action("search term", {keyword: s.replace(",", " ")})
+                result_list.extend(page_list)
         result = "\n".join(result_list)
         self.response_text_field.set_text(result)
 
 
     def test_pages_callback(self):
         granularity = self.sample_list.get_selected()
         start_dt = self.start_date_field.get_date()
         end_dt = self.end_date_field.get_date()
         topic_list = self.wiki_pages_text_field.get_list("\n")
         topic:str
         self.multi_count_list = []
         self.totals_dict = {}
         log_dict = {"granularity":granularity, "wiki_start": start_dt.strftime("%Y-%m-%d"), "wiki_end":end_dt.strftime("%Y-%m-%d")}
         for topic in topic_list:
-            query = topic.replace(" ", "_")
-            query = query.replace("&", "%26")
-            view_list, totals = ws.get_pageview_list(query, start_dt, end_dt, granularity, self.user_agent)
-            print("{} = {}".format(query, totals))
-            self.totals_dict[topic] = totals
-            view_list = sorted(view_list, key=lambda x: x.timestamp)
-            self.multi_count_list.append(view_list)
+            if len(topic) > 2:
+                query = topic.replace(" ", "_")
+                query = query.replace("&", "%26")
+                view_list, totals = ws.get_pageview_list(query, start_dt, end_dt, granularity, self.user_agent)
+                print("{} = {}".format(query, totals))
+                self.totals_dict[topic] = totals
+                view_list = sorted(view_list, key=lambda x: x.timestamp)
+                self.multi_count_list.append(view_list)
 
         for k, v in self.totals_dict.items():
             log_dict[k.replace(",", " ")] = v
         self.log_action("test_keyword", log_dict)
 
         self.plot_callback()
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/TwitterV2/TweetKeywords.py` & `keyword_explorer-0.5a0/keyword_explorer/TwitterV2/TweetKeywords.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/TwitterV2/TwitterV2Base.py` & `keyword_explorer-0.5a0/keyword_explorer/TwitterV2/TwitterV2Base.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/TwitterV2/TwitterV2Counts.py` & `keyword_explorer-0.5a0/keyword_explorer/TwitterV2/TwitterV2Counts.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/TwitterV2/tweet_lookup.py` & `keyword_explorer-0.5a0/keyword_explorer/TwitterV2/tweet_lookup.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/mastodon/post_lookup.py` & `keyword_explorer-0.5a0/keyword_explorer/mastodon/post_lookup.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/Buttons.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/Buttons.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 import tkinter as tk
 from tkinter import ttk
-from typing import List, Callable, Any
+from typing import Dict, Callable, Any
 
 class Buttons():
     tk_label:tk.Label
     tk_combo:ttk.Combobox
     tk_button:ttk.Button
     wrapper:tk.Frame
     row = 0
     col:int = 0
     parent:'tk.Frame'
+    label_dict:Dict
 
     def __init__(self, parent:'tk.Frame', row:int, label:str, label_width:int=20, sticky="nsew"):
+        self.label_dict = {}
         self.parent = parent
         self.row = row
         self.tk_label = tk.Label(parent, text=label, width=label_width, anchor="w")#, background="pink")
         self.tk_label.grid(column=0, row=row, sticky="w", padx=5)
 
         self.wrapper = tk.Frame(parent)#, background="pink")
         self.wrapper.grid(column=1, row=row, sticky=sticky)
 
         self.col = 0
 
     def add_button(self, name:str,  command:Callable, width:int = 10, sticky:Any = (tk.N, tk.W)) -> ttk.Button:
         if width < 0:
             width = len(name)+1
-        b = ttk.Button(self.wrapper, text=name, width=width, command=command)
+        sv = tk.StringVar()
+        sv.set(name)
+        b = ttk.Button(self.wrapper, textvariable=sv, width=width, command=command)
         b.grid(column=self.col, row=0, sticky=sticky, pady=2, padx=5)
         self.col += 1
+        self.label_dict[name] = sv
         return b
 
+    def change_button_label(self, name:str, label:str):
+        sv:tk.StringVar = self.label_dict[name]
+        sv.set(label)
+
+    def get_button_label(self, name:str) -> str:
+        sv:tk.StringVar = self.label_dict[name]
+        return sv.get()
+
+    def get_label_dict(self) -> Dict:
+        return self.label_dict
+
     def get_next_row(self):
         return self.row + 1
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/CanvasFrame.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/CanvasFrame.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/Checkboxes.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/Checkboxes.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 class DIR(Enum):
     COL = 0
     ROW = 1
 
 class Checkbox():
     bvar:tk.BooleanVar
+    ivar:tk.IntVar
     cb:ttk.Checkbutton
     name:str
 
     def __init__(self, wrapper:tk.Frame, name:str, command:Callable):
-        self.bvar = tk.BooleanVar()
-        self.bvar.set(False)
+        self.bvar = tk.BooleanVar(value=False)
         self.name = name
-        self.cb = ttk.Checkbutton(wrapper, text=name, command=command, variable=self.bvar)
+        self.cb = ttk.Checkbutton(wrapper, text=name, command=command, variable=self.bvar, offvalue=False, onvalue=True)
 
     def get_val(self) -> bool:
         return self.bvar.get()
 
     def set_val(self, val:bool):
         self.bvar.set(val)
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/ConsoleDprint.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/ConsoleDprint.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/DataField.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/DataField.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/DateEntryField.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/DateEntryField.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/LabeledParam.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/LabeledParam.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/ListField.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/ListField.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import tkinter as tk
 from tkinter import ttk
+import inspect
+import re
+
 from typing import Union, List, Callable
 
 
 
 class ListField:
     name:str = "unset"
     tk_labelttk:tk.Label = None
     tk_list:tk.Listbox = None
     row = 0
     term_list = ["call", "me", "Ishmael"]
     tvar:tk.StringVar = None
     lvar:tk.StringVar = None
-    callback_fn:Callable = None
-    callback_fn2:Callable = None
+    lf_callback_fn:Callable = Union[None, Callable]
     sel_list:List
     last_selected:str = None
     static_list:bool = False
 
     def __init__(self, parent:'ttk.Frame', row:int, label:str, width:int = 20, height: int = 3, selectmode=tk.BROWSE, label_width:int=20, static_list:bool = False):
         self.static_list = static_list
-        self.callback_fn = None
+        self.lf_callback_fn = None
+        self.name = label
         self.sel_list = []
         self.last_selected = 'unset'
         self.tvar = tk.StringVar(value=self.term_list)
         self.lvar = tk.StringVar(value=label)
         self.row = row
         self.tk_label = ttk.Label(parent, textvariable=self.lvar, width=label_width)
         list_wrapper = tk.Frame(parent, borderwidth=2)
@@ -106,22 +109,32 @@
             # find the first element in the list. It should be the only one
             for index in sel_list:
                 self.last_selected = self.tk_list.get(index)
                 break
         return self.last_selected
 
     def set_callback(self, fn:Callable):
-        self.callback_fn = fn
+        self.lf_callback_fn = fn
+
+    def inspect(self):
+        fi:inspect.FrameInfo
+        count = 0
+        print("ListField.inspect()\n\tlabel: {}\n".format(self.name))
+        for fi in inspect.stack():
+            filename = re.split(r"(/)|(\\)", fi.filename)
+            print("\tCall stack[{}] = {}() (line {} in {})".format(count, fi.function, fi.lineno, filename[-1]))
 
     def on_selected(self, event:tk.Event):
         if not self.static_list:
             sel_list =  self.tk_list.curselection()
             if len(sel_list) > 0:
                 for index in sel_list:
                     self.last_selected = self.tk_list.get(index)
                     # print("clicked on item[{}] = [{}]".format(index, s))
                     if index in self.sel_list:
                         self.tk_list.selection_clear(0, tk.END)
             self.sel_list = sel_list
 
-        if self.callback_fn != None:
-            self.callback_fn(event)
+        if self.lf_callback_fn != None:
+            print("ListField.on_selected()")
+            #self.inspect()
+            self.lf_callback_fn(event)
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/MoveableNode.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/MoveableNode.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/TextComparePopup.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/TextComparePopup.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/TextField.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/TextField.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,18 @@
         self.tk_text.delete('1.0', tk.END)
 
     def set_text(self, text:str, pos:int = 0):
         self.reference_text = text
         self.tk_text.delete('1.0', tk.END)
         self.tk_text.insert("1.0", text)
 
+    def insert_text(self, text:str, pos:int = 0):
+        self.reference_text = text
+        self.tk_text.insert("1.0", text)
+
     def set_animate_text(self, text:str, animate_delay:int = 30):
         self.reference_text = text
         self.animate_delay_ms = animate_delay
         self.animate_index = 0
         self.tk_text.delete('1.0', tk.END)
         self.animate()
 
@@ -96,16 +100,17 @@
         return self.reference_text
 
     def get_list(self, regex_str:str = ",") -> List:
         to_return = self.tk_text.get("1.0", tk.END)
         rlist = re.split(regex_str, to_return)
         to_return = []
         for t in rlist:
-            to_return.append(t.strip())
-        to_return = [x for x in to_return if x] # filter out the blanks
+            if t != None:
+                to_return.append(t.strip())
+        #to_return = [x for x in to_return if x] # filter out the blanks
         return to_return
 
     def get_selected(self, get_everything:bool = True) -> str:
         # if nothing is selected, the we'll grab everything. We take advantage of the exception that is thrown when
         # you try to get the index of a selection that is not there
         s = ""
         try:
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/TkCanvasBase.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/TkCanvasBase.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/ToolTip.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/ToolTip.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/TopicCombo.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/TopicCombo.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/tkUtils/TopicComboExt.py` & `keyword_explorer-0.5a0/keyword_explorer/tkUtils/TopicComboExt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import tkinter as tk
 from tkinter import ttk
 from typing import List, Callable, Union
 
 import keyword_explorer.tkUtils.ConsoleDprint as DP
 
 class TopicComboExt():
-    tk_label = tk.Label
-    tk_entry = tk.Entry
-    tk_text = tk.Text
-    tk_combo = ttk.Combobox
+    name:str
+    tk_label:tk.Label
+    tk_entry:tk.Entry
+    tk_text:tk.Text
+    tk_combo:ttk.Combobox
     wrapper:tk.Frame
-    row = 0
+    row:int = 0
     col:int = 0
     combo_str_var:tk.StringVar
     combo_vals:List
     parent:'tk.Frame'
     dp:DP.ConsoleDprint
-    callback_fn:Union[None, Callable]
+    callback_fn:Callable
+    callback_exists:bool
     default_behavior:bool
     use_text_field:bool
 
     def __init__(self, parent:'tk.Frame', row:int, label:str, dprint:DP.ConsoleDprint,
                  entry_width:int = 30, combo_width:int = 30, label_width:int=20, use_text_field:bool = False):
         self.parent = parent
-
+        self.name = label
         self.set_dprint(dprint)
         self.row = row
         self.combo_str_var = tk.StringVar(value="Option 4")
         self.combo_vals = []
         self.tk_label = ttk.Label(parent, text=label, width=label_width)
         self.use_text_field = use_text_field
         self.callback_fn = None
+        self.callback_exists = False
 
         self.wrapper = tk.Frame(parent)
         if self.use_text_field == True:
             self.tk_text = tk.Text(self.wrapper, width=entry_width, height=4, wrap=tk.WORD, borderwidth=2, relief="groove")
         else:
             self.tk_entry = ttk.Entry(self.wrapper, width=entry_width)
         self.tk_combo = ttk.Combobox(self.wrapper, values=self.combo_vals, width=combo_width)
@@ -55,14 +58,15 @@
         self.col += 1
         return b
 
     def set_label(self, s:str):
         self.tk_label.config(text = s)
 
     def set_callback(self, fn:Callable):
+        self.callback_exists = True
         self.callback_fn = fn
 
     def set_dprint(self, con:DP.ConsoleDprint):
         self.dp = con
 
     def get_next_row(self):
         return self.row + 1
@@ -94,13 +98,14 @@
 
     def add_to_combo_list(self, s:str):
         self.combo_vals.append(s)
         self.tk_combo.set(s)
         self.tk_combo['values'] = self.combo_vals
 
     def on_combobox_selected(self, event:tk.Event):
-        if self.callback_fn != None:
+        if self.callback_exists:
+            print("TopicComboExt.on_combobox_selected() name = {}".format(self.name))
             self.callback_fn(event)
         else:
             print("TopicCombo().on_combobox_selected: selected: {}".format(self.tk_combo.get()))
             self.clear()
             self.set_text(self.tk_combo.get())
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/utils/CorporaGenerator.py` & `keyword_explorer-0.5a0/keyword_explorer/utils/CorporaGenerator.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/utils/ManifoldReduction.py` & `keyword_explorer-0.5a0/keyword_explorer/utils/ManifoldReduction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,97 +1,152 @@
 #import umap
 import re
 import ast
+import pickle
 import numpy as np
 from sklearn.manifold import TSNE
 from sklearn.cluster import DBSCAN
 from sklearn.decomposition import PCA
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
+from statistics import mean
 
 from keyword_explorer.tkUtils.MoveableNode import MovableNode
 from typing import List, Dict, Union, Any, Pattern
 
 class EmbeddedText:
     row_id:int
-    raw_str:str
+    run_id:int
+    raw_str:[str, bytes]
     source:str
     text:Union[None, str]
     cluster_id:int
     cluster_name:str
     original:List
     reduced:List
     vis_dim:List
     mnode:Union[None, MovableNode]
-    reg:Pattern
+    reg:[None, Pattern]
     source_regex:Pattern
 
-    def __init__(self, row_id:int, raw_str:str):
+    def __init__(self, row_id:int, raw_str:Any, source_regex:str = r"\w+-\w+-\w+-\d+:", reg:str = r"-?\d+\.\d+"):
         self.row_id = row_id
         self.raw_str = raw_str
-        self.source_regex = re.compile(r"\w+-\w+-\w+-\d+:")
-        self.reg = re.compile(r"-?\d+\.\d+")
-        self.parse()
+        self.reg = None
+
+        if source_regex == None or reg == None:
+            self.parse_2()
+        else:
+            self.source_regex = re.compile(source_regex)
+            self.reg = re.compile(reg)
+            self.parse()
         self.reduced = [0, 0]
         self.cluster_id = -1
+        self.run_id = -1
         self.cluster_name = "unset"
         self.text = "unset"
         self.mnode = None
 
     def parse(self):
         # print("parsing {}".format(self.raw_str))
         split_list = self.raw_str.split(":")
         self.source = split_list[0]
         list_str = split_list[1]
         # print(self.source)
         self.original = ast.literal_eval(list_str)
         # for v in self.original:
         #     print(v)
 
+    def parse_2(self):
+        self.original = pickle.loads(self.raw_str)
+
     def safe_assign(self, val:Any, default:Any) -> Any:
         if val != None:
             return val
         return default
-    def set_optional(self, reduced_str:str, cluster_id:int, cluster_name:str):
+
+    def set_optional(self, reduced_str:bytes = None, cluster_id:int = None, cluster_name:str = None, run_id:int = None):
         #print("set_optional: reduced = {}".format(reduced_str))
         if reduced_str != None:
-            l = self.reg.findall(reduced_str)
-            ls = "[{}]".format(", ".join(l))
-            self.reduced = ast.literal_eval(ls)
+            try:
+                self.reduced = pickle.loads(reduced_str)
+            except pickle.UnpicklingError as e:
+                pass
 
         if cluster_id != None:
             self.cluster_id = cluster_id
 
         if cluster_name != None:
             self.cluster_name = cluster_name
 
+        if run_id != None:
+            self.run_id = run_id
+
+    def to_dict(self) -> Dict:
+        return{"id":self.row_id, "text":self.text, "embedding": np.array(self.original), "reduced":np.array(self.reduced), "distance":0}
 
     def to_string(self) -> str:
-        return "Tweet row = {}, Cluster ID = {}, Cluster Name = {}, Reduced = {}, Text = {}".format(
-            self.row_id, self.cluster_id, self.cluster_name, self.reduced, self.text)
+        return "Text row = {}, Cluster ID = {}, run_id = {}, Cluster Name = {}, Reduced = {}, Text = {}".format(
+            self.row_id, self.cluster_id, self.run_id, self.cluster_name.replace("\n", "-"), self.reduced, self.text)
+
+class ClusterInfo:
+    id:int
+    member_list:[List, None]
+    coordinate:List
+    reduced_coordinate:List
+    label:str
+
+    def __init__(self, id:int, members:List = None):
+        self.member_list = []
+        self.id = id
+        if members != None:
+            self.member_list = members
+
+    def add_member(self, et:EmbeddedText):
+        self.member_list.append(et)
+        self.label = et.cluster_name
+
+    def calc_cluster_info(self):
+        coordinate_list = []
+        reduced_list = []
+        et:EmbeddedText
+        for et in self.member_list:
+            coordinate_list.append(et.original)
+            reduced_list.append(et.reduced)
+        a = np.array(coordinate_list)
+        self.coordinate = np.mean(a, axis=0).tolist()
+        a = np.array(reduced_list)
+        self.reduced_coordinate = np.mean(a, axis=0).tolist()
+
+    def to_string(self):
+        return "Cluster {}\n\tLabel: {}\n\tReduced Coord: {}".format(self.id, self.label, self.reduced_coordinate)
+
+
 
 class ManifoldReduction:
     target_dim:int
     embedding_list:List
+    cluster_list:List
     min_x: float
     min_y: float
     max_x:float
     max_y: float
 
     def __init__(self, dim:int = 2):
-        print("ManifoldReduction.__init__()")
+        # print("ManifoldReduction.__init__()")
         self.target_dim:int = min(dim, 3)
         self.clear()
         self.min_x = self.min_y = self.max_x = self.max_y = 0
 
     def clear(self):
         self.embedding_list = []
+        self.cluster_list = []
 
-    def load_row(self, tweet_row:int, row_str:str) -> EmbeddedText:
-        et = EmbeddedText(int(tweet_row), row_str)
+    def load_row(self, text_row:int, row_str:str, source_regex:str = r"\w+-\w+-\w+-\d+:", reg:str = r"-?\d+\.\d+") -> EmbeddedText:
+        et = EmbeddedText(int(text_row), row_str, source_regex, reg)
         self.embedding_list.append(et)
         return et
 
     def calc_xy_range(self):
         self.min_x = self.min_y = self.max_x = self.max_y = 0
         et:EmbeddedText
         for et in self.embedding_list:
@@ -131,73 +186,126 @@
         l = []
         et:EmbeddedText
         for et in self.embedding_list:
             l.append(et.reduced)
         X = np.array(l)
         clustering = DBSCAN(eps=eps, min_samples=min_samples).fit(X)
         labels = clustering.labels_
+
         for i in range(len(labels)):
             et = self.embedding_list[i]
             et.cluster_id = labels[i]
             et.cluster_name = "cluster_{}".format(et.cluster_id)
         print("Clusters for eps = {}, min_samples = {}: {}".format(eps, min_samples, set(clustering.labels_)))
 
+    def calc_clusters(self):
+        cluster_id_set = set()
+        et:EmbeddedText
+        for et in self.embedding_list:
+            cluster_id_set.add(et.cluster_id)
+
+        for id in cluster_id_set:
+            self.cluster_list.append(ClusterInfo(id))
+
+        ci:ClusterInfo
+        for ci in self.cluster_list:
+            for et in self.embedding_list:
+                if et.cluster_id == ci.id:
+                    ci.add_member(et)
+            ci.calc_cluster_info()
+
+
+
+
+
     def get_cluster_color(self, i:int, cl:List) -> str:
         c_index = i % len(cl)
         return cl[c_index]
 
+
+
     def plot(self, title:str = None):
         et:EmbeddedText
         cluster_dict = {}
+        run_dict = {}
+        point_size = 2
         for et in self.embedding_list:
-            d:Dict
+            cd:Dict
+            rd:Dict
             if et.cluster_name not in cluster_dict:
-                d = {'x':[], 'y':[]}
-                cluster_dict[et.cluster_name] = d
+                cd = {'x':[], 'y':[]}
+                cluster_dict[et.cluster_name] = cd
             else:
-                d = cluster_dict[et.cluster_name]
+                cd = cluster_dict[et.cluster_name]
+            cd['x'].append(et.reduced[0])
+            cd['y'].append(et.reduced[1])
+
+            if et.run_id != -1:
+                point_size = 10
+                if et.run_id not in run_dict:
+                    rd = {'x':[], 'y':[]}
+                    run_dict[et.run_id] = rd
+                else:
+                    rd = run_dict[et.run_id]
+                rd['x'].append(et.reduced[0])
+                rd['y'].append(et.reduced[1])
 
-            d['x'].append(et.reduced[0])
-            d['y'].append(et.reduced[1])
         if title != None:
             plt.title(title)
 
         l1 = list(mcolors.TABLEAU_COLORS.values())
         c_index = 0
-        for name, d in cluster_dict.items():
-            x = d['x']
-            y = d['y']
+        for run_id, rd in run_dict.items():
+            x = rd['x']
+            y = rd['y']
             c = self.get_cluster_color(c_index, l1)
-            plt.scatter(x, y, s=2, c=c)
+            plt.plot(x, y, linewidth=2, alpha=0.1, c=c)
             c_index += 1
 
+        c_index = 0
+        for name, cd in cluster_dict.items():
+            x = cd['x']
+            y = cd['y']
+            c = self.get_cluster_color(c_index, l1)
+            plt.scatter(x, y, s=point_size, c=c)
+            c_index += 1
+
+        for ci in self.cluster_list:
+            # print(ci.to_string())
+            plt.annotate(ci.label, ci.reduced_coordinate)
+
     def plot_reduced(self, axs, title:str = None):
         et:EmbeddedText
+        ci:ClusterInfo
         cluster_dict = {}
         for et in self.embedding_list:
             d:Dict
             if et.cluster_name not in cluster_dict:
                 d = {'x':[], 'y':[]}
                 cluster_dict[et.cluster_name] = d
             else:
                 d = cluster_dict[et.cluster_name]
 
             d['x'].append(et.reduced[0])
             d['y'].append(et.reduced[1])
+
         if title != None:
             axs.title.set_text(title)
 
         l1 = list(mcolors.TABLEAU_COLORS.values())
         c_index = 0
         for name, d in cluster_dict.items():
             x = d['x']
             y = d['y']
             c = self.get_cluster_color(c_index, l1)
             axs.scatter(x, y, s=2, c=c)
             c_index += 1
+        for ci in self.cluster_list:
+            # print(ci.to_string())
+            axs.annotate(ci.label, ci.reduced_coordinate)
 
     def reduced_to_str(self) -> str:
         et:EmbeddedText
         s = "["
         for et in self.embedding_list:
             s += "[{}, {}],".format(et.reduced[0], et.reduced[1])
 
@@ -208,17 +316,20 @@
     # et = EmbeddedText(s)
     num_rows = 100
     mr:ManifoldReduction = ManifoldReduction(2)
     for scalar in [1, 10, 200]:
         print("creating data set [{}]".format(scalar))
         for i in range(num_rows):
             l = np.random.rand(100) *  scalar
-            row_str = "random_synthesized:{}".format( ', '.join(map(str,l)))
+            # testing tweet embedding
+            # row_str = "random_synthesized:{}".format( ', '.join(map(str,l)))
+            # testing narrative embedding
+            row_str =  ','.join(map(str,l))
             # print(row_str)
-            et = mr.load_row(row_str)
+            et = mr.load_row(i, row_str, None, None)
             et.cluster_id = 1
             et.cluster_name = "cluster {}".format(1)
 
     print("Calculating new manifolds")
     # mr.calc_embeding(perplexity=80, pca_components=10)
     # mr.dbscan(eps=8, min_samples=8)
     # mr.plot("perplex = {}".format(80))
@@ -232,10 +343,10 @@
         print("Plotting")
         row = int(i/3)
         col = i%3
         mr.plot_reduced(axs[row][col], "perplex = {}".format(perplexity))
         i += 1
     plt.show()
 
+
 if __name__ == "__main__":
-    #tsne_main()
     main()
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/utils/MySqlInterface.py` & `keyword_explorer-0.5a0/keyword_explorer/utils/MySqlInterface.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/utils/SharedObjects.py` & `keyword_explorer-0.5a0/keyword_explorer/utils/SharedObjects.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,24 +23,29 @@
                 return True
         return False
 
     def load_from_file(self, filename:str):
         """Load the dictionary from a JSON file. Currently sets the type as str
         filename: The name of the file
         """
-        print("loading{}".format(filename))
+        #print("loading {}".format(filename))
         with open(filename) as f:
-            d = json.load(f)
+            d = {}
+            try:
+                d = json.load(f)
+            except json.decoder.JSONDecodeError as e:
+                print("json.decoder.JSONDecodeError: {}".format(e.msg))
             for key, val in d.items():
                 self.add_object(key, val, str)
 
     def print_contents(self):
         d:Dict
+        print("SharedObjects.print_contents()")
         for d in self.object_dict_list:
-            print("name = '{}', type = {}, obj = '{}'".format(d['name'], d['type'], d['object']))
+            print("\tname = '{}', type = {}, obj = '{}'".format(d['name'], d['type'], d['object']))
 
 def main():
     so = SharedObjects()
     so.load_from_file("../ids.json")
     so.print_contents()
 
 if __name__ == "__main__":
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer/utils/TextSimilarity.py` & `keyword_explorer-0.5a0/keyword_explorer/utils/TextSimilarity.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer/utils/wikipedia_search.py` & `keyword_explorer-0.5a0/keyword_explorer/utils/wikipedia_search.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.4a0/keyword_explorer.egg-info/PKG-INFO` & `keyword_explorer-0.5a0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
-Name: keyword-explorer
-Version: 0.4a0
+Name: keyword_explorer
+Version: 0.5a0
 Summary: A set of tools for producing and exploring keywords on Twitter and the Wikipedia
 Home-page: https://github.com/pgfeldman/KeywordExplorer
 Author: Philip Feldman
 Author-email: phil@philfeldman.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 
 Explorer Apps
 ====================================
-There are four applications in this project, _KeywordExplorer_, _TweetsCountExplorer_, _TweetDownloader_, and _WikiPageviewExplorer_. They, and the classes that support them, can be installed with pip:
+There are six applications in this project: KeywordExplorer, TweetsCountExplorer, TweetDownloader, WikiPageviewExplorer, TweetEmbedExplorer, and ModelExplorer. They, and the classes that support them, can be installed with pip:
 
     pip install keyword-explorer
 
 **KeywordExplorer** is a Python desktop app that lets you use the GPT-3 to search for keywords and Twitter to see if those keywords are any good.
 
 **TweetCountsExplorer** is a Python desktop app that lets you explore the quantity of tweets containing keywords over days, weeks or months.
 
 **TweetDownloader** is a Python desktop app that lets you select and download tweets containing keywords into a database. The number of Tweets can be adjusted so that they are the same for each day or proportional. Users can apply daily and overall limits for each keyword corpora.
 
 **WikiPageviewExplorer**  is a Python desktop app that lets you explore keywords that appear as articles in the Wikipedia, and chart their relative page views.
 
+**TweetEmbedExplorer** is a Python desktop app for analyzing, filtering, and augmenting tweet information. Augmented information can them be used to create a train/test corpus for finetuning language models such as the GPT-2.
+
+**ModelExplorer** is a Python desktop app that lets a user interact with a finetuned GPT-2 model trained using EmbeddingExplorer
+
 Full documentation is available at https://github.com/pgfeldman/KeywordExplorer#readme
```

### Comparing `keyword_explorer-0.4a0/keyword_explorer.egg-info/SOURCES.txt` & `keyword_explorer-0.5a0/keyword_explorer.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,50 +6,78 @@
 keyword_explorer/__init__.py
 keyword_explorer.egg-info/PKG-INFO
 keyword_explorer.egg-info/SOURCES.txt
 keyword_explorer.egg-info/dependency_links.txt
 keyword_explorer.egg-info/requires.txt
 keyword_explorer.egg-info/top_level.txt
 keyword_explorer/Apps/AppBase.py
+keyword_explorer/Apps/ContextExplorer.py
 keyword_explorer/Apps/GoogleExplorer.py
 keyword_explorer/Apps/KeywordExplorer.py
 keyword_explorer/Apps/ModelExplorer.py
+keyword_explorer/Apps/NarrativeExplorer.py
+keyword_explorer/Apps/NarrativeExplorer2.py
+keyword_explorer/Apps/TerrainFromGML.py
 keyword_explorer/Apps/TweetCountExplorer.py
 keyword_explorer/Apps/TweetDownloader.py
 keyword_explorer/Apps/TweetEmbedExplorer.py
 keyword_explorer/Apps/WikiPageviewExplorer.py
 keyword_explorer/Apps/__init__.py
 keyword_explorer/OpenAI/OpenAIComms.py
+keyword_explorer/OpenAI/OpenAIEmbeddings.py
+keyword_explorer/Panda3D/DefinedColors.py
+keyword_explorer/Panda3D/DefinedColors_GOES.py
+keyword_explorer/Panda3D/ExampleHand.py
+keyword_explorer/Panda3D/HelloWorld.py
+keyword_explorer/Panda3D/LinePrimitives.py
+keyword_explorer/Panda3D/MouseEventHandler.py
+keyword_explorer/Panda3D/Pandas_main.py
+keyword_explorer/Panda3D/Primitives.py
+keyword_explorer/Panda3D/ProceduralCube.py
+keyword_explorer/Panda3D/ShapePrimitives.py
+keyword_explorer/Panda3D/__init__.py
 keyword_explorer/TwitterV2/TweetKeywords.py
 keyword_explorer/TwitterV2/TwitterV2Base.py
 keyword_explorer/TwitterV2/TwitterV2Counts.py
 keyword_explorer/TwitterV2/__init__.py
 keyword_explorer/TwitterV2/tweet_lookup.py
+keyword_explorer/huggingface/HFaceGPT.py
+keyword_explorer/huggingface/PatternCounter.py
+keyword_explorer/huggingface/__init__.py
+keyword_explorer/huggingface/test1.py
+keyword_explorer/huggingface/test2.py
+keyword_explorer/huggingface/test3.py
 keyword_explorer/mastodon/__init__.py
 keyword_explorer/mastodon/post_lookup.py
 keyword_explorer/tkUtils/Buttons.py
 keyword_explorer/tkUtils/CanvasData.py
 keyword_explorer/tkUtils/CanvasFrame.py
 keyword_explorer/tkUtils/Checkboxes.py
 keyword_explorer/tkUtils/ConsoleDprint.py
 keyword_explorer/tkUtils/DataField.py
 keyword_explorer/tkUtils/DateEntryField.py
+keyword_explorer/tkUtils/GPT3EmbeddingFrame.py
+keyword_explorer/tkUtils/GPT3GeneratorFrame.py
 keyword_explorer/tkUtils/LabeledParam.py
 keyword_explorer/tkUtils/ListField.py
 keyword_explorer/tkUtils/MoveableNode.py
+keyword_explorer/tkUtils/SelectParam.py
 keyword_explorer/tkUtils/TextComparePopup.py
 keyword_explorer/tkUtils/TextField.py
 keyword_explorer/tkUtils/TkCanvasBase.py
 keyword_explorer/tkUtils/ToolTip.py
 keyword_explorer/tkUtils/TopicCombo.py
 keyword_explorer/tkUtils/TopicComboExt.py
 keyword_explorer/tkUtils/__init__.py
+keyword_explorer/tkUtilsExt/GPTContextFrame.py
+keyword_explorer/tkUtilsExt/__init__.py
 keyword_explorer/utils/CorporaGenerator.py
 keyword_explorer/utils/ManifoldReduction.py
 keyword_explorer/utils/MySqlInterface.py
+keyword_explorer/utils/NetworkxGraphing.py
 keyword_explorer/utils/SharedObjects.py
 keyword_explorer/utils/TextSimilarity.py
 keyword_explorer/utils/app_test.py
 keyword_explorer/utils/excel_to_latex.py
 keyword_explorer/utils/find_transformer_models.py
 keyword_explorer/utils/google_search.py
 keyword_explorer/utils/wikipedia_search.py
```

### Comparing `keyword_explorer-0.4a0/setup.py` & `keyword_explorer-0.5a0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 # I spent a good deal of time trying to figure out how to deploy to PyPI using the JetBrains IDE. You can read
 # the details at https://viztales.com/2022/04/05/phil-4-5-2022/
 from  distutils.core import  setup
 
 long_s = '''Explorer Apps
 ====================================
-There are four applications in this project, _KeywordExplorer_, _TweetsCountExplorer_, _TweetDownloader_, and _WikiPageviewExplorer_. They, and the classes that support them, can be installed with pip:
+There are six applications in this project: KeywordExplorer, TweetsCountExplorer, TweetDownloader, WikiPageviewExplorer, TweetEmbedExplorer, and ModelExplorer. They, and the classes that support them, can be installed with pip:
 
     pip install keyword-explorer
 
 **KeywordExplorer** is a Python desktop app that lets you use the GPT-3 to search for keywords and Twitter to see if those keywords are any good.
 
 **TweetCountsExplorer** is a Python desktop app that lets you explore the quantity of tweets containing keywords over days, weeks or months.
 
 **TweetDownloader** is a Python desktop app that lets you select and download tweets containing keywords into a database. The number of Tweets can be adjusted so that they are the same for each day or proportional. Users can apply daily and overall limits for each keyword corpora.
 
 **WikiPageviewExplorer**  is a Python desktop app that lets you explore keywords that appear as articles in the Wikipedia, and chart their relative page views.
 
+**TweetEmbedExplorer** is a Python desktop app for analyzing, filtering, and augmenting tweet information. Augmented information can them be used to create a train/test corpus for finetuning language models such as the GPT-2.
+
+**ModelExplorer** is a Python desktop app that lets a user interact with a finetuned GPT-2 model trained using EmbeddingExplorer
+
 Full documentation is available at https://github.com/pgfeldman/KeywordExplorer#readme'''
 
 setup(
     name='keyword_explorer',
-    version= "0.4.alpha",
+    version= "0.5.alpha",
     packages=['keyword_explorer',
               'keyword_explorer.utils',
               'keyword_explorer.TwitterV2',
               'keyword_explorer.mastodon',
               'keyword_explorer.tkUtils',
+              'keyword_explorer.tkUtilsExt',
               'keyword_explorer.OpenAI',
+              'keyword_explorer.Panda3D',
+              'keyword_explorer.huggingface',
               'keyword_explorer.Apps'],
     url='https://github.com/pgfeldman/KeywordExplorer',
     license='MIT',
     author='Philip Feldman',
     author_email='phil@philfeldman.com',
     description='A set of tools for producing and exploring keywords on Twitter and the Wikipedia',
     long_description=long_s,
     install_requires=[
-        'pandas~=1.3.5',
-        'matplotlib~=3.2.2',
-        'numpy~=1.19.5',
-        'sklearn~=0.0',
-        'scikit-learn~=0.24.2',
-        'requests~=2.27.1',
-        'wikipedia~=1.4.0',
-        'openai~=0.11.5',
-        'networkx~=2.6.2',
-        'tkinterweb~=3.12.2',
-        'PyMySQL~=0.9.3',
-        'python-dateutil~=2.8.0'],
+        'pandas',
+        'matplotlib',
+        'numpy',
+        'scikit-learn',
+        'requests',
+        'transformers',
+        'wikipedia',
+        'openai[embeddings]',
+        'openai',
+        'networkx',
+        'tkinterweb',
+        'PyMySQL',
+        'python-dateutil',
+        'panda3d',
+        'XlsxWriter',
+        'pyperclip'],
 
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
         'Development Status :: 3 - Alpha',
```

