# Comparing `tmp/VDBforGenAI-0.21-py3-none-any.whl.zip` & `tmp/VDBforGenAI-0.22-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 16513 bytes, number of entries: 19
--rw-rw-rw-  2.0 fat    23654 b- defN 23-May-01 20:48 VDBforGenAI/VectorDatabase.py
+Zip file size: 16546 bytes, number of entries: 19
+-rw-rw-rw-  2.0 fat    23807 b- defN 23-May-01 22:17 VDBforGenAI/VectorDatabase.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-24 23:14 VDBforGenAI/__init__.py
 -rw-rw-rw-  2.0 fat     1087 b- defN 23-May-01 20:42 VDBforGenAI/Utilities/Loading.py
 -rw-rw-rw-  2.0 fat     1189 b- defN 23-Apr-25 00:13 VDBforGenAI/Utilities/StringUtilities.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-22 19:05 VDBforGenAI/Utilities/__init__.py
 -rw-rw-rw-  2.0 fat     2847 b- defN 23-May-01 20:40 VDBforGenAI/VectorisationAndIndexCreation/SearchFunctions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-19 17:31 VDBforGenAI/VectorisationAndIndexCreation/__init__.py
 -rw-rw-rw-  2.0 fat    16353 b- defN 23-Apr-24 23:27 VectorDatabase/VectorDatabase.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-24 23:14 VectorDatabase/__init__.py
 -rw-rw-rw-  2.0 fat     1103 b- defN 23-Apr-22 19:09 VectorDatabase/Utilities/Loading.py
 -rw-rw-rw-  2.0 fat     1171 b- defN 23-Apr-23 13:57 VectorDatabase/Utilities/StringUtilities.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-22 19:05 VectorDatabase/Utilities/__init__.py
 -rw-rw-rw-  2.0 fat     2524 b- defN 23-Apr-20 00:19 VectorDatabase/VectorisationAndIndexCreation/SearchFunctions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-19 17:31 VectorDatabase/VectorisationAndIndexCreation/__init__.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-01 21:04 VDBforGenAI-0.21.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3155 b- defN 23-May-01 21:04 VDBforGenAI-0.21.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-01 21:04 VDBforGenAI-0.21.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-01 21:04 VDBforGenAI-0.21.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1744 b- defN 23-May-01 21:04 VDBforGenAI-0.21.dist-info/RECORD
-19 files, 56022 bytes uncompressed, 13577 bytes compressed:  75.8%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-01 22:17 VDBforGenAI-0.22.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3155 b- defN 23-May-01 22:17 VDBforGenAI-0.22.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-01 22:17 VDBforGenAI-0.22.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-01 22:17 VDBforGenAI-0.22.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1744 b- defN 23-May-01 22:17 VDBforGenAI-0.22.dist-info/RECORD
+19 files, 56175 bytes uncompressed, 13610 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: VectorDatabase/VectorisationAndIndexCreation/SearchFunctions.py
 Comment: 
 
 Filename: VectorDatabase/VectorisationAndIndexCreation/__init__.py
 Comment: 
 
-Filename: VDBforGenAI-0.21.dist-info/LICENSE
+Filename: VDBforGenAI-0.22.dist-info/LICENSE
 Comment: 
 
-Filename: VDBforGenAI-0.21.dist-info/METADATA
+Filename: VDBforGenAI-0.22.dist-info/METADATA
 Comment: 
 
-Filename: VDBforGenAI-0.21.dist-info/WHEEL
+Filename: VDBforGenAI-0.22.dist-info/WHEEL
 Comment: 
 
-Filename: VDBforGenAI-0.21.dist-info/top_level.txt
+Filename: VDBforGenAI-0.22.dist-info/top_level.txt
 Comment: 
 
-Filename: VDBforGenAI-0.21.dist-info/RECORD
+Filename: VDBforGenAI-0.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## VDBforGenAI/VectorDatabase.py

