# Comparing `tmp/syncany-0.2.7.tar.gz` & `tmp/syncany-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncany-0.2.7.tar", last modified: Fri Apr 28 09:59:18 2023, max compression
+gzip compressed data, was "syncany-0.2.8.tar", last modified: Tue May  2 08:48:46 2023, max compression
```

## Comparing `syncany-0.2.7.tar` & `syncany-0.2.8.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:18.148139 syncany-0.2.7/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2022-08-13 12:36:15.000000 syncany-0.2.7/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-28 09:59:18.150139 syncany-0.2.7/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5832 2022-08-13 12:36:15.000000 syncany-0.2.7/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-28 09:59:18.161559 syncany-0.2.7/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1928 2023-04-26 02:13:49.000000 syncany-0.2.7/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:11.950712 syncany-0.2.7/syncany/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      607 2023-04-26 02:13:50.000000 syncany-0.2.7/syncany/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:12.689719 syncany-0.2.7/syncany/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4962 2023-04-25 03:51:51.000000 syncany-0.2.7/syncany/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    39895 2023-04-28 09:52:26.000000 syncany-0.2.7/syncany/calculaters/builtin.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4394 2023-03-24 09:30:00.000000 syncany-0.2.7/syncany/calculaters/calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7999 2023-03-27 08:30:23.000000 syncany-0.2.7/syncany/calculaters/convert_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4573 2023-03-23 03:10:08.000000 syncany-0.2.7/syncany/calculaters/datetime_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2731 2023-04-27 09:47:49.000000 syncany-0.2.7/syncany/calculaters/import_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3167 2023-03-23 03:10:08.000000 syncany-0.2.7/syncany/calculaters/textline_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13898 2023-04-27 03:28:48.000000 syncany-0.2.7/syncany/calculaters/transform_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:13.962514 syncany-0.2.7/syncany/database/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5187 2023-04-25 03:51:51.000000 syncany-0.2.7/syncany/database/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8756 2023-03-24 06:27:35.000000 syncany-0.2.7/syncany/database/beanstalk.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15594 2023-04-25 03:41:03.000000 syncany-0.2.7/syncany/database/clickhouse.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15749 2023-04-25 02:15:32.000000 syncany-0.2.7/syncany/database/csv.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10484 2023-04-26 02:09:40.000000 syncany-0.2.7/syncany/database/database.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12481 2023-02-24 09:33:28.000000 syncany-0.2.7/syncany/database/elasticsearch.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14490 2023-04-25 02:15:32.000000 syncany-0.2.7/syncany/database/excel.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14218 2023-02-22 05:00:17.000000 syncany-0.2.7/syncany/database/http.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    17931 2023-02-24 09:33:28.000000 syncany-0.2.7/syncany/database/influxdb.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12051 2023-04-25 02:15:32.000000 syncany-0.2.7/syncany/database/json.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11954 2023-04-25 02:15:32.000000 syncany-0.2.7/syncany/database/memory.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14642 2023-04-25 03:15:38.000000 syncany-0.2.7/syncany/database/mongodb.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14723 2023-04-25 03:35:50.000000 syncany-0.2.7/syncany/database/mysql.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14858 2023-04-25 03:37:13.000000 syncany-0.2.7/syncany/database/postgresql.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    18023 2023-04-25 02:22:52.000000 syncany-0.2.7/syncany/database/redis.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13949 2023-03-28 03:39:46.000000 syncany-0.2.7/syncany/database/sqlite.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15489 2023-04-25 03:39:10.000000 syncany-0.2.7/syncany/database/sqlserver.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    17928 2023-04-23 08:27:57.000000 syncany-0.2.7/syncany/database/textline.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      685 2022-08-23 12:03:29.000000 syncany-0.2.7/syncany/errors.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:14.145793 syncany-0.2.7/syncany/filters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2275 2023-04-25 03:51:51.000000 syncany-0.2.7/syncany/filters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    19439 2023-04-01 08:20:13.000000 syncany-0.2.7/syncany/filters/builtin.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      309 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/filters/filter.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2023-02-16 02:10:09.000000 syncany-0.2.7/syncany/hook.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:14.588097 syncany-0.2.7/syncany/loaders/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      927 2023-03-25 04:34:57.000000 syncany-0.2.7/syncany/loaders/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1403 2023-04-27 03:37:21.000000 syncany-0.2.7/syncany/loaders/cache.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1001 2023-04-27 10:25:51.000000 syncany-0.2.7/syncany/loaders/const.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6275 2023-04-27 09:34:08.000000 syncany-0.2.7/syncany/loaders/db.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8832 2023-04-28 01:46:51.000000 syncany-0.2.7/syncany/loaders/db_join.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1754 2023-04-27 03:37:21.000000 syncany-0.2.7/syncany/loaders/db_pull.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8749 2023-04-27 03:37:21.000000 syncany-0.2.7/syncany/loaders/loader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      214 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/logger.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13966 2023-03-24 04:36:02.000000 syncany-0.2.7/syncany/main.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:15.149055 syncany-0.2.7/syncany/outputers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1161 2023-03-25 04:34:57.000000 syncany-0.2.7/syncany/outputers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1491 2023-02-24 04:31:16.000000 syncany-0.2.7/syncany/outputers/db.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1962 2023-04-25 03:15:38.000000 syncany-0.2.7/syncany/outputers/db_delete_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      932 2023-04-25 03:15:38.000000 syncany-0.2.7/syncany/outputers/db_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5697 2023-04-25 03:15:38.000000 syncany-0.2.7/syncany/outputers/db_update_delete_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4210 2023-04-25 03:15:38.000000 syncany-0.2.7/syncany/outputers/db_update_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2864 2023-03-22 02:35:53.000000 syncany-0.2.7/syncany/outputers/outputer.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:15.450759 syncany-0.2.7/syncany/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       52 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:16.005719 syncany-0.2.7/syncany/taskers/config/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1794 2023-03-25 04:34:57.000000 syncany-0.2.7/syncany/taskers/config/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      405 2022-08-23 12:07:09.000000 syncany-0.2.7/syncany/taskers/config/file_reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      937 2022-08-23 12:07:09.000000 syncany-0.2.7/syncany/taskers/config/http_reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      195 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/config/json_parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      208 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/config/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      204 2022-08-23 11:55:44.000000 syncany-0.2.7/syncany/taskers/config/reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5006 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/config/yaml_parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1377 2023-02-24 02:44:01.000000 syncany-0.2.7/syncany/taskers/context.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:16.571060 syncany-0.2.7/syncany/taskers/core/
--rwxrwxrwx   0 snower    (1000) snower    (1000)    73215 2023-04-27 03:12:59.000000 syncany-0.2.7/syncany/taskers/core/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2192 2023-03-21 06:17:51.000000 syncany-0.2.7/syncany/taskers/core/loader_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      256 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/core/option.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2592 2023-02-10 08:39:32.000000 syncany-0.2.7/syncany/taskers/core/outputer_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4736 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/core/states.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15689 2023-02-25 11:47:43.000000 syncany-0.2.7/syncany/taskers/core/valuer_compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    42975 2023-04-28 01:45:52.000000 syncany-0.2.7/syncany/taskers/core/valuer_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      760 2023-02-25 12:43:51.000000 syncany-0.2.7/syncany/taskers/iterator.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      245 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/manager.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7122 2023-04-20 05:48:37.000000 syncany-0.2.7/syncany/taskers/tasker.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11025 2023-04-20 03:35:47.000000 syncany-0.2.7/syncany/utils.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:18.095853 syncany-0.2.7/syncany/valuers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2193 2023-04-27 03:26:45.000000 syncany-0.2.7/syncany/valuers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5565 2023-04-27 07:59:50.000000 syncany-0.2.7/syncany/valuers/aggregate.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5094 2023-04-27 07:59:50.000000 syncany-0.2.7/syncany/valuers/assign.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7021 2023-04-27 06:17:05.000000 syncany-0.2.7/syncany/valuers/cache.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5314 2023-04-27 08:52:53.000000 syncany-0.2.7/syncany/valuers/calculate.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8936 2023-04-27 06:17:04.000000 syncany-0.2.7/syncany/valuers/call.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6980 2023-04-28 06:13:22.000000 syncany-0.2.7/syncany/valuers/case.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6243 2023-04-28 06:13:22.000000 syncany-0.2.7/syncany/valuers/condition.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      548 2023-04-27 03:12:59.000000 syncany-0.2.7/syncany/valuers/const.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4916 2023-04-28 05:47:00.000000 syncany-0.2.7/syncany/valuers/data.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9997 2023-04-28 03:45:24.000000 syncany-0.2.7/syncany/valuers/db_join.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3424 2023-04-27 04:30:58.000000 syncany-0.2.7/syncany/valuers/db_load.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3082 2023-04-27 04:30:58.000000 syncany-0.2.7/syncany/valuers/function.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8557 2023-04-27 08:06:54.000000 syncany-0.2.7/syncany/valuers/generator.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5960 2023-04-28 06:00:35.000000 syncany-0.2.7/syncany/valuers/inherit.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5129 2023-04-27 06:17:05.000000 syncany-0.2.7/syncany/valuers/let.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    16860 2023-04-27 06:17:04.000000 syncany-0.2.7/syncany/valuers/loop.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8197 2023-04-28 06:13:22.000000 syncany-0.2.7/syncany/valuers/make.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12466 2023-04-28 06:13:22.000000 syncany-0.2.7/syncany/valuers/match.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2308 2023-04-27 06:17:04.000000 syncany-0.2.7/syncany/valuers/schema.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5717 2023-04-27 06:17:04.000000 syncany-0.2.7/syncany/valuers/state.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7804 2023-04-28 05:47:00.000000 syncany-0.2.7/syncany/valuers/valuer.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:12.201116 syncany-0.2.7/syncany.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-28 09:59:09.000000 syncany-0.2.7/syncany.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2889 2023-04-28 09:59:11.000000 syncany-0.2.7/syncany.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-28 09:59:09.000000 syncany-0.2.7/syncany.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       47 2023-04-28 09:59:09.000000 syncany-0.2.7/syncany.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2022-08-15 03:43:33.000000 syncany-0.2.7/syncany.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      371 2023-04-28 09:59:09.000000 syncany-0.2.7/syncany.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        8 2023-04-28 09:59:09.000000 syncany-0.2.7/syncany.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:46.435967 syncany-0.2.8/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2022-08-13 12:36:15.000000 syncany-0.2.8/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-05-02 08:48:46.437967 syncany-0.2.8/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5832 2022-08-13 12:36:15.000000 syncany-0.2.8/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-02 08:48:46.447486 syncany-0.2.8/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1928 2023-04-29 02:27:19.000000 syncany-0.2.8/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:40.958386 syncany-0.2.8/syncany/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      607 2023-04-29 02:27:19.000000 syncany-0.2.8/syncany/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:41.670417 syncany-0.2.8/syncany/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4962 2023-04-25 03:51:51.000000 syncany-0.2.8/syncany/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    39895 2023-04-28 09:52:26.000000 syncany-0.2.8/syncany/calculaters/builtin.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4394 2023-03-24 09:30:00.000000 syncany-0.2.8/syncany/calculaters/calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7999 2023-03-27 08:30:23.000000 syncany-0.2.8/syncany/calculaters/convert_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4573 2023-03-23 03:10:08.000000 syncany-0.2.8/syncany/calculaters/datetime_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2731 2023-04-27 09:47:49.000000 syncany-0.2.8/syncany/calculaters/import_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3167 2023-03-23 03:10:08.000000 syncany-0.2.8/syncany/calculaters/textline_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13898 2023-04-27 03:28:48.000000 syncany-0.2.8/syncany/calculaters/transform_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:42.732953 syncany-0.2.8/syncany/database/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5187 2023-04-25 03:51:51.000000 syncany-0.2.8/syncany/database/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8756 2023-03-24 06:27:35.000000 syncany-0.2.8/syncany/database/beanstalk.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15594 2023-04-25 03:41:03.000000 syncany-0.2.8/syncany/database/clickhouse.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15749 2023-04-25 02:15:32.000000 syncany-0.2.8/syncany/database/csv.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10484 2023-04-26 02:09:40.000000 syncany-0.2.8/syncany/database/database.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12481 2023-02-24 09:33:28.000000 syncany-0.2.8/syncany/database/elasticsearch.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14490 2023-04-25 02:15:32.000000 syncany-0.2.8/syncany/database/excel.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14218 2023-02-22 05:00:17.000000 syncany-0.2.8/syncany/database/http.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    17931 2023-02-24 09:33:28.000000 syncany-0.2.8/syncany/database/influxdb.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12051 2023-04-25 02:15:32.000000 syncany-0.2.8/syncany/database/json.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11954 2023-04-25 02:15:32.000000 syncany-0.2.8/syncany/database/memory.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14642 2023-04-25 03:15:38.000000 syncany-0.2.8/syncany/database/mongodb.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14723 2023-04-25 03:35:50.000000 syncany-0.2.8/syncany/database/mysql.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14858 2023-04-25 03:37:13.000000 syncany-0.2.8/syncany/database/postgresql.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    18023 2023-04-25 02:22:52.000000 syncany-0.2.8/syncany/database/redis.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13949 2023-03-28 03:39:46.000000 syncany-0.2.8/syncany/database/sqlite.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15489 2023-04-25 03:39:10.000000 syncany-0.2.8/syncany/database/sqlserver.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    17928 2023-04-23 08:27:57.000000 syncany-0.2.8/syncany/database/textline.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      685 2022-08-23 12:03:29.000000 syncany-0.2.8/syncany/errors.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:42.915979 syncany-0.2.8/syncany/filters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2275 2023-04-25 03:51:51.000000 syncany-0.2.8/syncany/filters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    19439 2023-04-01 08:20:13.000000 syncany-0.2.8/syncany/filters/builtin.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      309 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/filters/filter.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2023-02-16 02:10:09.000000 syncany-0.2.8/syncany/hook.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:43.331493 syncany-0.2.8/syncany/loaders/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      927 2023-03-25 04:34:57.000000 syncany-0.2.8/syncany/loaders/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1403 2023-04-27 03:37:21.000000 syncany-0.2.8/syncany/loaders/cache.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1001 2023-04-27 10:25:51.000000 syncany-0.2.8/syncany/loaders/const.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6587 2023-05-01 07:54:55.000000 syncany-0.2.8/syncany/loaders/db.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8832 2023-04-28 01:46:51.000000 syncany-0.2.8/syncany/loaders/db_join.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1754 2023-04-27 03:37:21.000000 syncany-0.2.8/syncany/loaders/db_pull.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9616 2023-04-30 15:15:40.000000 syncany-0.2.8/syncany/loaders/loader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      214 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/logger.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13966 2023-03-24 04:36:02.000000 syncany-0.2.8/syncany/main.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:43.750243 syncany-0.2.8/syncany/outputers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1161 2023-03-25 04:34:57.000000 syncany-0.2.8/syncany/outputers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1491 2023-02-24 04:31:16.000000 syncany-0.2.8/syncany/outputers/db.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1962 2023-04-25 03:15:38.000000 syncany-0.2.8/syncany/outputers/db_delete_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      932 2023-04-25 03:15:38.000000 syncany-0.2.8/syncany/outputers/db_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5697 2023-04-25 03:15:38.000000 syncany-0.2.8/syncany/outputers/db_update_delete_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4210 2023-04-25 03:15:38.000000 syncany-0.2.8/syncany/outputers/db_update_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2864 2023-03-22 02:35:53.000000 syncany-0.2.8/syncany/outputers/outputer.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:44.054012 syncany-0.2.8/syncany/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       52 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:44.561012 syncany-0.2.8/syncany/taskers/config/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1794 2023-03-25 04:34:57.000000 syncany-0.2.8/syncany/taskers/config/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      405 2022-08-23 12:07:09.000000 syncany-0.2.8/syncany/taskers/config/file_reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      937 2022-08-23 12:07:09.000000 syncany-0.2.8/syncany/taskers/config/http_reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      195 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/config/json_parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      208 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/config/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      204 2022-08-23 11:55:44.000000 syncany-0.2.8/syncany/taskers/config/reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5006 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/config/yaml_parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1377 2023-02-24 02:44:01.000000 syncany-0.2.8/syncany/taskers/context.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:45.069025 syncany-0.2.8/syncany/taskers/core/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    73709 2023-05-01 07:47:08.000000 syncany-0.2.8/syncany/taskers/core/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2192 2023-03-21 06:17:51.000000 syncany-0.2.8/syncany/taskers/core/loader_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      256 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/core/option.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2592 2023-02-10 08:39:32.000000 syncany-0.2.8/syncany/taskers/core/outputer_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4736 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/core/states.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15689 2023-02-25 11:47:43.000000 syncany-0.2.8/syncany/taskers/core/valuer_compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    42975 2023-04-28 01:45:52.000000 syncany-0.2.8/syncany/taskers/core/valuer_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      760 2023-02-25 12:43:51.000000 syncany-0.2.8/syncany/taskers/iterator.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      245 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/manager.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7122 2023-04-20 05:48:37.000000 syncany-0.2.8/syncany/taskers/tasker.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11025 2023-04-20 03:35:47.000000 syncany-0.2.8/syncany/utils.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:46.390869 syncany-0.2.8/syncany/valuers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2193 2023-04-27 03:26:45.000000 syncany-0.2.8/syncany/valuers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5565 2023-04-27 07:59:50.000000 syncany-0.2.8/syncany/valuers/aggregate.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5094 2023-04-27 07:59:50.000000 syncany-0.2.8/syncany/valuers/assign.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7021 2023-04-27 06:17:05.000000 syncany-0.2.8/syncany/valuers/cache.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5314 2023-04-27 08:52:53.000000 syncany-0.2.8/syncany/valuers/calculate.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8936 2023-04-27 06:17:04.000000 syncany-0.2.8/syncany/valuers/call.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6980 2023-04-28 06:13:22.000000 syncany-0.2.8/syncany/valuers/case.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6243 2023-04-28 06:13:22.000000 syncany-0.2.8/syncany/valuers/condition.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      548 2023-04-27 03:12:59.000000 syncany-0.2.8/syncany/valuers/const.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4916 2023-04-28 05:47:00.000000 syncany-0.2.8/syncany/valuers/data.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9997 2023-04-28 03:45:24.000000 syncany-0.2.8/syncany/valuers/db_join.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3424 2023-04-27 04:30:58.000000 syncany-0.2.8/syncany/valuers/db_load.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3082 2023-04-27 04:30:58.000000 syncany-0.2.8/syncany/valuers/function.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8557 2023-04-27 08:06:54.000000 syncany-0.2.8/syncany/valuers/generator.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5698 2023-05-01 07:19:03.000000 syncany-0.2.8/syncany/valuers/inherit.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5129 2023-04-27 06:17:05.000000 syncany-0.2.8/syncany/valuers/let.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    16860 2023-04-27 06:17:04.000000 syncany-0.2.8/syncany/valuers/loop.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8197 2023-04-28 06:13:22.000000 syncany-0.2.8/syncany/valuers/make.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12466 2023-04-28 06:13:22.000000 syncany-0.2.8/syncany/valuers/match.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2308 2023-04-27 06:17:04.000000 syncany-0.2.8/syncany/valuers/schema.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5717 2023-04-27 06:17:04.000000 syncany-0.2.8/syncany/valuers/state.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8187 2023-04-30 16:14:31.000000 syncany-0.2.8/syncany/valuers/valuer.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:41.226388 syncany-0.2.8/syncany.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-05-02 08:48:39.000000 syncany-0.2.8/syncany.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2889 2023-05-02 08:48:40.000000 syncany-0.2.8/syncany.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-02 08:48:39.000000 syncany-0.2.8/syncany.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       47 2023-05-02 08:48:39.000000 syncany-0.2.8/syncany.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2022-08-15 03:43:33.000000 syncany-0.2.8/syncany.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      371 2023-05-02 08:48:39.000000 syncany-0.2.8/syncany.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        8 2023-05-02 08:48:39.000000 syncany-0.2.8/syncany.egg-info/top_level.txt
```

### Comparing `syncany-0.2.7/LICENSE` & `syncany-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/PKG-INFO` & `syncany-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncany
-Version: 0.2.7
+Version: 0.2.8
 Summary: 简单易用的数据同步转换导出框架
 Home-page: https://github.com/snower/syncany
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany
```

### Comparing `syncany-0.2.7/README.md` & `syncany-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/setup.py` & `syncany-0.2.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 18/8/6
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.2.7"
+version = "0.2.8"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
```

### Comparing `syncany-0.2.7/syncany/__init__.py` & `syncany-0.2.8/syncany/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
-version = "0.2.7"
-version_info = (0, 2, 7)
+version = "0.2.8"
+version_info = (0, 2, 8)
 
 from .loaders import Loader, register_loader
 from .outputers import Outputer, register_outputer
 from .valuers import Valuer, register_valuer
 from .filters import Filter, register_filter
 from .database import DataBase, register_database
 from .calculaters import Calculater, TypeFormatCalculater, TypingCalculater, MathematicalCalculater, \
