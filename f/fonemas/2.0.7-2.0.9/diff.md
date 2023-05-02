# Comparing `tmp/fonemas-2.0.7.tar.gz` & `tmp/fonemas-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fonemas-2.0.7.tar", last modified: Mon May  9 12:14:44 2022, max compression
+gzip compressed data, was "fonemas-2.0.9.tar", last modified: Tue May 17 09:19:05 2022, max compression
```

## Comparing `fonemas-2.0.7.tar` & `fonemas-2.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2022-05-09 12:14:44.566322 fonemas-2.0.7/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     4868 2022-05-09 12:14:44.566322 fonemas-2.0.7/PKG-INFO
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3375 2022-05-09 12:13:51.000000 fonemas-2.0.7/README.md
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2022-05-09 12:14:44.562322 fonemas-2.0.7/fonemas/
--rw-r--r--   0 fernando  (1000) fernando  (1000)       23 2021-10-23 19:44:22.000000 fonemas-2.0.7/fonemas/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)    10631 2022-05-09 12:13:07.000000 fonemas-2.0.7/fonemas/fonemas.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2022-05-09 12:14:44.566322 fonemas-2.0.7/fonemas.egg-info/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     4868 2022-05-09 12:14:44.000000 fonemas-2.0.7/fonemas.egg-info/PKG-INFO
--rw-r--r--   0 fernando  (1000) fernando  (1000)      215 2022-05-09 12:14:44.000000 fonemas-2.0.7/fonemas.egg-info/SOURCES.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)        1 2022-05-09 12:14:44.000000 fonemas-2.0.7/fonemas.egg-info/dependency_links.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)       51 2022-05-09 12:14:44.000000 fonemas-2.0.7/fonemas.egg-info/entry_points.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)        8 2022-05-09 12:14:44.000000 fonemas-2.0.7/fonemas.egg-info/top_level.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)       38 2022-05-09 12:14:44.566322 fonemas-2.0.7/setup.cfg
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1382 2022-05-09 12:13:56.000000 fonemas-2.0.7/setup.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2022-05-17 09:19:05.946778 fonemas-2.0.9/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     5010 2022-05-17 09:19:05.946778 fonemas-2.0.9/PKG-INFO
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     3501 2022-05-17 09:15:28.000000 fonemas-2.0.9/README.md
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2022-05-17 09:19:05.946778 fonemas-2.0.9/fonemas/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       23 2021-10-23 19:44:22.000000 fonemas-2.0.9/fonemas/__init__.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     8728 2022-05-16 11:45:07.000000 fonemas-2.0.9/fonemas/fonemas.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2022-05-17 09:19:05.946778 fonemas-2.0.9/fonemas.egg-info/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     5010 2022-05-17 09:19:05.000000 fonemas-2.0.9/fonemas.egg-info/PKG-INFO
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      215 2022-05-17 09:19:05.000000 fonemas-2.0.9/fonemas.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)        1 2022-05-17 09:19:05.000000 fonemas-2.0.9/fonemas.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       51 2022-05-17 09:19:05.000000 fonemas-2.0.9/fonemas.egg-info/entry_points.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)        8 2022-05-17 09:19:05.000000 fonemas-2.0.9/fonemas.egg-info/top_level.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       38 2022-05-17 09:19:05.946778 fonemas-2.0.9/setup.cfg
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     1382 2022-05-17 09:15:05.000000 fonemas-2.0.9/setup.py
```

### Comparing `fonemas-2.0.7/PKG-INFO` & `fonemas-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fonemas
-Version: 2.0.7
+Version: 2.0.9
 Summary: Phonetic transcription of Spanish
 Home-page: https://github.com/fsanzl/fonemas
 Author: Fernando Sanz-Lázaro
 Author-email: fsanzl@gmail.com
 License: LGPL
 Project-URL: Source, https://github.com/fsanzl/fonemas/
 Project-URL: Tracker, https://github.com/fsanzl/fonemas/issues
 Description: [![License: LGPL](https://img.shields.io/github/license/fsanzl/fonemas)](https://opensource.org/licenses/LGPL-2.1)
-        [![Version: 2.0.7](https://img.shields.io/github/v/release/fsanzl/fonemas)](https://pypi.org/project/fonemas/)
+        [![Version: 2.0.9](https://img.shields.io/github/v/release/fsanzl/fonemas)](https://pypi.org/project/fonemas/)
         [![Python versions: 3.5, 3.6, 3.7, 3.8, 3.9](https://img.shields.io/pypi/pyversions/fonemas)](https://pypi.org/project/fonemas/)
         
         
         <h2 align="center">Fonemas</h2>
         <h3 align="center">A Python phonologic transcription library for Spanish</h2>
         
         
@@ -25,22 +25,24 @@
         
         ```bash
         pip3 install fonemas
         ```
         
         ## Use
         
-        The library provides the class  *transcription(sentence, mono, epenthesis, aspiration, sampastr)*. The class takes the obligatoy argument *sentence*, which is a string of characters with a Spanish word or words. It optionally takes two Boolean arguments *mono*,  *epenthesis* and *aspiration* set to False as default.
+        The library provides the class  *transcription(sentence, mono, epenthesis, aspiration, rehash, sampastr)*. The class takes the obligatoy argument *sentence*, which is a string of characters with a Spanish word or words. It optionally takes two Boolean arguments *mono*,  *epenthesis* and *aspiration* set to False as default.
         
         - *mono* sets whether the output shows graphic stresses for monosyllabic words
         
         - *epenthesis* set the behaviour S bfore consonant in onset (spiritu -> es pi ri tu|spi ri tu)
         
         - *aspiration* inserts an aspiration modifier 'ʰ' in onset. This may be useful when dealing with ambiguous verses in classic poetry to choose which synaloepha to break.
         
+        - *rehash* moves last consonan on last-syllable coda to next's words first-syllable onset if it begins with a vowel.
+        
         - *sampastr* allows an alternativestress symbol, as '"' to prevent issues e.g. when using in a CSV file.
         
         
         
         The class *transcription()* has three dataclass attributes, each with two attributes *{words, syllables}* containing each a list of strings, which may be words or syllables, respectively.
         
         - *phonology* for the phonological transcription (requires UNICODE support).
```

### Comparing `fonemas-2.0.7/README.md` & `fonemas-2.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![License: LGPL](https://img.shields.io/github/license/fsanzl/fonemas)](https://opensource.org/licenses/LGPL-2.1)
-[![Version: 2.0.7](https://img.shields.io/github/v/release/fsanzl/fonemas)](https://pypi.org/project/fonemas/)
+[![Version: 2.0.9](https://img.shields.io/github/v/release/fsanzl/fonemas)](https://pypi.org/project/fonemas/)
 [![Python versions: 3.5, 3.6, 3.7, 3.8, 3.9](https://img.shields.io/pypi/pyversions/fonemas)](https://pypi.org/project/fonemas/)
 
 
 <h2 align="center">Fonemas</h2>
 <h3 align="center">A Python phonologic transcription library for Spanish</h2>
 
 
@@ -15,22 +15,24 @@
 
 ```bash
 pip3 install fonemas
 ```
 
 ## Use
 
-The library provides the class  *transcription(sentence, mono, epenthesis, aspiration, sampastr)*. The class takes the obligatoy argument *sentence*, which is a string of characters with a Spanish word or words. It optionally takes two Boolean arguments *mono*,  *epenthesis* and *aspiration* set to False as default.
+The library provides the class  *transcription(sentence, mono, epenthesis, aspiration, rehash, sampastr)*. The class takes the obligatoy argument *sentence*, which is a string of characters with a Spanish word or words. It optionally takes two Boolean arguments *mono*,  *epenthesis* and *aspiration* set to False as default.
 
 - *mono* sets whether the output shows graphic stresses for monosyllabic words
 
 - *epenthesis* set the behaviour S bfore consonant in onset (spiritu -> es pi ri tu|spi ri tu)
 
 - *aspiration* inserts an aspiration modifier 'ʰ' in onset. This may be useful when dealing with ambiguous verses in classic poetry to choose which synaloepha to break.
 
+- *rehash* moves last consonan on last-syllable coda to next's words first-syllable onset if it begins with a vowel.
+
 - *sampastr* allows an alternativestress symbol, as '"' to prevent issues e.g. when using in a CSV file.
 
 
 
 The class *transcription()* has three dataclass attributes, each with two attributes *{words, syllables}* containing each a list of strings, which may be words or syllables, respectively.
 
 - *phonology* for the phonological transcription (requires UNICODE support).
```

### Comparing `fonemas-2.0.7/fonemas/fonemas.py` & `fonemas-2.0.9/fonemas/fonemas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,227 +1,170 @@
 import re
-import silabeador
+from silabeador import Syllabification
 from dataclasses import dataclass, replace
 
 
 @dataclass
 class Values:
     words: list
     syllables: list
 
 
 class Transcription:
-    def __init__(self, sentence, mono=False, epenthesis=False, aspiration=False,
-                 sampastr='"'):
-        self.sentence = self.__letters(sentence, epenthesis)
+    def __init__(self, sentence, mono = False, epenthesis = False,
+                 aspiration = False, rehash = False, stress = '"'):
+        self.sentence = self.__clean(sentence, epenthesis)
+        if rehash:
+            self.sentence = self.make_rehash(sentence)
         self.phonology = self.transcription_fnl(self.sentence, mono, aspiration)
         self.phonetics = self.transcription_fnt(self.phonology)
-        self.sampa = self.ipa2sampa(self.phonetics, sampastr)
+        self.sampa = self.ipa2sampa(self.phonetics, stress)
 
     @staticmethod
-    def __clean(sentence, epenthesis):
+    def __clean(raw_sentence, epen):
+        letters = {'b': 'be', 'c': 'θe', 'd': 'de', 'f': 'efe', 'g': 'ge',
+                   'h': 'haʧe', 'j': 'jota', 'k': 'ka', 'l': 'ele', 'm': 'eme',
+                   'n': 'ene', 'p': 'pe', 'q': 'ku', 'r': 'erre', 's': 'ese',
+                   't': 'te', 'v': 'ube', 'w': 'ubedoble', 'x': 'ekis', 'z': 'θeta'}
         symbols = ['(', ')', '¿', '?', '¡', '!', '«', '»', '“', '”', '‘', '’',
-                   '[', ']',
-                   '—', '…', ',', ';', ':', "'", '.', '–', '"', '-']
-        letters = {'õ': 'o', 'æ': 'e',
-                   ' à ': ' a ', ' ò ': 'o',
-                   'à': 'á', 'è': 'é', 'ì': 'í', 'ò': 'ó', 'ù': 'ú',
-                   'ö': '_o', 'ä': '_a', 'ë': '_e', 'ï': '_i',
-                   'â': 'a', 'ê': 'e', 'î': 'i', 'ô': 'o', 'û': 'u',
-                   'ç': 's'}
-        for x in symbols:
-            if x in sentence:
-                sentence = sentence.replace(x, ' ')
-        for x in letters:
-            if x in sentence:
-                sentence = sentence.replace(x, letters[x])
-        if epenthesis:
-            sentence = re.sub(r'\bs((?![aeiouáéíóúäëïöü]))', r'es\1', sentence)
-        return sentence
+                   '[', ']', '—', '…', ',', ';', ':', "'", '.', '–', '"', '-']
+        diacritics = { 'à': 'á', 'è': 'é', 'ì': 'í', 'ò': 'ó', 'ù': 'ú', 'æ': 'e',
+                      'ä': '_a', 'ë': '_e', 'ï': '_i',  'ö': '_o', 'ã': 'á', 'õ': 'ó',
+                      'â': 'a', 'ê': 'e', 'î': 'i', 'ô': 'o', 'û': 'u', 'ç': 'θ'}
+        raw_sentence = raw_sentence.lower()
+        for char in letters:
+            if re.search(rf'\b{char}\b', raw_sentence):
+                raw_sentence = re.sub(rf'\b{char}\b', letters[char], raw_sentence)
+        for match in letters:
+            raw_sentence = re.sub(rf'\b{match}\b', letters[char], raw_sentence)
+        for char in symbols:
+            if char in raw_sentence:
+                raw_sentence = raw_sentence.replace(char, ' ')
+        for char in diacritics:
+            if char in raw_sentence:
+                raw_sentence = raw_sentence.replace(char, letters[char])
+        if epen:
+            raw_sentence = re.sub(r'\bs((?![aeiouáéíóú]))', r'es\1', raw_sentence)
+        return raw_sentence
 
-    def __letters(self, sentence, epenthesis):
-        sentence = self.__clean(sentence.lower(), epenthesis)
-        letters = {'b': 'be', 'c': 'ce', 'd': 'de', 'f': 'efe', 'g': 'ge',
-                   'h': 'hache', 'j': 'jota', 'k': 'ka', 'l': 'ele',
-                   'm': 'eme', 'n': 'ene', 'p': 'pe', 'q': 'ku',
-                   'r': 'erre', 's': 'ese', 't': 'te', 'v': 'ube',
-                   'w': 'ubedoble', 'x': 'ekis', 'z': 'ceta', 'ph': 'peache'}
-        for letter in letters:
-            sentence = re.sub(rf'\b{letter}\b', 'letters[letter]', sentence)
+    @staticmethod
+    def make_rehash(sentence):
+        vowels = 'aeioujwăĕŏ'
+        for idx, syllable in enumerate(sentence):
+            if idx > 0:
+                if syllable[0].lower() in vowels and sentence[idx-1][-1] not in vowels:
+                    sentence[idx] = sentence[idx -1][-1] + syllable
+                    sentence[idx -1] = sentence[idx -1][:-1]
         return sentence
 
     def transcription_fnl(self, sentence, mono, aspiration):
-        diacritics = {'á': 'a', 'à': 'a', 'ä': 'a',
-                      'é': 'e', 'è': 'e', 'ë': 'e',
-                      'í': 'i', 'ì': 'i', 'ï': 'i',
-                      'ó': 'o', 'ò': 'o', 'ö': 'o',
-                      'ú': 'u', 'ù': 'u', 'ü': 'u',
-                      '_': ''}
-
-        consonants = {'w': 'b', 'v': 'b', 'z': 'θ', 'x': 'ks', 'j': 'x',
-                      'ñ': 'ɲ', 'qu': 'k', 'll': 'ʎ', 'ch': 'ʧ',
-                      'r': 'ɾ', 'R': 'r',
-                      'ce': 'θe', 'cé': 'θé', 'cë': 'θë',
-                      'ci': 'θi', 'cí': 'θí', 'cï': 'θï', 'cj': 'θj',
-                      'c': 'k', 'ph': 'f'}
-        sentence = re.sub(r'(?:([nls])r|rr|\br)', r'\1R', sentence)
-        sentence = sentence.replace('r', 'ɾ')
-        sentence = re.sub(r'\bh', 'ʰ', sentence)
+        diacritics = {'á': 'a', 'à': 'a', 'ä': 'a', 'é': 'e', 'è': 'e', 'ë': 'e',
+                      'ú': 'u', 'ù': 'u',  'ü': 'u', 'í': 'i', 'ì': 'i', 'ï': 'i',
+                      'ó': 'o', 'ò': 'o', 'ö': 'o',  '_': ''}
+        consonants = {'w': 'b', 'v': 'b', 'z': 'θ', 'ñ': 'ɲ', 'x': 'ks', 'j': 'x',
+                      'r': 'ɾ', 'R': 'r', 'ce': 'θe', 'cé': 'θé', 'cë': 'θë',
+                      'ci': 'θi', 'cí': 'θí', 'cï': 'θï', 'cj': 'θj', 'ch': 'ʧ',
+                      'c': 'k', 'qu': 'k', 'll': 'ʎ', 'ph': 'f', 'h': ''}
+        sentence = re.sub(r'(?:([nls])r|\br|rr)', r'\1R', sentence)
+        if aspiration:
+            sentence = re.sub(r'\bh', 'ʰ', sentence)
         for consonant in consonants:
             if consonant in sentence:
                 sentence = sentence.replace(consonant, consonants[consonant])
-        if aspiration:
-            sentence = re.sub(r'\bh', 'ʰ', sentence)
-        sentence = sentence.replace('h', '')
         if 'y' in sentence:
             sentence = re.sub(r'\by\b', 'i', sentence)
             sentence = re.sub(r'y\b', 'j', sentence)
             sentence = sentence.replace('y', 'ʝ')
             for key, value in diacritics.items():
                 if key in 'áéíóú':
                     sentence = re.sub(rf'{value}ʝ\b', f'{key}i', sentence)
-            # sentence = re.sub(r'y', 'ʝ', sentence)
-            # sentence = re.sub(r'ʝ\b', 'i', sentence)
             sentence = re.sub(r'ʝ((?![aeiouáéíóú]))', r'i\1', sentence)
         if 'g' in sentence:
-            for reg in [
-                [r'g([eiéíiëï])', rf'x\1'],
-                    [r'g[u]([eiéíëï])', rf'g\1']]:
+            for reg in [[r'g([eiéíiëï])', rf'x\1'], [r'g[u]([eiéíëï])', rf'g\1']]:
                 sentence = re.sub(reg[0], reg[1], sentence)
             sentence = re.sub(r'gü([ei])', r'gw\1', sentence)
             sentence = re.sub(r'gu([ao])', r'gw\1', sentence)
         transcription = self.__split_variables(sentence, mono)
-        words = transcription['words']
-        syllables = transcription['syllables']
         for letter in diacritics:
-            words = [word.replace(letter, diacritics[letter])
-                     for word in words]
-            syllables = [syllable.replace(letter, diacritics[letter]) for
-                         syllable in syllables]
-        return Values(words, syllables)
-
-    @staticmethod
-    def ipa2sampa(ipa, sampastr):
-        ipa = Values(ipa.words.copy(), ipa.syllables.copy())
-        transliteration = {'a': 'a', 'e': 'e', 'i': 'i', 'o': 'o', 'u': 'u',
-                           'j': 'j', 'w': 'w',
-                           'b': 'b', 'β': 'B', 'd': 'd', 'ð': 'D',
-                           'g': 'g', 'ɣ': 'G',
-                           'p': 'p', 't': 't', 'k': 'k',
-                           'l': 'l', 'ʎ': 'L', 'r': 'rr', 'ɾ': 'r',
-                           'm': 'm', 'ɱ': 'M', 'n': 'n', 'ŋ': 'N', 'ɲ': 'J',
-                           'ʧ': 'tS', 'ʝ': 'y', 'x': 'x', 'χ': '4',
-                           'f': 'f', 's': 's', 'z': 'z', 'θ': 'T',
-                           'ˈ': sampastr, 'ˌ': '%'}
-
-        for symbol in transliteration:
-            for idx, word in enumerate(ipa.words):
-                ipa.words[idx] = word.replace(symbol, transliteration[symbol])
-            for idx, syllable in enumerate(ipa.syllables):
-                ipa.syllables[idx] = syllable.replace(symbol,
-                                                      transliteration[symbol])
-        return ipa
+            transcription.words = [word.replace(letter, diacritics[letter])
+                                   for word in transcription.words]
+            transcription.syllables = [syllable.replace(letter, diacritics[letter])
+                                       for syllable in transcription.syllables]
+        return transcription
 
     def __split_variables(self, sentence, mono):
-        syllabic = []
         words = []
+        syllables_sentence = []
         for word in sentence.split():
             if len(word) > 5 and word.endswith('mente'):
-                syllabification = silabeador.syllabification(
-                    word[:-5], True, True)
+                syllabification = Syllabification(word[:-5], True, True)
                 syllables = syllabification.syllables
                 if len(syllables) > 1:
                     syllables = syllables + ['ˌmen', 'te']
                     stress = syllabification.stress - 2
                     word = word.replace('mente', 'ˌmente')
                 else:
-                    syllables = syllables + ["ˈmen", 'te']
+                    syllables = syllables + ['ˈmen', 'te']
                     stress = -2
             else:
-                syllabification = silabeador.syllabification(word, True, True)
+                syllabification = Syllabification(word, True, True)
                 syllables = syllabification.syllables
                 stress = syllabification.stress
-            conta = 0
-            diph = self.__diphthongs(word, syllables)
-            word = diph['word']
-            syllables = diph['syllables']
-            syllables[stress] = f"ˈ{syllables[stress]}"
-            for idx, slb in enumerate(syllables):
-                for char in slb:
-                    if char == "ˈ":
-                        word = word[:conta] + "ˈ" + word[conta:]
-                    else:
-                        conta += 1
-            for idx, syllable in enumerate(syllables):
+            syllables = self.__diphthongs(word, syllables)
+            syllables[stress] = f'ˈ{syllables[stress]}'
+            word = ''
+            for syllable in syllables:
                 if not mono and len(syllables) == 1:
-                    syllable = syllable.strip("ˈ")
-                syllabic += [syllable]
-            if len(syllables) == 1 and not mono:
-                word = word.replace('ˈ', '')
-            words += [word]
-        return {'words': words, 'syllables': syllabic}
+                    syllable = syllable.strip('ˈ')
+                syllables_sentence.append(syllable)
+                word += syllable
+            words.append(word)
+        return Values(words, syllables_sentence)
+
+    def __diphthongs(self, word, syllables):
+        for idx, syllable in enumerate(syllables):
+            if re.search(r'[aeiouáéó][ui]', syllable):
+                syllable = re.sub(r'([aeouáéó])i', r'\1j', syllable)
+                syllable = re.sub(r'([aeioáéó])u', r'\1w', syllable)
+            if re.search(r'[ui][aeiouáéó]', syllable):
+                syllable = re.sub(r'i([aeoáéó])', r'j\1', syllable)
+                syllable = re.sub(r'u([aeoáéó])', r'w\1', syllable)
+            syllables[idx] = syllable
+        return syllables
+
+    def transcription_fnt(self, phonology):
+        words = ' '.join(phonology.words)
+        syllables = '-'.join(phonology.syllables)
+        return Values(self.__fsubstitute(words), self.__fsubstitute(syllables))
 
     @staticmethod
     def __fsubstitute(words):
         words = words.replace('b', 'β').replace('d', 'ð').replace('g', 'ɣ')
         words = re.sub(r'([mnɲ ^])(\-*)β', r'\1\2b', words)
         words = re.sub(r'([mnɲlʎ ^])(\-*)ð', r'\1\2d', words)
         words = re.sub(r'([mnɲ ^])(\-*)ɣ', r'\1\2g', words)
         words = re.sub(r'θ(\-*)([bdgβðɣmnɲlʎrɾ])', r'ð\1\2', words)
         words = re.sub(r's(\-*)([bdgβðɣmnɲlʎrɾ])', r'z\1\2', words)
         words = re.sub(r'f(\-*)([bdgβðɣmnɲʎ])', r'v\1\2', words)
-        allophones = {'nb': 'mb', 'nˈb': 'mˈb',
-                      'nf': 'ɱf', 'nˈf': 'ɱˈf',
-                      'nk': 'ŋk', 'nˈk': 'ŋˈk',
-                      'ng': 'ŋg', 'nˈg': 'ŋˈg',
-                      'nx': 'ŋx', 'nˈx': 'ŋˈx',
-                      'xu': 'χu', 'xo': 'χo', 'xw': 'χw',
-                      'n-b': 'm-b', 'n-ˈb': 'm-ˈb',
-                      'n-f': 'ɱ-f', 'n-ˈf': 'ɱ-ˈf',
-                      'n-k': 'ŋ-k', 'n-ˈk': 'ŋ-ˈk',
-                      'n-g': 'ŋ-g', 'n-ˈg': 'ŋ-ˈg',
-                      'n-x': 'ŋ-x', 'n-ˈx': 'ŋ-ˈx'
-                      }
+        allophones = {'nb': 'mb', 'nˈb': 'mˈb', 'nf': 'ɱf', 'nˈf': 'ɱˈf',
+                      'nk': 'ŋk', 'nˈk': 'ŋˈk', 'ng': 'ŋg', 'nˈg': 'ŋˈg',
+                      'nx': 'ŋx', 'nˈx': 'ŋˈx', 'xu': 'χu', 'xo': 'χo', 'xw': 'χw',
+                      'n-b': 'm-b', 'n-ˈb': 'm-ˈb', 'n-f': 'ɱ-f', 'n-ˈf': 'ɱ-ˈf',
+                      'n-k': 'ŋ-k', 'n-ˈk': 'ŋ-ˈk', 'n-g': 'ŋ-g', 'n-ˈg': 'ŋ-ˈg',
+                      'n-x': 'ŋ-x', 'n-ˈx': 'ŋ-ˈx'}
         if any(allophone in words for allophone in allophones):
             for allophone in allophones:
                 words = words.replace(allophone, allophones[allophone])
-        return words.replace('-', ' ')
-
-    def transcription_fnt(self, phonology):
-        words = ' '.join(phonology.words)
-        syllables = '-'.join(phonology.syllables)
-        words = self.__fsubstitute(words)
-        syllables = self.__fsubstitute(syllables)
-        return Values(self.__fsubstitute(words).split(),
-                      self.__fsubstitute(syllables).split())
+        return words.replace('-', ' ').split()
 
     @staticmethod
-    def __replace_ocurrence(string, origin, to, num):
-        strange_char = '$&$@$$&'
-        if string.count(origin) < 0:
-            return string
-        elif string.count(origin) > 1:
-            return string.replace(origin, strange_char, num).replace(
-                strange_char, origin, num-1).replace(to, strange_char, 1)
-        else:
-            return string.replace(origin, to)
-
-    def __diphthongs(self, word, syllables):
-        i = 0
-        j = 0
-        for idx, syllable in enumerate(syllables):
-            if re.search(r'[aeiouáéíóú]{2,}', syllable):
-                i += 1
-                syllable = re.sub(r'([aeoáééóú])i', r'\1j', syllable)
-                syllable = re.sub(r'([aeoáééóú])u', r'\1w', syllable)
-                word = self.__replace_ocurrence(word,
-                                                syllables[idx],
-                                                syllable, i)
-            if re.search(r'[ui][aeiouáééiíóú]', syllable):
-                j += 1
-                syllable = re.sub(r'i([aeouáééiíóú])', r'j\1', syllable)
-                syllable = re.sub(r'u([aeioáééiíóú])', r'w\1', syllable)
-                word = self.__replace_ocurrence(word,
-                                                syllables[idx],
-                                                syllable, j)
-            syllables[idx] = syllable
-        return {'word': word, 'syllables': syllables}
+    def ipa2sampa(ipa, sampastr):
+        ipa = Values(ipa.words.copy(), ipa.syllables.copy())
+        transliteration = {'β': 'B', 'ð': 'D', 'ɣ': 'G', 'ʎ': 'L', 'r': 'rr',
+                           'ɾ': 'r', 'ɱ': 'M', 'ŋ': 'N', 'ɲ': 'J', 'ʧ': 'tS',
+                           'ʝ': 'y', 'χ': '4', 'θ': 'T', 'ˈ': sampastr, 'ˌ': '%'}
+        for symbol in transliteration:
+            for idx, word in enumerate(ipa.words):
+                ipa.words[idx] = word.replace(symbol, transliteration[symbol])
+            for idx, syllable in enumerate(ipa.syllables):
+                ipa.syllables[idx] = syllable.replace(symbol, transliteration[symbol])
+        return ipa
```

### Comparing `fonemas-2.0.7/fonemas.egg-info/PKG-INFO` & `fonemas-2.0.9/fonemas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fonemas
-Version: 2.0.7
+Version: 2.0.9
 Summary: Phonetic transcription of Spanish
 Home-page: https://github.com/fsanzl/fonemas
 Author: Fernando Sanz-Lázaro
 Author-email: fsanzl@gmail.com
 License: LGPL
 Project-URL: Source, https://github.com/fsanzl/fonemas/
 Project-URL: Tracker, https://github.com/fsanzl/fonemas/issues
 Description: [![License: LGPL](https://img.shields.io/github/license/fsanzl/fonemas)](https://opensource.org/licenses/LGPL-2.1)
-        [![Version: 2.0.7](https://img.shields.io/github/v/release/fsanzl/fonemas)](https://pypi.org/project/fonemas/)
+        [![Version: 2.0.9](https://img.shields.io/github/v/release/fsanzl/fonemas)](https://pypi.org/project/fonemas/)
         [![Python versions: 3.5, 3.6, 3.7, 3.8, 3.9](https://img.shields.io/pypi/pyversions/fonemas)](https://pypi.org/project/fonemas/)
         
         
         <h2 align="center">Fonemas</h2>
         <h3 align="center">A Python phonologic transcription library for Spanish</h2>
         
         
@@ -25,22 +25,24 @@
         
         ```bash
         pip3 install fonemas
         ```
         
         ## Use
         
-        The library provides the class  *transcription(sentence, mono, epenthesis, aspiration, sampastr)*. The class takes the obligatoy argument *sentence*, which is a string of characters with a Spanish word or words. It optionally takes two Boolean arguments *mono*,  *epenthesis* and *aspiration* set to False as default.
+        The library provides the class  *transcription(sentence, mono, epenthesis, aspiration, rehash, sampastr)*. The class takes the obligatoy argument *sentence*, which is a string of characters with a Spanish word or words. It optionally takes two Boolean arguments *mono*,  *epenthesis* and *aspiration* set to False as default.
         
         - *mono* sets whether the output shows graphic stresses for monosyllabic words
         
         - *epenthesis* set the behaviour S bfore consonant in onset (spiritu -> es pi ri tu|spi ri tu)
         
         - *aspiration* inserts an aspiration modifier 'ʰ' in onset. This may be useful when dealing with ambiguous verses in classic poetry to choose which synaloepha to break.
         
+        - *rehash* moves last consonan on last-syllable coda to next's words first-syllable onset if it begins with a vowel.
+        
         - *sampastr* allows an alternativestress symbol, as '"' to prevent issues e.g. when using in a CSV file.
         
         
         
         The class *transcription()* has three dataclass attributes, each with two attributes *{words, syllables}* containing each a list of strings, which may be words or syllables, respectively.
         
         - *phonology* for the phonological transcription (requires UNICODE support).
```

### Comparing `fonemas-2.0.7/setup.py` & `fonemas-2.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 install_requires = ['silabeador']
 
 
 # This call to setup() does all the work
 setup(
     name="fonemas",
-    version="2.0.7",
+    version="2.0.9",
     python_requires='>=3.5',
     description="Phonetic transcription of Spanish",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/fsanzl/fonemas",
     project_urls={
         'Source': 'https://github.com/fsanzl/fonemas/',
```

