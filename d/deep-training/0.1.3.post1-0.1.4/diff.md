# Comparing `tmp/deep_training-0.1.3.post1-py3-none-any.whl.zip` & `tmp/deep_training-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 284262 bytes, number of entries: 162
+Zip file size: 310384 bytes, number of entries: 173
 -rw-rw-rw-  2.0 fat       47 b- defN 23-Apr-10 11:44 deep_training/__init__.py
--rw-rw-rw-  2.0 fat      911 b- defN 23-Apr-28 11:51 deep_training/setup.py
+-rw-rw-rw-  2.0 fat      905 b- defN 23-May-02 16:26 deep_training/setup.py
 -rw-rw-rw-  2.0 fat       55 b- defN 23-Apr-10 11:44 deep_training/cv/__init__.py
 -rw-rw-rw-  2.0 fat      195 b- defN 23-Apr-10 11:44 deep_training/data_helper/__init__.py
--rw-rw-rw-  2.0 fat    17724 b- defN 23-Apr-28 11:47 deep_training/data_helper/data_helper.py
+-rw-rw-rw-  2.0 fat    17724 b- defN 23-May-02 04:53 deep_training/data_helper/data_helper.py
 -rw-rw-rw-  2.0 fat     5041 b- defN 23-Apr-28 11:47 deep_training/data_helper/data_module.py
 -rw-rw-rw-  2.0 fat    12121 b- defN 23-Apr-28 11:47 deep_training/data_helper/training_args.py
 -rw-rw-rw-  2.0 fat       70 b- defN 23-Apr-10 11:44 deep_training/nlp/__init__.py
 -rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-10 11:44 deep_training/nlp/layers/__init__.py
 -rw-rw-rw-  2.0 fat      241 b- defN 23-Apr-10 11:44 deep_training/nlp/layers/activate.py
 -rw-rw-rw-  2.0 fat    13271 b- defN 23-Apr-10 11:44 deep_training/nlp/layers/crf.py
 -rw-rw-rw-  2.0 fat     4653 b- defN 23-Apr-10 11:44 deep_training/nlp/layers/handshakingkernel.py
@@ -21,14 +21,20 @@
 -rw-rw-rw-  2.0 fat       72 b- defN 23-Apr-10 11:44 deep_training/nlp/layers/lora_v1/__init__.py
 -rw-rw-rw-  2.0 fat    15095 b- defN 23-Apr-10 11:44 deep_training/nlp/layers/lora_v1/layers.py
 -rw-rw-rw-  2.0 fat     1819 b- defN 23-Apr-10 11:44 deep_training/nlp/layers/lora_v1/utils.py
 -rw-rw-rw-  2.0 fat       72 b- defN 23-Apr-10 15:59 deep_training/nlp/layers/lora_v2/__init__.py
 -rw-rw-rw-  2.0 fat    15465 b- defN 23-Apr-11 15:24 deep_training/nlp/layers/lora_v2/adalora.py
 -rw-rw-rw-  2.0 fat     8565 b- defN 23-Apr-11 15:24 deep_training/nlp/layers/lora_v2/layers.py
 -rw-rw-rw-  2.0 fat     9106 b- defN 23-Apr-10 11:44 deep_training/nlp/layers/lora_v2/utils.py
+-rw-rw-rw-  2.0 fat       80 b- defN 23-May-02 03:45 deep_training/nlp/layers/prompt/__init__.py
+-rw-rw-rw-  2.0 fat    15541 b- defN 23-May-02 04:41 deep_training/nlp/layers/prompt/adaption_prompt.py
+-rw-rw-rw-  2.0 fat     5463 b- defN 23-May-02 04:41 deep_training/nlp/layers/prompt/p_tuning.py
+-rw-rw-rw-  2.0 fat     3053 b- defN 23-May-02 03:45 deep_training/nlp/layers/prompt/prefix_tuning.py
+-rw-rw-rw-  2.0 fat     3523 b- defN 23-May-02 04:42 deep_training/nlp/layers/prompt/prompt_tuning.py
+-rw-rw-rw-  2.0 fat     9106 b- defN 23-May-02 03:45 deep_training/nlp/layers/prompt/utils.py
 -rw-rw-rw-  2.0 fat     3662 b- defN 23-Apr-10 11:44 deep_training/nlp/losses/BatchAllTripletLoss.py
 -rw-rw-rw-  2.0 fat     3880 b- defN 23-Apr-10 11:44 deep_training/nlp/losses/BatchHardSoftMarginTripletLoss.py
 -rw-rw-rw-  2.0 fat     8358 b- defN 23-Apr-10 11:44 deep_training/nlp/losses/BatchHardTripletLoss.py
 -rw-rw-rw-  2.0 fat     4552 b- defN 23-Apr-10 11:44 deep_training/nlp/losses/BatchSemiHardTripletLoss.py
 -rw-rw-rw-  2.0 fat     2255 b- defN 23-Apr-10 11:44 deep_training/nlp/losses/ContrastiveLoss.py
 -rw-rw-rw-  2.0 fat     4573 b- defN 23-Apr-10 11:44 deep_training/nlp/losses/ContrastiveTensionLoss.py
 -rw-rw-rw-  2.0 fat     1359 b- defN 23-Apr-10 11:44 deep_training/nlp/losses/CosineSimilarityLoss.py
