# Comparing `tmp/text2term-2.1.0.tar.gz` & `tmp/text2term-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2term-2.1.0.tar", last modified: Mon Mar 27 17:47:41 2023, max compression
+gzip compressed data, was "text2term-2.2.0.tar", last modified: Tue May  2 13:43:38 2023, max compression
```

## Comparing `text2term-2.1.0.tar` & `text2term-2.2.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-03-27 17:47:41.269513 text2term-2.1.0/
--rw-r--r--   0 jason      (501) staff       (20)     1117 2022-08-03 13:24:07.000000 text2term-2.1.0/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)    13844 2023-03-27 17:47:41.269335 text2term-2.1.0/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)    13086 2023-03-27 17:45:54.000000 text2term-2.1.0/README.md
--rw-r--r--   0 jason      (501) staff       (20)       38 2023-03-27 17:47:41.269557 text2term-2.1.0/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1162 2023-03-27 17:45:54.000000 text2term-2.1.0/setup.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-03-27 17:47:41.268468 text2term-2.1.0/text2term/
--rw-r--r--   0 jason      (501) staff       (20)      406 2023-02-24 16:05:08.000000 text2term-2.1.0/text2term/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     4321 2022-11-15 20:43:11.000000 text2term-2.1.0/text2term/__main__.py
--rw-r--r--   0 jason      (501) staff       (20)     4416 2022-08-03 13:24:07.000000 text2term-2.1.0/text2term/bioportal_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)       17 2023-03-27 17:45:54.000000 text2term-2.1.0/text2term/config.py
--rw-r--r--   0 jason      (501) staff       (20)      469 2022-09-26 14:42:08.000000 text2term-2.1.0/text2term/mapper.py
--rw-r--r--   0 jason      (501) staff       (20)     6692 2023-03-27 17:45:54.000000 text2term-2.1.0/text2term/onto_utils.py
--rw-r--r--   0 jason      (501) staff       (20)     5540 2023-03-27 17:45:54.000000 text2term-2.1.0/text2term/preprocess.py
--rw-r--r--   0 jason      (501) staff       (20)     5403 2023-02-09 15:42:55.000000 text2term-2.1.0/text2term/syntactic_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)    13104 2023-03-27 17:45:54.000000 text2term-2.1.0/text2term/t2t.py
--rw-r--r--   0 jason      (501) staff       (20)      741 2023-02-24 16:05:08.000000 text2term-2.1.0/text2term/tagged_terms.py
--rw-r--r--   0 jason      (501) staff       (20)     2358 2022-11-15 20:43:11.000000 text2term-2.1.0/text2term/term.py
--rw-r--r--   0 jason      (501) staff       (20)    15349 2023-01-20 15:17:36.000000 text2term-2.1.0/text2term/term_collector.py
--rw-r--r--   0 jason      (501) staff       (20)     2697 2022-08-03 13:24:07.000000 text2term-2.1.0/text2term/term_graph.py
--rw-r--r--   0 jason      (501) staff       (20)     2991 2023-01-20 15:17:36.000000 text2term-2.1.0/text2term/term_graph_generator.py
--rw-r--r--   0 jason      (501) staff       (20)     2072 2023-03-27 17:45:54.000000 text2term-2.1.0/text2term/term_mapping.py
--rw-r--r--   0 jason      (501) staff       (20)     5108 2022-11-15 20:43:11.000000 text2term-2.1.0/text2term/tfidf_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)     4098 2023-02-09 15:42:55.000000 text2term-2.1.0/text2term/zooma_mapper.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-03-27 17:47:41.269147 text2term-2.1.0/text2term.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)    13844 2023-03-27 17:47:41.000000 text2term-2.1.0/text2term.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      607 2023-03-27 17:47:41.000000 text2term-2.1.0/text2term.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2023-03-27 17:47:41.000000 text2term-2.1.0/text2term.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)      248 2023-03-27 17:47:41.000000 text2term-2.1.0/text2term.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)       10 2023-03-27 17:47:41.000000 text2term-2.1.0/text2term.egg-info/top_level.txt
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-02 13:43:38.272933 text2term-2.2.0/
+-rw-r--r--   0 jason      (501) staff       (20)     1117 2022-08-03 13:24:07.000000 text2term-2.2.0/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)    14370 2023-05-02 13:43:38.272744 text2term-2.2.0/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)    13612 2023-04-25 19:02:20.000000 text2term-2.2.0/README.md
+-rw-r--r--   0 jason      (501) staff       (20)       38 2023-05-02 13:43:38.272975 text2term-2.2.0/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1162 2023-03-27 17:45:54.000000 text2term-2.2.0/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-02 13:43:38.269621 text2term-2.2.0/test/
+-rw-r--r--   0 jason      (501) staff       (20)     1435 2023-04-25 18:43:12.000000 text2term-2.2.0/test/test-pypi.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-02 13:43:38.271887 text2term-2.2.0/text2term/
+-rw-r--r--   0 jason      (501) staff       (20)      406 2023-05-02 13:41:43.000000 text2term-2.2.0/text2term/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4540 2023-04-25 19:04:10.000000 text2term-2.2.0/text2term/__main__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4416 2022-08-03 13:24:07.000000 text2term-2.2.0/text2term/bioportal_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)       17 2023-04-17 18:05:11.000000 text2term-2.2.0/text2term/config.py
+-rw-r--r--   0 jason      (501) staff       (20)      469 2022-09-26 14:42:08.000000 text2term-2.2.0/text2term/mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)     6692 2023-03-27 17:45:54.000000 text2term-2.2.0/text2term/onto_utils.py
+-rw-r--r--   0 jason      (501) staff       (20)     5540 2023-03-27 17:45:54.000000 text2term-2.2.0/text2term/preprocess.py
+-rw-r--r--   0 jason      (501) staff       (20)     5403 2023-02-09 15:42:55.000000 text2term-2.2.0/text2term/syntactic_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)    13355 2023-05-02 13:41:43.000000 text2term-2.2.0/text2term/t2t.py
+-rw-r--r--   0 jason      (501) staff       (20)      741 2023-02-24 16:05:08.000000 text2term-2.2.0/text2term/tagged_terms.py
+-rw-r--r--   0 jason      (501) staff       (20)     2479 2023-04-18 15:25:34.000000 text2term-2.2.0/text2term/term.py
+-rw-r--r--   0 jason      (501) staff       (20)    16757 2023-05-02 13:41:43.000000 text2term-2.2.0/text2term/term_collector.py
+-rw-r--r--   0 jason      (501) staff       (20)     2697 2022-08-03 13:24:07.000000 text2term-2.2.0/text2term/term_graph.py
+-rw-r--r--   0 jason      (501) staff       (20)     2991 2023-01-20 15:17:36.000000 text2term-2.2.0/text2term/term_graph_generator.py
+-rw-r--r--   0 jason      (501) staff       (20)     2158 2023-04-11 13:56:32.000000 text2term-2.2.0/text2term/term_mapping.py
+-rw-r--r--   0 jason      (501) staff       (20)     5108 2022-11-15 20:43:11.000000 text2term-2.2.0/text2term/tfidf_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)     4098 2023-02-09 15:42:55.000000 text2term-2.2.0/text2term/zooma_mapper.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-02 13:43:38.272562 text2term-2.2.0/text2term.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)    14370 2023-05-02 13:43:38.000000 text2term-2.2.0/text2term.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      625 2023-05-02 13:43:38.000000 text2term-2.2.0/text2term.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2023-05-02 13:43:38.000000 text2term-2.2.0/text2term.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)      248 2023-05-02 13:43:38.000000 text2term-2.2.0/text2term.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)       10 2023-05-02 13:43:38.000000 text2term-2.2.0/text2term.egg-info/top_level.txt
```

### Comparing `text2term-2.1.0/LICENSE` & `text2term-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `text2term-2.1.0/PKG-INFO` & `text2term-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2term
-Version: 2.1.0
+Version: 2.2.0
 Summary: A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies
 Home-page: https://github.com/ccb-hms/ontology-mapper
 Author: Center for Computational Biomedicine, Harvard Medical School
 Author-email: rafael_goncalves@hms.harvard.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,53 @@
 
 ## Installation
 Install package using **pip**:
 
 ```
 pip install text2term
 ```
+## Examples
+### Programmatic
+```python
+import text2term
+import pandas
+
+df1 = text2term.map_file("test/unstruct_terms.txt", "http://www.ebi.ac.uk/efo/efo.owl")
+df2 = text2term.map_terms(["asthma", "acute bronchitis"], "http://www.ebi.ac.uk/efo/efo.owl")
+```
+Below is an example of caching, assuming the same imports as above:
+```python
+text2term.cache_ontology("http://www.ebi.ac.uk/efo/efo.owl", "EFO")
+df1 = text2term.map_file("test/unstruct_terms.txt", "EFO", use_cache=True)
+df2 = text2term.map_terms(["asthma", "acute bronchitis"], "EFO", use_cache=True)
+text2term.clear_cache("EFO")
+```
+
+### Command Line
+The basic use of the tool requires a `source` file containing a list of terms to map to the given `target` ontology:  
+`python text2term -s test/unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl`
+
+Specify an output file where the mappings should be saved using `-o`:  
+`python text2term -s test/unstruct_terms.txt -t efo.owl -o /Documents/my-mappings.csv`
+
+Set the minimum acceptable similarity score for mapping each given term to an ontology term using `-min`:  
+`python text2term -s test/unstruct_terms.txt -t efo.owl -min 0.8`  
+The mapped terms returned will have been determined to be 0.8 similar to their source terms in a 0-1 scale.  
+
+Exclude deprecated ontology terms (declared as such via *owl:deprecated true*) using `-d`:  
+`python text2term -s test/unstruct_terms.txt -t efo.owl -d`
+
+Limit search to only terms whose IRIs start with any IRI given in a list specified using `-iris`:  
+`python text2term.py -s test/unstruct_terms.txt -t efo.owl -iris http://www.ebi.ac.uk/efo/EFO,http://purl.obolibrary.org/obo/HP`  
+Here, because EFO reuses terms from other ontologies such as HP and GO, the HP terms would be included but the GO terms would be excluded.
+
+Use the cache on the command line, first by flagging it, then in the future using the acronym:
+`python text2term -s test/unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl -c EFO`
+Then, after running this, the following command is equivalent:
+`python text2term -s test/unstruct_terms.txt -t EFO`
 
 ## Programmatic Usage
 The tool can be executed in Python with any of the three following functions:
 
 ```python
 text2term.map_file(input_file='/some/file.txt', 
                    target_ontology='http://some.ontology/v1.owl',
@@ -39,45 +78,48 @@
                    max_mappings=3, 
                    mapper=Mapper.TFIDF,
                    min_score=0.3, 
                    output_file='', 
                    save_graphs=False, 
                    save_mappings=False, 
                    separator=',', 
-                   use_cache=False)
+                   use_cache=False,
+                   term_type='classes')
 ```
 or
 ```python
 text2term.map_terms(source_terms=['term one', 'term two'],
                     target_ontology='http://some.ontology/v1.owl',
                     base_iris=(),
                     excl_deprecated=False,
                     max_mappings=3,
                     min_score=0.3,
                     mapper=Mapper.TFIDF,
                     output_file='',
                     save_graphs=False,
                     save_mappings=False,
                     source_terms_ids=(),
-                    use_cache=False)
+                    use_cache=False,
+                    term_type='classes')
 ```
 or
 ```python
 text2term.map_tagged_terms(tagged_terms_dict={'term one': ["tag 1", "tag 2"]},
                     target_ontology='http://some.ontology/v1.owl',
                     base_iris=(),
                     excl_deprecated=False,
                     max_mappings=3,
                     min_score=0.3,
                     mapper=Mapper.TFIDF,
                     output_file='',
                     save_graphs=False,
                     save_mappings=False,
                     source_terms_ids=(),
-                    use_cache=False)
+                    use_cache=False,
+                    term_type='classes')
 ```
 
 ### Arguments
 For `map_file`, the first argument 'input_file' specifies a path to a file containing the terms to be mapped. It also has a `csv_column` argument that allows the user to specify a column to map if a csv is passed in as the input file. 
 For `map_terms`, the first argument 'source_terms' takes in a list of the terms to be mapped.
 For `map_tagged_terms`, everything is the same as `map_terms` except the first argument is either a dictionary of terms to a list of tags, or a list of TaggedTerm objects (see below). Currently, the tags do not affect the mapping in any way, but they are added to the output dataframe at the end of the process.
 