```

### Comparing `syncany-0.2.7/syncany/calculaters/__init__.py` & `syncany-0.2.8/syncany/calculaters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/calculaters/builtin.py` & `syncany-0.2.8/syncany/calculaters/builtin.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/calculaters/calculater.py` & `syncany-0.2.8/syncany/calculaters/calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/calculaters/convert_calculater.py` & `syncany-0.2.8/syncany/calculaters/convert_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/calculaters/datetime_calculater.py` & `syncany-0.2.8/syncany/calculaters/datetime_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/calculaters/import_calculater.py` & `syncany-0.2.8/syncany/calculaters/import_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/calculaters/textline_calculater.py` & `syncany-0.2.8/syncany/calculaters/textline_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/calculaters/transform_calculater.py` & `syncany-0.2.8/syncany/calculaters/transform_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/__init__.py` & `syncany-0.2.8/syncany/database/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/beanstalk.py` & `syncany-0.2.8/syncany/database/beanstalk.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/clickhouse.py` & `syncany-0.2.8/syncany/database/clickhouse.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/csv.py` & `syncany-0.2.8/syncany/database/csv.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/database.py` & `syncany-0.2.8/syncany/database/database.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/elasticsearch.py` & `syncany-0.2.8/syncany/database/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/excel.py` & `syncany-0.2.8/syncany/database/excel.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/http.py` & `syncany-0.2.8/syncany/database/http.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/influxdb.py` & `syncany-0.2.8/syncany/database/influxdb.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/json.py` & `syncany-0.2.8/syncany/database/json.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/memory.py` & `syncany-0.2.8/syncany/database/memory.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/mongodb.py` & `syncany-0.2.8/syncany/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/mysql.py` & `syncany-0.2.8/syncany/database/mysql.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/postgresql.py` & `syncany-0.2.8/syncany/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/redis.py` & `syncany-0.2.8/syncany/database/redis.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/sqlite.py` & `syncany-0.2.8/syncany/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/sqlserver.py` & `syncany-0.2.8/syncany/database/sqlserver.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/database/textline.py` & `syncany-0.2.8/syncany/database/textline.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/errors.py` & `syncany-0.2.8/syncany/errors.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/filters/__init__.py` & `syncany-0.2.8/syncany/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/filters/builtin.py` & `syncany-0.2.8/syncany/filters/builtin.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/hook.py` & `syncany-0.2.8/syncany/hook.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/loaders/__init__.py` & `syncany-0.2.8/syncany/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/loaders/cache.py` & `syncany-0.2.8/syncany/loaders/cache.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/loaders/const.py` & `syncany-0.2.8/syncany/loaders/const.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/loaders/db.py` & `syncany-0.2.8/syncany/loaders/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
 import copy
 from collections import defaultdict, deque
 from .loader import Loader