@@ -84,45 +90,50 @@
 -rw-rw-rw-  2.0 fat     5149 b- defN 23-Apr-28 11:47 deep_training/nlp/models/pure_model.py
 -rw-rw-rw-  2.0 fat     3949 b- defN 23-Apr-28 11:47 deep_training/nlp/models/simcse.py
 -rw-rw-rw-  2.0 fat     6022 b- defN 23-Apr-28 11:47 deep_training/nlp/models/span_ner.py
 -rw-rw-rw-  2.0 fat    14454 b- defN 23-Apr-28 11:47 deep_training/nlp/models/spn4re.py
 -rw-rw-rw-  2.0 fat    11383 b- defN 23-Apr-28 11:47 deep_training/nlp/models/tplinker.py
 -rw-rw-rw-  2.0 fat     8157 b- defN 23-Apr-28 11:47 deep_training/nlp/models/tplinkerplus.py
 -rw-rw-rw-  2.0 fat     6624 b- defN 23-Apr-28 11:47 deep_training/nlp/models/transformer.py
--rw-rw-rw-  2.0 fat    26179 b- defN 23-Apr-28 11:49 deep_training/nlp/models/transformer_base.py
+-rw-rw-rw-  2.0 fat    26238 b- defN 23-May-02 15:42 deep_training/nlp/models/transformer_base.py
 -rw-rw-rw-  2.0 fat     7968 b- defN 23-Apr-28 11:47 deep_training/nlp/models/tsdae_model.py
 -rw-rw-rw-  2.0 fat     9040 b- defN 23-Apr-28 11:47 deep_training/nlp/models/w2ner.py
 -rw-rw-rw-  2.0 fat    16524 b- defN 23-Apr-28 11:47 deep_training/nlp/models/LLaMA/__init__.py
 -rw-rw-rw-  2.0 fat     5087 b- defN 23-Apr-10 11:44 deep_training/nlp/models/LLaMA/configuration.py
 -rw-rw-rw-  2.0 fat    19207 b- defN 23-Apr-28 11:47 deep_training/nlp/models/LLaMA_parallel/__init__.py
 -rw-rw-rw-  2.0 fat     5087 b- defN 23-Apr-10 11:44 deep_training/nlp/models/LLaMA_parallel/configuration.py
 -rw-rw-rw-  2.0 fat    31627 b- defN 23-Apr-10 11:44 deep_training/nlp/models/PaLM/__init__.py
 -rw-rw-rw-  2.0 fat     5890 b- defN 23-Apr-10 11:44 deep_training/nlp/models/PaLM/configuration.py
--rw-rw-rw-  2.0 fat    60508 b- defN 23-Apr-19 10:43 deep_training/nlp/models/chatglm/__init__.py
+-rw-rw-rw-  2.0 fat    60510 b- defN 23-May-02 03:45 deep_training/nlp/models/chatglm/__init__.py
 -rw-rw-rw-  2.0 fat     4575 b- defN 23-Apr-10 11:44 deep_training/nlp/models/chatglm/configuration.py
 -rw-rw-rw-  2.0 fat    15150 b- defN 23-Apr-10 11:44 deep_training/nlp/models/chatglm/quantization.py
 -rw-rw-rw-  2.0 fat    16642 b- defN 23-Apr-18 11:05 deep_training/nlp/models/chatglm/tokenization.py
 -rw-rw-rw-  2.0 fat    34123 b- defN 23-Apr-10 11:44 deep_training/nlp/models/laMDA/__init__.py
 -rw-rw-rw-  2.0 fat     5981 b- defN 23-Apr-10 11:44 deep_training/nlp/models/laMDA/configuration.py
 -rw-rw-rw-  2.0 fat      181 b- defN 23-Apr-11 10:52 deep_training/nlp/models/lora/__init__.py
 -rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-10 16:34 deep_training/nlp/models/lora/v1/__init__.py
 -rw-rw-rw-  2.0 fat     7054 b- defN 23-Apr-10 11:44 deep_training/nlp/models/lora/v1/configuration.py
--rw-rw-rw-  2.0 fat    13576 b- defN 23-Apr-12 10:45 deep_training/nlp/models/lora/v1/lora_wrapper.py
+-rw-rw-rw-  2.0 fat    13688 b- defN 23-May-02 06:57 deep_training/nlp/models/lora/v1/lora_wrapper.py
 -rw-rw-rw-  2.0 fat      206 b- defN 23-Apr-11 10:52 deep_training/nlp/models/lora/v2/__init__.py
 -rw-rw-rw-  2.0 fat    13112 b- defN 23-Apr-10 16:38 deep_training/nlp/models/lora/v2/adalora_model.py
 -rw-rw-rw-  2.0 fat    11285 b- defN 23-Apr-28 11:47 deep_training/nlp/models/lora/v2/configuration.py
 -rw-rw-rw-  2.0 fat    11745 b- defN 23-Apr-18 11:05 deep_training/nlp/models/lora/v2/lora_model.py
--rw-rw-rw-  2.0 fat    10265 b- defN 23-Apr-11 10:52 deep_training/nlp/models/lora/v2/lora_wrapper.py
+-rw-rw-rw-  2.0 fat    10415 b- defN 23-May-02 06:52 deep_training/nlp/models/lora/v2/lora_wrapper.py
 -rw-rw-rw-  2.0 fat     4889 b- defN 23-Apr-10 12:59 deep_training/nlp/models/lora/v2/save_and_load.py
 -rw-rw-rw-  2.0 fat      467 b- defN 23-Apr-28 11:47 deep_training/nlp/models/moss/__init__.py
 -rw-rw-rw-  2.0 fat     5097 b- defN 23-Apr-28 11:47 deep_training/nlp/models/moss/configuration_moss.py
 -rw-rw-rw-  2.0 fat     6735 b- defN 23-Apr-28 11:47 deep_training/nlp/models/moss/custom_autotune.py
 -rw-rw-rw-  2.0 fat    31079 b- defN 23-Apr-28 11:47 deep_training/nlp/models/moss/modeling_moss.py
