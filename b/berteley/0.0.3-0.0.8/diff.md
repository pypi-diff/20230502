# Comparing `tmp/berteley-0.0.3.tar.gz` & `tmp/berteley-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berteley-0.0.3.tar", last modified: Tue Apr 25 22:40:01 2023, max compression
+gzip compressed data, was "berteley-0.0.8.tar", last modified: Tue May  2 16:29:39 2023, max compression
```

## Comparing `berteley-0.0.3.tar` & `berteley-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:40:01.752371 berteley-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 22:39:51.000000 berteley-0.0.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-25 22:39:51.000000 berteley-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-25 22:39:51.000000 berteley-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-25 22:40:01.752371 berteley-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-25 22:39:51.000000 berteley-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:40:01.756371 berteley-0.0.3/berteley/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 22:39:51.000000 berteley-0.0.3/berteley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 22:40:01.756371 berteley-0.0.3/berteley/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-25 22:39:51.000000 berteley-0.0.3/berteley/berteley.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-25 22:39:51.000000 berteley-0.0.3/berteley/berteley_stopwords.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-04-25 22:39:51.000000 berteley-0.0.3/berteley/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 22:39:51.000000 berteley-0.0.3/berteley/recommendation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:40:01.752371 berteley-0.0.3/berteley.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-25 22:40:01.000000 berteley-0.0.3/berteley.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-25 22:40:01.000000 berteley-0.0.3/berteley.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:40:01.000000 berteley-0.0.3/berteley.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:40:01.000000 berteley-0.0.3/berteley.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-25 22:40:01.000000 berteley-0.0.3/berteley.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 22:40:01.000000 berteley-0.0.3/berteley.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:40:01.752371 berteley-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-25 22:39:51.000000 berteley-0.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-25 22:39:51.000000 berteley-0.0.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:40:01.752371 berteley-0.0.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-25 22:39:51.000000 berteley-0.0.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-25 22:40:01.752371 berteley-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-25 22:39:51.000000 berteley-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:40:01.752371 berteley-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 22:39:51.000000 berteley-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-25 22:39:51.000000 berteley-0.0.3/tests/test_berteley.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-25 22:39:51.000000 berteley-0.0.3/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 22:39:51.000000 berteley-0.0.3/tests/test_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-25 22:39:51.000000 berteley-0.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:39.364173 berteley-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 16:29:29.000000 berteley-0.0.8/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-02 16:29:29.000000 berteley-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-02 16:29:29.000000 berteley-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-02 16:29:39.364173 berteley-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-02 16:29:29.000000 berteley-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:39.364173 berteley-0.0.8/berteley/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 16:29:29.000000 berteley-0.0.8/berteley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-02 16:29:39.364173 berteley-0.0.8/berteley/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-02 16:29:29.000000 berteley-0.0.8/berteley/berteley_stopwords.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-05-02 16:29:29.000000 berteley-0.0.8/berteley/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-05-02 16:29:29.000000 berteley-0.0.8/berteley/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:29.000000 berteley-0.0.8/berteley/recommendation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:39.360169 berteley-0.0.8/berteley.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-02 16:29:39.000000 berteley-0.0.8/berteley.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-02 16:29:39.000000 berteley-0.0.8/berteley.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:29:39.000000 berteley-0.0.8/berteley.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:29:39.000000 berteley-0.0.8/berteley.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-02 16:29:39.000000 berteley-0.0.8/berteley.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 16:29:39.000000 berteley-0.0.8/berteley.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:39.360169 berteley-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-02 16:29:29.000000 berteley-0.0.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-02 16:29:29.000000 berteley-0.0.8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:39.364173 berteley-0.0.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-02 16:29:29.000000 berteley-0.0.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 16:29:39.364173 berteley-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-02 16:29:29.000000 berteley-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:39.364173 berteley-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:29:29.000000 berteley-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-02 16:29:29.000000 berteley-0.0.8/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-02 16:29:29.000000 berteley-0.0.8/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:29.000000 berteley-0.0.8/tests/test_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-02 16:29:29.000000 berteley-0.0.8/versioneer.py
```

### Comparing `berteley-0.0.3/LICENSE` & `berteley-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `berteley-0.0.3/PKG-INFO` & `berteley-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: berteley
-Version: 0.0.3
+Version: 0.0.8
 Summary: Topic modeling for scientific articles
 Home-page: https://github.com/lbl-camera/berteley
-Author: Eric Chagnon
+Author: Eric Chagnon, Ronald J. Pandolfi, Daniela Ushizima
 Author-email: echagnon@lbl.gov
 License: BSD license
 Keywords: berteley
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.8
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # BERTeley
```