-from ..valuers.valuer import Contexter, ContextRunner, LoadAllFieldsException
+from ..valuers.valuer import Contexter, ContextRunner, ContextDataer, LoadAllFieldsException
 
 
 class DBLoader(Loader):
     def __init__(self, db, name, *args, **kwargs):
         super(DBLoader, self).__init__(*args, **kwargs)
 
         self.db = db
         self.name = name
-        self.compiled = False
+        self.contexter = False
         self.last_data = None
 
     def clone(self):
         loader = self.__class__(self.db, self.name, self.primary_keys, self.valuer_type)
+        loader.contexter = self.contexter
         schema = {}
         for key, valuer in self.schema.items():
             schema[key] = valuer.clone()
         loader.schema = schema
         loader.filters = [filter for filter in self.filters]
         loader.orders = [order for order in self.orders]
         loader.intercepts = [intercept.clone() for intercept in self.intercepts]
@@ -98,54 +99,63 @@
         if self.current_cursor:
             query.filter_cursor(*self.current_cursor, primary_orders=primary_orders)
 
         self.datas, query = query.commit(), None
         self.last_data = copy.copy(self.datas[-1]) if self.datas else {}
         self.loader_state["query_count"] += 1
         self.loader_state["load_count"] += len(self.datas)
-        self.compiled = False
         self.loaded = True
 
     def get(self):
         if self.geted:
             return self.datas
         if not self.loaded:
             self.load()
 