--rw-rw-rw-  2.0 fat    18750 b- defN 23-Apr-28 11:47 deep_training/nlp/models/moss/quantization.py
+-rw-rw-rw-  2.0 fat    18744 b- defN 23-May-02 16:30 deep_training/nlp/models/moss/quantization.py
 -rw-rw-rw-  2.0 fat    15939 b- defN 23-Apr-28 11:47 deep_training/nlp/models/moss/tokenization_moss.py
+-rw-rw-rw-  2.0 fat      203 b- defN 23-May-02 06:07 deep_training/nlp/models/prompt/__init__.py
+-rw-rw-rw-  2.0 fat    12062 b- defN 23-May-02 16:25 deep_training/nlp/models/prompt/configuration.py
+-rw-rw-rw-  2.0 fat    52102 b- defN 23-May-02 16:22 deep_training/nlp/models/prompt/prompt_model.py
+-rw-rw-rw-  2.0 fat     3551 b- defN 23-May-02 15:49 deep_training/nlp/models/prompt/save_and_load.py
+-rw-rw-rw-  2.0 fat     1917 b- defN 23-May-02 05:50 deep_training/nlp/models/prompt/utils.py
 -rw-rw-rw-  2.0 fat      102 b- defN 23-Apr-10 11:44 deep_training/nlp/models/splinker/__init__.py
 -rw-rw-rw-  2.0 fat     2866 b- defN 23-Apr-28 11:47 deep_training/nlp/models/splinker/splinker.py
 -rw-rw-rw-  2.0 fat    14478 b- defN 23-Apr-10 11:44 deep_training/nlp/models/t5decoder/__init__.py
 -rw-rw-rw-  2.0 fat     6646 b- defN 23-Apr-10 11:44 deep_training/nlp/models/t5encoder/__init__.py
 -rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-10 11:44 deep_training/nlp/optimizer/__init__.py
 -rw-rw-rw-  2.0 fat     5225 b- defN 23-Apr-10 11:44 deep_training/nlp/optimizer/lamb.py
 -rw-rw-rw-  2.0 fat       99 b- defN 23-Apr-10 11:44 deep_training/nlp/optimizer/lion/__init__.py
@@ -153,12 +164,12 @@
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Apr-10 11:44 deep_training/tfnlp/scheduler/__init__.py
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Apr-10 11:44 deep_training/tfnlp/utils/__init__.py
 -rw-rw-rw-  2.0 fat       55 b- defN 23-Apr-10 11:44 deep_training/utils/__init__.py
 -rw-rw-rw-  2.0 fat     1941 b- defN 23-Apr-10 11:44 deep_training/utils/distributed.py
 -rw-rw-rw-  2.0 fat     1724 b- defN 23-Apr-10 11:44 deep_training/utils/func.py
 -rw-rw-rw-  2.0 fat     5117 b- defN 23-Apr-10 11:44 deep_training/utils/maskedlm.py
 -rw-rw-rw-  2.0 fat     7430 b- defN 23-Apr-28 11:47 deep_training/utils/trainer.py
--rw-rw-rw-  2.0 fat      596 b- defN 23-Apr-28 12:00 deep_training-0.1.3.post1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 12:00 deep_training-0.1.3.post1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-28 12:00 deep_training-0.1.3.post1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    15664 b- defN 23-Apr-28 12:00 deep_training-0.1.3.post1.dist-info/RECORD
-162 files, 964245 bytes uncompressed, 258884 bytes compressed:  73.2%
+-rw-rw-rw-  2.0 fat      590 b- defN 23-May-02 16:46 deep_training-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 16:46 deep_training-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-May-02 16:46 deep_training-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    16765 b- defN 23-May-02 16:46 deep_training-0.1.4.dist-info/RECORD
+173 files, 1072252 bytes uncompressed, 283222 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -72,14 +72,32 @@
 
 Filename: deep_training/nlp/layers/lora_v2/layers.py
 Comment: 
 
 Filename: deep_training/nlp/layers/lora_v2/utils.py
 Comment: 
 
+Filename: deep_training/nlp/layers/prompt/__init__.py
+Comment: 
+
+Filename: deep_training/nlp/layers/prompt/adaption_prompt.py
+Comment: 
+
+Filename: deep_training/nlp/layers/prompt/p_tuning.py
+Comment: 
+
+Filename: deep_training/nlp/layers/prompt/prefix_tuning.py
+Comment: 
+
+Filename: deep_training/nlp/layers/prompt/prompt_tuning.py
+Comment: 
+
+Filename: deep_training/nlp/layers/prompt/utils.py
+Comment: 
+
 Filename: deep_training/nlp/losses/BatchAllTripletLoss.py
 Comment: 
 
 Filename: deep_training/nlp/losses/BatchHardSoftMarginTripletLoss.py
 Comment: 
 
 Filename: deep_training/nlp/losses/BatchHardTripletLoss.py