### Comparing `berteley-0.0.3/README.md` & `berteley-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `berteley-0.0.3/berteley/berteley.py` & `berteley-0.0.8/berteley/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 
 
 def initialize_model(embedding_model: Union[SentenceTransformer, str] = "specter",
                      nr_topics: int = None,
                      n_gram_type: str = "unigram",
                      verbose="False"):
     """
-        Fits a BERTopic model on the data. After fitting the topic assigned to each document is stored
-        in the 'topics' attribute, the coherence and diversity measures are stored in the
-        'coherence' and 'diversity' attributes respectively, and the amount of documents assigned to each topic
-        are stored in the 'topic_sizes' attribute.
+        Conducts type checks on the input variables and converts certain parameters to the proper types dependent on their input.
+        Not intended to be called by the user, but instead used internally by the fit function.
 
 
         Parameters
         ----------
         embedding_model
                 Either a SentenceTransformer, or a string with values "specter". "aspire", or "scibert".
         nr_topics
@@ -34,15 +32,18 @@
         n_gram_type
                 String indicating whether the user would like unigram or bigram.
         verbose
                 Boolean indicating verbose output.
 
         Returns
         -------
-        The function sets attributes for topics, probabilities, and metrics.
+        embedding_model
+                SentenceTransformer language model
+        n_gram_range
+                tuple indicating the level of n_gram
             """
 
     if not isinstance(nr_topics, int) and nr_topics is not None:
         raise TypeError("nr_topics must be an int")
     if not isinstance(n_gram_type, str) and n_gram_type is not None:
         raise TypeError("n_gram_type must be an string")
     if not isinstance(verbose, bool) and nr_topics is not None:
@@ -102,32 +103,44 @@
         n_gram_type
                 String indicating whether the user would like unigram or bigram.
         verbose
                 Boolean indicating verbose output.
 
         Returns
         -------
-        The function sets attributes for topics, probabilities, and metrics.
-            """
+        topics
+                a list of integers representing the topic the corresponding document was assigned to
+        probabilities
+                a
+        metrics
+                a dictionary of the 2 metrics with keys "Coherence" and "Diversity"
+        topic_sizes
+                a dictionary with key: topic number and the value: the number of documents assigned the said topic
+        topic_model
+                the fitted BERTopic model
+        topic_words
+                a dictionary with key: the topic number and the value: a list of strings
+        """
 
     if not isinstance(embedding_model, SentenceTransformer) and not isinstance(n_gram_type, tuple):
         embedding_model, n_gram_range = initialize_model(embedding_model, nr_topics, n_gram_type, verbose)
 
     if not isinstance(data, list) or (isinstance(data, list) and not isinstance(data[0], str)):
         raise TypeError("Data must be a list of strings")
 
     topic_model = BERTopic(embedding_model=embedding_model,
                            nr_topics=nr_topics,
                            n_gram_range=n_gram_range,
                            verbose=verbose)
     topics, probabilities = topic_model.fit_transform(data)
     metrics = _calculate_metrics(data, topic_model, topics, n_gram_range)
     topic_sizes = _calculate_topic_sizes(topics)
+    topic_words = topic_model.topic_representations_
 
-    return topics, probabilities, metrics, topic_sizes, topic_model
+    return topics, probabilities, metrics, topic_sizes, topic_model, topic_words
 
 
 def _calculate_topic_sizes(topics: List[int]):
     """
     counts the number of documents assigned to each topic and stores the topic sizes in the 'topic_sizes'
     attribute in the form of a dict.
 
@@ -250,14 +263,18 @@
 
 def create_barcharts(topics, topic_model: BERTopic, path=""):
     """
     creates and saves the BERTopic barcharts
 
     Parameters
     ----------
+    topics
+            the list of topic assignments output from the fit function
+    topic_model
+            fitted BERTopic model output from the fit function
     path
         A string containing the desired path to save the barchart
 
     Returns
     -------
     Barcharts are saved in .html and .png format in the desired directory.
```

### Comparing `berteley-0.0.3/berteley/preprocessing.py` & `berteley-0.0.8/berteley/preprocessing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+import contextlib
 import re
 import string
+from functools import partial
 import spacy
 import numpy as np
 from nltk.tokenize import word_tokenize
 import nltk
 from nltk.corpus import stopwords
 from bs4 import BeautifulSoup
 import contractions
