# Comparing `tmp/shttst-0.0.2.tar.gz` & `tmp/shttst-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shttst-0.0.2.tar", last modified: Mon May  1 22:11:11 2023, max compression
+gzip compressed data, was "shttst-0.0.3.tar", last modified: Tue May  2 06:16:47 2023, max compression
```

## Comparing `shttst-0.0.2.tar` & `shttst-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 22:11:11.075062 shttst-0.0.2/
--rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 shttst-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      418 2023-05-01 22:11:11.073067 shttst-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       48 2023-04-24 20:31:57.000000 shttst-0.0.2/README.md
--rw-rw-rw-   0        0        0      582 2023-05-01 22:10:49.000000 shttst-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 22:11:11.075062 shttst-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 22:11:10.957813 shttst-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 22:11:10.969967 shttst-0.0.2/src/shttst/
-drwxrwxrwx   0        0        0        0 2023-05-01 22:11:11.013637 shttst-0.0.2/src/shttst/audio/
--rw-rw-rw-   0        0        0       20 2023-04-30 11:58:12.000000 shttst-0.0.2/src/shttst/audio/__init__.py
--rw-rw-rw-   0        0        0     2809 2023-05-01 09:32:23.000000 shttst-0.0.2/src/shttst/audio/tools.py
--rw-rw-rw-   0        0        0     1133 2023-04-30 12:00:44.000000 shttst-0.0.2/src/shttst/audio/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:11:11.023757 shttst-0.0.2/src/shttst/dataset/
--rw-rw-rw-   0        0        0       63 2023-04-27 05:40:53.000000 shttst-0.0.2/src/shttst/dataset/__init__.py
--rw-rw-rw-   0        0        0     1841 2023-04-28 14:00:24.000000 shttst-0.0.2/src/shttst/dataset/dataset_files.py
--rw-rw-rw-   0        0        0      471 2023-04-27 06:45:40.000000 shttst-0.0.2/src/shttst/dataset/transcription_line.py
--rw-rw-rw-   0        0        0      687 2023-04-27 06:23:23.000000 shttst-0.0.2/src/shttst/dataset/transcriptions.py
--rw-rw-rw-   0        0        0     1406 2023-04-30 08:58:14.000000 shttst-0.0.2/src/shttst/files.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:11:11.031546 shttst-0.0.2/src/shttst/models/
--rw-rw-rw-   0        0        0       55 2023-05-01 09:12:33.000000 shttst-0.0.2/src/shttst/models/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-04-30 18:46:06.000000 shttst-0.0.2/src/shttst/models/silero_vad.py
--rw-rw-rw-   0        0        0    19544 2023-05-01 09:28:43.000000 shttst-0.0.2/src/shttst/models/vocal_remover.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:11:11.045863 shttst-0.0.2/src/shttst/recipes/
--rw-rw-rw-   0        0        0        0 2023-05-01 09:52:26.000000 shttst-0.0.2/src/shttst/recipes/__init__.py
--rw-rw-rw-   0        0        0     2268 2023-05-01 21:51:19.000000 shttst-0.0.2/src/shttst/recipes/chomik.py
--rw-rw-rw-   0        0        0     1132 2023-05-01 18:14:58.000000 shttst-0.0.2/src/shttst/recipes/multiset.py
--rw-rw-rw-   0        0        0      922 2023-04-30 08:00:20.000000 shttst-0.0.2/src/shttst/recipes/prepare_tts_wavs.py
--rw-rw-rw-   0        0        0     2194 2023-04-30 19:34:16.000000 shttst-0.0.2/src/shttst/recipes/transcribe_directory.py
--rw-rw-rw-   0        0        0     2995 2023-05-01 09:44:55.000000 shttst-0.0.2/src/shttst/recipes/yt.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:11:11.070558 shttst-0.0.2/src/shttst/text/
--rw-rw-rw-   0        0        0       98 2023-04-25 09:35:07.000000 shttst-0.0.2/src/shttst/text/__init__.py
--rw-rw-rw-   0        0        0    13863 2023-04-25 09:44:50.000000 shttst-0.0.2/src/shttst/text/shmart_cleaner.py
--rw-rw-rw-   0        0        0     3637 2023-04-24 20:27:02.000000 shttst-0.0.2/src/shttst/text/shmart_nums.py
--rw-rw-rw-   0        0        0      171 2023-04-24 20:19:31.000000 shttst-0.0.2/src/shttst/text/symbols.py
--rw-rw-rw-   0        0        0      782 2023-04-25 09:35:28.000000 shttst-0.0.2/src/shttst/text/text.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:11:11.006608 shttst-0.0.2/src/shttst.egg-info/
--rw-rw-rw-   0        0        0      418 2023-05-01 22:11:10.000000 shttst-0.0.2/src/shttst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      886 2023-05-01 22:11:10.000000 shttst-0.0.2/src/shttst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 22:11:10.000000 shttst-0.0.2/src/shttst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-05-01 22:11:10.000000 shttst-0.0.2/src/shttst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 22:11:10.000000 shttst-0.0.2/src/shttst.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 06:16:47.609420 shttst-0.0.3/
+-rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 shttst-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      418 2023-05-02 06:16:47.608235 shttst-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2023-04-24 20:31:57.000000 shttst-0.0.3/README.md
+-rw-rw-rw-   0        0        0      582 2023-05-02 06:16:28.000000 shttst-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 06:16:47.609420 shttst-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 06:16:47.354138 shttst-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 06:16:47.376851 shttst-0.0.3/src/shttst/
+drwxrwxrwx   0        0        0        0 2023-05-02 06:16:47.433090 shttst-0.0.3/src/shttst/audio/
+-rw-rw-rw-   0        0        0       20 2023-04-30 11:58:12.000000 shttst-0.0.3/src/shttst/audio/__init__.py
+-rw-rw-rw-   0        0        0     2837 2023-05-02 06:16:16.000000 shttst-0.0.3/src/shttst/audio/tools.py
+-rw-rw-rw-   0        0        0     1133 2023-04-30 12:00:44.000000 shttst-0.0.3/src/shttst/audio/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:16:47.467272 shttst-0.0.3/src/shttst/dataset/
+-rw-rw-rw-   0        0        0       63 2023-04-27 05:40:53.000000 shttst-0.0.3/src/shttst/dataset/__init__.py
+-rw-rw-rw-   0        0        0     1841 2023-04-28 14:00:24.000000 shttst-0.0.3/src/shttst/dataset/dataset_files.py
+-rw-rw-rw-   0        0        0      471 2023-04-27 06:45:40.000000 shttst-0.0.3/src/shttst/dataset/transcription_line.py
+-rw-rw-rw-   0        0        0      687 2023-04-27 06:23:23.000000 shttst-0.0.3/src/shttst/dataset/transcriptions.py
+-rw-rw-rw-   0        0        0     1406 2023-04-30 08:58:14.000000 shttst-0.0.3/src/shttst/files.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:16:47.494224 shttst-0.0.3/src/shttst/models/
+-rw-rw-rw-   0        0        0       55 2023-05-01 09:12:33.000000 shttst-0.0.3/src/shttst/models/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-04-30 18:46:06.000000 shttst-0.0.3/src/shttst/models/silero_vad.py
+-rw-rw-rw-   0        0        0    19544 2023-05-01 09:28:43.000000 shttst-0.0.3/src/shttst/models/vocal_remover.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:16:47.543769 shttst-0.0.3/src/shttst/recipes/
+-rw-rw-rw-   0        0        0        0 2023-05-01 09:52:26.000000 shttst-0.0.3/src/shttst/recipes/__init__.py
+-rw-rw-rw-   0        0        0     2268 2023-05-01 21:51:19.000000 shttst-0.0.3/src/shttst/recipes/chomik.py
+-rw-rw-rw-   0        0        0     1132 2023-05-01 18:14:58.000000 shttst-0.0.3/src/shttst/recipes/multiset.py
+-rw-rw-rw-   0        0        0      922 2023-04-30 08:00:20.000000 shttst-0.0.3/src/shttst/recipes/prepare_tts_wavs.py
+-rw-rw-rw-   0        0        0     2194 2023-04-30 19:34:16.000000 shttst-0.0.3/src/shttst/recipes/transcribe_directory.py
+-rw-rw-rw-   0        0        0     2995 2023-05-01 09:44:55.000000 shttst-0.0.3/src/shttst/recipes/yt.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:16:47.605193 shttst-0.0.3/src/shttst/text/
+-rw-rw-rw-   0        0        0       98 2023-04-25 09:35:07.000000 shttst-0.0.3/src/shttst/text/__init__.py
+-rw-rw-rw-   0        0        0    13863 2023-04-25 09:44:50.000000 shttst-0.0.3/src/shttst/text/shmart_cleaner.py
+-rw-rw-rw-   0        0        0     3637 2023-04-24 20:27:02.000000 shttst-0.0.3/src/shttst/text/shmart_nums.py
+-rw-rw-rw-   0        0        0      171 2023-04-24 20:19:31.000000 shttst-0.0.3/src/shttst/text/symbols.py
+-rw-rw-rw-   0        0        0      782 2023-04-25 09:35:28.000000 shttst-0.0.3/src/shttst/text/text.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:16:47.402993 shttst-0.0.3/src/shttst.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-05-02 06:16:47.000000 shttst-0.0.3/src/shttst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      886 2023-05-02 06:16:47.000000 shttst-0.0.3/src/shttst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 06:16:47.000000 shttst-0.0.3/src/shttst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-05-02 06:16:47.000000 shttst-0.0.3/src/shttst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-02 06:16:47.000000 shttst-0.0.3/src/shttst.egg-info/top_level.txt
```

### Comparing `shttst-0.0.2/LICENSE` & `shttst-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/pyproject.toml` & `shttst-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "shttst"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Shmart", email="szprytnyd@gmail.com" },
 ]
 description = "Shmart TTS tools."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `shttst-0.0.2/src/shttst/audio/tools.py` & `shttst-0.0.3/src/shttst/audio/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import huggingface_hub
 import torch
-from torch import Tensor
 from typing import Tuple
 from faster_whisper import WhisperModel
 from nemo.collections.asr.models import EncDecSpeakerLabelModel
-from resemblyzer import VoiceEncoder, preprocess_wav
 
 from audclas.tortoise_audio_classifier import TortoiseAudioClassifier
 from shttst.audio.utils import save_audio
 from shttst.models import ShmartSileroVad, ShmartVocalRemover
 
 initialized_models= {}
 
@@ -19,14 +17,15 @@
         model = TortoiseAudioClassifier()
     elif type == 'denoiser':
         model = ShmartVocalRemover()
     elif type == 'titanet':
         model = EncDecSpeakerLabelModel.from_pretrained("nvidia/speakerverification_en_titanet_large", map_location='cpu')
         model.eval()
     elif type == 'resemblyzer':
+        from resemblyzer import VoiceEncoder
         model = VoiceEncoder('cpu', verbose=False)
         model.eval()
     elif type == 'vad':
         model = ShmartSileroVad()
     elif type == 'whisper':
         model_path = huggingface_hub.snapshot_download("shmart/shmisper-medium-PL")
         model = WhisperModel(model_path, device="cuda", compute_type="float16")
@@ -51,19 +50,20 @@
 def clean_audio_noise(file_path: str) -> str:
     model: ShmartVocalRemover = get_model('denoiser')
     vocals, instruments = model(file_path)
     save_audio(file_path, vocals)
 
 def get_custom_embedding(file_path, type='titanet'):
     if type == 'titanet':
-        model: VoiceEncoder = get_model(type)
+        model: EncDecSpeakerLabelModel = get_model(type)
         return model.get_embedding(file_path).tolist()
     elif type == 'resemblyzer':
+        from resemblyzer import VoiceEncoder, preprocess_wav
         wav = preprocess_wav(file_path)
-        model: EncDecSpeakerLabelModel = get_model(type)
+        model: VoiceEncoder = get_model(type)
         return torch.from_numpy(model.embed_utterance(wav)).tolist()
 
 def get_transcription(audio_path, options={
     'language': "pl",
     'beam_size': 5,
     'without_timestamps': True,
     'suppress_tokens': [],
```