@@ -354,14 +372,29 @@
 
 Filename: deep_training/nlp/models/moss/quantization.py
 Comment: 
 
 Filename: deep_training/nlp/models/moss/tokenization_moss.py
 Comment: 
 
+Filename: deep_training/nlp/models/prompt/__init__.py
+Comment: 
+
+Filename: deep_training/nlp/models/prompt/configuration.py
+Comment: 
+
+Filename: deep_training/nlp/models/prompt/prompt_model.py
+Comment: 
+
+Filename: deep_training/nlp/models/prompt/save_and_load.py
+Comment: 
+
+Filename: deep_training/nlp/models/prompt/utils.py
+Comment: 
+
 Filename: deep_training/nlp/models/splinker/__init__.py
 Comment: 
 
 Filename: deep_training/nlp/models/splinker/splinker.py
 Comment: 
 
 Filename: deep_training/nlp/models/t5decoder/__init__.py
@@ -468,20 +501,20 @@
 
 Filename: deep_training/utils/maskedlm.py
 Comment: 
 
 Filename: deep_training/utils/trainer.py
 Comment: 
 
-Filename: deep_training-0.1.3.post1.dist-info/METADATA
+Filename: deep_training-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: deep_training-0.1.3.post1.dist-info/WHEEL
+Filename: deep_training-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: deep_training-0.1.3.post1.dist-info/top_level.txt
+Filename: deep_training-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: deep_training-0.1.3.post1.dist-info/RECORD
+Filename: deep_training-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deep_training/setup.py

```diff
@@ -1,15 +1,15 @@
 #! -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 ignore = ['test','tests']
 setup(
     name='deep_training',
-    version='0.1.3@post1',
+    version='0.1.4',
     description='an easy training architecture',
     long_description='torch_training: https://github.com/ssbuild/deep_training.git',
     license='Apache License 2.0',
     url='https://github.com/ssbuild/deep_training',
     author='ssbuild',
     author_email='9727464@qq.com',
     install_requires=['pytorch-lightning>=2',
```

## deep_training/data_helper/data_helper.py

```diff
@@ -237,15 +237,15 @@
                                    class_name=tokenizer_class_name,
                                    model_name_or_path=model_name_or_path or model_args.model_name_or_path,
                                    cache_dir=model_args.cache_dir,
                                    do_lower_case=model_args.do_lower_case,
                                    use_fast_tokenizer=model_args.use_fast_tokenizer,
                                    model_revision=model_args.model_revision,
                                    use_auth_token=model_args.use_auth_token,
-                                   **config_kwargs,
+                                   **tokenizer_kwargs,
                                    )
         self.tokenizer = tokenizer
 
 
         self.max_seq_length_dict['train'] = data_args.train_max_seq_length
         self.max_seq_length_dict['eval'] = data_args.eval_max_seq_length
         self.max_seq_length_dict['val'] = data_args.eval_max_seq_length
@@ -266,15 +266,15 @@
             "bos_token_id": tokenizer.bos_token_id,
             "pad_token_id": tokenizer.pad_token_id,
             "eos_token_id": tokenizer.eos_token_id,
             "sep_token_id": tokenizer.sep_token_id,
             "return_dict": return_dict,
             "task_specific_params": task_specific_params,
         }
-        kwargs_args.update(tokenizer_kwargs)
+        kwargs_args.update(config_kwargs)
 
 
         if with_labels and self.label2id is not None:
             kwargs_args['label2id'] = self.label2id
             kwargs_args['id2label'] = self.id2label
             kwargs_args['num_labels'] = len(self.label2id) if self.label2id is not None else None
```

## deep_training/nlp/models/transformer_base.py

```diff
@@ -48,15 +48,15 @@
             hparams_file: typing.Optional[str] = None,
             strict: bool = True,
             **kwargs: Any,
     ) -> typing.Union["pl.LightningModule", "pl.LightningDataModule","MyLightningModule"]:
         return super(MyLightningModule, cls).load_from_checkpoint(checkpoint_path,map_location,hparams_file,strict,**kwargs)
 
     @property
-    def backbone(self):
+    def backbone(self) -> nn.Module:
         return self.__model
 
     @property
     def model(self):
         return self.__model
 
     def convert_to_onnx(self, file_path,
@@ -223,15 +223,16 @@
         assert self.base_model_prefix is not None, ValueError('base_model_prefix is not allow empty')
         setattr(self, self.base_model_prefix, model)
 
     def get_model_lr(self,model=None,lr=None):
         lr = lr if lr is not None else self.config.task_specific_params['learning_rate']
         if model is not None:
             return [(model,lr)]
-        return [(self.model if self.base_model_prefix is not None else self , lr), ]
+        # return [(self.model if self.base_model_prefix is not None else self , lr), ]
+        return [(self, lr), ]
 
 
 
 class TransformerLightningModule(MyLightningModule):
     def __init__(self, *args,**kwargs):
         config = get_value_from_args('config',PretrainedConfig,*args,**kwargs)
         model_args = get_value_from_args('model_args', ModelArguments, *args, **kwargs)
@@ -313,15 +314,15 @@
             if hasattr(tmp_obj, 'embeddings'):
                 return tmp_obj
             current_model = tmp_obj
             tmp_obj = getattr(current_model, base_model_prefix, None)
         return tmp_obj
 
     @property
-    def backbone(self):
+    def backbone(self) -> nn.Module:
         return self.__backbone
 
     @property
     def model(self):
         return self.__backbone
 
     @model.setter
```

