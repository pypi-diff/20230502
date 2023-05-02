# Comparing `tmp/syncanysql-0.1.1.tar.gz` & `tmp/syncanysql-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanysql-0.1.1.tar", last modified: Fri Apr 28 09:59:56 2023, max compression
+gzip compressed data, was "syncanysql-0.1.2.tar", last modified: Tue May  2 08:49:22 2023, max compression
```

## Comparing `syncanysql-0.1.1.tar` & `syncanysql-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:56.588028 syncanysql-0.1.1/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-04-28 09:59:56.589055 syncanysql-0.1.1/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3018 2023-04-25 10:14:55.000000 syncanysql-0.1.1/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-28 09:59:56.600409 syncanysql-0.1.1/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2030 2023-04-26 02:14:48.000000 syncanysql-0.1.1/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:55.221394 syncanysql-0.1.1/syncanysql/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9167 2023-04-26 01:56:02.000000 syncanysql-0.1.1/syncanysql/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:55.648537 syncanysql-0.1.1/syncanysql/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1130 2023-04-23 06:35:38.000000 syncanysql-0.1.1/syncanysql/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.1.1/syncanysql/calculaters/aggregate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.1/syncanysql/calculaters/mysql_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:55.985804 syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10157 2023-04-20 04:07:01.000000 syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/json_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6193 2023-04-24 06:11:11.000000 syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/number_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/string_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)   125599 2023-04-28 09:46:36.000000 syncanysql-0.1.1/syncanysql/compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12804 2023-04-27 09:12:49.000000 syncanysql-0.1.1/syncanysql/config.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.1.1/syncanysql/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7755 2023-04-27 09:10:45.000000 syncanysql-0.1.1/syncanysql/executor.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3750 2023-04-26 01:56:02.000000 syncanysql-0.1.1/syncanysql/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.1/syncanysql/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6965 2023-04-27 09:10:45.000000 syncanysql-0.1.1/syncanysql/prompt.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:56.539127 syncanysql-0.1.1/syncanysql/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.1/syncanysql/taskers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.1/syncanysql/taskers/delete.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1603 2023-04-24 02:15:57.000000 syncanysql-0.1.1/syncanysql/taskers/execute.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.1/syncanysql/taskers/explain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4258 2023-04-26 01:31:23.000000 syncanysql-0.1.1/syncanysql/taskers/into.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    19398 2023-04-28 03:15:43.000000 syncanysql-0.1.1/syncanysql/taskers/query.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.1.1/syncanysql/taskers/set.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.1.1/syncanysql/taskers/show.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-04-25 04:04:01.000000 syncanysql-0.1.1/syncanysql/taskers/use.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.1.1/syncanysql/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-04-26 02:14:48.000000 syncanysql-0.1.1/syncanysql/version.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:55.486511 syncanysql-0.1.1/syncanysql.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-04-28 09:59:54.000000 syncanysql-0.1.1/syncanysql.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1111 2023-04-28 09:59:54.000000 syncanysql-0.1.1/syncanysql.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-28 09:59:54.000000 syncanysql-0.1.1/syncanysql.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-04-28 09:59:54.000000 syncanysql-0.1.1/syncanysql.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.1/syncanysql.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-04-28 09:59:54.000000 syncanysql-0.1.1/syncanysql.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-04-28 09:59:54.000000 syncanysql-0.1.1/syncanysql.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:49:22.828186 syncanysql-0.1.2/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-02 08:49:22.829187 syncanysql-0.1.2/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3018 2023-04-25 10:14:55.000000 syncanysql-0.1.2/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-02 08:49:22.841188 syncanysql-0.1.2/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2030 2023-04-29 02:34:28.000000 syncanysql-0.1.2/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:49:21.453193 syncanysql-0.1.2/syncanysql/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9167 2023-04-26 01:56:02.000000 syncanysql-0.1.2/syncanysql/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:49:21.883188 syncanysql-0.1.2/syncanysql/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1130 2023-04-23 06:35:38.000000 syncanysql-0.1.2/syncanysql/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.1.2/syncanysql/calculaters/aggregate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.2/syncanysql/calculaters/mysql_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:49:22.251187 syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10157 2023-04-20 04:07:01.000000 syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/json_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6193 2023-04-24 06:11:11.000000 syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/number_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/string_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)   133990 2023-05-01 03:18:26.000000 syncanysql-0.1.2/syncanysql/compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12804 2023-04-27 09:12:49.000000 syncanysql-0.1.2/syncanysql/config.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.1.2/syncanysql/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7755 2023-04-27 09:10:45.000000 syncanysql-0.1.2/syncanysql/executor.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3750 2023-04-26 01:56:02.000000 syncanysql-0.1.2/syncanysql/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.2/syncanysql/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6965 2023-04-27 09:10:45.000000 syncanysql-0.1.2/syncanysql/prompt.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:49:22.783187 syncanysql-0.1.2/syncanysql/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.2/syncanysql/taskers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.2/syncanysql/taskers/delete.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1603 2023-04-24 02:15:57.000000 syncanysql-0.1.2/syncanysql/taskers/execute.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.2/syncanysql/taskers/explain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4258 2023-04-26 01:31:23.000000 syncanysql-0.1.2/syncanysql/taskers/into.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    21238 2023-05-01 03:07:04.000000 syncanysql-0.1.2/syncanysql/taskers/query.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.1.2/syncanysql/taskers/set.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.1.2/syncanysql/taskers/show.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-04-25 04:04:01.000000 syncanysql-0.1.2/syncanysql/taskers/use.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.1.2/syncanysql/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-04-29 02:34:28.000000 syncanysql-0.1.2/syncanysql/version.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:49:21.706187 syncanysql-0.1.2/syncanysql.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-02 08:49:20.000000 syncanysql-0.1.2/syncanysql.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1111 2023-05-02 08:49:20.000000 syncanysql-0.1.2/syncanysql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-02 08:49:20.000000 syncanysql-0.1.2/syncanysql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-05-02 08:49:20.000000 syncanysql-0.1.2/syncanysql.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.2/syncanysql.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-05-02 08:49:20.000000 syncanysql-0.1.2/syncanysql.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-05-02 08:49:20.000000 syncanysql-0.1.2/syncanysql.egg-info/top_level.txt
```

### Comparing `syncanysql-0.1.1/PKG-INFO` & `syncanysql-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
```

### Comparing `syncanysql-0.1.1/README.md` & `syncanysql-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/setup.py` & `syncanysql-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.1.1"
+version = "0.1.2"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -34,15 +34,15 @@
     author_email='sujian199@gmail.com',
     license='MIT',
     packages=find_packages(exclude=['*tests*']),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
         "sqlglot>=10.6.2",