-        if not self.compiled:
-            if not self.key_matchers:
-                require_loaded_schema_items = [(key, field, field.contexter if hasattr(field, "contexter") else None)
-                                               for key, field in self.schema.items() if field.require_loaded()]
-                if not require_loaded_schema_items:
-                    if not self.valuer_type:
-                        return self.fast_get()
-                    return super(DBLoader, self).get()
-                for i in range(len(self.datas)):
-                    data, contexter_values = copy.copy(self.datas[i]), {}
-                    for key, field, contexter in require_loaded_schema_items:
-                        if contexter is None:
-                            contexter = Contexter()
-                            field = field.clone(contexter)
-                        data[key] = ContextRunner(contexter, field, contexter_values).fill(data)
-                    self.datas[i] = data
-            else:
+        if not self.key_matchers:
+            loader_contexter = self.contexter
+            if loader_contexter is False:
+                if not self.valuer_type:
+                    return self.fast_get()
+                return super(DBLoader, self).get()
+
+            if loader_contexter is not None:
                 for i in range(len(self.datas)):
-                    data = {}
-                    for key, value in self.datas[i].items():
-                        if key in self.schema:
-                            data[key] = value
-                            continue
-                        for key_matcher in self.key_matchers:
-                            if not key_matcher.match(key):
-                                continue
-                            self.schema[key] = key_matcher.create_key(key)
-                            data[key] = value
-                            break
-                    self.datas[i] = data
+                    data, context_dataer = self.datas[i], ContextDataer(loader_contexter)
+                    loader_contexter.values = context_dataer.values
+                    for key, field in self.schema.items():
+                        field.fill(data)
+                    self.datas[i] = context_dataer
+                return super(DBLoader, self).get()
 
