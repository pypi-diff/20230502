# Comparing `tmp/werpy-0.0.2.tar.gz` & `tmp/werpy-0.0.3.tar.gz`

## Comparing `werpy-0.0.2.tar` & `werpy-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 werpy-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0    27165 2020-02-02 00:00:00.000000 werpy-0.0.2/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png
--rw-r--r--   0        0        0    93938 2020-02-02 00:00:00.000000 werpy-0.0.2/.github/assets/images/werpy-logo-word-error-rate.png
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 werpy-0.0.2/.github/workflows/codacy.yml
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 werpy-0.0.2/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 werpy-0.0.2/LICENSES/NUMPY_LICENSE
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 werpy-0.0.2/LICENSES/PANDAS_LICENSE
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/__init__.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/metrics.py
--rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/normalize.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/summary.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/wer.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/werp.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/werps.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/wers.py
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 werpy-0.0.2/.gitignore
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 werpy-0.0.2/LICENSE
--rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 werpy-0.0.2/README.md
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 werpy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 werpy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 werpy-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0    27165 2020-02-02 00:00:00.000000 werpy-0.0.3/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png
+-rw-r--r--   0        0        0    93938 2020-02-02 00:00:00.000000 werpy-0.0.3/.github/assets/images/werpy-logo-word-error-rate.png
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 werpy-0.0.3/.github/workflows/codacy.yml
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 werpy-0.0.3/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 werpy-0.0.3/LICENSES/NUMPY_LICENSE
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 werpy-0.0.3/LICENSES/PANDAS_LICENSE
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/__init__.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/metrics.py
+-rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/normalize.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/summary.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/wer.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/werp.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/werps.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/wers.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 werpy-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 werpy-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 werpy-0.0.3/README.md
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 werpy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 werpy-0.0.3/PKG-INFO
```

### Comparing `werpy-0.0.2/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png` & `werpy-0.0.3/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png`

 * *Files identical despite different names*

### Comparing `werpy-0.0.2/.github/assets/images/werpy-logo-word-error-rate.png` & `werpy-0.0.3/.github/assets/images/werpy-logo-word-error-rate.png`

 * *Files identical despite different names*

### Comparing `werpy-0.0.2/.github/workflows/codacy.yml` & `werpy-0.0.3/.github/workflows/codacy.yml`

 * *Files identical despite different names*

### Comparing `werpy-0.0.2/.github/workflows/codeql.yml` & `werpy-0.0.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `werpy-0.0.2/LICENSES/NUMPY_LICENSE` & `werpy-0.0.3/LICENSES/NUMPY_LICENSE`

 * *Files identical despite different names*

### Comparing `werpy-0.0.2/LICENSES/PANDAS_LICENSE` & `werpy-0.0.3/LICENSES/PANDAS_LICENSE`

 * *Files identical despite different names*

### Comparing `werpy-0.0.2/werpy/metrics.py` & `werpy-0.0.3/werpy/metrics.py`

 * *Files identical despite different names*

### Comparing `werpy-0.0.2/werpy/normalize.py` & `werpy-0.0.3/werpy/normalize.py`

 * *Files identical despite different names*

### Comparing `werpy-0.0.2/werpy/summary.py` & `werpy-0.0.3/werpy/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 DataFrame.
 
 This module defines the following function:
     - summary(reference, hypothesis)
 """
 
 import pandas as pd
-import werpy
+from .metrics import metrics
 
 
 def summary(reference, hypothesis):
     """
     This function provides a comprehensive breakdown of the calculated results including the WER, Levenshtein 
     Distance and all the insertion, deletion and substitution errors.
 
@@ -41,15 +41,15 @@
             substitutions - count of words needing to be transformed so the hypothesis matches the reference
             inserted_words - list of inserted words
             deleted_words - list of deleted words
             substituted_words - list of substitutions. Each substitution will be shown as a tuple with the reference
             word and the hypothesis word. For example: [(cited, sighted), (abnormally, normally)]
     """
     try:
-        word_error_rate_breakdown = werpy.metrics(reference, hypothesis)
+        word_error_rate_breakdown = metrics(reference, hypothesis)
     except ValueError:
         print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
     except AttributeError:
         print("AttributeError: All text should be in a string format. Please check your input does not include any "
               "Numeric data types.")
     else:
         if word_error_rate_breakdown[0].size == 1:
```

### Comparing `werpy-0.0.2/werpy/wer.py` & `werpy-0.0.3/werpy/wer.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 the hypothesis text into the reference text, divided by the number of words in the reference text.
 
 This module defines the following function:
     - wer(reference, hypothesis): Calculate the WER between a reference text and a hypothesis text.
 """
 
 import numpy as np
-import werpy
+from .metrics import metrics
 
 
 def wer(reference, hypothesis) -> float:
     """
     This function will calculate the overall Word Error Rate for the entire reference and hypothesis texts.
 
     Parameters
@@ -44,15 +44,15 @@
     >>> ref = ['i love cold pizza','the sugar bear character was popular']
     >>> hyp = ['i love pizza','the sugar bare character was popular']
     >>> wer_example_2 = wer(ref, hyp)
     >>> print(wer_example_2)
     0.2
     """
     try:
-        word_error_rate_breakdown = werpy.metrics(reference, hypothesis)
+        word_error_rate_breakdown = metrics(reference, hypothesis)
     except ValueError:
         print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
     except AttributeError:
         print("AttributeError: All text should be in a string format. Please check your input does not include any "
               "Numeric data types.")
     else:
         if isinstance(word_error_rate_breakdown[0], np.ndarray):
```

### Comparing `werpy-0.0.2/werpy/werp.py` & `werpy-0.0.3/werpy/werp.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 texts. It allows varying weights to be assigned to the insertion, deletion and substitution errors.
 
 This module defines the following function:
     - werp(reference, hypothesis)
 """
 
 import numpy as np
-import werpy
+from .metrics import metrics
 
 
 def werp(reference, hypothesis, insertions_weight=1, deletions_weight=1, substitutions_weight=1):
     """
     This function calculates a weighted Word Error Rate for the entire reference and hypothesis texts. It allows the
     insertion, deletion and substitution errors to be penalized or weighted at different rates.
 
@@ -58,15 +58,15 @@
     0.25
 
     >>> werp_example_4 = werp(ref, hyp, 0.5, 0.5, 1)
     >>> print(werp_example_4)
     0.25
     """
     try:
-        word_error_rate_breakdown = werpy.metrics(reference, hypothesis)
+        word_error_rate_breakdown = metrics(reference, hypothesis)
     except ValueError:
         print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
     except AttributeError:
         print(
             "AttributeError: All text should be in a string format. Please check your input does not include any "
             "Numeric data types.")
     else:
```

### Comparing `werpy-0.0.2/werpy/werps.py` & `werpy-0.0.3/werpy/werps.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 hypothesis texts. It allows varying weights to be assigned to the insertion, deletion and substitution errors.
 
 This module defines the following function:
     - werps(reference, hypothesis)
 """
 
 import numpy as np
-import werpy
+from .metrics import metrics
 
 
 def werps(reference, hypothesis, insertions_weight=1, deletions_weight=1, substitutions_weight=1):
     """
     This function calculates a list of weighted Word Error Rates for each of the reference and hypothesis texts. It
     allows the insertion, deletion and substitution errors to be penalized or weighted at different rates.
 
@@ -52,15 +52,15 @@
     [0.2857142857142857, 0.3333333333333333]
 
     >>> werps_example_2 = werps(ref, hyp, insertions_weight = 0.5, deletions_weight = 0.5, substitutions_weight = 1)
     >>> print(werps_example_2)
     [0.21428571428571427, 0.2777777777777778]
     """
     try:
-        word_error_rate_breakdown = werpy.metrics(reference, hypothesis)
+        word_error_rate_breakdown = metrics(reference, hypothesis)
     except ValueError:
         print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
     except AttributeError:
         print(
             "AttributeError: All text should be in a string format. Please check your input does not include any "
             "Numeric data types.")
     else:
```

### Comparing `werpy-0.0.2/werpy/wers.py` & `werpy-0.0.3/werpy/wers.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This module defines the following function:
     - wers(reference, hypothesis)
 """
 
 
 import numpy as np
-import werpy
+from .metrics import metrics
 
 
 def wers(reference, hypothesis):
     """
     This function calculates a list of the Word Error Rates for each of the reference and hypothesis texts.
 
     Parameters
@@ -41,15 +41,15 @@
     >>> hyp = ['no one else could claim that','she sighted multiple reasons why']
     >>> wers_example_1 = wers(ref, hyp)
     >>> print(wers_example_1)
     [0.0, 0.2]
     """
 
     try:
-        word_error_rate_breakdown = werpy.metrics(reference, hypothesis)
+        word_error_rate_breakdown = metrics(reference, hypothesis)
     except ValueError:
         print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
     except AttributeError:
         print("AttributeError: All text should be in a string format. Please check your input does not include any "
               "Numeric data types.")
     else:
         if isinstance(word_error_rate_breakdown[0], np.ndarray):
```

### Comparing `werpy-0.0.2/.gitignore` & `werpy-0.0.3/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -156,8 +156,11 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # VSCode
+.vscode
 .vscode/
+vscode
+vscode/
```

### Comparing `werpy-0.0.2/LICENSE` & `werpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `werpy-0.0.2/README.md` & `werpy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `werpy-0.0.2/pyproject.toml` & `werpy-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "werpy"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Ross Armstrong", email="ross.armstrong@analyticsinmotion.com" },
 ]
 description = "A powerful yet lightweight Python package to calculate and analyze the Word Error Rate (WER)."
 readme = "README.md"
 license = "BSD-3-Clause"
 requires-python = ">=3.8"
```

### Comparing `werpy-0.0.2/PKG-INFO` & `werpy-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A powerful yet lightweight Python package to calculate and analyze the Word Error Rate (WER).
 Project-URL: Homepage, https://github.com/analyticsinmotion/werpy
 Project-URL: Bug Tracker, https://github.com/analyticsinmotion/werpy/issues
 Author-email: Ross Armstrong <ross.armstrong@analyticsinmotion.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: levenshtein distance,nlp,python,python package,speech to text,stt,wer,word error rate
```