@@ -113,14 +155,20 @@
 
 `save_graphs` : bool
     Save vis.js graphs representing the neighborhood of each ontology term
 
 `save_mappings` : bool
     Save the generated mappings to a file (specified by `output_file`) 
 
+`use_cache` : bool
+    Use the cache for the ontology. More details are below.
+
+`term_type` : str
+    Determines whether the ontology should be parsed for its classes (ThingClass), properties (PropertyClass), or both. Possible values are ['classes', 'properties', 'both']. If it does not match one of these values, the program will throw a ValueError.
+
 All default values, if they exist, can be seen above.
 
 ### Return Value
 Both functions return the same value:
 
 `df` : Data frame containing the generated ontology mappings
 
@@ -131,27 +179,27 @@
 cache_ontology(ontology_url, ontology_acronym, base_iris=())
 ```
 
 ```python
 cache_ontology_set(ontology_registry_path)
 ```
 
-The first of these will cache a single ontology from a URL or file path, with it being referenced by an acronym that will be used to reference it later. An example can be found below.
+The first of these will cache a single ontology from a URL or file path, with it being referenced by an acronym that will be used to reference it later. An example can be found above.
 The second function allows the user to cache several ontologies at once by referencing a CSV file of the format:
 `acronym,version,url`. An example is provided in `resources/ontologies.csv`
 
 Once an ontology has been cached by either function, it is stored in a cache folder locally, and thus can be referenced even in different Python instances.
 
 NOTE: Due to how ontologies are processed in memory, `cache_ontology_set` must be used to cache multiple ontologies in a single Python instance. If `cache_ontology` is used multiple times in one instance, the behavior is undefined and may cause visible or invisible errors.
 
 After an ontology is cached, the user can access the cache by using the assigned acronym in the place of `target_ontology` and setting the `use_cache` flag to `True`.
 To clear the cache, one can call:
 `clear_cache(ontology_acronym='')`
 If no arguments are specified, the entire cache will be cleared. Otherwise, only the ontology with the given acronym will be cleared.
-Finally, `cache_exists(ontology_acronym)` is a simple function that returns `True` if the given acronym exists in the cache, and `False` otherwise. It is worth noting that while ontology URLs can repeat, acronyms must be distinct in a given environment.
+Finally, `cache_exists(ontology_acronym='')` is a simple function that returns `True` if the given acronym exists in the cache, and `False` otherwise. It is worth noting that while ontology URLs can repeat, acronyms must be distinct in a given environment.
 
 ### Input Preprocessing
 As of version 1.2.0, text2term includes regex-based preprocessing functionality for input terms. Specifically, these functions take the input terms and a collection of (user-defined) regular expressions, then match each term to each regular expression to simplify the input term.
 
 Like the "map" functions above, the two functions differ on whether the input is a file or a list of strings:
 ```python
 preprocess_file(file_path, template_path, output_file='', blocklist_path='', blocklist_char='', rem_duplicates=False)