+            contexter_schema = [(key, field, field.contexter if hasattr(field, "contexter") else None)
+                                for key, field in self.schema.items()]
+            for i in range(len(self.datas)):
+                data, odata, contexter_values = self.datas[i], {}, {}
+                for key, field, contexter in contexter_schema:
+                    if contexter is None:
+                        contexter = Contexter()
+                        field = field.clone(contexter)
+                    odata[key] = ContextRunner(contexter, field, contexter_values).fill(data)
+                self.datas[i] = odata
+            return super(DBLoader, self).get()
+
+        for i in range(len(self.datas)):
+            data = {}
+            for key, value in self.datas[i].items():
+                if key in self.schema:
+                    data[key] = value
+                    continue
+                for key_matcher in self.key_matchers:
+                    if not key_matcher.match(key):
+                        continue
+                    self.schema[key] = key_matcher.create_key(key)
+                    data[key] = value
+                    break
+            self.datas[i] = data
         return super(DBLoader, self).get()
 
     def fast_get(self):
         if not self.intercepts:
             for i in range(len(self.datas)):
                 data = self.datas[i]
                 self.datas[i] = {name: valuer.fill(data).get() for name, valuer in self.schema.items()}
```

### Comparing `syncany-0.2.7/syncany/loaders/db_join.py` & `syncany-0.2.8/syncany/loaders/db_join.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/loaders/db_pull.py` & `syncany-0.2.8/syncany/loaders/db_pull.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/loaders/loader.py` & `syncany-0.2.8/syncany/loaders/loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
 import types
 import re
 from collections import defaultdict, deque