-from joblib import delayed, Parallel
+from joblib import delayed, Parallel, parallel
 import csv
 from pathlib import Path
 import subprocess
+from alive_progress import alive_it, alive_bar
 
 from typing import List
 
 nltk.download('stopwords')
 try:
     nlp = spacy.load('en_core_web_lg')
 except OSError:
@@ -23,14 +26,15 @@
 
 here = Path(__file__).parent
 file = open(here / "berteley_stopwords.csv", "r")
 
 data = list(csv.reader(file, delimiter=","))
 
 STOPWORDS = [x[0] for x in data]
+NLTK_STOPWORDS = set(stopwords.words('english'))
 
 
 def combine_hyphens(doc: str):
     """
     Removes hyphens and concatenates all hyphenated words together
 
     Parameters
@@ -124,15 +128,15 @@
     if not isinstance(allow_abbrev, bool):
         raise TypeError("allow_abbrev must be a boolean")
 
     filt_combined = []
 
     for word in word_tokenize(doc):
         contains_letter = re.search('[a-zA-Z]', word) is not None
-        stopword_check = word.lower() not in stopwords.words('english')
+        stopword_check = word.lower() not in NLTK_STOPWORDS
         berteley_stopword_check = word.lower() not in STOPWORDS
 
         if contains_letter and stopword_check and berteley_stopword_check:
             if not allow_abbrev:
                 if len(word.lower()) > 2:
                     filt_combined.append(word)
 
@@ -191,95 +195,109 @@
 
     Examples
     won't -> will not
     """
     return contractions.fix(doc)
 
 
-def preprocess(docs: List[str], allow_abbrev: bool = True):
+def _identity(doc):
+    return doc
+
+
+def _map_docs(docs, func, filter=lambda doc: True):
+    return [func(doc) for doc in docs if filter(doc)]
+
+
+def preprocess(docs: List[str], allow_abbrev: bool = True, show_progress:bool=False) -> List[str]:
     """
     Wrapper function for all the preprocessing steps
 
     Parameters
     ----------
     docs
         A list of all the documents
     allow_abbrev
         Boolean indicating whether abbreviations should be allowed. If set to false all strings with length 2 or less will be removed
+    show_progress
+        If True, shows a progress bar for completion status
 
     Returns
     -------
     A list of strings that have been preprocessed
     """
 
-    # remove all empty strings
-    docs = list(filter(len, docs))
-
-    # remove all html tags
-    cleaned_docs = [remove_html(s) for s in docs]
-
-    # remove/change numbers
-
-    # expand contractions (don't -> do not)
-    cleaned_docs = [expand_contractions(s) for s in cleaned_docs]
+    cleaned_docs = docs.copy()
 
-    # lower case
-    cleaned_docs = [s.lower() for s in cleaned_docs]
+    steps = [('Removing empty strings...', _identity, len),
+             ('Removing all html tags...', remove_html),
+             ('Expanding contractions...', expand_contractions), # don't -> do not
+             ('Converting to lower case...', str.lower),
+             ('Removing all punctuation...', remove_punctuation), # make sure hyphenated words are properly combined and grammatical hyphens are spaced appropriately
+             ('Removing extra whitespace...', remove_extraspace),
+             ('Removing empty strings...', _identity, len),
+             ('Lemmatizing...', lemmatize),
+             ('Removing stopwords...', partial(remove_stopwords, allow_abbrev=allow_abbrev)),
+             ('Removing short strings', _identity, lambda doc: len(doc.split()) > 10)
+             ]
+
+    iterator = alive_it if show_progress else iter
+    bar = iterator(steps)
+    for title, func, *filter in bar:
+        if show_progress:
+            bar.title(title)
+        cleaned_docs = _map_docs(cleaned_docs, func, **{'filter': filter[0]} if filter else {})
 
-    # remove all punctuation (make sure hyphenated words are properly combined
-    # and grammatical hyphens are spaced appropriately)
-    cleaned_docs = [remove_punctuation(s) for s in cleaned_docs]
-
-    # remove excess white space
-
-    cleaned_docs = [remove_extraspace(s) for s in cleaned_docs]
-
-    # remove empty strings again
-    cleaned_docs = list(filter(len, cleaned_docs))
-
-    # lemmatize
-    cleaned_docs = [lemmatize(s) for s in cleaned_docs]
-
-    # remove stopwords
-    cleaned_docs = [remove_stopwords(s, allow_abbrev=allow_abbrev) for s in cleaned_docs]
+    return cleaned_docs
 
