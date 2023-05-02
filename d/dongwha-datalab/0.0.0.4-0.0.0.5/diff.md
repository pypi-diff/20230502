# Comparing `tmp/dongwha_datalab-0.0.0.4-py3-none-any.whl.zip` & `tmp/dongwha_datalab-0.0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5605 bytes, number of entries: 7
+Zip file size: 5602 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       29 b- defN 23-May-02 02:09 data_lab/__init__.py
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-14 06:58 data_lab/data_lab.py
--rw-rw-rw-  2.0 fat    16894 b- defN 23-May-02 03:59 data_lab/mlops.py
--rw-rw-rw-  2.0 fat      285 b- defN 23-May-02 04:00 dongwha_datalab-0.0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 04:00 dongwha_datalab-0.0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-02 04:00 dongwha_datalab-0.0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      561 b- defN 23-May-02 04:00 dongwha_datalab-0.0.0.4.dist-info/RECORD
-7 files, 17923 bytes uncompressed, 4601 bytes compressed:  74.3%
+-rw-rw-rw-  2.0 fat    16789 b- defN 23-May-02 04:13 data_lab/mlops.py
+-rw-rw-rw-  2.0 fat      285 b- defN 23-May-02 05:22 dongwha_datalab-0.0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 05:22 dongwha_datalab-0.0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-02 05:22 dongwha_datalab-0.0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      561 b- defN 23-May-02 05:22 dongwha_datalab-0.0.0.5.dist-info/RECORD
+7 files, 17818 bytes uncompressed, 4598 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: data_lab/data_lab.py
 Comment: 
 
 Filename: data_lab/mlops.py
 Comment: 
 
-Filename: dongwha_datalab-0.0.0.4.dist-info/METADATA
+Filename: dongwha_datalab-0.0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: dongwha_datalab-0.0.0.4.dist-info/WHEEL
+Filename: dongwha_datalab-0.0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: dongwha_datalab-0.0.0.4.dist-info/top_level.txt
+Filename: dongwha_datalab-0.0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: dongwha_datalab-0.0.0.4.dist-info/RECORD
+Filename: dongwha_datalab-0.0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## data_lab/mlops.py

```diff
@@ -68,18 +68,14 @@
 # In[3]:
 
 
 def mongodb_connection(  environment, collection_div, aws_access_key_id, aws_secret_access_key, ssm_path  ) : 
     
     
     print(  environment,  )
-    print(  aws_access_key_id,  )
-    print(  aws_secret_access_key,  )
-    print( ssm_path )
-    
     
     SSM_PATH = ssm_path.format(environment)
     print( SSM_PATH )
     CONN_INFO = get_ssm( SSM_PATH,  aws_access_key_id, aws_secret_access_key )
     MONGODB_HOST = CONN_INFO['host']
     MONGODB_PORT = CONN_INFO['port']
     DATABASE     = CONN_INFO['db_name']
@@ -188,15 +184,15 @@
                     user_image_config[key] = change_value
         user_image_config['deploy'] = True
         return user_image_config
 
 
 # # send_model_to_sagemaker():
 
-# In[1]:
+# In[15]:
 
 
 import boto3
 import tarfile
 import os.path
 import pymongo
 import datetime
@@ -307,25 +303,24 @@
         
         # return step function value 
         insert_info['init']['tar_to_s3_bucket'] = bucket
         insert_info['init']['tar_to_s3_file_path'] = script_path
         
         
         insert_info['init']['script_ver'] = script_ver
+        insert_info['init']['sourcedir_train_path']     = "/{0}/{1}".format( sourcedir_train_path, config['train_local_script_path'].split('/')[-1] )
         insert_info['init']['sagemaker_model_id']       = '{0}-{1}-{2}-{3}'.format( model_name, create_date, create_time, create_millisecond )
         insert_info['init']['bucket']                   = bucket
         insert_info['init']['======']                   = "###############추출###############"
         insert_info['init']['script_path']              = '{0}/script/{1}/{2}'.format( environment, model_name, str(script_ver) ) 
         insert_info['init']['extract_script_path']      =  config['extract_local_script_path'].split('/')[-1]
         insert_info['init']['transform_script_path']    =  config['transform_local_script_path'].split('/')[-1]
         insert_info['init']['create_model_script_path'] =  config['train_local_script_path'].split('/')[-1]
         insert_info['init']['endpoint_script_path']     =  config['endpoint_local_script_path'].split('/')[-1]
         
-        insert_info['init']['sourcedir_train_path'] =  "/{0}/{1}".format( sourcedir_train_path, config['train_local_script_path'].split('/')[-1] ) 
-        
         insert_info['init']['endp_name'] = config['endp_name']
         insert_info['init']['endp_config_mode'] = config['endp_config_mode']
         insert_info['init']['max_concurrency'] = config['max_concurrency']
         insert_info['init']['mem_size'] = config['mem_size']
         
 #         insert_info = config.copy()
```

## Comparing `dongwha_datalab-0.0.0.4.dist-info/RECORD` & `dongwha_datalab-0.0.0.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 data_lab/__init__.py,sha256=yTyPXIX49lH7Tm0VlJSswI5RsccKIyWXLqiMlYWfeA0,29
 data_lab/data_lab.py,sha256=VL85MuyDOhbHjMHO5kvwTtsJEYXuP1PBJNuK4M9Wsuo,53
-data_lab/mlops.py,sha256=LzNNyk31m7Na7Ibo09hZoIkIIPVvsip2csZxRCTttVM,16894
-dongwha_datalab-0.0.0.4.dist-info/METADATA,sha256=tybGNju3bXkfhevwbgwsRXj6YdQWik8IfESIyAoGUI8,285
-dongwha_datalab-0.0.0.4.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-dongwha_datalab-0.0.0.4.dist-info/top_level.txt,sha256=fabjZWKGTJaYtam2u8Sr7zSBLYZw5ux33pxUzJIVewc,9
-dongwha_datalab-0.0.0.4.dist-info/RECORD,,
+data_lab/mlops.py,sha256=VXmZLgcRKHdmjtQp5oh1hZGBLj1TwyGgUJOjkb05UeQ,16789
+dongwha_datalab-0.0.0.5.dist-info/METADATA,sha256=wgpdssL-0keX1jq9Sphd1uSbxcUy3YOsVTIJ4-EM2Gg,285
+dongwha_datalab-0.0.0.5.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+dongwha_datalab-0.0.0.5.dist-info/top_level.txt,sha256=fabjZWKGTJaYtam2u8Sr7zSBLYZw5ux33pxUzJIVewc,9
+dongwha_datalab-0.0.0.5.dist-info/RECORD,,
```