@@ -216,48 +264,8 @@
 
 `-iris BASE_IRIS` Map only to ontology terms whose IRIs start with a value given in this comma-separated list (eg 'http://www.ebi.ac.uk/efo,http://purl.obolibrary.org/obo/HP)').
 
 `-d EXCL_DEPRECATED` Exclude ontology terms stated as deprecated via `owl:deprecated true`.
 
 `-g SAVE_TERM_GRAPHS` Save [vis.js](https://visjs.org) graphs representing the neighborhood of each ontology term.
 
-`-c STORE_IN_CACHE` Using this flag followed by the acronym the ontology should be stored as, the program will same the target ontology to the cache. After that, referencing the acronym in `target` will reference the cache. Examples are below.
-
-## Examples
-### Programmatic
-```python
-import text2term
-import pandas
-
-df1 = text2term.map_file(unstruct_terms.txt, "http://www.ebi.ac.uk/efo/efo.owl")
-df2 = text2term.map_terms(["asthma", "acute bronchitis"], "http://www.ebi.ac.uk/efo/efo.owl")
-```
-Below is an example of caching, assuming the same imports as above:
-```python
-text2term.cache_ontology("http://www.ebi.ac.uk/efo/efo.owl", "EFO")
-df1 = text2term.map_file(unstruct_terms.txt, "EFO", use_cache=True)
-df2 = text2term.map_terms(["asthma", "acute bronchitis"], "EFO", use_cache=True)
-text2term.clear_cache("EFO")
-```
-
-### Command Line
-The basic use of the tool requires a `source` file containing a list of terms to map to the given `target` ontology:  
-`python text2term -s unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl`
-
-Specify an output file where the mappings should be saved using `-o`:  
-`python text2term -s unstruct_terms.txt -t efo.owl -o /Documents/my-mappings.csv`
-
-Set the minimum acceptable similarity score for mapping each given term to an ontology term using `-min`:  
-`python text2term -s unstruct_terms.txt -t efo.owl -min 0.8`  
-The mapped terms returned will have been determined to be 0.8 similar to their source terms in a 0-1 scale.  
-
-Exclude deprecated ontology terms (declared as such via *owl:deprecated true*) using `-d`:  
-`python text2term -s unstruct_terms.txt -t efo.owl -d`
-
-Limit search to only terms whose IRIs start with any IRI given in a list specified using `-iris`:  
-`python text2term.py -s unstruct_terms.txt -t efo.owl -iris http://www.ebi.ac.uk/efo/EFO,http://purl.obolibrary.org/obo/HP`  
-Here, because EFO reuses terms from other ontologies such as HP and GO, the HP terms would be included but the GO terms would be excluded.
-
-Use the cache on the command line, first by flagging it, then in the future using the acronym:
-`python text2term -s unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl -c EFO`
-Then, after running this, the following command is equivalent:
-`python text2term -s unstruct_terms.txt -t EFO`
+`-c STORE_IN_CACHE` Using this flag followed by the acronym the ontology should be stored as, the program will same the target ontology to the cache. After that, referencing the acronym in `target` will reference the cache. Examples are above.
```

### Comparing `text2term-2.1.0/README.md` & `text2term-2.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,53 @@
 
 ## Installation
 Install package using **pip**:
 
 ```
 pip install text2term
 ```
+## Examples
+### Programmatic
+```python
+import text2term
+import pandas
+
+df1 = text2term.map_file("test/unstruct_terms.txt", "http://www.ebi.ac.uk/efo/efo.owl")
+df2 = text2term.map_terms(["asthma", "acute bronchitis"], "http://www.ebi.ac.uk/efo/efo.owl")
+```
+Below is an example of caching, assuming the same imports as above:
+```python
+text2term.cache_ontology("http://www.ebi.ac.uk/efo/efo.owl", "EFO")
+df1 = text2term.map_file("test/unstruct_terms.txt", "EFO", use_cache=True)
+df2 = text2term.map_terms(["asthma", "acute bronchitis"], "EFO", use_cache=True)
+text2term.clear_cache("EFO")
+```
+
+### Command Line
+The basic use of the tool requires a `source` file containing a list of terms to map to the given `target` ontology:  
+`python text2term -s test/unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl`
+
+Specify an output file where the mappings should be saved using `-o`:  
+`python text2term -s test/unstruct_terms.txt -t efo.owl -o /Documents/my-mappings.csv`
+
+Set the minimum acceptable similarity score for mapping each given term to an ontology term using `-min`:  
+`python text2term -s test/unstruct_terms.txt -t efo.owl -min 0.8`  
+The mapped terms returned will have been determined to be 0.8 similar to their source terms in a 0-1 scale.  
+
+Exclude deprecated ontology terms (declared as such via *owl:deprecated true*) using `-d`:  
+`python text2term -s test/unstruct_terms.txt -t efo.owl -d`
+
+Limit search to only terms whose IRIs start with any IRI given in a list specified using `-iris`:  
+`python text2term.py -s test/unstruct_terms.txt -t efo.owl -iris http://www.ebi.ac.uk/efo/EFO,http://purl.obolibrary.org/obo/HP`  
+Here, because EFO reuses terms from other ontologies such as HP and GO, the HP terms would be included but the GO terms would be excluded.
+
+Use the cache on the command line, first by flagging it, then in the future using the acronym:
+`python text2term -s test/unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl -c EFO`
+Then, after running this, the following command is equivalent:
+`python text2term -s test/unstruct_terms.txt -t EFO`
 
 ## Programmatic Usage
 The tool can be executed in Python with any of the three following functions:
 
 ```python
 text2term.map_file(input_file='/some/file.txt', 
                    target_ontology='http://some.ontology/v1.owl',
@@ -20,45 +59,48 @@
                    max_mappings=3, 
                    mapper=Mapper.TFIDF,
                    min_score=0.3, 
                    output_file='', 
                    save_graphs=False, 
                    save_mappings=False, 
                    separator=',', 
-                   use_cache=False)
+                   use_cache=False,
+                   term_type='classes')
 ```
 or
 ```python
 text2term.map_terms(source_terms=['term one', 'term two'],
                     target_ontology='http://some.ontology/v1.owl',
                     base_iris=(),
                     excl_deprecated=False,
                     max_mappings=3,
                     min_score=0.3,
                     mapper=Mapper.TFIDF,
                     output_file='',
                     save_graphs=False,
                     save_mappings=False,
                     source_terms_ids=(),
-                    use_cache=False)
+                    use_cache=False,
+                    term_type='classes')
 ```
 or
 ```python
 text2term.map_tagged_terms(tagged_terms_dict={'term one': ["tag 1", "tag 2"]},
                     target_ontology='http://some.ontology/v1.owl',
                     base_iris=(),
                     excl_deprecated=False,
                     max_mappings=3,
                     min_score=0.3,
                     mapper=Mapper.TFIDF,
                     output_file='',
                     save_graphs=False,
                     save_mappings=False,
                     source_terms_ids=(),
-                    use_cache=False)
+                    use_cache=False,
+                    term_type='classes')
 ```
 
 ### Arguments
 For `map_file`, the first argument 'input_file' specifies a path to a file containing the terms to be mapped. It also has a `csv_column` argument that allows the user to specify a column to map if a csv is passed in as the input file. 
 For `map_terms`, the first argument 'source_terms' takes in a list of the terms to be mapped.
 For `map_tagged_terms`, everything is the same as `map_terms` except the first argument is either a dictionary of terms to a list of tags, or a list of TaggedTerm objects (see below). Currently, the tags do not affect the mapping in any way, but they are added to the output dataframe at the end of the process.
 
@@ -94,14 +136,20 @@
 
 `save_graphs` : bool
     Save vis.js graphs representing the neighborhood of each ontology term
 
 `save_mappings` : bool
     Save the generated mappings to a file (specified by `output_file`) 
 
+`use_cache` : bool
+    Use the cache for the ontology. More details are below.
+
+`term_type` : str
+    Determines whether the ontology should be parsed for its classes (ThingClass), properties (PropertyClass), or both. Possible values are ['classes', 'properties', 'both']. If it does not match one of these values, the program will throw a ValueError.
+
 All default values, if they exist, can be seen above.
 
 ### Return Value
 Both functions return the same value:
 
 `df` : Data frame containing the generated ontology mappings
 
@@ -112,27 +160,27 @@
 cache_ontology(ontology_url, ontology_acronym, base_iris=())
 ```
 
 ```python
 cache_ontology_set(ontology_registry_path)
 ```
 
-The first of these will cache a single ontology from a URL or file path, with it being referenced by an acronym that will be used to reference it later. An example can be found below.
+The first of these will cache a single ontology from a URL or file path, with it being referenced by an acronym that will be used to reference it later. An example can be found above.
 The second function allows the user to cache several ontologies at once by referencing a CSV file of the format:
 `acronym,version,url`. An example is provided in `resources/ontologies.csv`
 
 Once an ontology has been cached by either function, it is stored in a cache folder locally, and thus can be referenced even in different Python instances.
 
 NOTE: Due to how ontologies are processed in memory, `cache_ontology_set` must be used to cache multiple ontologies in a single Python instance. If `cache_ontology` is used multiple times in one instance, the behavior is undefined and may cause visible or invisible errors.
 
 After an ontology is cached, the user can access the cache by using the assigned acronym in the place of `target_ontology` and setting the `use_cache` flag to `True`.
 To clear the cache, one can call:
 `clear_cache(ontology_acronym='')`
 If no arguments are specified, the entire cache will be cleared. Otherwise, only the ontology with the given acronym will be cleared.
-Finally, `cache_exists(ontology_acronym)` is a simple function that returns `True` if the given acronym exists in the cache, and `False` otherwise. It is worth noting that while ontology URLs can repeat, acronyms must be distinct in a given environment.
+Finally, `cache_exists(ontology_acronym='')` is a simple function that returns `True` if the given acronym exists in the cache, and `False` otherwise. It is worth noting that while ontology URLs can repeat, acronyms must be distinct in a given environment.
 
 ### Input Preprocessing
 As of version 1.2.0, text2term includes regex-based preprocessing functionality for input terms. Specifically, these functions take the input terms and a collection of (user-defined) regular expressions, then match each term to each regular expression to simplify the input term.
 
 Like the "map" functions above, the two functions differ on whether the input is a file or a list of strings:
 ```python
 preprocess_file(file_path, template_path, output_file='', blocklist_path='', blocklist_char='', rem_duplicates=False)
@@ -197,48 +245,8 @@
 
 `-iris BASE_IRIS` Map only to ontology terms whose IRIs start with a value given in this comma-separated list (eg 'http://www.ebi.ac.uk/efo,http://purl.obolibrary.org/obo/HP)').
 
 `-d EXCL_DEPRECATED` Exclude ontology terms stated as deprecated via `owl:deprecated true`.
 
 `-g SAVE_TERM_GRAPHS` Save [vis.js](https://visjs.org) graphs representing the neighborhood of each ontology term.
 
-`-c STORE_IN_CACHE` Using this flag followed by the acronym the ontology should be stored as, the program will same the target ontology to the cache. After that, referencing the acronym in `target` will reference the cache. Examples are below.
-
-## Examples
-### Programmatic
-```python
-import text2term
-import pandas
-
-df1 = text2term.map_file(unstruct_terms.txt, "http://www.ebi.ac.uk/efo/efo.owl")
-df2 = text2term.map_terms(["asthma", "acute bronchitis"], "http://www.ebi.ac.uk/efo/efo.owl")
-```
-Below is an example of caching, assuming the same imports as above:
-```python
-text2term.cache_ontology("http://www.ebi.ac.uk/efo/efo.owl", "EFO")
-df1 = text2term.map_file(unstruct_terms.txt, "EFO", use_cache=True)
-df2 = text2term.map_terms(["asthma", "acute bronchitis"], "EFO", use_cache=True)
-text2term.clear_cache("EFO")
-```
-
-### Command Line
-The basic use of the tool requires a `source` file containing a list of terms to map to the given `target` ontology:  
-`python text2term -s unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl`
-
-Specify an output file where the mappings should be saved using `-o`:  
-`python text2term -s unstruct_terms.txt -t efo.owl -o /Documents/my-mappings.csv`
-
-Set the minimum acceptable similarity score for mapping each given term to an ontology term using `-min`:  
-`python text2term -s unstruct_terms.txt -t efo.owl -min 0.8`  
-The mapped terms returned will have been determined to be 0.8 similar to their source terms in a 0-1 scale.  
-
-Exclude deprecated ontology terms (declared as such via *owl:deprecated true*) using `-d`:  
-`python text2term -s unstruct_terms.txt -t efo.owl -d`
-
-Limit search to only terms whose IRIs start with any IRI given in a list specified using `-iris`:  
-`python text2term.py -s unstruct_terms.txt -t efo.owl -iris http://www.ebi.ac.uk/efo/EFO,http://purl.obolibrary.org/obo/HP`  
-Here, because EFO reuses terms from other ontologies such as HP and GO, the HP terms would be included but the GO terms would be excluded.
-
-Use the cache on the command line, first by flagging it, then in the future using the acronym:
-`python text2term -s unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl -c EFO`
-Then, after running this, the following command is equivalent:
-`python text2term -s unstruct_terms.txt -t EFO`
+`-c STORE_IN_CACHE` Using this flag followed by the acronym the ontology should be stored as, the program will same the target ontology to the cache. After that, referencing the acronym in `target` will reference the cache. Examples are above.
```

### Comparing `text2term-2.1.0/setup.py` & `text2term-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `text2term-2.1.0/text2term/__main__.py` & `text2term-2.2.0/text2term/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,16 @@
                              "list (eg 'http://www.ebi.ac.uk/efo,http://purl.obolibrary.org/obo/HP)')")
     parser.add_argument("-d", "--excl_deprecated", required=False, default=False, action="store_true",
                         help="Exclude ontology terms stated as deprecated via `owl:deprecated true` (default=False)")
     parser.add_argument("-g", "--save_term_graphs", required=False, default=False, action="store_true",
                         help="Save vis.js graphs representing the neighborhood of each ontology term (default=False)")
     parser.add_argument("-c", "--store_in_cache", required=False, type=str, default="",
                         help="Store the target ontology into local cache under acronym")
+    parser.add_argument("-type", "--term_type", required=False, type=str, default="classes",
+                        help="Define whether to return ontology classes, properties, or both")
 
     arguments = parser.parse_args()
     if not os.path.exists(arguments.source):
         parser.error("The file '{}' does not exist".format(arguments.source))
         sys.exit(1)
     mapper = Mapper(arguments.mapper)
     iris = arguments.base_iris
@@ -53,8 +55,8 @@
     acronym = arguments.store_in_cache
     if acronym != "":
         cache_ontology(target, acronym, iris)
         target = acronym
     map_file(arguments.source, target, output_file=arguments.output, csv_columns=csv_columns,
                          excl_deprecated=arguments.excl_deprecated, mapper=mapper, max_mappings=arguments.top_mappings,
                          min_score=arguments.min_score, base_iris=iris, save_graphs=arguments.save_term_graphs,
-                         save_mappings=True, separator=arguments.separator, use_cache=cache_exists(target))
+                         save_mappings=True, separator=arguments.separator, use_cache=cache_exists(target), term_type=arguments.term_type)
```

### Comparing `text2term-2.1.0/text2term/bioportal_mapper.py` & `text2term-2.2.0/text2term/bioportal_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.1.0/text2term/onto_utils.py` & `text2term-2.2.0/text2term/onto_utils.py`

 * *Files identical despite different names*

### Comparing `text2term-2.1.0/text2term/preprocess.py` & `text2term-2.2.0/text2term/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2term-2.1.0/text2term/syntactic_mapper.py` & `text2term-2.2.0/text2term/syntactic_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.1.0/text2term/t2t.py` & `text2term-2.2.0/text2term/t2t.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,28 +55,30 @@
 Returns
 ----------
 df
     Data frame containing the generated ontology mappings
 """
 def map_file(input_file, target_ontology, base_iris=(), csv_columns=(), excl_deprecated=False, max_mappings=3,
              mapper=Mapper.TFIDF, min_score=0.3, output_file='', save_graphs=False, save_mappings=False,
-             separator=',', use_cache=False):
+             separator=',', use_cache=False, term_type='classes'):
     source_terms, source_terms_ids = _load_data(input_file, csv_columns, separator)
     return map_terms(source_terms, target_ontology, source_terms_ids=source_terms_ids, base_iris=base_iris,
                     excl_deprecated=excl_deprecated, max_mappings=max_mappings, mapper=mapper, min_score=min_score,
-                    output_file=output_file, save_graphs=save_graphs, save_mappings=save_mappings, use_cache=use_cache)
+                    output_file=output_file, save_graphs=save_graphs, save_mappings=save_mappings, 
+                    use_cache=use_cache, term_type=term_type)
 
 """
 All parameters are the same as below, but tagged_terms_dict is a dictionary where the 
     key is the source term and the value is a list of all tags (or a single string for 
     one tag). It can also be a list of TaggedTerm objects. 
     The dataframe returned is the same but contains a tags column
 """
 def map_tagged_terms(tagged_terms_dict, target_ontology, base_iris=(), excl_deprecated=False, max_mappings=3, min_score=0.3,
-        mapper=Mapper.TFIDF, output_file='', save_graphs=False, save_mappings=False, source_terms_ids=(), use_cache=False):
+        mapper=Mapper.TFIDF, output_file='', save_graphs=False, save_mappings=False, source_terms_ids=(), use_cache=False,
+        term_type='classes'):
     # If the input is a dict, use keys. If it is a list, it is a list of TaggedTerms
     if isinstance(tagged_terms_dict, dict):
         terms = list(tagged_terms_dict.keys())
     else:
         terms = []
         source_terms_id_list = []
         for tagged_term in tagged_terms_dict:
@@ -85,15 +87,16 @@
                 source_terms_id_list.append(tagged_term.get_source_term_id())
         if len(source_terms_id_list) > 0:
             source_terms_ids = tuple(source_terms_id_list)
 
     # Run the mapper
     df = map_terms(terms, target_ontology, base_iris=base_iris, excl_deprecated=excl_deprecated, \
                     max_mappings=max_mappings, min_score=min_score, mapper=mapper, output_file=output_file, \
-                    save_graphs=save_graphs, source_terms_ids=source_terms_ids, use_cache=use_cache)
+                    save_graphs=save_graphs, source_terms_ids=source_terms_ids, use_cache=use_cache, \
+                    term_type=term_type)
 
     # For each term in dict, add tags to corresponding mappings row in "Tags" Column
     if isinstance(tagged_terms_dict, dict):
         for key, value in tagged_terms_dict.items():
             if isinstance(value, list):
                 to_store = ','.join(value)
             else:
@@ -141,26 +144,27 @@
 
 Returns
 ----------
 df
     Data frame containing the generated ontology mappings
 """
 def map_terms(source_terms, target_ontology, base_iris=(), excl_deprecated=False, max_mappings=3, min_score=0.3,
-        mapper=Mapper.TFIDF, output_file='', save_graphs=False, save_mappings=False, source_terms_ids=(), use_cache=False):
+        mapper=Mapper.TFIDF, output_file='', save_graphs=False, save_mappings=False, source_terms_ids=(), 
+        use_cache=False, term_type='classes'):
     if len(source_terms_ids) != len(source_terms):
         if len(source_terms_ids) > 0:
             sys.stderr.write("Warning: Source Term Ids are non-zero, but will not be used.")
         source_terms_ids = onto_utils.generate_iris(len(source_terms))
     if output_file == '':
         timestamp = datetime.datetime.now().strftime("%d-%m-%YT%H-%M-%S")
         output_file = "t2t-mappings-" + timestamp + ".csv"
     if mapper in {Mapper.ZOOMA, Mapper.BIOPORTAL}:
         target_terms = '' if target_ontology.lower() == 'all' else target_ontology
     else:
-        target_terms = _load_ontology(target_ontology, base_iris, excl_deprecated, use_cache)
+        target_terms = _load_ontology(target_ontology, base_iris, excl_deprecated, use_cache, term_type)
     mappings_df = _do_mapping(source_terms, source_terms_ids, target_terms, mapper, max_mappings, min_score)
     if save_mappings:
         _save_mappings(mappings_df, output_file, min_score, mapper, target_ontology, base_iris, excl_deprecated, max_mappings)
     if save_graphs:
         _save_graphs(target_terms, output_file)
     return mappings_df
 
@@ -175,25 +179,25 @@
             cache_ontology(row.url, row.acronym)
         except Exception as err:
             sys.stderr.write("Could not cache ontology", row.acronym, "due to error:", err)
         owlready2.default_world.ontologies.clear()
 
 # Caches a single ontology
 def cache_ontology(ontology_url, ontology_acronym, base_iris=()):
-    ontology_terms = _load_ontology(ontology_url, base_iris, exclude_deprecated=False)
+    ontology_terms = _load_ontology(ontology_url, base_iris, exclude_deprecated=False, term_type='both')
     cache_dir = "cache/" + ontology_acronym + "/"
     if not os.path.exists(cache_dir):
         os.makedirs(cache_dir)
 
     _serialize_ontology(ontology_terms, ontology_acronym, cache_dir)
     _save_graphs(ontology_terms, output_file=cache_dir + ontology_acronym)
     ontology_terms.clear()
 
 # Will check if an acronym exists in the cache
-def cache_exists(ontology_acronym):
+def cache_exists(ontology_acronym=''):
     return os.path.exists("cache/" + ontology_acronym)
 
 # Clears the cache
 def clear_cache(ontology_acronym=''):
     cache_dir = "cache/" 
     if ontology_acronym != '':
         cache_dir = os.path.join(cache_dir, ontology_acronym)
@@ -223,22 +227,23 @@
                                                     term_column_name=csv_column_names[0],
                                                     term_id_column_name=term_id_col_name)
     else:
         terms = onto_utils.parse_list_file(input_file_path)
         term_ids = onto_utils.generate_iris(len(terms))
     return terms, term_ids
 