-    # remove strings with small length
-    cleaned_docs = [s for s in cleaned_docs if len(s.split()) > 10]
 
-    return cleaned_docs
+@contextlib.contextmanager
+def alive_bar_joblib(bar):
+    """Context manager to patch joblib to report into progress bar given as argument"""
+    class AliveBatchCompletionCallback(parallel.BatchCompletionCallBack):
+        def __call__(self, *args, **kwargs):
+            if bar and not isinstance(bar, contextlib.nullcontext):
+                for i in range(self.batch_size):
+                    bar()
+            return super().__call__(*args, **kwargs)
+
+    old_batch_callback = parallel.BatchCompletionCallBack
+    parallel.BatchCompletionCallBack = AliveBatchCompletionCallback
+    try:
+        yield bar
+    finally:
+        parallel.BatchCompletionCallBack = old_batch_callback
 
 
-def preprocess_parallel(docs: List[str], n_workers: int = 4, allow_abbrev: bool = True):
+def preprocess_parallel(docs: List[str], n_workers: int = 4, allow_abbrev: bool = True, show_progress: bool=True) -> List[str]:
     """
     Parallelizes the preprocessing by splitting the documents evenly amongst the n_workers
 
     Parameters
     ----------
     docs
         List of documents
     n_workers
         Number of workers to be assigned preprocessing in joblib
 
     allow_abbrev
         Boolean indicating whether abbreviations should be allowed. If set to false all strings with length
         2 or less will be removed
 
+    show_progress: bool
+        If True, shows a progress bar for completion status
 
     Returns
     -------
     A list of strings that have been preprocessed
 
     """
     # remove all empty strings
     docs = list(filter(len, docs))
 
-    # split the docs equally among the workers
-    partitions = np.array_split(docs, n_workers)
-
-    # docs must be a list of strings
-    partitions = [list(p) for p in partitions]
-
-    clean_docs = Parallel(n_jobs=n_workers)(delayed(preprocess)(p, allow_abbrev) for p in partitions)
+    with alive_bar(len(docs)) if show_progress else contextlib.nullcontext() as bar:
+        with alive_bar_joblib(bar):
+            clean_docs = Parallel(n_jobs=n_workers)(delayed(preprocess)([doc], allow_abbrev, show_progress=False)
+                                                for doc in docs)
     # flatten the list of lists into a single list
     clean_docs = [item for sublist in clean_docs for item in sublist]
 
     return clean_docs
```

### Comparing `berteley-0.0.3/berteley.egg-info/PKG-INFO` & `berteley-0.0.8/berteley.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: berteley
-Version: 0.0.3
+Version: 0.0.8
 Summary: Topic modeling for scientific articles
 Home-page: https://github.com/lbl-camera/berteley
-Author: Eric Chagnon
+Author: Eric Chagnon, Ronald J. Pandolfi, Daniela Ushizima
 Author-email: echagnon@lbl.gov
 License: BSD license
 Keywords: berteley
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.8
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # BERTeley
```

### Comparing `berteley-0.0.3/berteley.egg-info/SOURCES.txt` & `berteley-0.0.8/berteley.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 berteley/__init__.py
 berteley/_version.py
-berteley/berteley.py
 berteley/berteley_stopwords.csv
+berteley/models.py
 berteley/preprocessing.py
 berteley/recommendation.py
 berteley.egg-info/PKG-INFO
 berteley.egg-info/SOURCES.txt
 berteley.egg-info/dependency_links.txt
 berteley.egg-info/not-zip-safe
 berteley.egg-info/requires.txt
 berteley.egg-info/top_level.txt
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 tests/__init__.py
-tests/test_berteley.py
+tests/test_models.py
 tests/test_preprocessing.py
 tests/test_recommendation.py
```

### Comparing `berteley-0.0.3/docs/Makefile` & `berteley-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `berteley-0.0.3/docs/make.bat` & `berteley-0.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `berteley-0.0.3/docs/source/conf.py` & `berteley-0.0.8/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = []
 
 autoclass_content = 'both'
 