## deep_training/nlp/models/chatglm/__init__.py

```diff
@@ -724,15 +724,15 @@
             block_position_ids = torch.stack(block_position_ids, dim=0)
             position_ids = torch.stack((position_ids, block_position_ids), dim=1)
         else:
             position_ids = torch.arange(seq_length, dtype=torch.long, device=device).unsqueeze(0).repeat(batch_size, 1)
 
             for i, context_length in enumerate(context_lengths):
                 if not use_gmasks[i]:
-                    position_ids[context_length:] = mask_positions[i]
+                    position_ids[i,context_length:] = mask_positions[i]
 
         return position_ids
 
 CHATGLM_6B_START_DOCSTRING = r"""
     This model is a PyTorch [torch.nn.Module](https://pytorch.org/docs/stable/nn.html#torch.nn.Module) sub-class.
     Use it as a regular PyTorch Module and refer to the PyTorch documentation for all matter related to general
     usage and behavior.
```

## deep_training/nlp/models/lora/v1/lora_wrapper.py

```diff
@@ -188,16 +188,18 @@
             new_module.to(old_module.weight.device)
 
     def __getattr__(self, name: str):
         """Forward missing attributes to the wrapped module."""
         try:
             return super().__getattr__(name)  # defer to nn.Module's logic
         except AttributeError:
-            return getattr(self.model, name)
-
+            try:
+                return getattr(self.model, name)
+            except AttributeError:
+                return getattr(self.model.model, name)
     @property
     def modules_to_save(self):
         return None
 
     def get_lora_config_as_dict(self, inference: bool = False):
         config = {k: v.value if isinstance(v, Enum) else v for k, v in asdict(self.lora_config).items()}
         if inference:
```

## deep_training/nlp/models/lora/v2/lora_wrapper.py

```diff
@@ -149,15 +149,19 @@
         )
 
     def __getattr__(self, name: str):
         """Forward missing attributes to the wrapped module."""
         try:
             return super().__getattr__(name)  # defer to nn.Module's logic
         except AttributeError:
-            return getattr(self.base_model, name)
+            try:
+                return getattr(self.base_model, name) # defer to nn.Module's logic
+            except AttributeError:
+                return getattr(self.base_model.model, name)
+
 
     def forward(self, *args, **kwargs):
         """
         Forward pass of the model.
         """
         return self.get_base_model()(*args, **kwargs)
```

## deep_training/nlp/models/moss/quantization.py

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import torch
 import torch.nn as nn
 from torch.cuda.amp import custom_bwd, custom_fwd
 import math
 import triton
 import triton.language as tl
-from models.custom_autotune import *
+from .custom_autotune import *
 
 
 def find_layers(module, layers=[nn.Conv2d, nn.Linear], name=''):
     if type(module) in layers:
         return {name: module}
     res = {}
     for name1, child in module.named_children():
```

## Comparing `deep_training-0.1.3.post1.dist-info/METADATA` & `deep_training-0.1.4.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-training
-Version: 0.1.3-post1
+Version: 0.1.4
 Summary: an easy training architecture
 Home-page: https://github.com/ssbuild/deep_training
 Author: ssbuild
 Author-email: 9727464@qq.com
 License: Apache License 2.0
 Requires-Dist: pytorch-lightning (>=2)
 Requires-Dist: numpy-io (<0.1.0,>=0.0.2)
```

## Comparing `deep_training-0.1.3.post1.dist-info/RECORD` & `deep_training-0.1.4.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 deep_training/__init__.py,sha256=bhATnUT4VEzwvA8_8IwxspnDRKf32ZgEeHYCN2E5Dd4,47
-deep_training/setup.py,sha256=iQSMbwmygDGrjcYWFGg-_WNf0z8QbVJgv1ZhMJFQq1w,911
+deep_training/setup.py,sha256=lfCUnxR3vFX4OlF9DejxOze7_l8xUQqOwZWr-eMqB2Q,905
 deep_training/cv/__init__.py,sha256=J-zlKxMsAfAgoO0vSAzgYJXSuMSJcJ7NKAPKeaeC3TM,55
 deep_training/data_helper/__init__.py,sha256=P8rAMalR6xNepAf-9ldGoOSsEiUtur8Px6gUpTXQhd8,195
-deep_training/data_helper/data_helper.py,sha256=kQEWL36NEhEoA7bw0zLA7CIYC_LYFtueXwr9deSthIM,17724
+deep_training/data_helper/data_helper.py,sha256=Pe45VeRSRl7izzI5TVfsZ6PnzGK3tyfGWMxGsoclnLs,17724
 deep_training/data_helper/data_module.py,sha256=EmXCTU2jLnldgHubQL4lpwzmlJErSVJf7YIotbQBQJU,5041
 deep_training/data_helper/training_args.py,sha256=XGUXdty0SE6n8xqk6J0lySFvaYSGMVo2zuq6paFQ8sM,12121
 deep_training/nlp/__init__.py,sha256=L4_ltrwpG8mrgN1hZRKimefLHgjhRYyXVtLMFzr1grw,70
 deep_training/nlp/layers/__init__.py,sha256=zbd9GfR02_YVgsTJSXjfyIcQwj8PmG4PscMdA0p6ONI,56
 deep_training/nlp/layers/activate.py,sha256=0q7htFl9Az2fdUjrjv-QMUCE5oenYPVTLZ3lRemIKzA,241
 deep_training/nlp/layers/crf.py,sha256=JTihPuJuBBp83I9UZzVg0wogwwpdJrs0VKtuLPBSCDM,13271
 deep_training/nlp/layers/handshakingkernel.py,sha256=BRJZbEjKM347q8zEMEtJXxXjmqhegmQgqebhqMy4UkI,4653