-def _load_ontology(ontology, iris, exclude_deprecated, use_cache=False):
+def _load_ontology(ontology, iris, exclude_deprecated, use_cache=False, term_type='classes'):
     term_collector = OntologyTermCollector()
     if use_cache:
         pickle_file = "cache/" + ontology + "/" + ontology + "-term-details.pickle"
         onto_terms_unfiltered = pickle.load(open(pickle_file, "rb"))
-        onto_terms = term_collector.filter_terms(onto_terms_unfiltered, iris, exclude_deprecated)
+        onto_terms = term_collector.filter_terms(onto_terms_unfiltered, iris, exclude_deprecated, term_type)
     else:
-        onto_terms = term_collector.get_ontology_terms(ontology, base_iris=iris, exclude_deprecated=exclude_deprecated)
+
+        onto_terms = term_collector.get_ontology_terms(ontology, base_iris=iris, exclude_deprecated=exclude_deprecated, term_type=term_type)
     if len(onto_terms) == 0:
         raise RuntimeError("Could not find any terms in the given ontology.")
     return onto_terms
 
 def _do_mapping(source_terms, source_term_ids, ontology_terms, mapper, max_mappings, min_score):
     if mapper == Mapper.TFIDF:
         term_mapper = TFIDFMapper(ontology_terms)
