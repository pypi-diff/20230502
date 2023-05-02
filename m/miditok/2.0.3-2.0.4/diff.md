# Comparing `tmp/miditok-2.0.3.tar.gz` & `tmp/miditok-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miditok-2.0.3.tar", last modified: Tue Apr  4 09:07:08 2023, max compression
+gzip compressed data, was "miditok-2.0.4.tar", last modified: Tue May  2 11:40:35 2023, max compression
```

## Comparing `miditok-2.0.3.tar` & `miditok-2.0.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:07:08.219348 miditok-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-04 09:06:57.000000 miditok-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-04-04 09:07:08.219348 miditok-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-04 09:06:57.000000 miditok-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:07:08.215348 miditok-2.0.3/miditok/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:07:08.215348 miditok-2.0.3/miditok/data_augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/data_augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22773 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/data_augmentation/data_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    83576 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/midi_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:07:08.219348 miditok-2.0.3/miditok/tokenizations/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/tokenizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/tokenizations/cp_word.py
--rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/tokenizations/midi_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/tokenizations/mumidi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/tokenizations/octuple.py
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/tokenizations/octuple_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    17968 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/tokenizations/remi.py
--rw-r--r--   0 runner    (1001) docker     (123)    28075 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/tokenizations/remi_plus.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/tokenizations/structured.py
--rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/tokenizations/tsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:07:08.219348 miditok-2.0.3/miditok/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-04-04 09:06:57.000000 miditok-2.0.3/miditok/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:07:08.215348 miditok-2.0.3/miditok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-04-04 09:07:08.000000 miditok-2.0.3/miditok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-04 09:07:08.000000 miditok-2.0.3/miditok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 09:07:08.000000 miditok-2.0.3/miditok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 09:07:08.000000 miditok-2.0.3/miditok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 09:07:08.000000 miditok-2.0.3/miditok.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 09:07:08.219348 miditok-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-04 09:06:57.000000 miditok-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:07:08.219348 miditok-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-04 09:06:57.000000 miditok-2.0.3/tests/test_bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-04 09:06:57.000000 miditok-2.0.3/tests/test_bpe_slow.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-04 09:06:57.000000 miditok-2.0.3/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-04-04 09:06:57.000000 miditok-2.0.3/tests/test_multitrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-04 09:06:57.000000 miditok-2.0.3/tests/test_one_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-04 09:06:57.000000 miditok-2.0.3/tests/test_saving_loading_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-04 09:06:57.000000 miditok-2.0.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-04-04 09:06:57.000000 miditok-2.0.3/tests/tests_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.005035 miditok-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 11:40:20.000000 miditok-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-02 11:40:35.005035 miditok-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-02 11:40:20.000000 miditok-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.001035 miditok-2.0.4/miditok/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.001035 miditok-2.0.4/miditok/data_augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/data_augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/data_augmentation/data_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83576 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/midi_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.005035 miditok-2.0.4/miditok/tokenizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/cp_word.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/midi_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/mumidi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/octuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/octuple_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17968 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/remi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28075 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/remi_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/tsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.005035 miditok-2.0.4/miditok/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.001035 miditok-2.0.4/miditok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-02 11:40:34.000000 miditok-2.0.4/miditok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-02 11:40:34.000000 miditok-2.0.4/miditok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:40:34.000000 miditok-2.0.4/miditok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 11:40:34.000000 miditok-2.0.4/miditok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 11:40:34.000000 miditok-2.0.4/miditok.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:40:35.005035 miditok-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-02 11:40:20.000000 miditok-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.005035 miditok-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_bpe_slow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_multitrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_one_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_saving_loading_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/tests_utils.py
```

### Comparing `miditok-2.0.3/LICENSE` & `miditok-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/PKG-INFO` & `miditok-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miditok
-Version: 2.0.3
+Version: 2.0.4
 Summary: A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies
 Home-page: https://github.com/Natooz/MidiTok
 Author: Nathan Fradet
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,midi,tokenization,music,mir
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `miditok-2.0.3/README.md` & `miditok-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok/classes.py` & `miditok-2.0.4/miditok/classes.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok/constants.py` & `miditok-2.0.4/miditok/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Constants for data encoding
 
 """
 
-CURRENT_VERSION_PACKAGE = "2.0.3"  # used when saving the config of a tokenizer
+CURRENT_VERSION_PACKAGE = "2.0.4"  # used when saving the config of a tokenizer
 
 MIDI_FILES_EXTENSIONS = [".mid", ".midi", ".MID", ".MIDI"]
 
 # Starting id of chr() method for BPE, as the 5 (0 to 4 included) firsts are ignored by 🤗tokenize
 # We also skip the 32nd (0x20) (space) as it causes issues when loading a BPE model with spaces in merged
 # Issue for reference: https://github.com/huggingface/tokenizers/issues/566
 # List of unicode characters: https://www.fileformat.info/info/charset/UTF-8/list.htm
```

