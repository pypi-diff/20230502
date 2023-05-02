# Comparing `tmp/qtex-0.0.1.tar.gz` & `tmp/qtex-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtex-0.0.1.tar", last modified: Tue May  2 02:06:42 2023, max compression
+gzip compressed data, was "qtex-0.0.3.tar", last modified: Tue May  2 02:51:26 2023, max compression
```

## Comparing `qtex-0.0.1.tar` & `qtex-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:06:42.554689 qtex-0.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:03:44.000000 qtex-0.0.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-05-02 02:06:42.554689 qtex-0.0.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:06:42.550689 qtex-0.0.1/qtex/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:19:14.000000 qtex-0.0.1/qtex/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:06:42.554689 qtex-0.0.1/qtex/jq/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:19:37.000000 qtex-0.0.1/qtex/jq/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:06:42.554689 qtex-0.0.1/qtex/jq/etl/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:54:50.000000 qtex-0.0.1/qtex/jq/etl/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2394 2023-05-02 02:01:48.000000 qtex-0.0.1/qtex/jq/etl/persist_ext.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1899 2023-05-02 01:56:55.000000 qtex-0.0.1/qtex/jq/persist_ext.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:06:42.554689 qtex-0.0.1/qtex/jq/sync/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:58:58.000000 qtex-0.0.1/qtex/jq/sync/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1674 2023-05-02 02:02:32.000000 qtex-0.0.1/qtex/jq/sync/position.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      679 2023-05-02 01:57:10.000000 qtex-0.0.1/qtex/jq/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-02 02:04:25.000000 qtex-0.0.1/qtex/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:06:42.554689 qtex-0.0.1/qtex.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-05-02 02:06:42.000000 qtex-0.0.1/qtex.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      380 2023-05-02 02:06:42.000000 qtex-0.0.1/qtex.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-02 02:06:42.000000 qtex-0.0.1/qtex.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-02 02:06:42.000000 qtex-0.0.1/qtex.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2023-05-02 02:06:42.000000 qtex-0.0.1/qtex.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-02 02:06:42.000000 qtex-0.0.1/qtex.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-02 02:06:42.554689 qtex-0.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      682 2023-05-02 02:05:38.000000 qtex-0.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:51:26.019989 qtex-0.0.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:03:44.000000 qtex-0.0.3/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-05-02 02:51:26.019989 qtex-0.0.3/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:51:26.015989 qtex-0.0.3/qtex/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:19:14.000000 qtex-0.0.3/qtex/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:51:26.019989 qtex-0.0.3/qtex/jq/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:19:37.000000 qtex-0.0.3/qtex/jq/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:51:26.019989 qtex-0.0.3/qtex/jq/etl/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:54:50.000000 qtex-0.0.3/qtex/jq/etl/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2885 2023-05-02 02:44:39.000000 qtex-0.0.3/qtex/jq/etl/factor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1899 2023-05-02 01:56:55.000000 qtex-0.0.3/qtex/jq/persist_ext.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:51:26.019989 qtex-0.0.3/qtex/jq/sync/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:58:58.000000 qtex-0.0.3/qtex/jq/sync/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1880 2023-05-02 02:44:59.000000 qtex-0.0.3/qtex/jq/sync/position.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-05-02 02:43:45.000000 qtex-0.0.3/qtex/jq/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-02 02:51:10.000000 qtex-0.0.3/qtex/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:51:26.019989 qtex-0.0.3/qtex.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-05-02 02:51:25.000000 qtex-0.0.3/qtex.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      375 2023-05-02 02:51:26.000000 qtex-0.0.3/qtex.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-02 02:51:25.000000 qtex-0.0.3/qtex.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-02 02:06:42.000000 qtex-0.0.3/qtex.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-05-02 02:51:25.000000 qtex-0.0.3/qtex.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-02 02:51:25.000000 qtex-0.0.3/qtex.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-02 02:51:26.019989 qtex-0.0.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      698 2023-05-02 02:07:22.000000 qtex-0.0.3/setup.py
```

### Comparing `qtex-0.0.1/qtex/jq/etl/persist_ext.py` & `qtex-0.0.3/qtex/jq/etl/factor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import pandas as pd
+import jqfactor as jqf
+import qtc.utils.datetime_utils as dtu
+import qtc.utils.misc_utils as mu
 import qtex.jq.utils as jqu
 import logging
 logger = logging.getLogger()
 
 
 DATA_TYPE_CONFIG = dict()
 
 def persist_cne5(dateid, securities=None,
-                 **kwargs):
+                 **db_config):
     global DATA_TYPE_CONFIG
 
     datestr = dtu.dateid_to_datestr(dateid=dateid)
     if securities is None:
         securities = get_all_securities(types=['stock'], date=datestr)
         securities = securities.index.to_list()
     else:
@@ -30,25 +34,35 @@
     data = pd.concat([factor_data[fn].unstack().to_frame(fn) for fn in factor_data.keys()], axis=1)
     data.index.names = ['ts_code', 'trade_date']
     data.reset_index(inplace=True)
     data['trade_date'] = data['trade_date'].dt.strftime('%Y%m%d').astype(int)
     data['ts_code'] = data['ts_code'].apply(lambda x: x.replace('.XSHE', '.SZ').replace('.XSHG', 'SH'))
     logger.info(f'data.shape={data.shape}. Examples:\n{data.head()}')
 
-    user_d, password_d, database_d = \
-        DATA_TYPE_CONFIG.get('CNE5',
-                             (None, None, 'CN-EQUITY-VENDOR'))
-    if 'user' not in kwargs:
-        user = user_d
-    if 'password' not in kwargs:
-        password = password_d
-    if 'database' not in kwargs:
-        database = database_d
-
-    conn = jqu.get_conn(user=user, password=password, database=database)
+    # db_type_d, host_d, port_d, user_d, password_d, database_d = \
+    #     DATA_TYPE_CONFIG.get('CNE5',
+    #                          ('POSTGRES', None, None, None, None, None))
+    #
+    # db_type = kwargs.get('db_type', db_type_d)
+    # host = kwargs.get('host', host_d)
+    # port = kwargs.get('port', port_d)
+    # user = kwargs.get('user', user_d)
+    # password = kwargs.get('password', password_d)
+    # database = kwargs.get('database', database_d)
+    #
+    # conn = jqu.get_conn(
+    #     db_type=db_type,
+    #     host=host,
+    #     port=port,
+    #     user=user,
+    #     password=password,
+    #     database=database
+    # )
+    conn = jqu.get_conn_data_type(data_type='CNE5',
+                                  **db_config)
     schema = 'joinquant'
     table_name = 'CNE5'
     # upsert_method = dbu.create_upsert_method(db_code=database, schema=schema,
     #                                          extra_update_fields={'UpdateDateTime': "NOW()"})
 
     # conn.execute(f'DELETE FROM "{schema}"."{table_name}" WHERE "DateId"={dateid}')
     num_rows = data.to_sql(table_name,
```

### Comparing `qtex-0.0.1/qtex/jq/persist_ext.py` & `qtex-0.0.3/qtex/jq/persist_ext.py`

 * *Files identical despite different names*

### Comparing `qtex-0.0.1/setup.py` & `qtex-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,12 +20,13 @@
     install_requires=[
         'pandas>=1.3.4',
         'joblib',
         'sqlalchemy',
         'pymssql',
         'psycopg2',
         'pyyaml',
+        'qtc',
     ],
     tests_require=[
         'pytest'
     ],
 )
```