-from ..valuers import ContextRunner
+from ..valuers.valuer import ContextRunner, ContextDataer
 
 
 class KeyMatcher(object):
     def __init__(self, matcher, valuer):
         if isinstance(matcher, str):
             self.matcher = re.compile(matcher)
         else:
@@ -105,41 +105,60 @@
         if not self.loaded:
             self.load()
 
         datas, self.datas = deque(self.datas), []
         if not self.valuer_type:
             while datas:
                 data, odata = datas.popleft(), {}
-                for name, valuer in self.schema.items():
-                    if name not in data or not isinstance(data[name], ContextRunner):
-                        odata[name] = valuer.fill(data).get()
-                    else:
-                        odata[name] = data[name].get()
+                if isinstance(data, ContextDataer):
+                    data.use_values()
+                    for name, valuer in self.schema.items():
+                        odata[name] = valuer.get()
+                else:
+                    for name, valuer in self.schema.items():
+                        if name not in data or not isinstance(data[name], ContextRunner):
+                            odata[name] = valuer.fill(data).get()
+                        else:
+                            odata[name] = data[name].get()
                 if self.intercepts and self.check_intercepts(odata):
                     continue
                 self.datas.append(odata)
             self.geted = True
             return self.datas
 
         while datas:
             data, odata, oyields, ofuncs = datas.popleft(), {}, {}, {}
-            for name, valuer in self.schema.items():
-                if name not in data or not isinstance(data[name], ContextRunner):
-                    value = valuer.fill(data).get()
-                else:
-                    value = data[name].get()
-                if isinstance(value, types.FunctionType):
-                    ofuncs[name] = value
-                    odata[name] = None
-                    continue
-                if isinstance(value, types.GeneratorType):
-                    oyields[name] = value
-                    odata[name] = None
-                    continue
-                odata[name] = value
+            if isinstance(data, ContextDataer):
+                data.use_values()
+                for name, valuer in self.schema.items():
+                    value = valuer.get()
+                    if isinstance(value, types.FunctionType):
+                        ofuncs[name] = value
+                        odata[name] = None
+                        continue
+                    if isinstance(value, types.GeneratorType):
+                        oyields[name] = value
+                        odata[name] = None
+                        continue
+                    odata[name] = value
+            else:
+                for name, valuer in self.schema.items():
+                    if name not in data or not isinstance(data[name], ContextRunner):
+                        value = valuer.fill(data).get()
+                    else:
+                        value = data[name].get()
+                    if isinstance(value, types.FunctionType):
+                        ofuncs[name] = value
+                        odata[name] = None
+                        continue
+                    if isinstance(value, types.GeneratorType):
+                        oyields[name] = value
+                        odata[name] = None
+                        continue
+                    odata[name] = value
 
             if oyields:
                 while oyields:
                     oyield_data = {name: value for name, value in odata.items()}
                     has_oyield_data = False
                     for name, oyield in tuple(oyields.items()):
                         try:
@@ -180,21 +199,19 @@
                         self.datas.append(odata)
                 else:
                     self.datas.append(odata)
         self.geted = True
         return self.datas
 
     def check_intercepts(self, data):
-        intercept_stoped = False
         for intercept in self.intercepts:
             intercept_result = intercept.fill(data).get()
             if intercept_result is not None and not intercept_result:
-                intercept_stoped = True
-                break
-        return intercept_stoped
+                return True
+        return False
 
     def add_filter(self, key, exp, value):
         self.filters.append([key, exp, value])
 
     def filter_gt(self, key, value):
         for filter in self.filters:
             if key == filter[0] and "gt" == filter[1]:
```

### Comparing `syncany-0.2.7/syncany/main.py` & `syncany-0.2.8/syncany/main.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/outputers/__init__.py` & `syncany-0.2.8/syncany/outputers/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/outputers/db.py` & `syncany-0.2.8/syncany/outputers/db.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/outputers/db_delete_insert.py` & `syncany-0.2.8/syncany/outputers/db_delete_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/outputers/db_insert.py` & `syncany-0.2.8/syncany/outputers/db_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/outputers/db_update_delete_insert.py` & `syncany-0.2.8/syncany/outputers/db_update_delete_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/outputers/db_update_insert.py` & `syncany-0.2.8/syncany/outputers/db_update_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/outputers/outputer.py` & `syncany-0.2.8/syncany/outputers/outputer.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/taskers/config/__init__.py` & `syncany-0.2.8/syncany/taskers/config/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/taskers/config/http_reader.py` & `syncany-0.2.8/syncany/taskers/config/http_reader.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/taskers/config/yaml_parser.py` & `syncany-0.2.8/syncany/taskers/config/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/taskers/context.py` & `syncany-0.2.8/syncany/taskers/context.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/taskers/core/__init__.py` & `syncany-0.2.8/syncany/taskers/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -770,32 +770,42 @@
             "valuer_type": 0,
         })
         if "loader_arguments" in self.config and isinstance(self.config["loader_arguments"], dict):
             loader_config.update(self.config["loader_arguments"])
         self.loader = self.create_loader(loader_config, input_loader["foreign_key"])
 
         if isinstance(self.schema, dict):