```

### Comparing `text2term-2.1.0/text2term/tagged_terms.py` & `text2term-2.2.0/text2term/tagged_terms.py`

 * *Files identical despite different names*

### Comparing `text2term-2.1.0/text2term/term.py` & `text2term-2.2.0/text2term/term.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Provides OntologyTerm class"""
 
 
 class OntologyTerm:
 
-    def __init__(self, iri, labels, definitions=(), synonyms=(), parents=(), children=(), instances=(), deprecated=False):
+    def __init__(self, iri, labels, definitions=(), synonyms=(), parents=(), children=(), instances=(), deprecated=False, termtype='class'):
         """
         Constructor for a succinct representation of an ontology term
         :param iri: IRI of the ontology term
         :param labels: Set of human-readable labels for the term (e.g., rdfs:label, skos:prefLabel)
         :param definitions: Set of textual definitions of the term
         :param synonyms: Set of synonyms of the term (e.g., alternative labels)
         :param parents: Dictionary containing the IRIs of parent terms (superclasses) and their label(s)
@@ -18,14 +18,15 @@
         self._labels = labels
         self._synonyms = synonyms
         self._definitions = definitions
         self._parents = parents
         self._children = children
         self._instances = instances
         self._deprecated = deprecated
+        self._termtype = termtype
 
     @property
     def iri(self):
         return self._iri
 
     @property
     def labels(self):