-        "syncany>=0.2.7",
+        "syncany>=0.2.8",
         'Pygments>=2.14.0',
         'Pygments>=2.14.0',
         'prompt-toolkit>=3.0.36',
         "rich>=9.11.1",
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
```

### Comparing `syncanysql-0.1.1/syncanysql/__init__.py` & `syncanysql-0.1.2/syncanysql/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/calculaters/__init__.py` & `syncanysql-0.1.2/syncanysql/calculaters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/calculaters/aggregate_calculater.py` & `syncanysql-0.1.2/syncanysql/calculaters/aggregate_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/calculaters/mysql_calculater.py` & `syncanysql-0.1.2/syncanysql/calculaters/mysql_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/datetime_funcs.py` & `syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/datetime_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/json_funcs.py` & `syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/json_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/number_funcs.py` & `syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/number_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/string_funcs.py` & `syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/string_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/compiler.py` & `syncanysql-0.1.2/syncanysql/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             "querys": {},
             "schema": "$.*",
         })
 
         table_info = self.parse_table(expression.args["this"], config, arguments)
         where_expression = expression.args.get("where")
         if where_expression and isinstance(where_expression, sqlglot_expressions.Where):
-            self.compile_where_condition(where_expression.args["this"], config, arguments, table_info)
+            self.compile_where_condition(where_expression.args["this"], config, arguments, table_info, [])
             self.parse_condition_typing_filter(expression, config, arguments)
         config["output"] = "".join(["&.", table_info["db"], ".", table_info["name"], "::id use DI"])
         return config
 
     def compile_query(self, expression, arguments):
         config = {key: copy.deepcopy(self.config.get(key)) for key in CoreTasker.DEFAULT_CONFIG}
         config.update({
@@ -277,15 +277,14 @@
                 for name in subquery_config["schema"]:
                     config["schema"][name] = "$." + name
             config["dependencys"].append(subquery_config)
         config["input"] = "&.--." + query_name + "::" + config["dependencys"][0]["output"].split("::")[-1].split(" ")[0]
         config["output"] = config["output"].split("::")[0] + "::" + config["input"].split("::")[-1].split(" ")[0]
         arguments["@primary_order"] = False
         arguments["@limit"] = 0
-        arguments["@batch"] = 0
 
     def compile_select(self, expression, config, arguments):
         primary_table = {"db": None, "name": None, "table_name": None, "table_alias": None, "seted_primary_keys": False,
                          "loader_primary_keys": [], "outputer_primary_keys": [], "columns": {}, "subquery": None}
 
         from_expression = expression.args.get("from")
         if not from_expression:
@@ -409,35 +408,52 @@
             for name, column in config["schema"].items():
                 if name in config["aggregate"]["schema"]:
                     continue
                 config["aggregate"]["distinct_keys"].append(copy.deepcopy(column))
 
         where_expression = expression.args.get("where")
         if where_expression and isinstance(where_expression, sqlglot_expressions.Where):
-            self.compile_where_condition(where_expression.args["this"], config, arguments, primary_table)
+            where_condition = self.compile_where_condition(where_expression.args["this"], config, arguments, primary_table, join_tables)
+            if where_condition:
+                if not config["intercepts"]:
+                    config["intercepts"] = [["#const", True], ["#const", True]]
+                config["intercepts"][0] = where_condition
             self.parse_condition_typing_filter(expression, config, arguments)
 
         having_expression = expression.args.get("having")
         if having_expression:
-            config["intercepts"].append(self.compile_having_condition(having_expression.args["this"], config, arguments,
-                                                                      primary_table))
-            if config.get("aggregate") and config["aggregate"].get("schema") and config["aggregate"].get("having_columns"):
+            having_condition = self.compile_having_condition(having_expression.args["this"], config, arguments, primary_table)
+            if config.get("aggregate") and config["aggregate"]["having_columns"]:
                 if len({True if having_column in config["aggregate"]["schema"] else False
                         for having_column in config["aggregate"]["having_columns"]}) != 1:
-                    raise SyncanySqlCompileException('error having condition, cannot contain the values before and after the aggregate calculation at the same time, related sql "%s"'
-                                                     % self.to_sql(expression))
-
-        limit_expression = expression.args.get("limit")
-        if limit_expression:
-            arguments["@limit"] = int(limit_expression.args["expression"].args["this"])
+                    raise SyncanySqlCompileException(
+                        'error having condition, cannot contain the values before and after the aggregate calculation at the same time, related sql "%s"'
+                        % self.to_sql(expression))
+            if not config["intercepts"]:
+                config["intercepts"] = [["#const", True], ["#const", True]]
+            config["intercepts"][1] = having_condition
 
         order_expression = expression.args.get("order")
         if order_expression:
             self.compile_order(order_expression.args["expressions"], config, arguments, primary_table)
 
+        if expression.args.get("offset"):
+            offset_expression, limit_expression = expression.args.get("limit"), expression.args.get("offset")
+        else:
+            offset_expression, limit_expression = None, expression.args.get("limit")
+        if limit_expression:
+            offset_value = max(int(offset_expression.args["expression"].args["this"]), 0) if offset_expression else 0
+            limit_value = max(int(limit_expression.args["expression"].args["this"]), 1)
+            if limit_value > 0:
+                if config["intercepts"] or (config.get("aggregate") and config["aggregate"]["schema"]) \
+                        or config["pipelines"] or offset_value > 0:
+                    config["pipelines"].append([">>@array::slice", "$.*|array", offset_value, offset_value + limit_value])
+                else:
+                    arguments["@limit"] = limit_value
+
         if group_expression and ("aggregate" not in config or not config["aggregate"] or not config["aggregate"]["schema"]):
             self.compile_group_column(group_expression, config, arguments, primary_table, join_tables)
         if not from_expression and not primary_table["outputer_primary_keys"] and isinstance(config["schema"], dict):
             for column_alias in config["schema"]:
                 if not column_alias.isidentifier():
                     continue
                 primary_table["outputer_primary_keys"] = [column_alias]
@@ -469,15 +485,14 @@
         config["input"] = "".join(["&.", primary_table["db"], ".", primary_table["name"], "::",
                                    "+".join(primary_table["loader_primary_keys"]) if primary_table["loader_primary_keys"] else "id"])
         config["output"] = "".join([config["output"].split("::")[0], "::",
                                     "+".join(primary_table["outputer_primary_keys"]) if primary_table["outputer_primary_keys"] else "id",
                                     (" use " + config["output"].split(" use ")[-1]) if " use " in config["output"] else " use I"])
         arguments["@primary_order"] = False
         arguments["@limit"] = 0
-        arguments["@batch"] = 0
         return config
 
     def compile_select_into(self, expression, arguments):
         config = {"variables": []}
         if not isinstance(expression.args["this"], sqlglot_expressions.Table):
             raise SyncanySqlCompileException('unknown select into variable, related sql "%s"' % self.to_sql(expression))
         if not isinstance(expression.args["this"].args["this"], sqlglot_expressions.Parameter):
@@ -620,86 +635,186 @@
 
     def compile_join_column_field(self, expression, config, arguments, primary_table, ci, join_column, column_join_tables):
         if not join_column["table_name"] or join_column["table_name"] == primary_table["table_name"]:
             return self.compile_column(expression, config, arguments, join_column, len(column_join_tables) - ci)
         ji = [j for j in range(len(column_join_tables)) if join_column["table_name"] == column_join_tables[j]["name"]][0]
         return self.compile_column(expression, config, arguments, join_column, ji - ci)
 
-    def compile_where_condition(self, expression, config, arguments, primary_table):
-        if not expression:
-            return
+    def compile_where_condition(self, expression, config, arguments, primary_table, join_tables, is_query_condition=True):
         if isinstance(expression, sqlglot_expressions.And):
-            self.compile_where_condition(expression.args.get("this"), config, arguments, primary_table)
-            self.compile_where_condition(expression.args.get("expression"), config, arguments, primary_table)
-            return
+            left_condition = self.compile_where_condition(expression.args.get("this"), config, arguments,
+                                                          primary_table, join_tables, True)
+            right_condition = self.compile_where_condition(expression.args.get("expression"), config, arguments,
+                                                           primary_table, join_tables, True)
+            if left_condition and right_condition:
+                return ["@and", left_condition, right_condition]
+            return left_condition or right_condition or None
+        if isinstance(expression, sqlglot_expressions.Or):
+            return [
+                "@or",
+                self.compile_where_condition(expression.args.get("this"), config, arguments, primary_table, join_tables, False),
+                self.compile_where_condition(expression.args.get("expression"), config, arguments, primary_table, join_tables, False)
+            ]
+
+        def parse_calucate(calculate_expression):
+            if not isinstance(config.get("schema"), dict):
+                return calculate_expression
+            if self.is_column(calculate_expression, config, arguments):
+                calculate_name = "__where_condition_value_%d__" % id(calculate_expression)
+                self.compile_select_calculate_column(calculate_expression, config, arguments, primary_table,
+                                                     calculate_name, join_tables)
+                setattr(calculate_expression, "syncany_valuer", ["$." + calculate_name])
+                if "where_schema" not in config:
+                    config["where_schema"] = {}
+                config["where_schema"][calculate_name] = copy.deepcopy(config["schema"][calculate_name])
+                return calculate_expression
+            if not self.is_calculate(calculate_expression, config, arguments):
+                return calculate_expression
+            for _, child_expression in calculate_expression.args.items():
+                if isinstance(child_expression, list):
+                    for child_expression_item in child_expression:
+                        parse_calucate(child_expression_item)
+                else:
+                    parse_calucate(child_expression)
+            return calculate_expression
 
         def parse(expression):
-            if expression.args.get("query"):
-                table_expression, value_expression = expression.args["this"], expression.args["query"]
-            elif expression.args.get("expressions"):
-                table_expression, value_expression = expression.args["this"], expression.args["expressions"]
-            elif isinstance(expression.args["expression"], sqlglot_expressions.Subquery):
-                table_expression, value_expression = expression.args["this"], expression.args["expression"].args["this"]
+            is_query_column, left_column, left_calculater = False, None, None
+            if expression.args.get("expressions"):
+                left_expression, right_expression = expression.args["this"], expression.args["expressions"]
+            elif expression.args.get("query"):
+                left_expression, right_expression = expression.args["this"], expression.args["query"]
             else:
-                table_expression, value_expression = expression.args["this"], expression.args["expression"]
-            if not self.is_column(table_expression, config, arguments):
-                raise SyncanySqlCompileException('unknown where condition, related sql "%s"' % self.to_sql(expression))
-            condition_table = table_expression.args["table"].name if "table" in table_expression.args else None
-            if condition_table and condition_table != primary_table["table_name"]:
-                raise SyncanySqlCompileException('error where condition, Only the primary table query conditions can be added, related sql "%s"'
-                                                 % self.to_sql(expression))
+                left_expression, right_expression = expression.args["this"], expression.args["expression"]
+            if self.is_column(left_expression, config, arguments):
+                left_column = self.parse_column(left_expression, config, arguments)
+                if is_query_condition and (left_column["table_name"] and primary_table["table_alias"] == left_column["table_name"]) \
+                        or not left_column["table_name"]:
+                    is_query_column = True
+            if not is_query_column:
+                if not isinstance(config["schema"], dict):
+                    raise SyncanySqlCompileException(
+                        'error where condition, only "=,!=,>,>=,<,<=,in" operations executed by the database cannot be transparently transmitted,'
+                        ' and it is executed with the having statement, column unkown, related sql "%s"'
+                        % self.to_sql(expression))
+                left_calculater = self.compile_calculate(parse_calucate(left_expression), config, arguments,
+                                                         primary_table, [])
 
-            condition_column = self.parse_column(table_expression, config, arguments)
-            if isinstance(value_expression, (sqlglot_expressions.Select, sqlglot_expressions.Subquery, sqlglot_expressions.Union)):
-                value_column = self.compile_query_condition(value_expression, config, arguments, primary_table,
-                                                            condition_column["typing_filters"])
-                if isinstance(expression, sqlglot_expressions.In):
-                    value_column = ["@convert_array", value_column]
-                else:
-                    value_column = ["@convert_array", value_column, ":$.:0"]
-            elif isinstance(value_expression, list):
-                value_column = []
-                for value_expression_item in value_expression:
+            if isinstance(right_expression, list):
+                value_items = []
+                for value_expression_item in right_expression:
                     if not self.is_const(value_expression_item, config, arguments):
-                        raise SyncanySqlCompileException('error where condition, array must be const value, related sql "%s"' % self.to_sql(expression))
-                    value_column.append(self.parse_const(value_expression_item, config, arguments)["value"])
-            else:
-                calculate_fields = []
-                self.parse_calculate(value_expression, config, arguments, primary_table, calculate_fields)
-                if calculate_fields:
-                    raise SyncanySqlCompileException('error where condition, the value of other tables when the query condition cannot, related sql "%s"'
-                                                     % self.to_sql(expression))
-                value_column = self.compile_calculate(value_expression, config, arguments, primary_table, [])
-            if condition_column["typing_name"] not in config["querys"]:
-                config["querys"][condition_column["typing_name"]] = {}
-            return condition_column, value_column
+                        raise SyncanySqlCompileException('error where condition, array must be const value, related sql "%s"'
+                                                         % self.to_sql(expression))
+                    value_items.append(self.parse_const(value_expression_item, config, arguments)["value"])
+                return is_query_column, left_column, left_calculater, value_items
+            if self.is_column(right_expression, config, arguments):
+                if not isinstance(config["schema"], dict):
+                    raise SyncanySqlCompileException(
+                        'error where condition, only "=,!=,>,>=,<,<=,in" operations executed by the database cannot be transparently transmitted,'
+                        ' and it is executed with the having statement, column unkown, related sql "%s"'
+                        % self.to_sql(expression))
+                if not left_calculater:
+                    left_calculater = self.compile_calculate(parse_calucate(left_expression), config, arguments, primary_table, [])
+                right_calculater = self.compile_calculate(parse_calucate(right_expression), config, arguments, primary_table, [])
+                return False, left_column, left_calculater, right_calculater
+            if isinstance(right_expression, (sqlglot_expressions.Select, sqlglot_expressions.Subquery, sqlglot_expressions.Union)):
+                value_column = self.compile_query_condition(right_expression, config, arguments, primary_table,
+                                                            left_column["typing_filters"] if left_column else None)
+                if isinstance(expression, sqlglot_expressions.In):
+                    return is_query_column, left_column, left_calculater, ["@convert_array", value_column]
+                return is_query_column, left_column, left_calculater, ["@convert_array", value_column, ":$.:0"]
+            calculate_fields = []
+            self.parse_calculate(right_expression, config, arguments, primary_table, calculate_fields)
+            if is_query_column and not calculate_fields:
+                return (is_query_column, left_column, left_calculater,
+                        self.compile_calculate(parse_calucate(right_expression), config, arguments, primary_table, []))
+            if not isinstance(config["schema"], dict):
+                raise SyncanySqlCompileException(
+                    'error where condition, only "=,!=,>,>=,<,<=,in" operations executed by the database cannot be transparently transmitted,'
+                    ' and it is executed with the having statement, column must be in the query result, related sql "%s"'
+                    % self.to_sql(expression))
+            if not left_calculater:
+                left_calculater = self.compile_calculate(parse_calucate(left_expression), config, arguments,
+                                                      primary_table, [])
+            right_calculater = self.compile_calculate(parse_calucate(right_expression), config, arguments,
+                                                      primary_table, [])
+            return False, left_column, left_calculater, right_calculater
 
         if isinstance(expression, sqlglot_expressions.EQ):
-            condition_column, value_column = parse(expression)
-            config["querys"][condition_column["typing_name"]]["=="] = value_column
+            is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
+            if is_query_condition and is_query_column:
+                if condition_column["typing_name"] not in config["querys"]:
+                    config["querys"][condition_column["typing_name"]] = {}
+                config["querys"][condition_column["typing_name"]]["=="] = right_calculater
+                return None
+            return ["@eq", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.NEQ):
-            condition_column, value_column = parse(expression)
-            config["querys"][condition_column["typing_name"]]["!="] = value_column
+            is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
+            if is_query_condition and is_query_column:
+                if condition_column["typing_name"] not in config["querys"]:
+                    config["querys"][condition_column["typing_name"]] = {}
+                config["querys"][condition_column["typing_name"]]["!="] = right_calculater
+                return None
+            return ["@neq", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.GT):
-            condition_column, value_column = parse(expression)
-            config["querys"][condition_column["typing_name"]][">"] = value_column
+            is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
+            if is_query_condition and is_query_column:
+                if condition_column["typing_name"] not in config["querys"]:
+                    config["querys"][condition_column["typing_name"]] = {}
+                config["querys"][condition_column["typing_name"]][">"] = right_calculater
+                return None
+            return ["@gt", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.GTE):
-            condition_column, value_column = parse(expression)
-            config["querys"][condition_column["typing_name"]][">="] = value_column
+            is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
+            if is_query_condition and is_query_column:
+                if condition_column["typing_name"] not in config["querys"]:
+                    config["querys"][condition_column["typing_name"]] = {}
+                config["querys"][condition_column["typing_name"]][">="] = right_calculater
+                return None
+            return ["@gte", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.LT):
-            condition_column, value_column = parse(expression)
-            config["querys"][condition_column["typing_name"]]["<"] = value_column
+            is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
+            if is_query_condition and is_query_column:
+                if condition_column["typing_name"] not in config["querys"]:
+                    config["querys"][condition_column["typing_name"]] = {}
+                config["querys"][condition_column["typing_name"]]["<"] = right_calculater
+                return None
+            return ["@lt", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.LTE):
-            condition_column, value_column = parse(expression)
-            config["querys"][condition_column["typing_name"]]["<="] = value_column
+            is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
+            if is_query_condition and is_query_column:
+                if condition_column["typing_name"] not in config["querys"]:
+                    config["querys"][condition_column["typing_name"]] = {}
+                config["querys"][condition_column["typing_name"]]["<="] = right_calculater
+                return None
+            return ["@lte", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.In):
-            condition_column, value_column = parse(expression)
-            config["querys"][condition_column["typing_name"]]["in"] = value_column
+            is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
+            if is_query_condition and is_query_column:
+                if condition_column["typing_name"] not in config["querys"]:
+                    config["querys"][condition_column["typing_name"]] = {}
+                config["querys"][condition_column["typing_name"]]["in"] = ["@convert_array", right_calculater]
+                return None
+            return ["@in", left_calculater, ["@convert_array", right_calculater]]
+        elif isinstance(expression, sqlglot_expressions.Like):
+            is_query_condition = False
+            is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
+            if not isinstance(right_calculater, list) or len(right_calculater) != 2 or right_calculater[0] != "#const":
+                raise SyncanySqlCompileException(
+                    'error having condition, like condition value must be const, related sql "%s"'
+                    % self.to_sql(expression))
+            return ["#if", ["@re::match", right_calculater[1].replace("%", ".*").replace(".*.*", "%"), left_calculater],
+                    ["#const", True], ["#const", False]]
+        elif isinstance(expression, (sqlglot_expressions.Not, sqlglot_expressions.Is)):
+            return self.compile_calculate(parse_calucate(expression), config, arguments, primary_table, [])
+        elif isinstance(expression, sqlglot_expressions.Paren):
+            return self.compile_where_condition(expression.args.get("this"), config, arguments, primary_table, join_tables, False)
         else:
-            raise SyncanySqlCompileException('error where condition, only "=,!=,>,>=,<,<=,in" operations are supported, related sql "%s"'
+            raise SyncanySqlCompileException('unknown where condition, only "=,!=,>,>=,<,<=,in" operations are supported, related sql "%s"'
                                              % self.to_sql(expression))
 
     def compile_query_condition(self, expression, config, arguments, primary_table, typing_filters):
         if isinstance(expression, sqlglot_expressions.Select):
             select_expressions = expression.args.get("expressions")
             if not select_expressions or len(select_expressions) != 1 or \
                     (not isinstance(select_expressions[0], sqlglot_expressions.Alias) and
@@ -750,15 +865,15 @@
         else:
             column_info = self.parse_column(select_expressions[0], config, arguments)
         if column_info["typing_filters"] and typing_filters:
             column_info["typing_filters"] = typing_filters
         querys = {"querys": {}}
         where_expression = expression.args.get("where")
         if where_expression and isinstance(where_expression, sqlglot_expressions.Where):
-            self.compile_where_condition(where_expression.args["this"], querys, arguments, primary_table)
+            self.compile_where_condition(where_expression.args["this"], querys, arguments, primary_table, [])
             self.parse_condition_typing_filter(expression, querys, arguments)
         db_table = "&." + table_info["db"] + "." + table_info["name"] + "::" + column_info["column_name"]
         if querys.get("querys"):
             return [[db_table, querys["querys"]], self.compile_column(select_expressions[0], config, arguments, column_info)]
         return [db_table, self.compile_column(select_expressions[0], config, arguments, column_info)]
 
     def compile_group_column(self, expression, config, arguments, primary_table, join_tables):
@@ -860,15 +975,15 @@
                 aggregate_calculate, reduce_calculate, final_calculate = self.compile_aggregate_calculate(aggregate_expressions[i])
                 value_column[1][aggregate_value_key] = aggregate_value_column
                 calculate_column[1][aggregate_value_key] = [aggregate_calculate, "$." + column_alias + "." + aggregate_value_key,
                                                                       "$$.value." + aggregate_value_key]
                 reduce_column[1][aggregate_value_key] = [reduce_calculate,
                                                                    "$." + column_alias + "." + aggregate_value_key,
                                                                    "$$." + column_alias + "." + aggregate_value_key]
-                setattr(aggregate_expressions[i], "final_column",
+                setattr(aggregate_expressions[i], "syncany_valuer",
                         [final_calculate, "$." + column_alias + "." + aggregate_value_key]
                         if final_calculate else ("$." + column_alias + "." + aggregate_value_key))
             self.compile_select_calculate_column(expression, config, arguments, primary_table, column_alias, join_tables)
             aggregate_column = {
                 "key": group_column,
                 "value": value_column,
                 "calculate": calculate_column,
@@ -967,16 +1082,16 @@
                         ("@" + calculater_name + "::final_value" if hasattr(aggregate_calculater, "final_value") else None))
             except CalculaterUnknownException:
                 raise SyncanySqlCompileException('unknown aggregate calculate, related sql "%s"' % self.to_sql(expression))
         else:
             raise SyncanySqlCompileException('unknown aggregate calculate, related sql "%s"' % self.to_sql(expression))
         
     def compile_calculate(self, expression, config, arguments, primary_table, column_join_tables, join_index=-1):
-        if self.is_aggregate(expression, config, arguments) and hasattr(expression, "final_column"):
-            return expression.final_column
+        if hasattr(expression, "syncany_valuer"):
+            return expression.syncany_valuer
         if isinstance(expression, sqlglot_expressions.Neg):
             return ["@neg", self.compile_calculate(expression.args["this"], config, arguments, primary_table, 
                                                    column_join_tables, join_index)]
         elif isinstance(expression, sqlglot_expressions.Anonymous):
             calculater_name = expression.args["this"].lower()
             if calculater_name == "get_value":
                 get_value_expressions = expression.args.get("expressions")
@@ -1289,17 +1404,14 @@
             sort_keys.append((column["column_name"], True if order_expression.args["desc"] else False))
         if sort_keys and len(primary_sort_keys) < len(sort_keys):
             if isinstance(config["schema"], dict):
                 for sort_key, _ in sort_keys:
                     if sort_key not in config["schema"]:
                         raise SyncanySqlCompileException('unknown order by column, related sql "%s"' % self.to_sql(expression))
             config["pipelines"].append([">>@sort", "$.*|array", False, sort_keys])
-            if "@limit" in arguments and arguments["@limit"] > 0:
-                config["pipelines"].append([">>@array::slice", "$.*|array", 0, arguments["@limit"]])
-                arguments["@limit"] = 0
         if primary_sort_keys:
             config["orders"].extend(primary_sort_keys)
         
     def compile_column(self, expression, config, arguments, column, scope_depth=1):
         if column["typing_filters"]:
             typing_filter_column = ("$" * scope_depth) + "." + column["column_name"] + "|" + column["typing_filters"][0]
             if len(column["typing_filters"]) == 1:
@@ -1494,15 +1606,15 @@
                 join_table["querys"][condition_column["typing_name"]] = {}
             join_table["querys"][condition_column["typing_name"]]["in"] = value_column
         else:
             raise SyncanySqlCompileException('error join on condition, only "=,!=,>,>=,<,<=,in" operations are supported, related sql "%s"'
                                              % self.to_sql(expression))
 
     def parse_calculate(self, expression, config, arguments, primary_table, calculate_fields):
-        if self.is_aggregate(expression, config, arguments) and hasattr(expression, "final_column"):
+        if hasattr(expression, "syncany_valuer"):
             return
         if isinstance(expression, sqlglot_expressions.Anonymous):
             for arg_expression in expression.args.get("expressions", []):
                 self.parse_calculate(arg_expression, config, arguments, primary_table, calculate_fields)
         elif isinstance(expression, sqlglot_expressions.Cast):
             self.parse_calculate(expression.args["this"], config, arguments, primary_table, calculate_fields)
         elif isinstance(expression, sqlglot_expressions.If):
@@ -1552,15 +1664,19 @@
 
     def parse_aggregate(self, expression, config, arguments, aggregate_expressions):
         if self.is_aggregate(expression, config, arguments):
             aggregate_expressions.append(expression)
         if not self.is_calculate(expression, config, arguments):
             return
         for _, child_expression in expression.args.items():
-            self.parse_aggregate(child_expression, config, arguments, aggregate_expressions)
+            if isinstance(child_expression, list):
+                for child_expression_item in child_expression:
+                    self.parse_aggregate(child_expression_item, config, arguments, aggregate_expressions)
+            else:
+                self.parse_aggregate(child_expression, config, arguments, aggregate_expressions)
 
     def parse_table(self, expression, config, arguments):
         db_name = expression.args["db"].name if "db" in expression.args and expression.args["db"] else None
         if isinstance(expression.args["this"], sqlglot_expressions.Dot):
             def parse(expression):
                 return (parse(expression.args["this"]) if isinstance(expression.args["this"],
                                                                      sqlglot_expressions.Dot) else expression.args["this"].name) \
```

### Comparing `syncanysql-0.1.1/syncanysql/config.py` & `syncanysql-0.1.2/syncanysql/config.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/executor.py` & `syncanysql-0.1.2/syncanysql/executor.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/main.py` & `syncanysql-0.1.2/syncanysql/main.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/parser.py` & `syncanysql-0.1.2/syncanysql/parser.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/prompt.py` & `syncanysql-0.1.2/syncanysql/prompt.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/taskers/delete.py` & `syncanysql-0.1.2/syncanysql/taskers/delete.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/taskers/execute.py` & `syncanysql-0.1.2/syncanysql/taskers/execute.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/taskers/explain.py` & `syncanysql-0.1.2/syncanysql/taskers/explain.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/taskers/into.py` & `syncanysql-0.1.2/syncanysql/taskers/into.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/taskers/query.py` & `syncanysql-0.1.2/syncanysql/taskers/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,20 +28,20 @@
         self.config = config
         self.batch = batch
         self.aggregate = aggregate
         self.count = 0
         self.batch_count = 0
 
     def outputed(self, tasker, datas):
-        self.count += len(datas)
-        self.batch_count += 1
-        if self.batch > 0 and self.count >= self.batch:
+        if self.batch > 0 and self.count > 0 and self.count + len(datas) >= self.batch:
             self.count, self.batch_count = 0, 1
             self.tasker.run_reduce(self.executor, self.session_config, self.manager, self.arguments, False)
         else:
+            self.count += len(datas)
+            self.batch_count += 1
             limit = tasker.arguments["@limit"] if "@limit" in tasker.arguments and tasker.arguments["@limit"] > 0 else 0
             if 0 < limit <= tasker.status["store_count"]:
                 self.count, self.batch_count = 0, 1
                 self.tasker.run_reduce(self.executor, self.session_config, self.manager, self.arguments, False)
 
     def finaled(self, tasker, e=None):
         if e is not None or self.batch_count <= 1:
@@ -60,62 +60,65 @@
         self.arguments = None
         self.tasker_generator = None
         self.updaters = []
         self.temporary_memory_collections = set([])
         self.run_start_time = 0
 
     def start(self, name, executor, session_config, manager, arguments):
-        dependency_taskers, aggregate = [], self.config.pop("aggregate", None)
+        dependency_taskers, where_schema, aggregate = [], self.config.get("where_schema", None), self.config.pop("aggregate", None)
         if aggregate and aggregate.get("distinct_keys"):
-            self.config, distinct_config = self.compile_distinct_config(aggregate), self.config
+            self.config, distinct_config = self.compile_distinct_config(where_schema, aggregate), self.config
             distinct_config["name"] = distinct_config["name"] + "#select@distinct"
             distinct_tasker = QueryTasker(distinct_config)
             distinct_tasker.start(name, executor, session_config, manager, copy.deepcopy(arguments))
             dependency_taskers.append(distinct_tasker)
-            arguments["@limit"], arguments["@batch"] = 0, 0
-            arguments["@primary_order"] = False
+            arguments["@limit"] = 0
 
         for dependency_config in self.config.get("dependencys", []):
             kn, knl = (dependency_config["name"] + "@"), len(dependency_config["name"] + "@")
             dependency_arguments = {}
             for key, value in arguments.items():
                 if key[:knl] != kn:
                     continue
                 dependency_arguments[key[knl:]] = value
                 dependency_arguments.pop(key, None)
             dependency_tasker = QueryTasker(dependency_config)
             dependency_tasker.start(name, executor, session_config, manager, dependency_arguments)
             dependency_taskers.append(dependency_tasker)
 
+        where_schema = self.config.pop("where_schema", None)
         limit, batch = int(arguments.get("@limit", 0)), int(arguments.get("@batch", 0))
         require_reduce, reduce_intercept, sorted_limit = False, False, len(self.config.get("pipelines", [])) == 2
         if self.config.get("intercepts"):
             if aggregate and aggregate.get("schema") and aggregate.get("having_columns"):
                 if [having_column for having_column in aggregate["having_columns"] if having_column in aggregate["schema"]]:
                     require_reduce, reduce_intercept = True, True
             if (batch > 0 or limit > 0 or sorted_limit):
                 require_reduce = True
         if aggregate and aggregate.get("schema"):
             if batch > 0 or limit > 0 or sorted_limit:
                 require_reduce = True
             elif [aggregate_column["final_value"] for aggregate_column in aggregate["schema"].values()
                   if aggregate_column["final_value"]]:
                 require_reduce = True
+        if where_schema:
+            require_reduce = True
         if require_reduce and isinstance(self.config["schema"], dict) and not arguments.get("@streaming"):
-            if limit > 0 and batch <= 0:
-                batch = min(max(*(int(arguments.get(key, 0)) for key in ("@limit", "@batch", "@join_batch"))), 1000)
-                arguments["@batch"] = batch
             if not aggregate:
                 aggregate = copy.deepcopy(DEAULT_AGGREGATE)
-            self.compile_reduce_config(aggregate)
+            self.compile_reduce_config(where_schema, aggregate)
             if reduce_intercept:
-                self.reduce_config["intercepts"] = self.config.pop("intercepts", [])
+                intercepts = self.config.pop("intercepts", [])
+                self.config["intercepts"], self.reduce_config["intercepts"] = intercepts[:1], intercepts[1:]
             self.reduce_config["pipelines"] = self.config.pop("pipelines", [])
         elif 0 < limit < batch:
             arguments["@batch"] = limit
+        if "intercepts" in self.config:
+            self.config["intercepts"] = [intercept for intercept in self.config["intercepts"] if
+                                         intercept != ["#const", True]]
         tasker = CoreTasker(self.config, manager)
         if "#" not in tasker.config["name"]:
             tasker.config["name"] = tasker.config["name"] + "#select"
         if self.reduce_config and "_aggregate_key_" in self.reduce_config["schema"]:
             tasker.add_hooker(ReduceHooker(executor, session_config, manager, arguments,
                                            self, copy.deepcopy(self.config), batch, aggregate))
         arguments = self.compile_tasker(arguments, tasker)
@@ -182,15 +185,15 @@
 
     def terminate(self):
         if not self.tasker:
             return
         self.tasker.terminate()
         self.tasker = None
 
-    def compile_distinct_config(self, aggregate):
+    def compile_distinct_config(self, where_schema, aggregate):
         subquery_name = "__subquery_" + str(uuid.uuid1().int) + "_distinct"
         config = copy.deepcopy(self.config)
         config.pop("loader", None)
         config.pop("loader_arguments", None)
         config.update({
             "input": "&.--." + subquery_name + "::" + self.config["output"].split("::")[-1].split(" ")[0],
             "output": self.config["output"],
@@ -223,41 +226,49 @@
                 self.config["schema"][key] = ["#make", {
                     "key": group_column,
                     "value": aggregate["schema"][key]["value"]
                 }, aggregate["schema"][key]["aggregate"]]
                 distinct_aggregate["schema"][key] = copy.deepcopy(aggregate["schema"][key])
                 distinct_aggregate["schema"][key]["final_value"] = None
                 config["schema"][key] = ["#aggregate", "$._aggregate_distinct_key_", aggregate["schema"][key]["reduce"]]
+            elif where_schema and key in where_schema:
+                continue
             else:
                 config["schema"][key] = "$." + key
 
         if aggregate["key"]:
             self.config["schema"]["_aggregate_distinct_key_"] = aggregate["key"]
+            aggregate["key"] = "$._aggregate_distinct_key_"
         self.config["schema"]["_aggregate_distinct_aggregate_key_"] = ["#aggregate", group_column, ["#const", 0]]
         distinct_aggregate["key"] = group_column
         distinct_aggregate["schema"]["_aggregate_distinct_aggregate_key_"] = {
             "key": group_column,
             "value": ["#const", 0],
             "calculate": ["#const", 0],
             "aggregate": [":#aggregate", "$.key", ["#const", 0]],
             "reduce": ["#const", 0],
             "final_value": None
         }
         self.config["aggregate"] = distinct_aggregate
         if [having_column for having_column in aggregate["having_columns"] if having_column in aggregate["schema"]]:
-            config["intercepts"] = self.config.pop("intercepts", [])
+            intercepts = self.config.pop("intercepts", [])
+            if intercepts and len(intercepts) >= 1:
+                self.config["intercepts"] = [intercepts[0], ["#const", True]]
+            if intercepts and len(intercepts) >= 2:
+                config["intercepts"] = [["#const", True], intercepts[1]]
         else:
             distinct_aggregate["having_columns"] = aggregate["having_columns"]
+        config.pop("where_schema", None)
         config["pipelines"] = self.config.pop("pipelines", [])
         self.config["output"] = "&.--." + subquery_name + "::" + self.config["output"].split("::")[-1].split(" ")[0] + " use I"
         self.config.pop("outputer", None)
         self.config.pop("outputer_arguments", None)
         return config
 
-    def compile_reduce_config(self, aggregate):
+    def compile_reduce_config(self, where_schema, aggregate):
         subquery_name = "__subquery_" + str(uuid.uuid1().int) + "_reduce"
         config = copy.deepcopy(self.config)
         config.pop("loader", None)
         config.pop("loader_arguments", None)
         config.update({
             "input": "&.--." + subquery_name + "::" + self.config["output"].split("::")[-1].split(" ")[0],
             "output": self.config["output"],
@@ -280,37 +291,44 @@
                 config["schema"][key] = ["#aggregate", "$._aggregate_key_", aggregate["schema"][key]["reduce"]]
             else:
                 config["schema"][key] = "$." + key
         if aggregate["key"]:
             config["schema"]["_aggregate_key_"] = "$._aggregate_key_"
             self.config["schema"]["_aggregate_key_"] = aggregate["key"]
         config["aggregate"] = aggregate
+        config["where_schema"] = where_schema
         self.config["output"] = "&.--." + subquery_name + "::" + self.config["output"].split("::")[-1].split(" ")[0] + " use I"
         self.config.pop("outputer", None)
         self.config.pop("outputer_arguments", None)
         self.reduce_config = config
 
     def run_reduce(self, executor, session_config, manager, arguments, final_reduce=False):
         config, arguments = copy.deepcopy(self.reduce_config), copy.deepcopy(arguments)
+        where_schema, aggregate = config.pop("where_schema", None), config.pop("aggregate", None)
         if final_reduce:
             config["schema"].pop("_aggregate_key_", None)
+            if where_schema:
+                for key in where_schema:
+                    config.pop(key, None)
             for key, column in config["schema"].items():
-                if key in config["aggregate"]["schema"] and config["aggregate"]["schema"][key]["final_value"]:
-                    config["schema"][key] = config["aggregate"]["schema"][key]["final_value"]
+                if key in aggregate["schema"] and aggregate["schema"][key]["final_value"]:
+                    config["schema"][key] = aggregate["schema"][key]["final_value"]
                 else:
                     config["schema"][key] = "$." + key
             config["name"] = config["name"] + "#select@final_reduce"
         else:
             config["output"] = config["input"] + " use DI"
             config["name"] = config["name"] + "#select@reduce"
             config["intercepts"] = []
             config["pipelines"] = []
+        if "intercepts" in config:
+            config["intercepts"] = [intercept for intercept in config["intercepts"] if
+                                    intercept != ["#const", True]]
         tasker = CoreTasker(config, manager)
         arguments["@primary_order"] = False
-        arguments["@batch"] = 0
         arguments["@limit"] = 0
         self.compile_tasker(arguments, tasker)
         tasker_generator = self.run_tasker(executor, session_config, manager, tasker, [])
         while True:
             try:
                 tasker_generator.send(None)
             except StopIteration as e:
@@ -323,14 +341,19 @@
         return 0
 
     def compile_tasker(self, arguments, tasker):
         tasker.load()
         compile_arguments = {}
         compile_arguments.update({key.lower(): value for key, value in os.environ.items()})
         compile_arguments.update(arguments)
+        if self.is_local_memory_database(tasker.config):
+            if isinstance(tasker.config["input"], str) and "&.--." in tasker.config["input"]:
+                compile_arguments["@batch"] = 0
+            if isinstance(tasker.config["output"], str) and "&.--." in tasker.config["output"]:
+                compile_arguments["@insert_batch"] = 0
 
         tasker.compile(compile_arguments)
         if "@verbose" in compile_arguments and compile_arguments["@verbose"]:
             warp_database_logging(tasker)
 
         if hasattr(tasker.outputer, "name"):
             if tasker.outputer.name.startswith("--.__subquery_") or tasker.outputer.name.startswith("--.__unionquery_"):
@@ -393,7 +416,15 @@
             dependency_tasker.execute_updater(executor, session_config, manager)
 
     def get_temporary_memory_collections(self):
         names = list(self.temporary_memory_collections)
         for dependency_tasker in self.dependency_taskers:
             names.extend(dependency_tasker.get_temporary_memory_collections())
         return names
+
+    def is_local_memory_database(self, config, name="--"):
+        try:
+            database_config = dict(**[database for database in config["databases"]
+                                      if database["name"] == name][0])
+            return database_config["driver"] == "memory"
+        except (TypeError, KeyError, IndexError):
+            return False
```

### Comparing `syncanysql-0.1.1/syncanysql/taskers/set.py` & `syncanysql-0.1.2/syncanysql/taskers/set.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/taskers/show.py` & `syncanysql-0.1.2/syncanysql/taskers/show.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/taskers/use.py` & `syncanysql-0.1.2/syncanysql/taskers/use.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql/utils.py` & `syncanysql-0.1.2/syncanysql/utils.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.1/syncanysql.egg-info/PKG-INFO` & `syncanysql-0.1.2/syncanysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
```

### Comparing `syncanysql-0.1.1/syncanysql.egg-info/SOURCES.txt` & `syncanysql-0.1.2/syncanysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