-            aggregate_valuers = []
+            loader_schema, aggregate_valuers, require_loaded = {}, [], False
             for name, valuer in self.schema.items():
                 inherit_valuers, yield_valuers = [], []
                 valuer = self.create_valuer(valuer, schema_field_name=name, inherit_valuers=inherit_valuers,
                                             join_loaders=self.join_loaders, yield_valuers=yield_valuers,
                                             aggregate_valuers=aggregate_valuers, define_valuers={},
                                             global_variables=self.global_variables, global_states=self.states)
-                if valuer:
-                    if valuer.require_loaded():
-                        valuer = valuer.clone(Contexter())
-                    self.loader.add_valuer(name, valuer)
+                if not valuer:
+                    continue
+                if valuer.require_loaded():
+                    require_loaded = True
+                loader_schema[name] = valuer
                 if inherit_valuers:
                     raise OverflowError(name + " inherit out of range")
                 if yield_valuers:
                     loader_config["valuer_type"] |= 0x01
                 if aggregate_valuers:
                     loader_config["valuer_type"] |= 0x02
-                self.loader.valuer_type = loader_config["valuer_type"]
+            if require_loaded:
+                contexter = Contexter()
+                for name, valuer in loader_schema.items():
+                    self.loader.add_valuer(name, valuer.clone(contexter))
+                if hasattr(self.loader, "contexter"):
+                    self.loader.contexter = contexter
+            else:
+                for name, valuer in loader_schema.items():
+                    self.loader.add_valuer(name, valuer)
+            self.loader.valuer_type = loader_config["valuer_type"]
         elif self.schema == ".*":
             self.loader.add_key_matcher(".*", self.create_valuer(self.valuer_compiler.compile_data_valuer("", None)))
 
         for query in self.config["querys"]:
             for query_exp in query["exps"]:
                 if not hasattr(self.loader, "filter_%s" % query_exp["exp_name"]):
                     continue
```

### Comparing `syncany-0.2.7/syncany/taskers/core/loader_creater.py` & `syncany-0.2.8/syncany/taskers/core/loader_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/taskers/core/outputer_creater.py` & `syncany-0.2.8/syncany/taskers/core/outputer_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/taskers/core/states.py` & `syncany-0.2.8/syncany/taskers/core/states.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/taskers/core/valuer_compiler.py` & `syncany-0.2.8/syncany/taskers/core/valuer_compiler.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/taskers/core/valuer_creater.py` & `syncany-0.2.8/syncany/taskers/core/valuer_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/taskers/iterator.py` & `syncany-0.2.8/syncany/taskers/iterator.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/taskers/tasker.py` & `syncany-0.2.8/syncany/taskers/tasker.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/utils.py` & `syncany-0.2.8/syncany/utils.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/__init__.py` & `syncany-0.2.8/syncany/valuers/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/aggregate.py` & `syncany-0.2.8/syncany/valuers/aggregate.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/assign.py` & `syncany-0.2.8/syncany/valuers/assign.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/cache.py` & `syncany-0.2.8/syncany/valuers/cache.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/calculate.py` & `syncany-0.2.8/syncany/valuers/calculate.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/call.py` & `syncany-0.2.8/syncany/valuers/call.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/case.py` & `syncany-0.2.8/syncany/valuers/case.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/condition.py` & `syncany-0.2.8/syncany/valuers/condition.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/const.py` & `syncany-0.2.8/syncany/valuers/const.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/data.py` & `syncany-0.2.8/syncany/valuers/data.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/db_join.py` & `syncany-0.2.8/syncany/valuers/db_join.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/db_load.py` & `syncany-0.2.8/syncany/valuers/db_load.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/function.py` & `syncany-0.2.8/syncany/valuers/function.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/generator.py` & `syncany-0.2.8/syncany/valuers/generator.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/inherit.py` & `syncany-0.2.8/syncany/valuers/inherit.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,27 @@
 # create by: snower
 
 import weakref
 from .valuer import Valuer
 
 
 class InheritValuer(Valuer):
-    filled = False
-
     def __init__(self, value_valuer, *args, **kwargs):
         if isinstance(self, ContextInheritValuer):
             self.child_valuer = ContextInheritChildValuer(self, value_valuer, *args, **kwargs, contexter=self.contexter)
         else:
             self.child_valuer = InheritChildValuer(self, value_valuer, *args, **kwargs)
         self.value_valuer = value_valuer
         self.cloned_child_valuer = None
         super(InheritValuer, self).__init__(*args, **kwargs)
 
     def get_inherit_child_valuer(self):
         return self.child_valuer
 
     def clone(self, contexter=None):
-        if self.filled:
-            return self
-
         if self.child_valuer.cloned_inherit_valuer:
             inherit_valuer = self.child_valuer.cloned_inherit_valuer
             self.child_valuer.cloned_inherit_valuer = None
             return inherit_valuer
 
         value_valuer = self.value_valuer.clone(contexter) if self.value_valuer else None
         if contexter is not None:
@@ -38,24 +33,19 @@
             inherit_valuer = ContextInheritValuer(value_valuer, self.key, self.filter, from_valuer=self,
                                                   contexter=self.contexter)
         else:
             inherit_valuer = self.__class__(value_valuer, self.key, self.filter, from_valuer=self)
         self.cloned_child_valuer = inherit_valuer.get_inherit_child_valuer()
         return inherit_valuer
 