```diff
@@ -12,21 +12,22 @@
 import os
 from VDBforGenAI.Utilities.Loading import load_docx, load_pdf
 from transformers import DPRContextEncoder, DPRContextEncoderTokenizer
 
 
 class VectorDatabase:
     def __init__(self,
-                 encoder: Union[str, transformers.PreTrainedModel] = None,
+                 encoder: Union[str, transformers.PreTrainedModel, bool] = None,
                  tokenizer: Union[str, transformers.PreTrainedTokenizer] = None,
                  batch_size: int = 128,
                  splitting_choice: str = "length",
                  index_location: str = './index',
                  preload_index: bool = False,
-                 index_of_summarised_vector: int = 0
+                 index_of_summarised_vector: int = 0,
+                 hidden_size: int = False
                  ):
         """
 
         :param encoder: Transformer model from huggingface in torch, defaults to facebook/dpr-ctx_encoder-single-nq-base
         , can be given as model or string location or string huggingface repo, it has to have the property self.encoder.config.hidden_size
         :param tokenizer: Tokenizer of the above model, defaults to
         facebook/dpr-ctx_encoder-single-nq-base, can be a different location than the model
@@ -49,28 +50,31 @@
             self.load_index()
             self.index_loaded = True
         else:
             self.index_loaded = False
 
         # This instantiates the dictionary holding the levels and their possible values (usually based on folder structure of import)
         self.dlv = None
-        if encoder is not None:
+        if encoder is not None and encoder is not False:
             if encoder is str:
                 self.encoder = AutoModel.from_pretrained(encoder)
                 if tokenizer is None:
                     self.tokenizer = AutoTokenizer.from_pretrained(encoder)
                 elif tokenizer is str:
                     self.tokenizer = AutoTokenizer.from_pretrained(tokenizer)
             else:
                 self.encoder = encoder
                 self.tokenizer = tokenizer
         else:
             self.encoder = DPRContextEncoder.from_pretrained("facebook/dpr-ctx_encoder-single-nq-base")
             self.tokenizer = DPRContextEncoderTokenizer.from_pretrained("facebook/dpr-ctx_encoder-single-nq-base")
-        self.d = self.encoder.config.hidden_size
+        if hidden_size:
+            self.d = hidden_size
+        else:
+            self.d = self.encoder.config.hidden_size
 
         self.batch_size = batch_size
         self.splitting_choice = splitting_choice
 
     def reload_total_index(self):
         self.index = faiss.IndexFlatIP(self.d)
         self.index.add(self.list_of_context_vectors_flattened)
```

## Comparing `VDBforGenAI-0.21.dist-info/LICENSE` & `VDBforGenAI-0.22.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `VDBforGenAI-0.21.dist-info/METADATA` & `VDBforGenAI-0.22.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VDBforGenAI
-Version: 0.21
+Version: 0.22
 Summary: A simple package for generating and querying Vector Databases for Generative AI as well any other reason
 Home-page: https://github.com/JakubJDolezal/VDBforGenAI
 Author: Jakub Dolezal
 Author-email: jakubdolezal93@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `VDBforGenAI-0.21.dist-info/RECORD` & `VDBforGenAI-0.22.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-VDBforGenAI/VectorDatabase.py,sha256=oyAgfR8L_aWXxpw3bagu1bP0QcpI6xZKx_Uws4AdCuo,23654
+VDBforGenAI/VectorDatabase.py,sha256=0rhC3TWs3TZeq5xipqhNb6B7j2ekCD2Wri-efmT8KEQ,23807
 VDBforGenAI/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 VDBforGenAI/Utilities/Loading.py,sha256=noCEuxau81lGqvmdVTq9x1VZFH5f3RpE_SjP8HUvXzg,1087
 VDBforGenAI/Utilities/StringUtilities.py,sha256=KOscPd2U6S2Breg5dCkS2DaQZsjvqo3A8tXElfk5UTs,1189
 VDBforGenAI/Utilities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 VDBforGenAI/VectorisationAndIndexCreation/SearchFunctions.py,sha256=vKyRMDiTz8VitDBzsUXT1JNsOMN0tncYdVEOTkPuaSE,2847
 VDBforGenAI/VectorisationAndIndexCreation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 VectorDatabase/VectorDatabase.py,sha256=l6qP1Lwp8_Qf0lIClbp8-QUNq6MFFDdEjw-pdsvEgvs,16353
 VectorDatabase/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 VectorDatabase/Utilities/Loading.py,sha256=NXC2_PIQk0t5Msb5DBo445z6ImnPZmkaM8ine_wcvYY,1103
 VectorDatabase/Utilities/StringUtilities.py,sha256=OWT573n2Gt_79OHsLkLUch8WclKvY4ky2O4B4U9xNdk,1171
 VectorDatabase/Utilities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 VectorDatabase/VectorisationAndIndexCreation/SearchFunctions.py,sha256=bQhPPEEhegOlQUs-nGREvAneCunjAwcF5iunGz5MYNw,2524
 VectorDatabase/VectorisationAndIndexCreation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-VDBforGenAI-0.21.dist-info/LICENSE,sha256=XvXL9_dkYukNDtEFE1Sx0GChpa6Ejczjl8fhLdAnFXE,1091
-VDBforGenAI-0.21.dist-info/METADATA,sha256=ZCqtc1UevIo-P6xNo0HdEgHAQSa2GK0OkO8vabcftv0,3155
-VDBforGenAI-0.21.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-VDBforGenAI-0.21.dist-info/top_level.txt,sha256=gni5yin_KrggSq7r-iFVXjkFa8UWZUmcIvxx8-sUJ-w,12
-VDBforGenAI-0.21.dist-info/RECORD,,
+VDBforGenAI-0.22.dist-info/LICENSE,sha256=XvXL9_dkYukNDtEFE1Sx0GChpa6Ejczjl8fhLdAnFXE,1091
+VDBforGenAI-0.22.dist-info/METADATA,sha256=dududiTNwKx_OuGq7CAbPZU-7IPOIXE1GCKe8K5ztsc,3155
+VDBforGenAI-0.22.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+VDBforGenAI-0.22.dist-info/top_level.txt,sha256=gni5yin_KrggSq7r-iFVXjkFa8UWZUmcIvxx8-sUJ-w,12
+VDBforGenAI-0.22.dist-info/RECORD,,
```