@@ -20,14 +20,20 @@
 deep_training/nlp/layers/lora_v1/__init__.py,sha256=gmwJqLmiKqPfh5_VGWWr38y8lLgdPWw6JrjNVrvsLEY,72
 deep_training/nlp/layers/lora_v1/layers.py,sha256=JWz9RtqA-hLsTxyhZPBlz82aN_VaPjNoDYRhssKV1H0,15095
 deep_training/nlp/layers/lora_v1/utils.py,sha256=1ouFUmTF9IXzum97eIlrTeT6J4OAnEwIaWkZdgXMjSc,1819
 deep_training/nlp/layers/lora_v2/__init__.py,sha256=dGpWUx0v7UoVgwZY5srCDCBvt_hlI77zA6mQO3CxMaE,72
 deep_training/nlp/layers/lora_v2/adalora.py,sha256=dOqXcfqFfs4tpiwqU52bEzO1WoX9wP2itSBysw9rQ90,15465
 deep_training/nlp/layers/lora_v2/layers.py,sha256=giRQXEolkWGhU0CsNoOMOZBXrgwBbp6_FvOf9_Cjdeg,8565
 deep_training/nlp/layers/lora_v2/utils.py,sha256=Hl3i9r0eP5lUzSqyPAXKnO0oEgDCY8lC3ZGV0scmNRs,9106
+deep_training/nlp/layers/prompt/__init__.py,sha256=J8P_z5Lrd5h9c6mhMG1BY8ZP4Vl5l8Tc5yukwlzg9Ag,80
+deep_training/nlp/layers/prompt/adaption_prompt.py,sha256=J9iDQOQQSE98GN1Tmd9Yjo7v0QtCA6yXpyPsRGRXe1I,15541
+deep_training/nlp/layers/prompt/p_tuning.py,sha256=LTvyxWmSrMq6nIi8v8Ohx8knkvFYqvPUSuQ_hssGOpc,5463
+deep_training/nlp/layers/prompt/prefix_tuning.py,sha256=QwgiIoEPPjKy34gH7t1dHg4sh5RRdcbbMl_iMcYH-uA,3053
+deep_training/nlp/layers/prompt/prompt_tuning.py,sha256=STLP8rRqT1XEjcts3lwgjLWhd0_NZT6YvqYSN9nsMkI,3523
+deep_training/nlp/layers/prompt/utils.py,sha256=Hl3i9r0eP5lUzSqyPAXKnO0oEgDCY8lC3ZGV0scmNRs,9106
 deep_training/nlp/losses/BatchAllTripletLoss.py,sha256=_2Og7Hf3Bjd1GT55UFmbZq5QLxdcKUyv4T00loPrKUo,3662
 deep_training/nlp/losses/BatchHardSoftMarginTripletLoss.py,sha256=Caif480bvgTWAQueadlAGSODpdaxVyRaik5-3j84wwg,3880
 deep_training/nlp/losses/BatchHardTripletLoss.py,sha256=xDdaQkcr6KCehSWlasABBkjPS9D6u_H5EngmppBkpXc,8358
 deep_training/nlp/losses/BatchSemiHardTripletLoss.py,sha256=xcfR8X3zyEs7YFoAT0q78iuZ2CJPtsrRUkp1Q8v5-QA,4552
 deep_training/nlp/losses/ContrastiveLoss.py,sha256=f7ZO4BUrqsSj0_Q670B6yIGHaSjYNOxwehBMPfRSEdg,2255
 deep_training/nlp/losses/ContrastiveTensionLoss.py,sha256=MNigl0maM6IpRasB83cf2UHPm4E73-J4N3F6y-F-uxc,4573
 deep_training/nlp/losses/CosineSimilarityLoss.py,sha256=UzWqQBE1JvASO2uZ-HzlX2YSDCLmMS-2DgoGLHqfXno,1359
@@ -83,45 +89,50 @@
 deep_training/nlp/models/pure_model.py,sha256=LD8cYvvRirnP8iMFCyRhsNXRHpZt93Kh2WGoUZoEnFw,5149
 deep_training/nlp/models/simcse.py,sha256=ubVGkeMatDeIUqySV8Tc2TJHvaRKb4p3JOvUTOOhaRo,3949
 deep_training/nlp/models/span_ner.py,sha256=rD0TY2K-zesfRFGfDguqkSAfxHGgbQHG3K5QZ6gc7Zg,6022
 deep_training/nlp/models/spn4re.py,sha256=g_pk3bNqpH41EnzJ77oWPsKvbUwzJfaBYMux5FiEc60,14454
 deep_training/nlp/models/tplinker.py,sha256=PJ9smipeIiA1CDi8xz1gIg2DBWzO5C1B2wITItEsd1A,11383
 deep_training/nlp/models/tplinkerplus.py,sha256=hP4KD3rf2hktfQzHnI7RA2j_2cjk_0G5v6CkbLt1gvQ,8157
 deep_training/nlp/models/transformer.py,sha256=ZuywgLt3HZhsR4sJ4SyZvrYgaVJW8lCn5JH1j_IceXE,6624