-    def reinit(self):
-        self.filled = False
-        return super(InheritValuer, self).reinit()
-
     def fill(self, data):
         if self.value_valuer:
             self.value_valuer.fill(self.do_filter(data))
         else:
             super(InheritValuer, self).fill(data)
-        self.filled = True
         return self
 
     def get(self):
         return None
 
     def childs(self):
         if not self.value_valuer:
@@ -70,16 +60,16 @@
     def get_final_filter(self):
         return None
 
 
 class ContextInheritValuer(InheritValuer):
     def __init__(self, *args, **kwargs):
         self.contexter = kwargs.pop("contexter")
-        self.value_context_id = (id(self), "value")
         super(ContextInheritValuer, self).__init__(*args, **kwargs)
+        self.value_context_id = (id(self.child_valuer), "value")
 
     @property
     def value(self):
         try:
             return self.contexter.values[self.value_context_id]
         except KeyError:
             return None
@@ -97,17 +87,14 @@
     def __init__(self, inherit_valuer, value_valuer, *args, **kwargs):
         self.inherit_valuer = weakref.proxy(inherit_valuer)
         self.value_valuer = value_valuer
         self.cloned_inherit_valuer = None
         super(InheritChildValuer, self).__init__(*args, **kwargs)
 
     def clone(self, contexter=None):
-        if self.inherit_valuer.filled:
-            return self
-
         if self.inherit_valuer.cloned_child_valuer:
             child_valuer = self.inherit_valuer.cloned_child_valuer
             self.inherit_valuer.cloned_child_valuer = None
             return child_valuer
 
         value_valuer = self.value_valuer.clone(contexter) if self.value_valuer else None
         if contexter is not None:
```

### Comparing `syncany-0.2.7/syncany/valuers/let.py` & `syncany-0.2.8/syncany/valuers/let.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/loop.py` & `syncany-0.2.8/syncany/valuers/loop.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/make.py` & `syncany-0.2.8/syncany/valuers/make.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/match.py` & `syncany-0.2.8/syncany/valuers/match.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/schema.py` & `syncany-0.2.8/syncany/valuers/schema.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/state.py` & `syncany-0.2.8/syncany/valuers/state.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.7/syncany/valuers/valuer.py` & `syncany-0.2.8/syncany/valuers/valuer.py`

 * *Files 12% similar despite different names*

```diff
@@ -90,14 +90,36 @@
         return self
 
     def get(self):
         self.contexter.values = self.values
         return self.valuer.get()
 
 
+class ContextDataer(object):
+    def __init__(self, contexter):
+        self.contexter = contexter
+        self.values = {}
+
+    def fill(self, valuer, data):
+        return valuer.fill(data)
+
+    def get(self, valuer):
+        return valuer.get()
+
+    def use_values(self):
+        self.contexter.values = self.values
+        return self
+
+    def __enter__(self):
+        self.contexter.values = self.values
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
+
+
 class Contexter(object):
     def __init__(self):
         self.values = {}
 
     def create_runner(self, valuer, values=None):
         return ContextRunner(self, valuer, values)
 
@@ -112,19 +134,17 @@
         if from_valuer is None:
             self.new_init()
         else:
             self.clone_init(from_valuer)
 
     def new_init(self):
         self.key_getters = []
-        self.child_valuers = self.childs()
 
     def clone_init(self, from_valuer):
         self.key_getters = from_valuer.key_getters
-        self.child_valuers = from_valuer.child_valuers
 
     def parse_key(self):
         if self.key in self.KEY_GETTER_CACHES:
             self.key_getters = self.KEY_GETTER_CACHES[self.key]
             return
 
         keys = self.key.split(".")
@@ -158,15 +178,15 @@
             return ContextValuer(self.key, self.filter, from_valuer=self, contexter=contexter)
         if isinstance(self, ContextValuer):
             return ContextValuer(self.key, self.filter, from_valuer=self, contexter=self.contexter)
         return self.__class__(self.key, self.filter, from_valuer=self)
 
     def reinit(self):
         self.value = None
-        for valuer in self.child_valuers:
+        for valuer in self.childs():
             valuer.reinit()
         return self
 
     def fill(self, data):
         if isinstance(data, dict) and self.key in data:
             self.value = self.do_filter(data[self.key])
             return self
@@ -194,15 +214,15 @@
             self.value = self.do_filter(None)
         return self
 
     def get(self):
         return self.value
 
     def reset(self):
-        for valuer in self.child_valuers:
+        for valuer in self.childs():
             valuer.reset()
 
     def do_filter(self, value):
         if not self.filter:
             if isinstance(value, datetime.datetime):
                 value = ensure_timezone(value)
             return value
@@ -214,15 +234,15 @@
     def get_fields(self):
         return []
 
     def get_final_filter(self):
         return self.filter
 
     def require_loaded(self):
-        for child in self.child_valuers:
+        for child in self.childs():
             if child.require_loaded():
                 return True
         return False
 
 
 class ContextValuer(Valuer):
     def __init__(self, *args, **kwargs):
```

### Comparing `syncany-0.2.7/syncany.egg-info/PKG-INFO` & `syncany-0.2.8/syncany.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncany
-Version: 0.2.7
+Version: 0.2.8
 Summary: 简单易用的数据同步转换导出框架
 Home-page: https://github.com/snower/syncany
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany
```

### Comparing `syncany-0.2.7/syncany.egg-info/SOURCES.txt` & `syncany-0.2.8/syncany.egg-info/SOURCES.txt`

 * *Files identical despite different names*

