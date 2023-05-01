# Comparing `tmp/CmonCrawl-0.8.0.tar.gz` & `tmp/CmonCrawl-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CmonCrawl-0.8.0.tar", last modified: Mon May  1 15:14:22 2023, max compression
+gzip compressed data, was "CmonCrawl-0.8.1.tar", last modified: Mon May  1 22:06:37 2023, max compression
```

## Comparing `CmonCrawl-0.8.0.tar` & `CmonCrawl-0.8.1.tar`

### file list

```diff
@@ -1,917 +1,917 @@
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.716757 CmonCrawl-0.8.0/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       50 2023-04-30 17:35:29.000000 CmonCrawl-0.8.0/.flake8
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     3078 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/.gitignore
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      377 2023-04-30 17:38:23.000000 CmonCrawl-0.8.0/.pre-commit-config.yaml
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.622700 CmonCrawl-0.8.0/.vscode/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1367 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/.vscode/launch.json
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      459 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/.vscode/settings.json
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.625700 CmonCrawl-0.8.0/CmonCrawl.egg-info/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     3856 2023-05-01 15:14:21.000000 CmonCrawl-0.8.0/CmonCrawl.egg-info/PKG-INFO
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    59389 2023-05-01 15:14:21.000000 CmonCrawl-0.8.0/CmonCrawl.egg-info/SOURCES.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)        1 2023-05-01 15:14:21.000000 CmonCrawl-0.8.0/CmonCrawl.egg-info/dependency_links.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      136 2023-05-01 15:14:21.000000 CmonCrawl-0.8.0/CmonCrawl.egg-info/entry_points.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      433 2023-05-01 15:14:21.000000 CmonCrawl-0.8.0/CmonCrawl.egg-info/requires.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       10 2023-05-01 15:14:21.000000 CmonCrawl-0.8.0/CmonCrawl.egg-info/top_level.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1077 2023-04-27 23:09:07.000000 CmonCrawl-0.8.0/LICENSE
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     3856 2023-05-01 15:14:22.714757 CmonCrawl-0.8.0/PKG-INFO
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     3377 2023-05-01 13:07:40.000000 CmonCrawl-0.8.0/README.md
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.585698 CmonCrawl-0.8.0/cmoncrawl/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.627700 CmonCrawl-0.8.0/cmoncrawl/aggregator/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.629701 CmonCrawl-0.8.0/cmoncrawl/aggregator/.vscode/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-30 17:35:29.000000 CmonCrawl-0.8.0/cmoncrawl/aggregator/.vscode/settings.json
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)        0 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/cmoncrawl/aggregator/__init__.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14169 2023-04-30 17:35:32.000000 CmonCrawl-0.8.0/cmoncrawl/aggregator/index_query.py
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.633701 CmonCrawl-0.8.0/cmoncrawl/aggregator/utils/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)        0 2023-04-26 11:59:53.000000 CmonCrawl-0.8.0/cmoncrawl/aggregator/utils/__init__.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      865 2023-04-30 17:35:31.000000 CmonCrawl-0.8.0/cmoncrawl/aggregator/utils/helpers.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      209 2023-04-30 17:35:30.000000 CmonCrawl-0.8.0/cmoncrawl/aggregator/utils/ndjson_decoder.py
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.634701 CmonCrawl-0.8.0/cmoncrawl/common/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      996 2023-04-30 17:35:31.000000 CmonCrawl-0.8.0/cmoncrawl/common/loggers.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2012 2023-04-30 23:02:02.000000 CmonCrawl-0.8.0/cmoncrawl/common/types.py
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.635701 CmonCrawl-0.8.0/cmoncrawl/integrations/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     8280 2023-05-01 13:06:04.000000 CmonCrawl-0.8.0/cmoncrawl/integrations/commands.py
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.636701 CmonCrawl-0.8.0/cmoncrawl/middleware/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9566 2023-05-01 10:51:18.000000 CmonCrawl-0.8.0/cmoncrawl/middleware/stompware.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2077 2023-04-30 20:18:57.000000 CmonCrawl-0.8.0/cmoncrawl/middleware/synchronized.py
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.636701 CmonCrawl-0.8.0/cmoncrawl/processor/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)        0 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/cmoncrawl/processor/__init__.py
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.637701 CmonCrawl-0.8.0/cmoncrawl/processor/extraction/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      889 2023-04-30 17:35:31.000000 CmonCrawl-0.8.0/cmoncrawl/processor/extraction/filters.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4877 2023-04-30 21:20:37.000000 CmonCrawl-0.8.0/cmoncrawl/processor/extraction/utils.py
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.640701 CmonCrawl-0.8.0/cmoncrawl/processor/pipeline/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7218 2023-04-30 17:35:32.000000 CmonCrawl-0.8.0/cmoncrawl/processor/pipeline/downloader.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4666 2023-04-30 17:35:31.000000 CmonCrawl-0.8.0/cmoncrawl/processor/pipeline/extractor.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2123 2023-04-30 20:18:57.000000 CmonCrawl-0.8.0/cmoncrawl/processor/pipeline/pipeline.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4471 2023-04-30 23:07:42.000000 CmonCrawl-0.8.0/cmoncrawl/processor/pipeline/router.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6949 2023-04-30 17:35:32.000000 CmonCrawl-0.8.0/cmoncrawl/processor/pipeline/streamer.py
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.649701 CmonCrawl-0.8.0/docs/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)        0 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/.nojekyll
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      638 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/Makefile
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.650702 CmonCrawl-0.8.0/docs/build/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.651702 CmonCrawl-0.8.0/docs/build/_templates/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1196 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/_templates/module.rst
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.664702 CmonCrawl-0.8.0/docs/build/doctrees/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4988 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/api.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   432023 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/environment.pickle
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.852712 CmonCrawl-0.8.0/docs/build/doctrees/generated/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6830 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7703 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.DomainCrawl.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18142 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.DomainCrawl.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    11535 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.DomainRecord.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    28776 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.DomainRecord.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15987 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9300 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.aclose.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4780 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.aopen.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    37306 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6931 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    11573 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9802 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6959 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.RetrieveResponse.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16217 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.RetrieveResponse.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    12195 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    13894 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6099 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.decode.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    25669 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5998 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5313 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2836 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.utils.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6678 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.aggregator.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5704 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    23297 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7163 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6855 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7122 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6296 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6365 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    63109 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7415 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5989 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6188 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6257 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6156 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5623 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22264 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_utils.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6230 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6228 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4108 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     8687 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6863 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.download.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     8901 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9338 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4819 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    21971 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5334 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.download.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7300 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6343 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     8635 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    21634 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5485 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5156 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5139 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5784 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5521 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7253 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4131 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17494 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7235 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5817 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5733 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6077 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6001 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5357 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4134 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17329 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7176 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7645 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6005 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6074 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5939 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5244 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    13578 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor_utils.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7331 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4214 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4499 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    10160 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6911 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5407 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4146 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4966 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9930 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7282 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5296 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    10859 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4988 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    26191 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5369 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6452 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7370 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7997 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5048 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20487 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5429 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6516 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7430 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     8146 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4943 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20720 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5324 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6404 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7325 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     8033 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5103 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Pipeline.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6675 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14037 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5595 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5338 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5045 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7838 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Route.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    19442 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Route.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     3956 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    12897 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4819 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.load_module.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4809 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.load_modules.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9888 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.register_route.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6057 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.register_routes.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6505 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.route.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6097 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    10563 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    11571 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.processor_utils.DomainRecord.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    30222 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.processor_utils.DomainRecord.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7292 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.processor_utils.PipeMetadata.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    21042 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.processor_utils.PipeMetadata.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6542 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.processor_utils.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6611 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5813 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.process_article.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5991 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    29297 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5904 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_before_message.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5697 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_connected.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6832 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_connecting.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4587 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_disconnected.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4345 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_disconnecting.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5507 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_error.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4265 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_heartbeat.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4542 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_heartbeat_timeout.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6147 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_message.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5693 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_receipt.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4750 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_receiver_loop_completed.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5519 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_send.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6915 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.ListnerStats.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15725 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.ListnerStats.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6504 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Message.__init__.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14780 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Message.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    12891 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5144 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/index.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5145 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/installation.doctree
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.856712 CmonCrawl-0.8.0/docs/build/doctrees/quickstart/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5390 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/quickstart/artemis-queue.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2146 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/quickstart/download_article.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2887 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/quickstart/index.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4063 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/quickstart/installation.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2140 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/quickstart/middleware.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    25389 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/quickstart/overview.doctree
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    45690 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/doctrees/quickstart/quick-start.doctree
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.868713 CmonCrawl-0.8.0/docs/build/html/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      230 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/.buildinfo
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.873713 CmonCrawl-0.8.0/docs/build/html/_sources/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      105 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/api.rst.txt
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.999720 CmonCrawl-0.8.0/docs/build/html/_sources/generated/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      190 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainCrawl.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      441 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainCrawl.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      193 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainRecord.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      558 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainRecord.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      202 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      188 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.aclose.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      185 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.aopen.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      230 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      240 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      233 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      512 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      205 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.RetrieveResponse.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      475 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.RetrieveResponse.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      433 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      187 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      173 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.Decoder.decode.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      187 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      347 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.Decoder.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      246 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      272 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      135 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.utils.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      249 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.aggregator.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      219 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      259 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      274 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      271 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      271 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      282 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      285 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      248 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      265 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      259 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      262 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      257 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      903 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      300 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      711 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_utils.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      316 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      212 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.Downloader.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      204 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.Downloader.download.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      354 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.Downloader.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      224 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      210 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      207 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      216 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.download.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      460 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      210 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      286 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      247 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      239 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      250 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      253 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      256 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      507 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      290 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      299 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Downloader.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      223 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      212 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      229 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      223 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      226 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      601 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      278 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      204 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      218 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      213 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      629 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      262 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      467 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.extractor_utils.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      335 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      238 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      232 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      414 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      224 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      285 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      391 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      207 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      272 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      347 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      267 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      261 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      278 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      293 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      563 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      253 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      279 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      273 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      290 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      305 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      595 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      265 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      258 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      252 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      269 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      284 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      539 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      244 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      355 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      256 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      390 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      260 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Pipeline.pipeline.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      244 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Pipeline.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      173 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Router.router.Route.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      412 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Router.router.Route.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      176 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Router.router.Router.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      179 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Router.router.Router.load_module.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      182 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Router.router.Router.load_modules.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      188 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Router.router.Router.register_route.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      191 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Router.router.Router.register_routes.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      159 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Router.router.Router.route.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      419 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Router.router.Router.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      249 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Router.router.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      234 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Router.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      202 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.processor_utils.DomainRecord.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      567 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.processor_utils.DomainRecord.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      202 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.processor_utils.PipeMetadata.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      559 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.processor_utils.PipeMetadata.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      270 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.processor_utils.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      379 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      239 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.process_article.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      158 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      181 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.on_before_message.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      164 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.on_connected.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      167 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.on_connecting.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      173 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.on_disconnected.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      176 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.on_disconnecting.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      152 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.on_error.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      164 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.on_heartbeat.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      190 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.on_heartbeat_timeout.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      158 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.on_message.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      158 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.on_receipt.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      210 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.on_receiver_loop_completed.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      149 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.on_send.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      641 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      170 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.ListnerStats.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      409 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.ListnerStats.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      155 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Message.__init__.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      363 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Message.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      420 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      242 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      526 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      658 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/installation.rst.txt
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.003720 CmonCrawl-0.8.0/docs/build/html/_sources/quickstart/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      665 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/quickstart/artemis-queue.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       32 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/quickstart/download_article.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      138 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/quickstart/index.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      421 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/quickstart/installation.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)        0 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/quickstart/middleware.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5429 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/quickstart/overview.rst.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    12222 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_sources/quickstart/quick-start.rst.txt
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.018720 CmonCrawl-0.8.0/docs/build/html/_static/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4418 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14621 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/basic.css
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      313 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/check-solid.svg
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9031 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/clipboard.min.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      411 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/copy-button.svg
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2010 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/copybutton.css
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7479 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/copybutton.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2198 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/copybutton_funcs.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4472 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/doctools.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      417 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/documentation_options.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      286 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/file.png
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.020721 CmonCrawl-0.8.0/docs/build/html/_static/images/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1186 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/images/logo_binder.svg
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7601 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/images/logo_colab.png
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      681 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1758 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   288580 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/jquery-3.6.0.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    89501 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/jquery.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4758 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/language_data.js
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.610700 CmonCrawl-0.8.0/docs/build/html/_static/locales/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.594699 CmonCrawl-0.8.0/docs/build/html/_static/locales/ar/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.020721 CmonCrawl-0.8.0/docs/build/html/_static/locales/ar/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1608 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.595699 CmonCrawl-0.8.0/docs/build/html/_static/locales/bg/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.021721 CmonCrawl-0.8.0/docs/build/html/_static/locales/bg/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1789 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.595699 CmonCrawl-0.8.0/docs/build/html/_static/locales/bn/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.021721 CmonCrawl-0.8.0/docs/build/html/_static/locales/bn/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1667 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.596699 CmonCrawl-0.8.0/docs/build/html/_static/locales/ca/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.022721 CmonCrawl-0.8.0/docs/build/html/_static/locales/ca/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1231 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.596699 CmonCrawl-0.8.0/docs/build/html/_static/locales/cs/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.022721 CmonCrawl-0.8.0/docs/build/html/_static/locales/cs/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1449 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.596699 CmonCrawl-0.8.0/docs/build/html/_static/locales/da/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.023721 CmonCrawl-0.8.0/docs/build/html/_static/locales/da/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1343 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.597699 CmonCrawl-0.8.0/docs/build/html/_static/locales/de/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.023721 CmonCrawl-0.8.0/docs/build/html/_static/locales/de/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1444 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.597699 CmonCrawl-0.8.0/docs/build/html/_static/locales/el/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.023721 CmonCrawl-0.8.0/docs/build/html/_static/locales/el/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1816 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.598699 CmonCrawl-0.8.0/docs/build/html/_static/locales/eo/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.024721 CmonCrawl-0.8.0/docs/build/html/_static/locales/eo/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1384 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.598699 CmonCrawl-0.8.0/docs/build/html/_static/locales/es/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.024721 CmonCrawl-0.8.0/docs/build/html/_static/locales/es/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1438 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.598699 CmonCrawl-0.8.0/docs/build/html/_static/locales/et/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.025721 CmonCrawl-0.8.0/docs/build/html/_static/locales/et/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1391 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.599699 CmonCrawl-0.8.0/docs/build/html/_static/locales/fi/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.025721 CmonCrawl-0.8.0/docs/build/html/_static/locales/fi/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1409 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.599699 CmonCrawl-0.8.0/docs/build/html/_static/locales/fr/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.026721 CmonCrawl-0.8.0/docs/build/html/_static/locales/fr/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1469 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.600699 CmonCrawl-0.8.0/docs/build/html/_static/locales/hr/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.026721 CmonCrawl-0.8.0/docs/build/html/_static/locales/hr/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1449 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.600699 CmonCrawl-0.8.0/docs/build/html/_static/locales/id/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.026721 CmonCrawl-0.8.0/docs/build/html/_static/locales/id/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1360 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.600699 CmonCrawl-0.8.0/docs/build/html/_static/locales/it/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.027721 CmonCrawl-0.8.0/docs/build/html/_static/locales/it/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1447 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.601699 CmonCrawl-0.8.0/docs/build/html/_static/locales/iw/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.027721 CmonCrawl-0.8.0/docs/build/html/_static/locales/iw/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1490 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.601699 CmonCrawl-0.8.0/docs/build/html/_static/locales/ja/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.028721 CmonCrawl-0.8.0/docs/build/html/_static/locales/ja/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1518 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.601699 CmonCrawl-0.8.0/docs/build/html/_static/locales/ko/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.028721 CmonCrawl-0.8.0/docs/build/html/_static/locales/ko/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1406 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.601699 CmonCrawl-0.8.0/docs/build/html/_static/locales/lt/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.028721 CmonCrawl-0.8.0/docs/build/html/_static/locales/lt/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1461 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.602699 CmonCrawl-0.8.0/docs/build/html/_static/locales/lv/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.029721 CmonCrawl-0.8.0/docs/build/html/_static/locales/lv/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1450 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.602699 CmonCrawl-0.8.0/docs/build/html/_static/locales/ml/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.029721 CmonCrawl-0.8.0/docs/build/html/_static/locales/ml/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1890 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.602699 CmonCrawl-0.8.0/docs/build/html/_static/locales/mr/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.029721 CmonCrawl-0.8.0/docs/build/html/_static/locales/mr/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1675 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.603699 CmonCrawl-0.8.0/docs/build/html/_static/locales/ms/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.030721 CmonCrawl-0.8.0/docs/build/html/_static/locales/ms/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1189 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.603699 CmonCrawl-0.8.0/docs/build/html/_static/locales/nl/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.030721 CmonCrawl-0.8.0/docs/build/html/_static/locales/nl/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1398 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.603699 CmonCrawl-0.8.0/docs/build/html/_static/locales/no/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.030721 CmonCrawl-0.8.0/docs/build/html/_static/locales/no/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1357 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.604699 CmonCrawl-0.8.0/docs/build/html/_static/locales/pl/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.031721 CmonCrawl-0.8.0/docs/build/html/_static/locales/pl/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1420 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.604699 CmonCrawl-0.8.0/docs/build/html/_static/locales/pt/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.031721 CmonCrawl-0.8.0/docs/build/html/_static/locales/pt/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1409 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.604699 CmonCrawl-0.8.0/docs/build/html/_static/locales/ro/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.032721 CmonCrawl-0.8.0/docs/build/html/_static/locales/ro/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1441 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.605699 CmonCrawl-0.8.0/docs/build/html/_static/locales/ru/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.032721 CmonCrawl-0.8.0/docs/build/html/_static/locales/ru/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1797 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.605699 CmonCrawl-0.8.0/docs/build/html/_static/locales/sk/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.033721 CmonCrawl-0.8.0/docs/build/html/_static/locales/sk/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1441 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.605699 CmonCrawl-0.8.0/docs/build/html/_static/locales/sl/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.033721 CmonCrawl-0.8.0/docs/build/html/_static/locales/sl/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1418 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.606699 CmonCrawl-0.8.0/docs/build/html/_static/locales/sr/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.033721 CmonCrawl-0.8.0/docs/build/html/_static/locales/sr/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1760 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.606699 CmonCrawl-0.8.0/docs/build/html/_static/locales/sv/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.034721 CmonCrawl-0.8.0/docs/build/html/_static/locales/sv/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1391 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.606699 CmonCrawl-0.8.0/docs/build/html/_static/locales/ta/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.034721 CmonCrawl-0.8.0/docs/build/html/_static/locales/ta/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1968 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.607699 CmonCrawl-0.8.0/docs/build/html/_static/locales/te/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.035721 CmonCrawl-0.8.0/docs/build/html/_static/locales/te/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1834 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.607699 CmonCrawl-0.8.0/docs/build/html/_static/locales/tg/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.036722 CmonCrawl-0.8.0/docs/build/html/_static/locales/tg/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1710 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.607699 CmonCrawl-0.8.0/docs/build/html/_static/locales/th/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.037721 CmonCrawl-0.8.0/docs/build/html/_static/locales/th/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1860 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.608699 CmonCrawl-0.8.0/docs/build/html/_static/locales/tl/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.037721 CmonCrawl-0.8.0/docs/build/html/_static/locales/tl/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1259 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.608699 CmonCrawl-0.8.0/docs/build/html/_static/locales/tr/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.038722 CmonCrawl-0.8.0/docs/build/html/_static/locales/tr/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1405 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.608699 CmonCrawl-0.8.0/docs/build/html/_static/locales/uk/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.038722 CmonCrawl-0.8.0/docs/build/html/_static/locales/uk/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1756 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.609699 CmonCrawl-0.8.0/docs/build/html/_static/locales/ur/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.039722 CmonCrawl-0.8.0/docs/build/html/_static/locales/ur/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1460 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.609699 CmonCrawl-0.8.0/docs/build/html/_static/locales/vi/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.039722 CmonCrawl-0.8.0/docs/build/html/_static/locales/vi/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1487 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.610700 CmonCrawl-0.8.0/docs/build/html/_static/locales/zh_CN/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.040722 CmonCrawl-0.8.0/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1279 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.610700 CmonCrawl-0.8.0/docs/build/html/_static/locales/zh_TW/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.040722 CmonCrawl-0.8.0/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1323 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       90 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/minus.png
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       90 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/plus.png
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5510 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/pygments.css
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      419 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/sbt-webpack-macros.html
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.043722 CmonCrawl-0.8.0/docs/build/html/_static/scripts/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    87299 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     3388 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15106 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/searchtools.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4712 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.046722 CmonCrawl-0.8.0/docs/build/html/_static/styles/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   162094 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20970 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5488 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/styles/theme.css
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    68420 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    19530 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/underscore.js
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.611699 CmonCrawl-0.8.0/docs/build/html/_static/vendor/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.611699 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.047722 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1548 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.047722 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/css/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    58578 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.114725 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   133034 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   715890 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   132728 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    89824 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    76612 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    34390 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   144322 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    34092 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16800 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    13584 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   202902 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   897426 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   202616 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   103300 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    79444 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1361 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/_static/webpack-macros.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14884 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/api.html
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.395740 CmonCrawl-0.8.0/docs/build/html/generated/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15433 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17399 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.DomainCrawl.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20855 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.DomainCrawl.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18729 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.DomainRecord.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    24159 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.DomainRecord.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20332 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18026 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.aclose.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16729 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.aopen.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17323 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    19039 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18171 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    28037 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17093 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.RetrieveResponse.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20354 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.RetrieveResponse.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16683 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20028 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16884 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.decode.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    24580 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16881 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15016 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.ndjson_decoder.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14329 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.utils.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14859 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.aggregator.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14923 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22512 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17934 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17801 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17957 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17767 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17754 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17987 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17499 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17640 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17647 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    35243 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17503 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15382 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18043 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_utils.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15594 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16326 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17530 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.download.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18286 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17916 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18174 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16837 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16918 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.download.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22820 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17667 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15390 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17869 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17079 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16854 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16876 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22678 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16909 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15276 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15191 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16373 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17539 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17091 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17083 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17239 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20711 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17115 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15044 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16349 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17515 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17657 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17208 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20629 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17123 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15140 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16355 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor_utils.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15787 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16479 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16595 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18928 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17315 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15098 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15699 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16383 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16705 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18768 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17457 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15184 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18754 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16961 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17216 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    24427 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17443 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17777 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17817 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17045 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17300 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22651 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17527 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17817 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17812 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16898 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17153 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22694 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17380 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17546 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16214 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14984 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Pipeline.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17657 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20930 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16946 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15017 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Pipeline.pipeline.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14956 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17281 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Route.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20799 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Route.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16110 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    19510 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16408 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.load_module.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16436 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.load_modules.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18032 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.register_route.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16805 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.register_routes.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17244 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.route.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15177 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16649 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18771 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.processor_utils.DomainRecord.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    24125 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.processor_utils.DomainRecord.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17699 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.processor_utils.PipeMetadata.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22093 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.processor_utils.PipeMetadata.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15405 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.processor_utils.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15281 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14868 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.process_article.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16886 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    24450 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16619 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_before_message.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16532 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_connected.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16819 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_connecting.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16361 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_disconnected.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_disconnecting.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16409 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_error.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16181 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_heartbeat.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16334 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_heartbeat_timeout.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16570 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_message.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16546 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_receipt.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16420 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_receiver_loop_completed.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16414 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_send.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17119 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.ListnerStats.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20228 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.ListnerStats.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16511 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Message.__init__.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    19876 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Message.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16556 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    56110 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/genindex.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    19730 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/index.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16148 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/installation.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    12364 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/objects.inv
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20823 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/py-modindex.html
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.399740 CmonCrawl-0.8.0/docs/build/html/quickstart/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15316 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/quickstart/artemis-queue.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14124 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/quickstart/download_article.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16829 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/quickstart/index.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14023 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/quickstart/installation.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    13934 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/quickstart/middleware.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    25924 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/quickstart/overview.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    42595 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/quickstart/quick-start.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    13374 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/search.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    75786 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/html/searchindex.js
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       71 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/build/index.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       71 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/index.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      769 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/make.bat
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.402741 CmonCrawl-0.8.0/docs/source/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      105 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/api.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2756 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/conf.py
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.600751 CmonCrawl-0.8.0/docs/source/generated/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      190 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.DomainCrawl.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      441 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.DomainCrawl.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      193 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.DomainRecord.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      558 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.DomainRecord.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      202 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.IndexAggregator.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      188 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.IndexAggregator.aclose.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      185 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.IndexAggregator.aopen.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      230 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      240 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      233 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      512 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.IndexAggregator.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      205 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.RetrieveResponse.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      475 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.RetrieveResponse.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      433 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      187 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      173 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.ndjson_decoder.Decoder.decode.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      187 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      347 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.ndjson_decoder.Decoder.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      246 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.ndjson_decoder.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      272 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      135 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.utils.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      249 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.aggregator.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      219 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Aggregator.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      259 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      274 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      271 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      271 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      282 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      285 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      248 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      265 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      259 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      262 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      257 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      903 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      300 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      711 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_utils.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      316 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      212 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.downloader.Downloader.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      204 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.downloader.Downloader.download.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      354 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.downloader.Downloader.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      224 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      210 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      207 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      216 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.download.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      460 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      210 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      286 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.downloader.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      247 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      239 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      250 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      253 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      256 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      507 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      290 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.dummy_downloader.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      299 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Downloader.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      223 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      212 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      229 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      223 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      226 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      601 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      278 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.dummy_extractor.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      204 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      218 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      213 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      629 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      262 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.extractor.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      467 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.extractor_utils.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      335 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      238 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      232 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      414 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      224 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      285 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      391 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      207 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      272 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.outstreamer.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      347 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      267 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      261 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      278 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      293 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      563 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      253 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      279 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      273 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      290 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      305 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      595 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      265 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      258 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      252 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      269 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      284 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      539 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      244 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      355 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      256 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      390 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      260 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Pipeline.pipeline.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      244 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Pipeline.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      173 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Router.router.Route.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      412 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Router.router.Route.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      176 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Router.router.Router.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      179 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Router.router.Router.load_module.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      182 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Router.router.Router.load_modules.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      188 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Router.router.Router.register_route.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      191 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Router.router.Router.register_routes.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      159 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Router.router.Router.route.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      419 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Router.router.Router.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      249 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Router.router.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      234 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.Router.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      202 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.processor_utils.DomainRecord.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      567 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.processor_utils.DomainRecord.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      202 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.processor_utils.PipeMetadata.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      559 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.processor_utils.PipeMetadata.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      270 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.processor_utils.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      379 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.App.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      239 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.process_article.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      158 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      181 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.on_before_message.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      164 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.on_connected.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      167 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.on_connecting.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      173 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.on_disconnected.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      176 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.on_disconnecting.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      152 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.on_error.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      164 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.on_heartbeat.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      190 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.on_heartbeat_timeout.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      158 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.on_message.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      158 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.on_receipt.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      210 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.on_receiver_loop_completed.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      149 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.on_send.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      641 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      170 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.ListnerStats.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      409 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.ListnerStats.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      155 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Message.__init__.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      363 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Message.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      420 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.processor.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      242 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/generated/Processor.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      526 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/index.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      658 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/installation.rst
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.617752 CmonCrawl-0.8.0/docs/source/quickstart/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      665 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/quickstart/artemis-queue.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      138 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/quickstart/index.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5429 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/quickstart/overview.rst
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    12222 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/docs/source/quickstart/quick-start.rst
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:21.613700 CmonCrawl-0.8.0/examples/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.622752 CmonCrawl-0.8.0/examples/extractor_tutorial/
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.626752 CmonCrawl-0.8.0/examples/extractor_tutorial/Extractors/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1357 2023-04-26 09:40:00.000000 CmonCrawl-0.8.0/examples/extractor_tutorial/Extractors/bbc_extractor.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      181 2023-04-30 17:35:08.000000 CmonCrawl-0.8.0/examples/extractor_tutorial/config.json
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1368 2023-05-01 13:08:22.000000 CmonCrawl-0.8.0/pyproject.toml
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      433 2023-04-30 17:44:12.000000 CmonCrawl-0.8.0/requirements.txt
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       38 2023-05-01 15:14:22.717757 CmonCrawl-0.8.0/setup.cfg
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.635753 CmonCrawl-0.8.0/tests/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7126 2023-04-27 23:19:10.000000 CmonCrawl-0.8.0/tests/aggregator_tests.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2822 2023-04-30 17:35:31.000000 CmonCrawl-0.8.0/tests/end_to_end_tests.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4642 2023-04-30 17:35:09.000000 CmonCrawl-0.8.0/tests/processor_tests.py
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.638753 CmonCrawl-0.8.0/tests/test_extract/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      272 2023-04-30 17:35:29.000000 CmonCrawl-0.8.0/tests/test_extract/cfg.json
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.641753 CmonCrawl-0.8.0/tests/test_extract/extractors/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      495 2023-04-30 17:35:31.000000 CmonCrawl-0.8.0/tests/test_extract/extractors/test_extract.py
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.668754 CmonCrawl-0.8.0/tests/test_extract/files/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   828135 2023-04-30 17:35:30.000000 CmonCrawl-0.8.0/tests/test_extract/files/file.html
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)  1743032 2023-04-30 13:23:44.000000 CmonCrawl-0.8.0/tests/test_extract/files/file.json
-drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 15:14:22.712756 CmonCrawl-0.8.0/tests/test_routes/
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      401 2023-04-27 21:31:25.000000 CmonCrawl-0.8.0/tests/test_routes/a.py
--rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      400 2023-04-27 21:31:36.000000 CmonCrawl-0.8.0/tests/test_routes/b.py
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:37.369255 CmonCrawl-0.8.1/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       50 2023-04-30 17:35:29.000000 CmonCrawl-0.8.1/.flake8
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     3078 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/.gitignore
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      377 2023-04-30 17:38:23.000000 CmonCrawl-0.8.1/.pre-commit-config.yaml
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.622253 CmonCrawl-0.8.1/.vscode/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1367 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/.vscode/launch.json
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      459 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/.vscode/settings.json
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.634253 CmonCrawl-0.8.1/CmonCrawl.egg-info/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4271 2023-05-01 22:06:35.000000 CmonCrawl-0.8.1/CmonCrawl.egg-info/PKG-INFO
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    59389 2023-05-01 22:06:35.000000 CmonCrawl-0.8.1/CmonCrawl.egg-info/SOURCES.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)        1 2023-05-01 22:06:35.000000 CmonCrawl-0.8.1/CmonCrawl.egg-info/dependency_links.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      136 2023-05-01 22:06:35.000000 CmonCrawl-0.8.1/CmonCrawl.egg-info/entry_points.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      433 2023-05-01 22:06:35.000000 CmonCrawl-0.8.1/CmonCrawl.egg-info/requires.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       10 2023-05-01 22:06:35.000000 CmonCrawl-0.8.1/CmonCrawl.egg-info/top_level.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1077 2023-04-27 23:09:07.000000 CmonCrawl-0.8.1/LICENSE
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4271 2023-05-01 22:06:37.368255 CmonCrawl-0.8.1/PKG-INFO
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     3793 2023-05-01 15:38:11.000000 CmonCrawl-0.8.1/README.md
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.543253 CmonCrawl-0.8.1/cmoncrawl/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.639253 CmonCrawl-0.8.1/cmoncrawl/aggregator/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.641253 CmonCrawl-0.8.1/cmoncrawl/aggregator/.vscode/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-30 17:35:29.000000 CmonCrawl-0.8.1/cmoncrawl/aggregator/.vscode/settings.json
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)        0 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/cmoncrawl/aggregator/__init__.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14212 2023-05-01 22:00:39.000000 CmonCrawl-0.8.1/cmoncrawl/aggregator/index_query.py
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.649253 CmonCrawl-0.8.1/cmoncrawl/aggregator/utils/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)        0 2023-04-26 11:59:53.000000 CmonCrawl-0.8.1/cmoncrawl/aggregator/utils/__init__.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      865 2023-04-30 17:35:31.000000 CmonCrawl-0.8.1/cmoncrawl/aggregator/utils/helpers.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      209 2023-04-30 17:35:30.000000 CmonCrawl-0.8.1/cmoncrawl/aggregator/utils/ndjson_decoder.py
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.657253 CmonCrawl-0.8.1/cmoncrawl/common/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      996 2023-04-30 17:35:31.000000 CmonCrawl-0.8.1/cmoncrawl/common/loggers.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2012 2023-04-30 23:02:02.000000 CmonCrawl-0.8.1/cmoncrawl/common/types.py
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.666253 CmonCrawl-0.8.1/cmoncrawl/integrations/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     8283 2023-05-01 15:38:08.000000 CmonCrawl-0.8.1/cmoncrawl/integrations/commands.py
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.674253 CmonCrawl-0.8.1/cmoncrawl/middleware/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    10071 2023-05-01 22:02:31.000000 CmonCrawl-0.8.1/cmoncrawl/middleware/stompware.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2077 2023-04-30 20:18:57.000000 CmonCrawl-0.8.1/cmoncrawl/middleware/synchronized.py
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.680253 CmonCrawl-0.8.1/cmoncrawl/processor/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)        0 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/cmoncrawl/processor/__init__.py
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.686253 CmonCrawl-0.8.1/cmoncrawl/processor/extraction/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      889 2023-04-30 17:35:31.000000 CmonCrawl-0.8.1/cmoncrawl/processor/extraction/filters.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4882 2023-05-01 15:38:08.000000 CmonCrawl-0.8.1/cmoncrawl/processor/extraction/utils.py
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.709253 CmonCrawl-0.8.1/cmoncrawl/processor/pipeline/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7218 2023-04-30 17:35:32.000000 CmonCrawl-0.8.1/cmoncrawl/processor/pipeline/downloader.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4666 2023-04-30 17:35:31.000000 CmonCrawl-0.8.1/cmoncrawl/processor/pipeline/extractor.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2123 2023-04-30 20:18:57.000000 CmonCrawl-0.8.1/cmoncrawl/processor/pipeline/pipeline.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4471 2023-04-30 23:07:42.000000 CmonCrawl-0.8.1/cmoncrawl/processor/pipeline/router.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6949 2023-04-30 17:35:32.000000 CmonCrawl-0.8.1/cmoncrawl/processor/pipeline/streamer.py
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.728253 CmonCrawl-0.8.1/docs/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)        0 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/.nojekyll
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      638 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/Makefile
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.731253 CmonCrawl-0.8.1/docs/build/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.737253 CmonCrawl-0.8.1/docs/build/_templates/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1196 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/_templates/module.rst
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.756253 CmonCrawl-0.8.1/docs/build/doctrees/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4988 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/api.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   432023 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/environment.pickle
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.065254 CmonCrawl-0.8.1/docs/build/doctrees/generated/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6830 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7703 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.DomainCrawl.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18142 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.DomainCrawl.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    11535 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.DomainRecord.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    28776 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.DomainRecord.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15987 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9300 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.aclose.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4780 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.aopen.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    37306 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6931 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    11573 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9802 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6959 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.RetrieveResponse.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16217 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.RetrieveResponse.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    12195 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    13894 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6099 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.decode.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    25669 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5998 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5313 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2836 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.utils.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6678 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.aggregator.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5704 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    23297 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7163 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6855 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7122 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6296 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6365 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    63109 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7415 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5989 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6188 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6257 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6156 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5623 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22264 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_utils.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6230 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6228 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4108 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     8687 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6863 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.download.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     8901 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9338 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4819 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    21971 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5334 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.download.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7300 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6343 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     8635 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    21634 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5485 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5156 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5139 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5784 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5521 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7253 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4131 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17494 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7235 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5817 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5733 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6077 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6001 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5357 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4134 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17329 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7176 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7645 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6005 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6074 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5939 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5244 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    13578 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor_utils.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7331 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4214 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4499 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    10160 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6911 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5407 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4146 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4966 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9930 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7282 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5296 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    10859 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4988 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    26191 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5369 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6452 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7370 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7997 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5048 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20487 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5429 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6516 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7430 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     8146 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4943 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20720 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5324 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6404 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7325 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     8033 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5103 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Pipeline.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6675 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14037 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5595 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5338 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5045 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7838 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Route.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    19442 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Route.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     3956 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    12897 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4819 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.load_module.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4809 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.load_modules.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9888 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.register_route.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6057 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.register_routes.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6505 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.route.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6097 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    10563 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    11571 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.processor_utils.DomainRecord.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    30222 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.processor_utils.DomainRecord.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7292 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.processor_utils.PipeMetadata.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    21042 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.processor_utils.PipeMetadata.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6542 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.processor_utils.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6611 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5813 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.process_article.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5991 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    29297 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5904 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_before_message.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5697 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_connected.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6832 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_connecting.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4587 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_disconnected.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4345 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_disconnecting.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5507 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_error.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4265 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_heartbeat.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4542 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_heartbeat_timeout.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6147 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_message.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5693 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_receipt.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4750 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_receiver_loop_completed.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5519 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_send.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6915 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.ListnerStats.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15725 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.ListnerStats.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     6504 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Message.__init__.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14780 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Message.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    12891 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5144 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/index.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5145 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/installation.doctree
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.073254 CmonCrawl-0.8.1/docs/build/doctrees/quickstart/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5390 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/quickstart/artemis-queue.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2146 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/quickstart/download_article.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2887 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/quickstart/index.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4063 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/quickstart/installation.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2140 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/quickstart/middleware.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    25389 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/quickstart/overview.doctree
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    45690 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/doctrees/quickstart/quick-start.doctree
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.083254 CmonCrawl-0.8.1/docs/build/html/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      230 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/.buildinfo
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.089254 CmonCrawl-0.8.1/docs/build/html/_sources/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      105 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/api.rst.txt
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.207254 CmonCrawl-0.8.1/docs/build/html/_sources/generated/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      190 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainCrawl.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      441 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainCrawl.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      193 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainRecord.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      558 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainRecord.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      202 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      188 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.aclose.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      185 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.aopen.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      230 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      240 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      233 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      512 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      205 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.RetrieveResponse.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      475 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.RetrieveResponse.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      433 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      187 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      173 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.Decoder.decode.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      187 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      347 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.Decoder.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      246 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      272 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      135 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.utils.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      249 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.aggregator.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      219 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      259 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      274 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      271 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      271 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      282 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      285 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      248 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      265 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      259 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      262 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      257 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      903 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      300 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      711 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_utils.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      316 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      212 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.Downloader.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      204 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.Downloader.download.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      354 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.Downloader.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      224 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      210 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      207 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      216 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.download.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      460 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      210 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      286 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      247 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      239 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      250 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      253 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      256 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      507 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      290 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      299 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Downloader.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      223 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      212 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      229 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      223 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      226 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      601 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      278 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      204 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      218 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      213 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      629 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      262 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      467 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.extractor_utils.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      335 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      238 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      232 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      414 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      224 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      285 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      391 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      207 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      272 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      347 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      267 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      261 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      278 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      293 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      563 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      253 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      279 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      273 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      290 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      305 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      595 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      265 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      258 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      252 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      269 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      284 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      539 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      244 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      355 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      256 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      390 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      260 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Pipeline.pipeline.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      244 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Pipeline.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      173 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Router.router.Route.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      412 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Router.router.Route.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      176 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Router.router.Router.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      179 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Router.router.Router.load_module.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      182 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Router.router.Router.load_modules.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      188 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Router.router.Router.register_route.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      191 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Router.router.Router.register_routes.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      159 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Router.router.Router.route.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      419 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Router.router.Router.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      249 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Router.router.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      234 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Router.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      202 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.processor_utils.DomainRecord.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      567 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.processor_utils.DomainRecord.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      202 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.processor_utils.PipeMetadata.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      559 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.processor_utils.PipeMetadata.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      270 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.processor_utils.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      379 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      239 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.process_article.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      158 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      181 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.on_before_message.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      164 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.on_connected.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      167 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.on_connecting.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      173 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.on_disconnected.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      176 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.on_disconnecting.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      152 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.on_error.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      164 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.on_heartbeat.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      190 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.on_heartbeat_timeout.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      158 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.on_message.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      158 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.on_receipt.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      210 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.on_receiver_loop_completed.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      149 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.on_send.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      641 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      170 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.ListnerStats.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      409 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.ListnerStats.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      155 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Message.__init__.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      363 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Message.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      420 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      242 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      526 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      658 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/installation.rst.txt
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.211254 CmonCrawl-0.8.1/docs/build/html/_sources/quickstart/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      665 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/quickstart/artemis-queue.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       32 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/quickstart/download_article.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      138 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/quickstart/index.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      421 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/quickstart/installation.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)        0 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/quickstart/middleware.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5429 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/quickstart/overview.rst.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    12222 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_sources/quickstart/quick-start.rst.txt
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.242254 CmonCrawl-0.8.1/docs/build/html/_static/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4418 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14621 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/basic.css
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      313 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/check-solid.svg
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     9031 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/clipboard.min.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      411 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/copy-button.svg
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2010 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/copybutton.css
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7479 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/copybutton.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2198 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/copybutton_funcs.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4472 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/doctools.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      417 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      286 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/file.png
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.247254 CmonCrawl-0.8.1/docs/build/html/_static/images/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1186 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/images/logo_binder.svg
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7601 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/images/logo_colab.png
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      681 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1758 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   288580 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    89501 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/jquery.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4758 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/language_data.js
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.584253 CmonCrawl-0.8.1/docs/build/html/_static/locales/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.548253 CmonCrawl-0.8.1/docs/build/html/_static/locales/ar/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.247254 CmonCrawl-0.8.1/docs/build/html/_static/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1608 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.549253 CmonCrawl-0.8.1/docs/build/html/_static/locales/bg/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.248254 CmonCrawl-0.8.1/docs/build/html/_static/locales/bg/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1789 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.549253 CmonCrawl-0.8.1/docs/build/html/_static/locales/bn/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.248254 CmonCrawl-0.8.1/docs/build/html/_static/locales/bn/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1667 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.550253 CmonCrawl-0.8.1/docs/build/html/_static/locales/ca/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.249254 CmonCrawl-0.8.1/docs/build/html/_static/locales/ca/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1231 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.550253 CmonCrawl-0.8.1/docs/build/html/_static/locales/cs/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.249254 CmonCrawl-0.8.1/docs/build/html/_static/locales/cs/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1449 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.551253 CmonCrawl-0.8.1/docs/build/html/_static/locales/da/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.250254 CmonCrawl-0.8.1/docs/build/html/_static/locales/da/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1343 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.551253 CmonCrawl-0.8.1/docs/build/html/_static/locales/de/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.251254 CmonCrawl-0.8.1/docs/build/html/_static/locales/de/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1444 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.552253 CmonCrawl-0.8.1/docs/build/html/_static/locales/el/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.252254 CmonCrawl-0.8.1/docs/build/html/_static/locales/el/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1816 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.554253 CmonCrawl-0.8.1/docs/build/html/_static/locales/eo/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.254254 CmonCrawl-0.8.1/docs/build/html/_static/locales/eo/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1384 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.555253 CmonCrawl-0.8.1/docs/build/html/_static/locales/es/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.256254 CmonCrawl-0.8.1/docs/build/html/_static/locales/es/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1438 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.556253 CmonCrawl-0.8.1/docs/build/html/_static/locales/et/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.257254 CmonCrawl-0.8.1/docs/build/html/_static/locales/et/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1391 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.561253 CmonCrawl-0.8.1/docs/build/html/_static/locales/fi/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.259254 CmonCrawl-0.8.1/docs/build/html/_static/locales/fi/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1409 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.562253 CmonCrawl-0.8.1/docs/build/html/_static/locales/fr/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.260254 CmonCrawl-0.8.1/docs/build/html/_static/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1469 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.563253 CmonCrawl-0.8.1/docs/build/html/_static/locales/hr/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.261254 CmonCrawl-0.8.1/docs/build/html/_static/locales/hr/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1449 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.564253 CmonCrawl-0.8.1/docs/build/html/_static/locales/id/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.262254 CmonCrawl-0.8.1/docs/build/html/_static/locales/id/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1360 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.564253 CmonCrawl-0.8.1/docs/build/html/_static/locales/it/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.263254 CmonCrawl-0.8.1/docs/build/html/_static/locales/it/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1447 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.566253 CmonCrawl-0.8.1/docs/build/html/_static/locales/iw/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.263254 CmonCrawl-0.8.1/docs/build/html/_static/locales/iw/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1490 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.566253 CmonCrawl-0.8.1/docs/build/html/_static/locales/ja/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.264254 CmonCrawl-0.8.1/docs/build/html/_static/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1518 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.566253 CmonCrawl-0.8.1/docs/build/html/_static/locales/ko/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.264254 CmonCrawl-0.8.1/docs/build/html/_static/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1406 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.568253 CmonCrawl-0.8.1/docs/build/html/_static/locales/lt/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.265254 CmonCrawl-0.8.1/docs/build/html/_static/locales/lt/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1461 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.570253 CmonCrawl-0.8.1/docs/build/html/_static/locales/lv/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.265254 CmonCrawl-0.8.1/docs/build/html/_static/locales/lv/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1450 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.571253 CmonCrawl-0.8.1/docs/build/html/_static/locales/ml/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.266254 CmonCrawl-0.8.1/docs/build/html/_static/locales/ml/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1890 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.572253 CmonCrawl-0.8.1/docs/build/html/_static/locales/mr/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.267254 CmonCrawl-0.8.1/docs/build/html/_static/locales/mr/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1675 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.572253 CmonCrawl-0.8.1/docs/build/html/_static/locales/ms/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.268254 CmonCrawl-0.8.1/docs/build/html/_static/locales/ms/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1189 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.573253 CmonCrawl-0.8.1/docs/build/html/_static/locales/nl/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.271254 CmonCrawl-0.8.1/docs/build/html/_static/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1398 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.573253 CmonCrawl-0.8.1/docs/build/html/_static/locales/no/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.272254 CmonCrawl-0.8.1/docs/build/html/_static/locales/no/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1357 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.574253 CmonCrawl-0.8.1/docs/build/html/_static/locales/pl/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.273254 CmonCrawl-0.8.1/docs/build/html/_static/locales/pl/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1420 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.574253 CmonCrawl-0.8.1/docs/build/html/_static/locales/pt/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.274254 CmonCrawl-0.8.1/docs/build/html/_static/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1409 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.575253 CmonCrawl-0.8.1/docs/build/html/_static/locales/ro/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.274254 CmonCrawl-0.8.1/docs/build/html/_static/locales/ro/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1441 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.575253 CmonCrawl-0.8.1/docs/build/html/_static/locales/ru/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.275254 CmonCrawl-0.8.1/docs/build/html/_static/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1797 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.576253 CmonCrawl-0.8.1/docs/build/html/_static/locales/sk/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.276254 CmonCrawl-0.8.1/docs/build/html/_static/locales/sk/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1441 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.576253 CmonCrawl-0.8.1/docs/build/html/_static/locales/sl/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.277254 CmonCrawl-0.8.1/docs/build/html/_static/locales/sl/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1418 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.577253 CmonCrawl-0.8.1/docs/build/html/_static/locales/sr/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.278254 CmonCrawl-0.8.1/docs/build/html/_static/locales/sr/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1760 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.578253 CmonCrawl-0.8.1/docs/build/html/_static/locales/sv/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.279254 CmonCrawl-0.8.1/docs/build/html/_static/locales/sv/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1391 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.578253 CmonCrawl-0.8.1/docs/build/html/_static/locales/ta/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.280254 CmonCrawl-0.8.1/docs/build/html/_static/locales/ta/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1968 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.579253 CmonCrawl-0.8.1/docs/build/html/_static/locales/te/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.280254 CmonCrawl-0.8.1/docs/build/html/_static/locales/te/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1834 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.580253 CmonCrawl-0.8.1/docs/build/html/_static/locales/tg/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.281254 CmonCrawl-0.8.1/docs/build/html/_static/locales/tg/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1710 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.580253 CmonCrawl-0.8.1/docs/build/html/_static/locales/th/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.281254 CmonCrawl-0.8.1/docs/build/html/_static/locales/th/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1860 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.581253 CmonCrawl-0.8.1/docs/build/html/_static/locales/tl/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.282254 CmonCrawl-0.8.1/docs/build/html/_static/locales/tl/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1259 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.581253 CmonCrawl-0.8.1/docs/build/html/_static/locales/tr/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.283254 CmonCrawl-0.8.1/docs/build/html/_static/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1405 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.582253 CmonCrawl-0.8.1/docs/build/html/_static/locales/uk/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.284254 CmonCrawl-0.8.1/docs/build/html/_static/locales/uk/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1756 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.582253 CmonCrawl-0.8.1/docs/build/html/_static/locales/ur/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.285254 CmonCrawl-0.8.1/docs/build/html/_static/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1460 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.583253 CmonCrawl-0.8.1/docs/build/html/_static/locales/vi/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.288254 CmonCrawl-0.8.1/docs/build/html/_static/locales/vi/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1487 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.584253 CmonCrawl-0.8.1/docs/build/html/_static/locales/zh_CN/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.289254 CmonCrawl-0.8.1/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1279 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.584253 CmonCrawl-0.8.1/docs/build/html/_static/locales/zh_TW/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.290254 CmonCrawl-0.8.1/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1323 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       90 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/minus.png
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       90 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/plus.png
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5510 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/pygments.css
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      419 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/sbt-webpack-macros.html
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.294254 CmonCrawl-0.8.1/docs/build/html/_static/scripts/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    87299 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     3388 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15106 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/searchtools.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4712 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.298254 CmonCrawl-0.8.1/docs/build/html/_static/styles/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   162094 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20970 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5488 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/styles/theme.css
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    68420 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    19530 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/underscore.js
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.585253 CmonCrawl-0.8.1/docs/build/html/_static/vendor/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.585253 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.299254 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1548 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.300254 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/css/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    58578 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.351254 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   133034 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   715890 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   132728 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    89824 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    76612 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    34390 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   144322 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    34092 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16800 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    13584 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   202902 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   897426 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   202616 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   103300 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    79444 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1361 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/_static/webpack-macros.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14884 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/api.html
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.724254 CmonCrawl-0.8.1/docs/build/html/generated/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15433 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17399 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.DomainCrawl.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20855 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.DomainCrawl.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18729 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.DomainRecord.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    24159 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.DomainRecord.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20332 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18026 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.aclose.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16729 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.aopen.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17323 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    19039 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18171 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    28037 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17093 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.RetrieveResponse.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20354 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.RetrieveResponse.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16683 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20028 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16884 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.decode.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    24580 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16881 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15016 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.ndjson_decoder.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14329 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.utils.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14859 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.aggregator.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14923 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22512 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17934 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17801 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17957 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17767 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17754 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17987 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17499 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17640 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17647 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    35243 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17503 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15382 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18043 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_utils.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15594 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16326 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17530 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.download.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18286 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17916 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18174 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16837 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16918 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.download.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22820 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17667 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15390 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17869 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17079 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16854 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16876 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22678 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16909 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15276 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15191 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16373 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17539 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17091 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17083 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17239 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20711 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17115 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15044 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16349 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17515 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17657 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17208 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20629 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17123 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15140 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16355 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor_utils.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15787 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16479 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16595 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18928 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17315 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15098 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15699 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16383 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16705 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18768 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17457 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15184 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18754 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16961 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17216 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    24427 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17443 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17777 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17817 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17045 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17300 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22651 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17527 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17817 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17812 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16898 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17153 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22694 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17380 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17546 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16214 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14984 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Pipeline.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17657 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20930 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16946 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15017 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Pipeline.pipeline.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14956 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17281 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Route.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20799 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Route.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16110 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    19510 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16408 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.load_module.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16436 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.load_modules.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18032 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.register_route.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16805 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.register_routes.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17244 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.route.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15177 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16649 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    18771 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.processor_utils.DomainRecord.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    24125 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.processor_utils.DomainRecord.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17699 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.processor_utils.PipeMetadata.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    22093 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.processor_utils.PipeMetadata.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15405 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.processor_utils.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15281 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14868 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.process_article.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16886 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    24450 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16619 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_before_message.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16532 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_connected.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16819 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_connecting.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16361 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_disconnected.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_disconnecting.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16409 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_error.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16181 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_heartbeat.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16334 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_heartbeat_timeout.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16570 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_message.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16546 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_receipt.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16420 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_receiver_loop_completed.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16414 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_send.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    17119 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.ListnerStats.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20228 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.ListnerStats.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16511 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Message.__init__.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    19876 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Message.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16556 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    56110 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/genindex.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    19730 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/index.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16148 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/installation.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    12364 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/objects.inv
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    20823 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/py-modindex.html
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.740254 CmonCrawl-0.8.1/docs/build/html/quickstart/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    15316 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/quickstart/artemis-queue.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14124 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/quickstart/download_article.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    16829 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/quickstart/index.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    14023 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/quickstart/installation.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    13934 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/quickstart/middleware.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    25924 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/quickstart/overview.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    42595 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/quickstart/quick-start.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    13374 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/search.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    75786 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/html/searchindex.js
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       71 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/build/index.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       71 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/index.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      769 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/make.bat
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:36.761254 CmonCrawl-0.8.1/docs/source/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      105 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/api.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2756 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/conf.py
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:37.293255 CmonCrawl-0.8.1/docs/source/generated/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      190 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.DomainCrawl.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      441 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.DomainCrawl.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      193 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.DomainRecord.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      558 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.DomainRecord.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      202 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.IndexAggregator.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      188 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.IndexAggregator.aclose.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      185 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.IndexAggregator.aopen.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      230 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      240 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      233 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      512 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.IndexAggregator.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      205 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.RetrieveResponse.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      475 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.RetrieveResponse.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      433 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      187 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      173 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.ndjson_decoder.Decoder.decode.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      187 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      347 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.ndjson_decoder.Decoder.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      246 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.ndjson_decoder.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      272 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      135 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.utils.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      249 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.aggregator.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      219 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Aggregator.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      259 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      274 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      271 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      271 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      282 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      285 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      248 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      265 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      259 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      262 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      257 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      903 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      300 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      711 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_utils.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      316 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      212 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.downloader.Downloader.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      204 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.downloader.Downloader.download.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      354 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.downloader.Downloader.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      224 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      210 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      207 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      216 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.download.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      460 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      210 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      286 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.downloader.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      247 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      239 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      250 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      253 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      256 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      507 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      290 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.dummy_downloader.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      299 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Downloader.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      223 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      212 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      229 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      223 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      226 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      601 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      278 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.dummy_extractor.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      204 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      218 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      213 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      629 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      262 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.extractor.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      467 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.extractor_utils.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      335 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      238 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      232 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      414 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      224 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      285 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      215 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      391 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      207 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      272 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.outstreamer.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      347 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      267 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      261 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      278 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      293 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      563 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      253 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      279 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      273 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      290 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      305 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      595 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      265 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      258 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      252 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      269 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      284 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      539 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      244 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      355 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      221 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      256 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      390 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      260 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Pipeline.pipeline.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      244 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Pipeline.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      173 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Router.router.Route.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      412 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Router.router.Route.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      176 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Router.router.Router.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      179 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Router.router.Router.load_module.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      182 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Router.router.Router.load_modules.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      188 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Router.router.Router.register_route.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      191 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Router.router.Router.register_routes.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      159 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Router.router.Router.route.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      419 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Router.router.Router.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      249 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Router.router.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      234 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.Router.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      202 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.processor_utils.DomainRecord.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      567 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.processor_utils.DomainRecord.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      202 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.processor_utils.PipeMetadata.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      559 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.processor_utils.PipeMetadata.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      270 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.processor_utils.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      379 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.App.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      239 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.process_article.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      158 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      181 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.on_before_message.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      164 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.on_connected.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      167 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.on_connecting.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      173 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.on_disconnected.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      176 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.on_disconnecting.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      152 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.on_error.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      164 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.on_heartbeat.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      190 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.on_heartbeat_timeout.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      158 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.on_message.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      158 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.on_receipt.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      210 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.on_receiver_loop_completed.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      149 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.on_send.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      641 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      170 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.ListnerStats.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      409 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.ListnerStats.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      155 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Message.__init__.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      363 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Message.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      420 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.processor.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      242 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/generated/Processor.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      526 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/index.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      658 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/installation.rst
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:37.305255 CmonCrawl-0.8.1/docs/source/quickstart/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      665 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/quickstart/artemis-queue.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      138 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/quickstart/index.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     5429 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/quickstart/overview.rst
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)    12222 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/docs/source/quickstart/quick-start.rst
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:35.591253 CmonCrawl-0.8.1/examples/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:37.312255 CmonCrawl-0.8.1/examples/extractor_tutorial/
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:37.317255 CmonCrawl-0.8.1/examples/extractor_tutorial/Extractors/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1357 2023-04-26 09:40:00.000000 CmonCrawl-0.8.1/examples/extractor_tutorial/Extractors/bbc_extractor.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      181 2023-04-30 17:35:08.000000 CmonCrawl-0.8.1/examples/extractor_tutorial/config.json
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     1368 2023-05-01 22:03:52.000000 CmonCrawl-0.8.1/pyproject.toml
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      433 2023-04-30 17:44:12.000000 CmonCrawl-0.8.1/requirements.txt
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)       38 2023-05-01 22:06:37.369255 CmonCrawl-0.8.1/setup.cfg
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:37.331255 CmonCrawl-0.8.1/tests/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     7126 2023-04-27 23:19:10.000000 CmonCrawl-0.8.1/tests/aggregator_tests.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     2822 2023-04-30 17:35:31.000000 CmonCrawl-0.8.1/tests/end_to_end_tests.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)     4642 2023-04-30 17:35:09.000000 CmonCrawl-0.8.1/tests/processor_tests.py
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:37.332255 CmonCrawl-0.8.1/tests/test_extract/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      272 2023-04-30 17:35:29.000000 CmonCrawl-0.8.1/tests/test_extract/cfg.json
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:37.333255 CmonCrawl-0.8.1/tests/test_extract/extractors/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      495 2023-04-30 17:35:31.000000 CmonCrawl-0.8.1/tests/test_extract/extractors/test_extract.py
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:37.347255 CmonCrawl-0.8.1/tests/test_extract/files/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)   828135 2023-04-30 17:35:30.000000 CmonCrawl-0.8.1/tests/test_extract/files/file.html
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)  1743032 2023-04-30 13:23:44.000000 CmonCrawl-0.8.1/tests/test_extract/files/file.json
+drwxr-xr-x   0 kydliceh  (1000) kydliceh  (1000)        0 2023-05-01 22:06:37.366255 CmonCrawl-0.8.1/tests/test_routes/
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      401 2023-04-27 21:31:25.000000 CmonCrawl-0.8.1/tests/test_routes/a.py
+-rw-r--r--   0 kydliceh  (1000) kydliceh  (1000)      400 2023-04-27 21:31:36.000000 CmonCrawl-0.8.1/tests/test_routes/b.py
```

### Comparing `CmonCrawl-0.8.0/.gitignore` & `CmonCrawl-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/.vscode/launch.json` & `CmonCrawl-0.8.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/CmonCrawl.egg-info/PKG-INFO` & `CmonCrawl-0.8.1/CmonCrawl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CmonCrawl
-Version: 0.8.0
+Version: 0.8.1
 Project-URL: Source, https://github.com/hynky1999/Rocnikovy-Projekt
 Keywords: Common Crawl,Crawl,Extractor,Common Crawl Extractor,Web Crawler,Web Extractor,Web Scraper
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
@@ -51,15 +51,15 @@
 # Make sure to instantiate your extractor into extractor variable
 # The name must match so that the framework can find it
 extractor = MyExtractor()
 ```
 
 ### Config creation
 Once you have your extractor, you need to create a config file to run the extractor.
-For ou
+In our case the config would look like this:
 
 ```json
 {
     "extractors_path": "./extractors",
     "routes": [
         {
             # Define which url match the extractor, use regex
@@ -81,28 +81,37 @@
 ### Run the extractor
 To test the extraction, you can use the following command:
 
 ```bash
 $ cmonextract --mode=html html_file1 html_file2 ... html_fileN extraction_output_dir config_file
 ```
 
-### Get records from dataset
+### Crawl the sites
 Once you have your extractor tested, we can start crawling.
 To do this you will proceed in two steps:
 
 #### 1. Get the list of records to extract
 To do this, you can use the following command:
 
 ```bash
-$ cmoncrawl --limit=100000 --output_type=record yoursite.com output_dir
+$ cmondownload --limit=100000 --output_type=record yoursite.com output_dir
 ```
 
 This will download the first 100000 records from yoursite.com and save them in output_dir. By default it saves 100_000 records per file, you can change this with the --max_crawl_per_file option.
 
 #### 2. Extract the records
 Once you have the records, you can use the following command to extract them:
 
 ```bash
 $ cmonextract --nproc=4 --mode=record record_file1 record_file2 ... record_fileN extraction_output_dir config_file
 ```
 
 Note that you can use the --nproc option to specify the number of processes to use for the extraction. Multiprocessing is done on file level, so if you have just one file it will not be used.
+
+
+### Advanced usage
+The whole project was written with modularity in mind. That means that you
+can adjust the framework to your needs.
+
+#TODO add more info about pipeline
+
+Instead of first getting the records and then extracting them, you can do both in a distributed setting. For more info look at [CZE-NEC](https://github.com/hynky1999/Czech-News-Classification-dataset) project.
```

### Comparing `CmonCrawl-0.8.0/CmonCrawl.egg-info/SOURCES.txt` & `CmonCrawl-0.8.1/CmonCrawl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/LICENSE` & `CmonCrawl-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/PKG-INFO` & `CmonCrawl-0.8.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CmonCrawl
-Version: 0.8.0
+Version: 0.8.1
 Project-URL: Source, https://github.com/hynky1999/Rocnikovy-Projekt
 Keywords: Common Crawl,Crawl,Extractor,Common Crawl Extractor,Web Crawler,Web Extractor,Web Scraper
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
@@ -51,15 +51,15 @@
 # Make sure to instantiate your extractor into extractor variable
 # The name must match so that the framework can find it
 extractor = MyExtractor()
 ```
 
 ### Config creation
 Once you have your extractor, you need to create a config file to run the extractor.
-For ou
+In our case the config would look like this:
 
 ```json
 {
     "extractors_path": "./extractors",
     "routes": [
         {
             # Define which url match the extractor, use regex
@@ -81,28 +81,37 @@
 ### Run the extractor
 To test the extraction, you can use the following command:
 
 ```bash
 $ cmonextract --mode=html html_file1 html_file2 ... html_fileN extraction_output_dir config_file
 ```
 
-### Get records from dataset
+### Crawl the sites
 Once you have your extractor tested, we can start crawling.
 To do this you will proceed in two steps:
 
 #### 1. Get the list of records to extract
 To do this, you can use the following command:
 
 ```bash
-$ cmoncrawl --limit=100000 --output_type=record yoursite.com output_dir
+$ cmondownload --limit=100000 --output_type=record yoursite.com output_dir
 ```
 
 This will download the first 100000 records from yoursite.com and save them in output_dir. By default it saves 100_000 records per file, you can change this with the --max_crawl_per_file option.
 
 #### 2. Extract the records
 Once you have the records, you can use the following command to extract them:
 
 ```bash
 $ cmonextract --nproc=4 --mode=record record_file1 record_file2 ... record_fileN extraction_output_dir config_file
 ```
 
 Note that you can use the --nproc option to specify the number of processes to use for the extraction. Multiprocessing is done on file level, so if you have just one file it will not be used.
+
+
+### Advanced usage
+The whole project was written with modularity in mind. That means that you
+can adjust the framework to your needs.
+
+#TODO add more info about pipeline
+
+Instead of first getting the records and then extracting them, you can do both in a distributed setting. For more info look at [CZE-NEC](https://github.com/hynky1999/Czech-News-Classification-dataset) project.
```

### Comparing `CmonCrawl-0.8.0/README.md` & `CmonCrawl-0.8.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 # Make sure to instantiate your extractor into extractor variable
 # The name must match so that the framework can find it
 extractor = MyExtractor()
 ```
 
 ### Config creation
 Once you have your extractor, you need to create a config file to run the extractor.
-For ou
+In our case the config would look like this:
 
 ```json
 {
     "extractors_path": "./extractors",
     "routes": [
         {
             # Define which url match the extractor, use regex
@@ -69,28 +69,37 @@
 ### Run the extractor
 To test the extraction, you can use the following command:
 
 ```bash
 $ cmonextract --mode=html html_file1 html_file2 ... html_fileN extraction_output_dir config_file
 ```
 
-### Get records from dataset
+### Crawl the sites
 Once you have your extractor tested, we can start crawling.
 To do this you will proceed in two steps:
 
 #### 1. Get the list of records to extract
 To do this, you can use the following command:
 
 ```bash
-$ cmoncrawl --limit=100000 --output_type=record yoursite.com output_dir
+$ cmondownload --limit=100000 --output_type=record yoursite.com output_dir
 ```
 
 This will download the first 100000 records from yoursite.com and save them in output_dir. By default it saves 100_000 records per file, you can change this with the --max_crawl_per_file option.
 
 #### 2. Extract the records
 Once you have the records, you can use the following command to extract them:
 
 ```bash
 $ cmonextract --nproc=4 --mode=record record_file1 record_file2 ... record_fileN extraction_output_dir config_file
 ```
 
-Note that you can use the --nproc option to specify the number of processes to use for the extraction. Multiprocessing is done on file level, so if you have just one file it will not be used.
+Note that you can use the --nproc option to specify the number of processes to use for the extraction. Multiprocessing is done on file level, so if you have just one file it will not be used.
+
+
+### Advanced usage
+The whole project was written with modularity in mind. That means that you
+can adjust the framework to your needs.
+
+#TODO add more info about pipeline
+
+Instead of first getting the records and then extracting them, you can do both in a distributed setting. For more info look at [CZE-NEC](https://github.com/hynky1999/Czech-News-Classification-dataset) project.
```

### Comparing `CmonCrawl-0.8.0/cmoncrawl/aggregator/index_query.py` & `CmonCrawl-0.8.1/cmoncrawl/aggregator/index_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         cc_indexes_server: str = "http://index.commoncrawl.org/collinfo.json",
         cc_servers: List[str] = [],
         since: datetime = datetime.min,
         to: datetime = datetime.max,
         limit: int | None = None,
         max_retry: int = 5,
         prefetch_size: int = 3,
-        sleep_step: int = 10,
+        sleep_step: int = 20,
     ) -> None:
         self.domains = domains
         self.cc_indexes_server = cc_indexes_server
         self.cc_servers = cc_servers
         self.since = since
         self.to = to
         self.limit = limit
@@ -228,18 +228,19 @@
                 )
                 for js in reponse.content
             ]
         return reponse
 
     @staticmethod
     async def get_all_CC_indexes(client: ClientSession, cdx_server: str) -> List[str]:
-        async with client.get(cdx_server) as response:
-            r_json = await response.json(content_type="application/json")
-            CC_servers = [js["cdx-api"] for js in r_json]
-            return CC_servers
+        for _ in range(3):
+            async with client.get(cdx_server) as response:
+                r_json = await response.json(content_type="application/json")
+                CC_servers = [js["cdx-api"] for js in r_json]
+                return CC_servers
 
     class IndexAggregatorIterator(AsyncIterator[DomainRecord]):
         def __init__(
             self,
             client: ClientSession,
             domains: List[str],
             CC_files: List[str],
```

### Comparing `CmonCrawl-0.8.0/cmoncrawl/aggregator/utils/helpers.py` & `CmonCrawl-0.8.1/cmoncrawl/aggregator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/cmoncrawl/common/loggers.py` & `CmonCrawl-0.8.1/cmoncrawl/common/loggers.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/cmoncrawl/common/types.py` & `CmonCrawl-0.8.1/cmoncrawl/common/types.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/cmoncrawl/integrations/commands.py` & `CmonCrawl-0.8.1/cmoncrawl/integrations/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,25 +63,28 @@
     return [DomainRecord.schema().load(record["domain_record"]) for record in js]
 
 
 def get_domain_records_html(url: str | None, date: datetime | None):
     # Just return dummy as correct crawl will be loaded from dummy downloader
     return [DomainRecord("", url=url, offset=0, length=0, timestamp=date)]
 
+
 def load_config(config_path: Path) -> ExtractConfig:
     with open(config_path, "r") as f:
         config = json.load(f)
     return ExtractConfig.schema().load(config)
 
+
 def create_router(config: ExtractConfig) -> Router:
     router = Router()
     router.load_modules(config.extractors_path)
     router.register_routes(config.routes)
     return router
 
+
 async def extract_from_files(
     files: List[Path],
     output_path: Path,
     config: ExtractConfig,
     mode: ExtractMode,
     url: str | None,
     date: datetime | None,
```

### Comparing `CmonCrawl-0.8.0/cmoncrawl/middleware/stompware.py` & `CmonCrawl-0.8.1/cmoncrawl/middleware/stompware.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,29 +32,36 @@
 class ListnerStats:
     messages: int = 0
     last_message_time: datetime = datetime.now()
 
 
 class ArtemisAggregator:
     def __init__(
-        self, queue_host: str, queue_port: int, url: str, index_agg: IndexAggregator
+        self,
+        queue_host: str,
+        queue_port: int,
+        url: str,
+        index_agg: IndexAggregator,
+        heartbeat: int = 10000,
     ):
         self.queue_host = queue_host
         self.queue_port = queue_port
         self.index_agg = index_agg
         self.url = url
+        self.heartbeat = heartbeat
 
     def _init_connection(self, conn: Connection):
         conn.connect(login="producer", passcode="producer", wait=True)
         all_purpose_logger.info(f"Connected to queue")
         return conn
 
-    async def aggregate(self):
+    async def aggregate(self, filter_duplicates: bool = True):
         conn = Connection(
-            [(self.queue_host, self.queue_port)], heartbeats=(10000, 10000)
+            [(self.queue_host, self.queue_port)],
+            heartbeats=(self.heartbeat, self.heartbeat),
         )
         # make sure we have connection so that we cant send the poission pill
         while conn.is_connected() is False:
             try:
                 conn = self._init_connection(conn)
             except StompException:
                 pass
@@ -62,28 +69,34 @@
         async with self.index_agg as aggregator:
             async for domain_record in aggregator:
                 try:
                     while not conn.is_connected():
                         conn = self._init_connection(conn)
 
                     json_str = json.dumps(domain_record.__dict__, default=str)
-                    id = unify_url_id(domain_record.url)
+                    headers = {}
+                    if filter_duplicates:
+                        id = unify_url_id(domain_record.url)
+                        headers[DUPL_ID_HEADER] = id
                     conn.send(
                         f"queue.{self.url}",
                         json_str,
-                        headers={DUPL_ID_HEADER: id},
+                        headers=headers,
                     )
                     all_purpose_logger.debug(
                         f"Sent url: {domain_record.url} with id: {id}"
                     )
                     i += 1
-                except (KeyboardInterrupt) as e:
-                    break
+                except StompException as e:
+                    all_purpose_logger.error(e, exc_info=True)
+                    continue
+
                 except Exception as e:
                     all_purpose_logger.error(e, exc_info=True)
+                    break
 
         all_purpose_logger.info(f"Sent {i} messages")
         conn.send(
             f"topic.poisson_pill.{self.url}", "", headers={"type": "poisson_pill"}
         )
         conn.disconnect()
 
@@ -94,26 +107,30 @@
         queue_host: str,
         queue_port: int,
         pills_to_die: int | None,
         queue_size: int,
         timeout: int,
         addresses: List[str],
         pipeline: ProcessorPipeline,
+        heartbeat: int = 10000,
     ):
         self.queue_host = queue_host
         self.queue_port = queue_port
         self.pills_to_die = pills_to_die
         self.queue_size = queue_size
         self.timeout = timeout
         self.pipeline = pipeline
         self.addresses = addresses
+        self.heartbeat = heartbeat
 
     class Listener(ConnectionListener):
         def __init__(
-            self, messages: asyncio.Queue[Message], listener_stats: ListnerStats
+            self,
+            messages: asyncio.Queue[Message],
+            listener_stats: ListnerStats,
         ):
             self.messages = messages
             self.pills = 0
             self.listener_stats = listener_stats
 
         def on_message(self, frame: Frame):
             if frame.headers.get("type") == "poisson_pill":
@@ -136,15 +153,18 @@
         for address in addresses:
             conn.subscribe(address, id=address, ack="client-individual")
         conn.subscribe("topic.poisson_pill.#", id="poisson_pill", ack="auto")
         all_purpose_logger.info("Connected to queue")
         return conn
 
     async def _call_pipeline_with_ack(
-        self, pipeline: ProcessorPipeline, msg: Message, client: Connection
+        self,
+        pipeline: ProcessorPipeline,
+        msg: Message,
+        client: Connection,
     ):
         # Make sure no exception is thrown from this function
         # So that we can nack it if needed
         paths = []
         try:
             paths = await pipeline.process_domain_record(msg.dr)
             # Ack at any result
@@ -161,15 +181,15 @@
     async def process(self):
         timeout_delta = timedelta(minutes=self.timeout)
         # Set's extractor path based on config
         pending_extracts: Set[asyncio.Task[Tuple[Message, List[Path]]]] = set()
         conn = Connection(
             [(self.queue_host, self.queue_port)],
             reconnect_attempts_max=-1,
-            heartbeats=(10000, 10000),
+            heartbeats=(self.heartbeat, self.heartbeat),
         )
         listener_stats = ListnerStats()
         listener = self.Listener(asyncio.Queue(0), listener_stats)
         conn.set_listener("", listener)
         all_purpose_logger.debug("Connecting to queue")
         extracted_num = 0
         try:
```

### Comparing `CmonCrawl-0.8.0/cmoncrawl/middleware/synchronized.py` & `CmonCrawl-0.8.1/cmoncrawl/middleware/synchronized.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/cmoncrawl/processor/extraction/filters.py` & `CmonCrawl-0.8.1/cmoncrawl/processor/extraction/filters.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/cmoncrawl/processor/extraction/utils.py` & `CmonCrawl-0.8.1/cmoncrawl/processor/extraction/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,17 @@
             return recursive_get(key, dicts, i + 1)
         return val
 
     keys = [key for d in dicts for key in d.keys()]
     return {key: recursive_get(key, dicts, 0) for key in keys}
 
 
-
-def check_required(required_fields: Dict[str, bool], extractor_name: str, non_empty: bool = False):
-
+def check_required(
+    required_fields: Dict[str, bool], extractor_name: str, non_empty: bool = False
+):
     def inner(extracted_dict: Dict[Any, Any], metadata: PipeMetadata):
         for key, value in required_fields.items():
             if key not in extracted_dict:
                 metadata_logger.warn(
                     f"{extractor_name} failed to extract {key}",
                     extra={"domain_record": metadata.domain_record},
                 )
@@ -153,8 +153,8 @@
                         metadata_logger.warn(
                             f"{extractor_name}: empty list for key: {key} is not allowed",
                             extra={"domain_record": metadata.domain_record},
                         )
                         return False
         return True
 
-    return inner
+    return inner
```

### Comparing `CmonCrawl-0.8.0/cmoncrawl/processor/pipeline/downloader.py` & `CmonCrawl-0.8.1/cmoncrawl/processor/pipeline/downloader.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/cmoncrawl/processor/pipeline/extractor.py` & `CmonCrawl-0.8.1/cmoncrawl/processor/pipeline/extractor.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/cmoncrawl/processor/pipeline/pipeline.py` & `CmonCrawl-0.8.1/cmoncrawl/processor/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/cmoncrawl/processor/pipeline/router.py` & `CmonCrawl-0.8.1/cmoncrawl/processor/pipeline/router.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/cmoncrawl/processor/pipeline/streamer.py` & `CmonCrawl-0.8.1/cmoncrawl/processor/pipeline/streamer.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/Makefile` & `CmonCrawl-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/_templates/module.rst` & `CmonCrawl-0.8.1/docs/build/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/api.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/environment.pickle` & `CmonCrawl-0.8.1/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.DomainCrawl.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.DomainCrawl.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.DomainCrawl.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.DomainCrawl.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.DomainRecord.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.DomainRecord.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.DomainRecord.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.DomainRecord.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.aclose.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.aclose.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.aopen.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.aopen.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.RetrieveResponse.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.RetrieveResponse.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.RetrieveResponse.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.RetrieveResponse.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.index_query.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.index_query.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.decode.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.decode.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.App.utils.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.App.utils.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.aggregator.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.aggregator.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Aggregator.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Aggregator.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_utils.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_utils.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.ArticleUtils.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.ArticleUtils.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.download.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.download.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.download.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.download.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.downloader.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.downloader.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Extractor.extractor_utils.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Extractor.extractor_utils.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Pipeline.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Pipeline.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Route.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Route.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Route.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Route.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.load_module.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.load_module.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.load_modules.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.load_modules.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.register_route.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.register_route.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.register_routes.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.register_routes.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.Router.route.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.Router.route.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.Router.router.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.Router.router.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.processor_utils.DomainRecord.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.processor_utils.DomainRecord.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.processor_utils.DomainRecord.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.processor_utils.DomainRecord.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.processor_utils.PipeMetadata.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.processor_utils.PipeMetadata.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.processor_utils.PipeMetadata.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.processor_utils.PipeMetadata.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.App.processor_utils.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.App.processor_utils.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.process_article.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.process_article.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_before_message.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_before_message.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_connected.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_connected.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_connecting.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_connecting.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_disconnected.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_disconnected.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_disconnecting.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_disconnecting.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_error.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_error.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_heartbeat.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_heartbeat.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_heartbeat_timeout.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_heartbeat_timeout.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_message.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_message.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_receipt.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_receipt.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_receiver_loop_completed.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_receiver_loop_completed.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Listener.on_send.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Listener.on_send.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.ListnerStats.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.ListnerStats.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.ListnerStats.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.ListnerStats.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Message.__init__.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Message.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.Message.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.Message.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/generated/Processor.processor.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/generated/Processor.processor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/index.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/installation.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/quickstart/artemis-queue.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/quickstart/artemis-queue.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/quickstart/download_article.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/quickstart/download_article.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/quickstart/index.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/quickstart/index.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/quickstart/installation.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/quickstart/installation.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/quickstart/middleware.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/quickstart/middleware.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/quickstart/overview.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/quickstart/overview.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/doctrees/quickstart/quick-start.doctree` & `CmonCrawl-0.8.1/docs/build/doctrees/quickstart/quick-start.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainRecord.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainRecord.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_utils.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_utils.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.processor_utils.DomainRecord.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.processor_utils.DomainRecord.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.App.processor_utils.PipeMetadata.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.App.processor_utils.PipeMetadata.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/generated/Processor.processor.Listener.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/generated/Processor.processor.Listener.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/index.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/installation.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/quickstart/artemis-queue.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/quickstart/artemis-queue.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/quickstart/overview.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/quickstart/overview.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_sources/quickstart/quick-start.rst.txt` & `CmonCrawl-0.8.1/docs/build/html/_sources/quickstart/quick-start.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `CmonCrawl-0.8.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/basic.css` & `CmonCrawl-0.8.1/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/clipboard.min.js` & `CmonCrawl-0.8.1/docs/build/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/copybutton.css` & `CmonCrawl-0.8.1/docs/build/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/copybutton.js` & `CmonCrawl-0.8.1/docs/build/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/copybutton_funcs.js` & `CmonCrawl-0.8.1/docs/build/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/doctools.js` & `CmonCrawl-0.8.1/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/images/logo_binder.svg` & `CmonCrawl-0.8.1/docs/build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/images/logo_colab.png` & `CmonCrawl-0.8.1/docs/build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/images/logo_deepnote.svg` & `CmonCrawl-0.8.1/docs/build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/images/logo_jupyterhub.svg` & `CmonCrawl-0.8.1/docs/build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/jquery-3.6.0.js` & `CmonCrawl-0.8.1/docs/build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/jquery.js` & `CmonCrawl-0.8.1/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/language_data.js` & `CmonCrawl-0.8.1/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `CmonCrawl-0.8.1/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/pygments.css` & `CmonCrawl-0.8.1/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/scripts/pydata-sphinx-theme.js` & `CmonCrawl-0.8.1/docs/build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/scripts/sphinx-book-theme.js` & `CmonCrawl-0.8.1/docs/build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/scripts/sphinx-book-theme.js.map` & `CmonCrawl-0.8.1/docs/build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/searchtools.js` & `CmonCrawl-0.8.1/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/sphinx_highlight.js` & `CmonCrawl-0.8.1/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/styles/pydata-sphinx-theme.css` & `CmonCrawl-0.8.1/docs/build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/styles/sphinx-book-theme.css` & `CmonCrawl-0.8.1/docs/build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/styles/theme.css` & `CmonCrawl-0.8.1/docs/build/html/_static/styles/theme.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/underscore-1.13.1.js` & `CmonCrawl-0.8.1/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/underscore.js` & `CmonCrawl-0.8.1/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2` & `CmonCrawl-0.8.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/_static/webpack-macros.html` & `CmonCrawl-0.8.1/docs/build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/api.html` & `CmonCrawl-0.8.1/docs/build/html/api.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.DomainCrawl.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.DomainCrawl.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.DomainCrawl.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.DomainCrawl.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.DomainRecord.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.DomainRecord.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.DomainRecord.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.DomainRecord.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.aclose.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.aclose.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.aopen.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.aopen.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.RetrieveResponse.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.RetrieveResponse.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.RetrieveResponse.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.RetrieveResponse.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.index_query.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.index_query.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.decode.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.decode.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.ndjson_decoder.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.ndjson_decoder.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.App.utils.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.App.utils.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.aggregator.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.aggregator.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Aggregator.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Aggregator.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.article_utils.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.article_utils.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.ArticleUtils.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.ArticleUtils.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.download.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.download.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.download.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.download.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.downloader.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.downloader.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Downloader.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Downloader.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.extractor_utils.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.extractor_utils.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Extractor.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Extractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Pipeline.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Pipeline.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Pipeline.pipeline.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Pipeline.pipeline.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Route.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Route.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Route.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Route.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.load_module.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.load_module.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.load_modules.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.load_modules.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.register_route.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.register_route.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.register_routes.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.register_routes.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.Router.route.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.Router.route.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.Router.router.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.Router.router.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.processor_utils.DomainRecord.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.processor_utils.DomainRecord.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.processor_utils.DomainRecord.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.processor_utils.DomainRecord.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.processor_utils.PipeMetadata.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.processor_utils.PipeMetadata.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.processor_utils.PipeMetadata.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.processor_utils.PipeMetadata.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.App.processor_utils.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.App.processor_utils.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.process_article.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.process_article.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_before_message.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_before_message.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_connected.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_connected.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_connecting.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_connecting.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_disconnected.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_disconnected.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_disconnecting.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_disconnecting.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_error.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_error.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_heartbeat.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_heartbeat.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_heartbeat_timeout.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_heartbeat_timeout.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_message.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_message.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_receipt.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_receipt.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_receiver_loop_completed.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_receiver_loop_completed.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Listener.on_send.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Listener.on_send.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.ListnerStats.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.ListnerStats.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.ListnerStats.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.ListnerStats.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Message.__init__.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Message.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.Message.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.Message.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/generated/Processor.processor.html` & `CmonCrawl-0.8.1/docs/build/html/generated/Processor.processor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/genindex.html` & `CmonCrawl-0.8.1/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/index.html` & `CmonCrawl-0.8.1/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/installation.html` & `CmonCrawl-0.8.1/docs/build/html/installation.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/objects.inv` & `CmonCrawl-0.8.1/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/py-modindex.html` & `CmonCrawl-0.8.1/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/quickstart/artemis-queue.html` & `CmonCrawl-0.8.1/docs/build/html/quickstart/artemis-queue.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/quickstart/download_article.html` & `CmonCrawl-0.8.1/docs/build/html/quickstart/download_article.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/quickstart/index.html` & `CmonCrawl-0.8.1/docs/build/html/quickstart/index.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/quickstart/installation.html` & `CmonCrawl-0.8.1/docs/build/html/quickstart/installation.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/quickstart/middleware.html` & `CmonCrawl-0.8.1/docs/build/html/quickstart/middleware.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/quickstart/overview.html` & `CmonCrawl-0.8.1/docs/build/html/quickstart/overview.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/quickstart/quick-start.html` & `CmonCrawl-0.8.1/docs/build/html/quickstart/quick-start.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/search.html` & `CmonCrawl-0.8.1/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/build/html/searchindex.js` & `CmonCrawl-0.8.1/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/make.bat` & `CmonCrawl-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/conf.py` & `CmonCrawl-0.8.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.DomainRecord.rst` & `CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.DomainRecord.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/generated/Aggregator.App.index_query.IndexAggregator.rst` & `CmonCrawl-0.8.1/docs/source/generated/Aggregator.App.index_query.IndexAggregator.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.rst` & `CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/generated/Processor.App.ArticleUtils.article_utils.rst` & `CmonCrawl-0.8.1/docs/source/generated/Processor.App.ArticleUtils.article_utils.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.rst` & `CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.rst` & `CmonCrawl-0.8.1/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.rst` & `CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.rst` & `CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.rst` & `CmonCrawl-0.8.1/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/generated/Processor.App.processor_utils.DomainRecord.rst` & `CmonCrawl-0.8.1/docs/source/generated/Processor.App.processor_utils.DomainRecord.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/generated/Processor.App.processor_utils.PipeMetadata.rst` & `CmonCrawl-0.8.1/docs/source/generated/Processor.App.processor_utils.PipeMetadata.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/generated/Processor.processor.Listener.rst` & `CmonCrawl-0.8.1/docs/source/generated/Processor.processor.Listener.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/index.rst` & `CmonCrawl-0.8.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/installation.rst` & `CmonCrawl-0.8.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/quickstart/artemis-queue.rst` & `CmonCrawl-0.8.1/docs/source/quickstart/artemis-queue.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/quickstart/overview.rst` & `CmonCrawl-0.8.1/docs/source/quickstart/overview.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/docs/source/quickstart/quick-start.rst` & `CmonCrawl-0.8.1/docs/source/quickstart/quick-start.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/examples/extractor_tutorial/Extractors/bbc_extractor.py` & `CmonCrawl-0.8.1/examples/extractor_tutorial/Extractors/bbc_extractor.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/pyproject.toml` & `CmonCrawl-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "CmonCrawl"
-version = "0.8.0"
+version = "0.8.1"
 dependencies = [
 "aiofiles==0.8.0",
 "aiohttp==3.8.1",
 "aiosignal==1.2.0",
 "async-timeout==4.0.2",
 "attrs==21.4.0",
 "beautifulsoup4==4.11.1",
```

### Comparing `CmonCrawl-0.8.0/tests/aggregator_tests.py` & `CmonCrawl-0.8.1/tests/aggregator_tests.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/tests/end_to_end_tests.py` & `CmonCrawl-0.8.1/tests/end_to_end_tests.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/tests/processor_tests.py` & `CmonCrawl-0.8.1/tests/processor_tests.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/tests/test_extract/files/file.html` & `CmonCrawl-0.8.1/tests/test_extract/files/file.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.8.0/tests/test_extract/files/file.json` & `CmonCrawl-0.8.1/tests/test_extract/files/file.json`

 * *Files identical despite different names*