### Comparing `shttst-0.0.2/src/shttst/audio/utils.py` & `shttst-0.0.3/src/shttst/audio/utils.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/dataset/dataset_files.py` & `shttst-0.0.3/src/shttst/dataset/dataset_files.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/dataset/transcriptions.py` & `shttst-0.0.3/src/shttst/dataset/transcriptions.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/files.py` & `shttst-0.0.3/src/shttst/files.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/models/silero_vad.py` & `shttst-0.0.3/src/shttst/models/silero_vad.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/models/vocal_remover.py` & `shttst-0.0.3/src/shttst/models/vocal_remover.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/recipes/chomik.py` & `shttst-0.0.3/src/shttst/recipes/chomik.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/recipes/multiset.py` & `shttst-0.0.3/src/shttst/recipes/multiset.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/recipes/prepare_tts_wavs.py` & `shttst-0.0.3/src/shttst/recipes/prepare_tts_wavs.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/recipes/transcribe_directory.py` & `shttst-0.0.3/src/shttst/recipes/transcribe_directory.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/recipes/yt.py` & `shttst-0.0.3/src/shttst/recipes/yt.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/text/shmart_cleaner.py` & `shttst-0.0.3/src/shttst/text/shmart_cleaner.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/text/shmart_nums.py` & `shttst-0.0.3/src/shttst/text/shmart_nums.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst/text/text.py` & `shttst-0.0.3/src/shttst/text/text.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.2/src/shttst.egg-info/SOURCES.txt` & `shttst-0.0.3/src/shttst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