@@ -56,14 +57,18 @@
         """Return a single label for this term"""
         return next(iter(self.labels))
 
     @property
     def deprecated(self):
         return self._deprecated
 
+    @property
+    def termtype(self):
+        return self._termtype
+
     def __eq__(self, other):
         if isinstance(other, OntologyTerm):
             return self._iri == other._iri
         return False
 
     def __hash__(self):
         return hash(str(self._iri))
```

### Comparing `text2term-2.1.0/text2term/term_collector.py` & `text2term-2.2.0/text2term/term_collector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Provides OntologyTermCollector class"""
 
 from owlready2 import *
 from text2term import onto_utils
 from text2term.term import OntologyTerm
 import logging
 
+options = ['classes', 'properties', 'both']
 
 class OntologyTermCollector:
 
     def __init__(self, log_level=logging.INFO):
         self.logger = onto_utils.get_logger(__name__, level=log_level)
 
-    def get_ontology_terms(self, ontology_iri, base_iris=(), use_reasoning=False, exclude_deprecated=False):
+    def get_ontology_terms(self, ontology_iri, base_iris=(), use_reasoning=False, exclude_deprecated=False, term_type="classes"):
         """
         Collect the terms described in the ontology at the specified IRI
         :param ontology_iri: IRI of the ontology (e.g., path of ontology document in the local file system, URL)
         :param base_iris: Limit ontology term collection to terms whose IRIs start with any IRI given in this tuple
         :param use_reasoning: Use a reasoner to compute inferred class hierarchy
         :param exclude_deprecated: Exclude ontology terms stated as deprecated using owl:deprecated 'true'
         :return: Dictionary of ontology term IRIs and their respective details in the specified ontology
@@ -28,70 +29,96 @@
         ontology_terms = dict()
         if len(base_iris) > 0:
             for iri in base_iris:
                 iri = iri.strip()
                 query = iri + "*"
                 self.logger.info("...collecting terms with IRIs starting in: " + iri)
                 iris = list(default_world.search(iri=query))
-                ontology_terms = ontology_terms | self._get_ontology_terms(iris, ontology, exclude_deprecated)
+                ontology_terms = ontology_terms | self._get_ontology_terms(iris, ontology, exclude_deprecated, term_type)
         else:
             ontology_signature = self._get_ontology_signature(ontology)
-            ontology_terms = self._get_ontology_terms(ontology_signature, ontology, exclude_deprecated)
+            ontology_terms = self._get_ontology_terms(ontology_signature, ontology, exclude_deprecated, term_type)
         end = time.time()
         self.logger.info("...done: collected %i ontology terms (collection time: %.2fs)", len(ontology_terms),
                          end - start)
         # when multiple ontologies are loaded with owlready2, and they reference the same ontology term (IRI), a lookup
         # for that IRI returns the term from the first ontology loaded —> need to unload previously loaded ontologies
         try:
             ontology.destroy()
         except Exception as err:
             self.logger.debug("Unable to destroy ontology: ", err)
         return ontology_terms
 
-    def filter_terms(self, onto_terms, iris=(), excl_deprecated=False):
+    def filter_terms(self, onto_terms, iris=(), excl_deprecated=False, term_type='classes'):
         filtered_onto_terms = {}
         for base_iri, term in onto_terms.items():
             if type(iris) == str:
                 begins_with_iri = (iris == ()) or base_iri.startswith(iris)
             else:
                 begins_with_iri = (iris == ()) or any(base_iri.startswith(iri) for iri in iris)
             is_not_deprecated = (not excl_deprecated) or (not term.deprecated)
-            if begins_with_iri and is_not_deprecated:
+            include = self._filter_term_type(term, term_type, True) 
+            if begins_with_iri and is_not_deprecated and include:
                 filtered_onto_terms.update({base_iri: term})
         return filtered_onto_terms
 
-    def _get_ontology_signature(self, ontology):
+    def _get_ontology_signature(self, ontology, term_type='classes'):
         signature = list(ontology.classes())
+        signature.extend(list(ontology.properties()))
         # ontology.classes() does not include classes in imported ontologies; we need to explicitly add them to our list
         for imported_ontology in ontology.imported_ontologies:
             signature.extend(list(imported_ontology.classes()))
+            signature.extend(list(imported_ontology.properties()))
         return signature
 
-    def _get_ontology_terms(self, term_list, ontology, exclude_deprecated):
+    def _get_ontology_terms(self, term_list, ontology, exclude_deprecated, term_type):
         ontology_terms = dict()
         for ontology_term in term_list:
-            if not isinstance(ontology_term, PropertyClass) and ontology_term is not Thing \
-                    and ontology_term is not Nothing:
+            # Parse if should include ontology classes, properties, or both
+            include = self._filter_term_type(ontology_term, term_type, False)
+            if include and ontology_term is not Thing and ontology_term is not Nothing:
                 if (exclude_deprecated and not deprecated[ontology_term]) or (not exclude_deprecated):
                     iri = ontology_term.iri
                     labels = self._get_labels(ontology_term)
                     synonyms = self._get_synonyms(ontology_term)
                     parents = self._get_parents(ontology_term)
                     children = self._get_children(ontology_term, ontology)
                     instances = self._get_instances(ontology_term, ontology)
                     definitions = self._get_definitions(ontology_term)
                     is_deprecated = deprecated[ontology_term] == [True]
+                    if self._filter_term_type(ontology_term, "classes", False):
+                        termtype = 'class'
+                    elif self._filter_term_type(ontology_term, "properties", False):
+                        termtype = 'property'
+                    else:
+                        termtype = None
                     term_details = OntologyTerm(iri, labels, definitions=definitions, synonyms=synonyms,
                                                 parents=parents, children=children, instances=instances,
-                                                deprecated=is_deprecated)
+                                                deprecated=is_deprecated, termtype=termtype)
                     ontology_terms[iri] = term_details
                 else:
                     self.logger.debug("Excluding deprecated ontology term: %s", ontology_term.iri)
         return ontology_terms
 
+    def _filter_term_type(self, ontology_term, term_type, cached):
+        if term_type == 'classes':
+            if cached:
+                return ontology_term.termtype == 'class'
+            else:
+                return not isinstance(ontology_term, PropertyClass)
+        elif term_type == 'properties':
+            if cached:
+                return ontology_term.termtype == 'property'
+            else:
+                return isinstance(ontology_term, PropertyClass)
+        elif term_type == 'both':
+            return True 
+        else:
+            raise ValueError("Option to include Properties or Classes is not valid")
+
     def _get_parents(self, ontology_term):
         parents = dict()  # named/atomic superclasses except owl:Thing
         try:
             all_parents = ontology_term.is_a  # obtain direct parents of this entity
             for parent in all_parents:
                 # exclude OWL restrictions and owl:Thing and Self
                 if isinstance(parent, ThingClass) and parent is not Thing and parent is not ontology_term:
```

### Comparing `text2term-2.1.0/text2term/term_graph.py` & `text2term-2.2.0/text2term/term_graph.py`

 * *Files identical despite different names*

### Comparing `text2term-2.1.0/text2term/term_graph_generator.py` & `text2term-2.2.0/text2term/term_graph_generator.py`

 * *Files identical despite different names*

### Comparing `text2term-2.1.0/text2term/term_mapping.py` & `text2term-2.2.0/text2term/term_mapping.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,23 +32,27 @@
         return self._mapped_term_label
 
     @property
     def mapped_term_iri(self):
         return self._mapped_term_iri
 
     @property
+    def mapped_term_curie(self):
+        return onto_utils.curie_from_iri(self.mapped_term_iri)
+
+    @property
     def mapping_score(self):
         return self._mapping_score
 
     def to_dict(self):
         return {
             self.SRC_TERM_ID: self.source_term_id,
             self.SRC_TERM: self.source_term,
             self.TGT_TERM_LBL: self.mapped_term_label,
-            self.TGT_TERM_CURIE: onto_utils.curie_from_iri(self.mapped_term_iri),
+            self.TGT_TERM_CURIE: self.mapped_term_curie,
             self.TGT_TERM_IRI: self.mapped_term_iri,
             self.MAPPING_SCORE: self.mapping_score
         }
 
     def __eq__(self, other):
         if isinstance(other, TermMapping):
             return self.source_term == other.source_term and self.mapped_term_iri == other.mapped_term_iri
```

### Comparing `text2term-2.1.0/text2term/tfidf_mapper.py` & `text2term-2.2.0/text2term/tfidf_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.1.0/text2term/zooma_mapper.py` & `text2term-2.2.0/text2term/zooma_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.1.0/text2term.egg-info/PKG-INFO` & `text2term-2.2.0/text2term.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2term
-Version: 2.1.0
+Version: 2.2.0
 Summary: A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies
 Home-page: https://github.com/ccb-hms/ontology-mapper
 Author: Center for Computational Biomedicine, Harvard Medical School
 Author-email: rafael_goncalves@hms.harvard.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,53 @@
 
 ## Installation
 Install package using **pip**:
 
 ```
 pip install text2term
 ```
+## Examples
+### Programmatic
+```python
+import text2term
+import pandas
+
+df1 = text2term.map_file("test/unstruct_terms.txt", "http://www.ebi.ac.uk/efo/efo.owl")
+df2 = text2term.map_terms(["asthma", "acute bronchitis"], "http://www.ebi.ac.uk/efo/efo.owl")
+```
+Below is an example of caching, assuming the same imports as above:
+```python
+text2term.cache_ontology("http://www.ebi.ac.uk/efo/efo.owl", "EFO")
+df1 = text2term.map_file("test/unstruct_terms.txt", "EFO", use_cache=True)
+df2 = text2term.map_terms(["asthma", "acute bronchitis"], "EFO", use_cache=True)
+text2term.clear_cache("EFO")
+```
+
+### Command Line
+The basic use of the tool requires a `source` file containing a list of terms to map to the given `target` ontology:  
+`python text2term -s test/unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl`
+
+Specify an output file where the mappings should be saved using `-o`:  
+`python text2term -s test/unstruct_terms.txt -t efo.owl -o /Documents/my-mappings.csv`
+
+Set the minimum acceptable similarity score for mapping each given term to an ontology term using `-min`:  
+`python text2term -s test/unstruct_terms.txt -t efo.owl -min 0.8`  
+The mapped terms returned will have been determined to be 0.8 similar to their source terms in a 0-1 scale.  
+
+Exclude deprecated ontology terms (declared as such via *owl:deprecated true*) using `-d`:  
+`python text2term -s test/unstruct_terms.txt -t efo.owl -d`
+
+Limit search to only terms whose IRIs start with any IRI given in a list specified using `-iris`:  
+`python text2term.py -s test/unstruct_terms.txt -t efo.owl -iris http://www.ebi.ac.uk/efo/EFO,http://purl.obolibrary.org/obo/HP`  
+Here, because EFO reuses terms from other ontologies such as HP and GO, the HP terms would be included but the GO terms would be excluded.
+
+Use the cache on the command line, first by flagging it, then in the future using the acronym:
+`python text2term -s test/unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl -c EFO`
+Then, after running this, the following command is equivalent:
+`python text2term -s test/unstruct_terms.txt -t EFO`
 
 ## Programmatic Usage
 The tool can be executed in Python with any of the three following functions:
 
 ```python
 text2term.map_file(input_file='/some/file.txt', 
                    target_ontology='http://some.ontology/v1.owl',
@@ -39,45 +78,48 @@
                    max_mappings=3, 
                    mapper=Mapper.TFIDF,
                    min_score=0.3, 
                    output_file='', 
                    save_graphs=False, 
                    save_mappings=False, 
                    separator=',', 
-                   use_cache=False)
+                   use_cache=False,
+                   term_type='classes')
 ```
 or
 ```python
 text2term.map_terms(source_terms=['term one', 'term two'],
                     target_ontology='http://some.ontology/v1.owl',
                     base_iris=(),
                     excl_deprecated=False,
                     max_mappings=3,
                     min_score=0.3,
                     mapper=Mapper.TFIDF,
                     output_file='',
                     save_graphs=False,
                     save_mappings=False,
                     source_terms_ids=(),
-                    use_cache=False)
+                    use_cache=False,
+                    term_type='classes')
 ```
 or
 ```python
 text2term.map_tagged_terms(tagged_terms_dict={'term one': ["tag 1", "tag 2"]},
                     target_ontology='http://some.ontology/v1.owl',
                     base_iris=(),
                     excl_deprecated=False,
                     max_mappings=3,
                     min_score=0.3,
                     mapper=Mapper.TFIDF,
                     output_file='',
                     save_graphs=False,
                     save_mappings=False,
                     source_terms_ids=(),
-                    use_cache=False)
+                    use_cache=False,
+                    term_type='classes')
 ```
 
 ### Arguments
 For `map_file`, the first argument 'input_file' specifies a path to a file containing the terms to be mapped. It also has a `csv_column` argument that allows the user to specify a column to map if a csv is passed in as the input file. 
 For `map_terms`, the first argument 'source_terms' takes in a list of the terms to be mapped.
 For `map_tagged_terms`, everything is the same as `map_terms` except the first argument is either a dictionary of terms to a list of tags, or a list of TaggedTerm objects (see below). Currently, the tags do not affect the mapping in any way, but they are added to the output dataframe at the end of the process.
 