-deep_training/nlp/models/transformer_base.py,sha256=pam0type1O9aZe6WReiDYImSyHLUppRgEvpZM7ZIMf0,26179
+deep_training/nlp/models/transformer_base.py,sha256=vxDVNUxRbSMpnLLxwtqS4aOmI_Teg5ggSY-KVHRuCEE,26238
 deep_training/nlp/models/tsdae_model.py,sha256=lb04RIGkhHhilD-vdkfb8YK9hnTck1nN79WX1Pngbbk,7968
 deep_training/nlp/models/w2ner.py,sha256=z0BortOquZSzmma355wNLz1ofLku_hMb2CjL4KDf-PM,9040
 deep_training/nlp/models/LLaMA/__init__.py,sha256=asn9Wxkl4lG12dRVgxq7Lz4BGCNDaRFL155haVMDNso,16524
 deep_training/nlp/models/LLaMA/configuration.py,sha256=HNzzhIIdR9HBN9Y4Oavv6cGgIf0ExcphwsbVkltJ2ZM,5087
 deep_training/nlp/models/LLaMA_parallel/__init__.py,sha256=4fOhbq0tQOTSH5e3X6XN3PnI6athUR8tsTCn4AUg94Q,19207
 deep_training/nlp/models/LLaMA_parallel/configuration.py,sha256=HNzzhIIdR9HBN9Y4Oavv6cGgIf0ExcphwsbVkltJ2ZM,5087
 deep_training/nlp/models/PaLM/__init__.py,sha256=P1qwWPUycRmZ6I48tov6janJUNpp4L-iMoVN54ykcQw,31627
 deep_training/nlp/models/PaLM/configuration.py,sha256=kIb3nj-2pQB2wyNrYHSZqr_ta1F0Cg-VbGEbnM5icPc,5890
-deep_training/nlp/models/chatglm/__init__.py,sha256=t9u927aSHY0mVpxtGrY7_jMEx25g9rsHKcE0HR3GWGc,60508
+deep_training/nlp/models/chatglm/__init__.py,sha256=osBnXXXUoHwREHqXRX6WIEY0OQ0K1Yg7MKjQf04FNIQ,60510
 deep_training/nlp/models/chatglm/configuration.py,sha256=4w-Kbp_FJ2crIQVyu6kie9lbMSuE3U4nnjwjVPos2E8,4575
 deep_training/nlp/models/chatglm/quantization.py,sha256=sqX_poTcYNLJLDPbCwfRllDCF0enhshjX_dw7yZa604,15150
 deep_training/nlp/models/chatglm/tokenization.py,sha256=XPdz8DFekZ3qsYakyP2iZbk0Iu1cCXgnXjrBKHDO_s8,16642
 deep_training/nlp/models/laMDA/__init__.py,sha256=fvxTQQ8jfU-msPRdC8KsGlCwzM6u8-WBmayu6gE-s0E,34123
 deep_training/nlp/models/laMDA/configuration.py,sha256=8ZvPEl1C1KUGYWw7a8XcgIgl3gWH9WXa_-ZNDqz34PE,5981
 deep_training/nlp/models/lora/__init__.py,sha256=YyYmxdwz0IdyE4QXMPWhjUNmvOccqO8kJzPblfPwGJI,181
 deep_training/nlp/models/lora/v1/__init__.py,sha256=zwGdNKqudVj7c8sMWbmZ9CnnncWXuEapAucWY-VEhLs,123
 deep_training/nlp/models/lora/v1/configuration.py,sha256=MAkg2BQCqL6XvHd2SRXsijtPToNMuN-4Hmm_02HVCmU,7054
-deep_training/nlp/models/lora/v1/lora_wrapper.py,sha256=449xBRufJ8Tt4p_OLsp7TZ3v8Y3iIBdpccgReGDzUng,13576
+deep_training/nlp/models/lora/v1/lora_wrapper.py,sha256=c7X2raQW6tEN1stIIBJxoHA87mHEsDJZjcPDl_8D9g0,13688
 deep_training/nlp/models/lora/v2/__init__.py,sha256=2XorjeFlyNuH6xTXiyNO1A8A3P5acBApOjxVv3YEon0,206
 deep_training/nlp/models/lora/v2/adalora_model.py,sha256=iKfKWnW--iY2gmXkMcBv6QWJr9vu-uSll57r1UNvRrY,13112
 deep_training/nlp/models/lora/v2/configuration.py,sha256=zqzbz7ljON4JH9ozp6m128fV1nvVAv7KR3V1HszGhj8,11285
 deep_training/nlp/models/lora/v2/lora_model.py,sha256=5k09kzj8bSvU-CQm5GJWtg5isXUEUYPmvKuxdLPc_V4,11745
-deep_training/nlp/models/lora/v2/lora_wrapper.py,sha256=tzDCWUiGYC81cbfNiu4ZKo3VZsftM_SF8NwH8r56BO0,10265
+deep_training/nlp/models/lora/v2/lora_wrapper.py,sha256=f5Q6CUVU6jloiyxGIMc1GLZMOSWidVjnBaa_vDbEi2s,10415
 deep_training/nlp/models/lora/v2/save_and_load.py,sha256=U7_ZaPm8gpg8gQhZei6UG5KvsJXDtSNZfZk1gWo6nWc,4889
 deep_training/nlp/models/moss/__init__.py,sha256=_dQslDggRX8ZsR6RPTUuBzAHotQt8MPAqZ1-nGULPns,467
 deep_training/nlp/models/moss/configuration_moss.py,sha256=Qqp7anpWGnsotkqd5UOfc9e5zhxgx7j5xetSQUOmhaQ,5097
 deep_training/nlp/models/moss/custom_autotune.py,sha256=O-C9w-hZkcrUgDfK4B1iPtKjHQAZwELNefYhlLABHyc,6735
 deep_training/nlp/models/moss/modeling_moss.py,sha256=Trm6zkUFQo9SkgInIuusSFekRvyLa6x2W6WyRE9CswI,31079