### Comparing `miditok-2.0.3/miditok/data_augmentation/data_augmentation.py` & `miditok-2.0.4/miditok/data_augmentation/data_augmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,18 +88,21 @@
             )
             augmented_tokens: Dict[
                 Tuple[int, int, int], List[Union[int, List[int]]]
             ] = {}
             for track, (_, is_drum) in zip(ids, programs):
                 if is_drum:  # we dont augment drums
                     continue
+                corrected_offsets = deepcopy(offsets)
+                vel_dim = int(128 / len(tokenizer.velocities))
+                corrected_offsets[1] = [int(off / vel_dim) for off in corrected_offsets[1]]
                 aug = data_augmentation_tokens(
                     np.array(track),
                     tokenizer,
-                    *offsets,
+                    *corrected_offsets,
                     all_offset_combinations=all_offset_combinations,
                 )
                 if len(aug) == 0:
                     continue
                 for aug_offsets, seq in aug:
                     if tokenizer.unique_track:
                         augmented_tokens[aug_offsets] = seq
@@ -216,15 +219,15 @@
             as a tuple of two booleans. (default: (True, True))
     :param vel_directions: directions to shift the velocity augmentation, for up / down
             as a tuple of two booleans. (default: (True, True))
     :param dur_directions: directions to shift the duration augmentation, for up / down
             as a tuple of two booleans. (default: (True, True))
     :param midi: midi object to augment (default: None)
     :param ids: token ids as a list of tracks (default: None)
-    :return: augmented MIDI objects.
+    :return: the offsets of pitch, velocity and duration features, in "absolute" value
     """
     offsets = []
 
     if nb_octave_offset is not None:
         # Get the maximum and lowest pitch in original track
         all_pitches = []
         if midi is not None:
```

### Comparing `miditok-2.0.3/miditok/midi_tokenizer.py` & `miditok-2.0.4/miditok/midi_tokenizer.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok/tokenizations/cp_word.py` & `miditok-2.0.4/miditok/tokenizations/cp_word.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok/tokenizations/midi_like.py` & `miditok-2.0.4/miditok/tokenizations/midi_like.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok/tokenizations/mumidi.py` & `miditok-2.0.4/miditok/tokenizations/mumidi.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok/tokenizations/octuple.py` & `miditok-2.0.4/miditok/tokenizations/octuple.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok/tokenizations/octuple_mono.py` & `miditok-2.0.4/miditok/tokenizations/octuple_mono.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok/tokenizations/remi.py` & `miditok-2.0.4/miditok/tokenizations/remi.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok/tokenizations/remi_plus.py` & `miditok-2.0.4/miditok/tokenizations/remi_plus.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok/tokenizations/structured.py` & `miditok-2.0.4/miditok/tokenizations/structured.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok/tokenizations/tsd.py` & `miditok-2.0.4/miditok/tokenizations/tsd.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok/utils/utils.py` & `miditok-2.0.4/miditok/utils/utils.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/miditok.egg-info/PKG-INFO` & `miditok-2.0.4/miditok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miditok
-Version: 2.0.3
+Version: 2.0.4
 Summary: A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies
 Home-page: https://github.com/Natooz/MidiTok
 Author: Nathan Fradet
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,midi,tokenization,music,mir
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `miditok-2.0.3/miditok.egg-info/SOURCES.txt` & `miditok-2.0.4/miditok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/setup.py` & `miditok-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name='miditok',
     author='Nathan Fradet',
     url='https://github.com/Natooz/MidiTok',
     packages=find_packages(exclude=("tests",)),
-    version='2.0.3',
+    version='2.0.4',
     license='MIT',
     description='A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
         'artificial intelligence',
         'deep learning',
```

### Comparing `miditok-2.0.3/tests/test_bpe.py` & `miditok-2.0.4/tests/test_bpe.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/tests/test_bpe_slow.py` & `miditok-2.0.4/tests/test_bpe_slow.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/tests/test_methods.py` & `miditok-2.0.4/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/tests/test_multitrack.py` & `miditok-2.0.4/tests/test_multitrack.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/tests/test_one_track.py` & `miditok-2.0.4/tests/test_one_track.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/tests/test_saving_loading_config.py` & `miditok-2.0.4/tests/test_saving_loading_config.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/tests/test_utils.py` & `miditok-2.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.3/tests/tests_utils.py` & `miditok-2.0.4/tests/tests_utils.py`

 * *Files identical despite different names*

