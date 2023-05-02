# Comparing `tmp/dongwha_datalab-0.0.0.7-py3-none-any.whl.zip` & `tmp/dongwha_datalab-0.0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5692 bytes, number of entries: 7
+Zip file size: 5693 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       29 b- defN 23-May-02 02:09 data_lab/__init__.py
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-14 06:58 data_lab/data_lab.py
--rw-rw-rw-  2.0 fat    16789 b- defN 23-May-02 04:13 data_lab/mlops.py
--rw-rw-rw-  2.0 fat      414 b- defN 23-May-02 05:31 dongwha_datalab-0.0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 05:31 dongwha_datalab-0.0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-02 05:31 dongwha_datalab-0.0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      561 b- defN 23-May-02 05:31 dongwha_datalab-0.0.0.7.dist-info/RECORD
-7 files, 17947 bytes uncompressed, 4688 bytes compressed:  73.9%
+-rw-rw-rw-  2.0 fat    16790 b- defN 23-May-02 06:17 data_lab/mlops.py
+-rw-rw-rw-  2.0 fat      414 b- defN 23-May-02 06:18 dongwha_datalab-0.0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 06:18 dongwha_datalab-0.0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-02 06:18 dongwha_datalab-0.0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      561 b- defN 23-May-02 06:18 dongwha_datalab-0.0.0.8.dist-info/RECORD
+7 files, 17948 bytes uncompressed, 4689 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: data_lab/data_lab.py
 Comment: 
 
 Filename: data_lab/mlops.py
 Comment: 
 
-Filename: dongwha_datalab-0.0.0.7.dist-info/METADATA
+Filename: dongwha_datalab-0.0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: dongwha_datalab-0.0.0.7.dist-info/WHEEL
+Filename: dongwha_datalab-0.0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: dongwha_datalab-0.0.0.7.dist-info/top_level.txt
+Filename: dongwha_datalab-0.0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: dongwha_datalab-0.0.0.7.dist-info/RECORD
+Filename: dongwha_datalab-0.0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## data_lab/mlops.py

```diff
@@ -303,15 +303,15 @@
         
         # return step function value 
         insert_info['init']['tar_to_s3_bucket'] = bucket
         insert_info['init']['tar_to_s3_file_path'] = script_path
         
         
         insert_info['init']['script_ver'] = script_ver
-        insert_info['init']['sourcedir_train_path']     = "/{0}/{1}".format( sourcedir_train_path, config['train_local_script_path'].split('/')[-1] )
+        insert_info['init']['sourcedir_train_path']     = "./{0}/{1}".format( sourcedir_train_path, config['train_local_script_path'].split('/')[-1] )
         insert_info['init']['sagemaker_model_id']       = '{0}-{1}-{2}-{3}'.format( model_name, create_date, create_time, create_millisecond )
         insert_info['init']['bucket']                   = bucket
         insert_info['init']['======']                   = "###############추출###############"
         insert_info['init']['script_path']              = '{0}/script/{1}/{2}'.format( environment, model_name, str(script_ver) ) 
         insert_info['init']['extract_script_path']      =  config['extract_local_script_path'].split('/')[-1]
         insert_info['init']['transform_script_path']    =  config['transform_local_script_path'].split('/')[-1]
         insert_info['init']['create_model_script_path'] =  config['train_local_script_path'].split('/')[-1]
```