@@ -113,14 +155,20 @@
 
 `save_graphs` : bool
     Save vis.js graphs representing the neighborhood of each ontology term
 
 `save_mappings` : bool
     Save the generated mappings to a file (specified by `output_file`) 
 
+`use_cache` : bool
+    Use the cache for the ontology. More details are below.
+
+`term_type` : str
+    Determines whether the ontology should be parsed for its classes (ThingClass), properties (PropertyClass), or both. Possible values are ['classes', 'properties', 'both']. If it does not match one of these values, the program will throw a ValueError.
+
 All default values, if they exist, can be seen above.
 
 ### Return Value
 Both functions return the same value:
 
 `df` : Data frame containing the generated ontology mappings
 
@@ -131,27 +179,27 @@
 cache_ontology(ontology_url, ontology_acronym, base_iris=())
 ```
 
 ```python
 cache_ontology_set(ontology_registry_path)
 ```
 
-The first of these will cache a single ontology from a URL or file path, with it being referenced by an acronym that will be used to reference it later. An example can be found below.
+The first of these will cache a single ontology from a URL or file path, with it being referenced by an acronym that will be used to reference it later. An example can be found above.
 The second function allows the user to cache several ontologies at once by referencing a CSV file of the format:
 `acronym,version,url`. An example is provided in `resources/ontologies.csv`
 
 Once an ontology has been cached by either function, it is stored in a cache folder locally, and thus can be referenced even in different Python instances.
 
 NOTE: Due to how ontologies are processed in memory, `cache_ontology_set` must be used to cache multiple ontologies in a single Python instance. If `cache_ontology` is used multiple times in one instance, the behavior is undefined and may cause visible or invisible errors.
 
 After an ontology is cached, the user can access the cache by using the assigned acronym in the place of `target_ontology` and setting the `use_cache` flag to `True`.
 To clear the cache, one can call:
 `clear_cache(ontology_acronym='')`
 If no arguments are specified, the entire cache will be cleared. Otherwise, only the ontology with the given acronym will be cleared.
-Finally, `cache_exists(ontology_acronym)` is a simple function that returns `True` if the given acronym exists in the cache, and `False` otherwise. It is worth noting that while ontology URLs can repeat, acronyms must be distinct in a given environment.
+Finally, `cache_exists(ontology_acronym='')` is a simple function that returns `True` if the given acronym exists in the cache, and `False` otherwise. It is worth noting that while ontology URLs can repeat, acronyms must be distinct in a given environment.
 
 ### Input Preprocessing
 As of version 1.2.0, text2term includes regex-based preprocessing functionality for input terms. Specifically, these functions take the input terms and a collection of (user-defined) regular expressions, then match each term to each regular expression to simplify the input term.
 
 Like the "map" functions above, the two functions differ on whether the input is a file or a list of strings:
 ```python
 preprocess_file(file_path, template_path, output_file='', blocklist_path='', blocklist_char='', rem_duplicates=False)
@@ -216,48 +264,8 @@
 
 `-iris BASE_IRIS` Map only to ontology terms whose IRIs start with a value given in this comma-separated list (eg 'http://www.ebi.ac.uk/efo,http://purl.obolibrary.org/obo/HP)').
 
 `-d EXCL_DEPRECATED` Exclude ontology terms stated as deprecated via `owl:deprecated true`.
 
 `-g SAVE_TERM_GRAPHS` Save [vis.js](https://visjs.org) graphs representing the neighborhood of each ontology term.
 
-`-c STORE_IN_CACHE` Using this flag followed by the acronym the ontology should be stored as, the program will same the target ontology to the cache. After that, referencing the acronym in `target` will reference the cache. Examples are below.
-
-## Examples
-### Programmatic
-```python
-import text2term
-import pandas
-
-df1 = text2term.map_file(unstruct_terms.txt, "http://www.ebi.ac.uk/efo/efo.owl")
-df2 = text2term.map_terms(["asthma", "acute bronchitis"], "http://www.ebi.ac.uk/efo/efo.owl")
-```
-Below is an example of caching, assuming the same imports as above:
-```python
-text2term.cache_ontology("http://www.ebi.ac.uk/efo/efo.owl", "EFO")
-df1 = text2term.map_file(unstruct_terms.txt, "EFO", use_cache=True)
-df2 = text2term.map_terms(["asthma", "acute bronchitis"], "EFO", use_cache=True)
-text2term.clear_cache("EFO")
-```
-
-### Command Line
-The basic use of the tool requires a `source` file containing a list of terms to map to the given `target` ontology:  
-`python text2term -s unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl`
-
-Specify an output file where the mappings should be saved using `-o`:  
-`python text2term -s unstruct_terms.txt -t efo.owl -o /Documents/my-mappings.csv`
-
-Set the minimum acceptable similarity score for mapping each given term to an ontology term using `-min`:  
-`python text2term -s unstruct_terms.txt -t efo.owl -min 0.8`  
-The mapped terms returned will have been determined to be 0.8 similar to their source terms in a 0-1 scale.  
-
-Exclude deprecated ontology terms (declared as such via *owl:deprecated true*) using `-d`:  
-`python text2term -s unstruct_terms.txt -t efo.owl -d`
-
-Limit search to only terms whose IRIs start with any IRI given in a list specified using `-iris`:  
-`python text2term.py -s unstruct_terms.txt -t efo.owl -iris http://www.ebi.ac.uk/efo/EFO,http://purl.obolibrary.org/obo/HP`  
-Here, because EFO reuses terms from other ontologies such as HP and GO, the HP terms would be included but the GO terms would be excluded.
-
-Use the cache on the command line, first by flagging it, then in the future using the acronym:
-`python text2term -s unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl -c EFO`
-Then, after running this, the following command is equivalent:
-`python text2term -s unstruct_terms.txt -t EFO`
+`-c STORE_IN_CACHE` Using this flag followed by the acronym the ontology should be stored as, the program will same the target ontology to the cache. After that, referencing the acronym in `target` will reference the cache. Examples are above.
```

### Comparing `text2term-2.1.0/text2term.egg-info/SOURCES.txt` & `text2term-2.2.0/text2term.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 setup.py
+test/test-pypi.py
 text2term/__init__.py
 text2term/__main__.py
 text2term/bioportal_mapper.py
 text2term/config.py
 text2term/mapper.py
 text2term/onto_utils.py
 text2term/preprocess.py
```