-deep_training/nlp/models/moss/quantization.py,sha256=AWHuzdahL7uYwTCcSpXOqD4o2g-q-es_s1nStOCkfQ8,18750
+deep_training/nlp/models/moss/quantization.py,sha256=FBkz_BJ0s1AxvpStE6wEklGH7Ot63bGuO5D4XaVsWqc,18744
 deep_training/nlp/models/moss/tokenization_moss.py,sha256=Ft7hwLBfYoAqn33anM0sbkvU7GuXJQW8NJ1Ddko_1hk,15939
+deep_training/nlp/models/prompt/__init__.py,sha256=D8B65xX2WyGoV4PBPmc1NujefRcgOz1DUq9zcYbBE2g,203
+deep_training/nlp/models/prompt/configuration.py,sha256=q08sC6BzMcS8yoyV3aMWCXeeZH2fleIB0rn_i98Iw_Y,12062
+deep_training/nlp/models/prompt/prompt_model.py,sha256=BE3eaxzg-tWCy8PSp4aQo7tJdXZDpYtQs4o2KAudH90,52102
+deep_training/nlp/models/prompt/save_and_load.py,sha256=A0RtSZUp_Cn7A-zWIEZKtTAa_quWhVTTi9AtsWB5VlE,3551
+deep_training/nlp/models/prompt/utils.py,sha256=nvNO26eHmgIuY2WrfX3IyyH6jDwEJmQv7ieZqUA-n-0,1917
 deep_training/nlp/models/splinker/__init__.py,sha256=QtgnpJa78vAq9bzfjN67NmHU3dXU6WH84jeyZoD1sBs,102
 deep_training/nlp/models/splinker/splinker.py,sha256=AhIWyfUtNOLqwZn520J-mv8LJwIoDZpo8yNoc4V5Gss,2866
 deep_training/nlp/models/t5decoder/__init__.py,sha256=R9Op4Ysli9isootQQ2FcjhpbG13fNESlmUROu6cfGH0,14478
 deep_training/nlp/models/t5encoder/__init__.py,sha256=692ChfLf2sZWgzhBM37g1PdpmEmsU1R9RRl_uTHRET0,6646
 deep_training/nlp/optimizer/__init__.py,sha256=c4cmx9ebIdqwXBu3N9QbcNNHb32t2MV6fTK9aC2VBGQ,56
 deep_training/nlp/optimizer/lamb.py,sha256=htvZQHPWHG5GCDgo9xCaZikWwRyaD2PjDioIQvX7qXw,5225
 deep_training/nlp/optimizer/lion/__init__.py,sha256=AvYkLp7sOpRIC3a5ejuniUUKyQmmBA1TPJdt2RA7Nqg,99
@@ -152,11 +163,11 @@
 deep_training/tfnlp/scheduler/__init__.py,sha256=69flKnae4cQQyWUDwuYE0w0iaPonvH0P_WjBd_t-IqU,53
 deep_training/tfnlp/utils/__init__.py,sha256=kAmlOWNSpQCHbtT-mAsKGQzQFoWKp2jQf3neCJ0cCRY,53
 deep_training/utils/__init__.py,sha256=JFm7m_LPsS9Oavyxn9rbWqllCmV_zBho19rISlHNX4c,55
 deep_training/utils/distributed.py,sha256=-dhvJ6YHpRxvtZ1_on50IE33fUFW3zKXBKqqK-L1HGM,1941
 deep_training/utils/func.py,sha256=1p8hiQDCyk_gQGKrF7y6Dt66k3jLXSAt2IQeJuHQEl8,1724
 deep_training/utils/maskedlm.py,sha256=o8EB2BbDdh7wdgqz9Oi6SsVr1uBWxV15qfTk2VPjWsU,5117
 deep_training/utils/trainer.py,sha256=kbojvTgVcYX8bJ141J7VS14-JrD480Oh33P_tnwjlks,7430
-deep_training-0.1.3.post1.dist-info/METADATA,sha256=PM18Z_FBHZlOqH6V13fBje9lrX6cTn5OpmVqTskLWFY,596
-deep_training-0.1.3.post1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-deep_training-0.1.3.post1.dist-info/top_level.txt,sha256=P4qengiW56PZRm1VvlGcseSUCmAaBCsalCviUABZtO0,14
-deep_training-0.1.3.post1.dist-info/RECORD,,
+deep_training-0.1.4.dist-info/METADATA,sha256=WtZsIB5gkHwQZrE3exfwuusipVuDxvhZF65mPQGcZzw,590
+deep_training-0.1.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+deep_training-0.1.4.dist-info/top_level.txt,sha256=P4qengiW56PZRm1VvlGcseSUCmAaBCsalCviUABZtO0,14
+deep_training-0.1.4.dist-info/RECORD,,
```