+add_module_names = False
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = 'sphinx_rtd_theme'
```

### Comparing `berteley-0.0.3/setup.py` & `berteley-0.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,35 +15,35 @@
     # Parse requirements.txt, ignoring any commented-out lines.
     requirements = [line for line in requirements_file.read().splitlines()
                     if not line.startswith('#')]
 
 with open(path.join(here, 'requirements-dev.txt')) as requirements_file:
     # Parse requirements.txt, ignoring any commented-out lines.
     dev = [line for line in requirements_file.read().splitlines()
-                    if not line.startswith('#')]
+           if not line.startswith('#')]
 
 with open(path.join(here, 'requirements-docs.txt')) as requirements_file:
     # Parse requirements.txt, ignoring any commented-out lines.
     docs = [line for line in requirements_file.read().splitlines()
-                    if not line.startswith('#')]
+            if not line.startswith('#')]
 
 setup(
-    author="Eric Chagnon",
-    author_email='echagnon@lbl.gov',
-    python_requires='>=3.8',
+    author="Eric Chagnon, Ronald J. Pandolfi, Daniela Ushizima",
+    author_email="echagnon@lbl.gov",
+    python_requires='>=3.8, <3.11',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: BSD License',
     ],
     description="Topic modeling for scientific articles",
     entry_points={
         'console_scripts': [
-            #'berteley=berteley:some_function',
+            # 'berteley=berteley:some_function',
         ],
     },
     install_requires=requirements,
     license="BSD license",
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
@@ -55,9 +55,9 @@
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     zip_safe=False,
     extras_require={
         'tests': dev,
         'docs': docs
     },
-    setup_requires = ["wheel"]
+    setup_requires=["wheel"]
 )
```

### Comparing `berteley-0.0.3/tests/test_berteley.py` & `berteley-0.0.8/tests/test_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import pytest
 import os
-from berteley import berteley
-import pandas as pd
-from sentence_transformers import SentenceTransformer
 from sklearn.datasets import fetch_20newsgroups
 import numpy as np
 
-from berteley.berteley import initialize_model
+from berteley.models import initialize_model, fit, create_barcharts
 
 # gets rid of extraneous warnings
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 
 @pytest.fixture
 def data():
     return fetch_20newsgroups(subset='all', remove=('headers', 'footers', 'quotes'))['data'][:100]
 
 
 @pytest.fixture
 def test(data):
     model = "specter"
-    topics, probabilities, metrics, topic_sizes, topic_model = berteley.fit(data, embedding_model=model, n_gram_type="bigram", verbose=True)
-    return {"topics": topics, "probs": probabilities,"metrics": metrics, "topic_sizes": topic_sizes, "topic_model": topic_model}
+    topics, probabilities, metrics, topic_sizes, topic_model, topic_words = fit(data, embedding_model=model, n_gram_type="bigram", verbose=True)
+    return {"topics": topics, "probs": probabilities,"metrics": metrics, "topic_sizes": topic_sizes, "topic_model": topic_model, "topic_words": topic_words}
 
 
 def test_berteley_init():
     # modelPath = "../bert-base-nli-mean-tokens"
     with pytest.raises(AttributeError):
         initialize_model(embedding_model="default")
 
@@ -38,28 +35,29 @@
     with pytest.raises(AttributeError):
         initialize_model(n_gram_type='2')
 
 
 def test_fit_input_type(data):
     df = {"data": data}
     with pytest.raises(TypeError):
-        berteley.fit(df, embedding_model="specter", n_gram_type="bigram", verbose=True)
+        fit(df, embedding_model="specter", n_gram_type="bigram", verbose=True)
 
 
 def test_fit_attributes(test):
     assert isinstance(test["topic_sizes"], dict)
     assert isinstance(test["metrics"]["Coherence"], np.float64)
     assert isinstance(test["metrics"]["Diversity"], float)
+    assert isinstance(test["topic_words"], dict)
 
 
 def test_figures(test, tmp_path):
     # os.remove(path + "barchart.html")
     # os.remove(path + "barchart.png")
     #test["topic_model"].visualize_barchart(path=tmp_path)
-    berteley.create_barcharts(test["topics"], test["topic_model"], path = str(tmp_path) + "/")
+    create_barcharts(test["topics"], test["topic_model"], path = str(tmp_path) + "/")
     # self.assertTrue(os.path.exists(path + "barchart.html"))
     # self.assertTrue(os.path.exists(path + "barchart.png"))
     assert os.path.exists(str(tmp_path) + "/" + "barchart.html")
     assert os.path.exists(str(tmp_path) + "/" + "barchart.png")
     with pytest.raises(TypeError):
         test["topic_model"].visualize_barchart(123)
```

### Comparing `berteley-0.0.3/tests/test_preprocessing.py` & `berteley-0.0.8/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `berteley-0.0.3/versioneer.py` & `berteley-0.0.8/versioneer.py`

 * *Files identical despite different names*

