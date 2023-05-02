# Comparing `tmp/unit_syntax-0.1.0.tar.gz` & `tmp/unit_syntax-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit_syntax-0.1.0.tar", max compression
+gzip compressed data, was "unit_syntax-0.1.1.tar", max compression
```

## Comparing `unit_syntax-0.1.0.tar` & `unit_syntax-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5212 2023-05-01 17:13:53.695136 unit_syntax-0.1.0/README.md
--rw-r--r--   0        0        0      595 2023-05-01 17:13:05.524000 unit_syntax-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      689 2023-05-01 17:13:05.524000 unit_syntax-0.1.0/unit_syntax/__init__.py
--rw-r--r--   0        0        0   149012 2023-05-01 17:13:05.524000 unit_syntax-0.1.0/unit_syntax/parser.py
--rw-r--r--   0        0        0     4608 2023-04-30 23:00:44.629093 unit_syntax-0.1.0/unit_syntax/transform.py
--rw-r--r--   0        0        0     5849 1970-01-01 00:00:00.000000 unit_syntax-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5212 2023-05-02 04:55:17.995066 unit_syntax-0.1.1/README.md
+-rw-r--r--   0        0        0      641 2023-05-02 04:55:17.995066 unit_syntax-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      689 2023-05-02 04:55:17.995066 unit_syntax-0.1.1/unit_syntax/__init__.py
+-rw-r--r--   0        0        0   149012 2023-05-02 04:55:17.995066 unit_syntax-0.1.1/unit_syntax/parser.py
+-rw-r--r--   0        0        0     4608 2023-05-02 04:55:17.995066 unit_syntax-0.1.1/unit_syntax/transform.py
+-rw-r--r--   0        0        0     5895 1970-01-01 00:00:00.000000 unit_syntax-0.1.1/PKG-INFO
```

### Comparing `unit_syntax-0.1.0/README.md` & `unit_syntax-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,124 +7,123 @@
 10 meter
 ```
 
 Behind the scenes this is translated into standard Python that uses the excellent [Pint](https://pint.readthedocs.io/) units library.
 
 ## Getting Started
 
-Install the package with `pip install unit_syntax`.  Tip: In Google Colab, you can run this directly in a cell by prefixing the command with `!`.
+Install the package:
+
+```shell
+$ pip install unit-syntax
+```
 
 To enable unit-syntax in a Jupyter/IPython session run:
 
 ```python
 import unit_syntax
 unit_syntax.enable_ipython()
 ```
 
-Note that in Jupyter this must be run in its own cell before any units expressions are evaluated.
+Note: in Jupyter this must be run in its own cell before any units expressions are evaluated.
+
+## Usage
 
-## Syntax
+[An interactive notebook to play around with units](https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV)
 
-Units apply to the preceding value (literal, variable, function call or indexing), and have higher precedence than other operators:
+Units apply to the preceding value (a literal, variable, function call or indexing), and have higher precedence than other operators:
 
 ```python
 x * 1.21 gigawatts
 ```
 
 This is equivalent to `x * (1.21 gigawatts)`, and desugars to something like `x * Quantity(1.21, "gigawatts")`.  The high precedence means units apply to the literal not the whole expression.
 
 Values can be converted to another measurement system:
 
 ```python
 (88 miles / hour) furlongs / fortnight
 ```
 
-Pint transparently supports numpy when available:
+Pint transparently [supports numpy](https://pint.readthedocs.io/en/stable/user/numpy.html) when available:
 
 ```python
 velocity = [5, 7] meters/second**2
 location = velocity * 2 seconds
 distance_traveled = numpy.linalg.norm(location)
 ```
 
-Units must start with an identifier
-
-```python
-10 cm * sin(45 degrees)
-```
-
-This is a syntax error because `sin` is parsed as part of the units; to resolve add parentheses: `(10 cm) * sin(45 degrees)`
-
-
 The units term follows this grammar:
 
 ```
 units:
-    | '(' units ')'
     | NAME '/' units
     | NAME '*' units
     | NAME units
     | NAME '**' NUMBER
     | NAME
 ```
 
-The syntax takes advantage of the fact that that in python its illegal for a NAME to follow a "primary" (literal, function call etc), so there's no ambiguity.  
-
 ## Why?  How?
 
 I like using Python+[Jupyter Notebook](https://jupyter.org/) as a calculator for physical problems and often wish it had the clarity and type checking of explicit units. [Pint](https://pint.readthedocs.io/) is great, but (IMO) its necessary verbosity makes it hard to see the underlying calculation that's going.
 
 `unit-syntax` is an IPython/Jupyter [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) that rewrites expressions with units into calls to `pint.Quantity`.
 
 This is possible without ambiguity in the python grammar because it's otherwise invalid for a "primary" (literal, function call etc) to be immediately followed by 
 
 `unit-syntax` cannot (currently) be used for standalone python scripts outside of IPython/Jupyter, but that's in principle possible through [meta_path import hooks](https://docs.python.org/3/reference/import.html#the-meta-path).
 
+The syntax takes advantage of the fact that that in python its illegal for a NAME to follow a "primary" (literal, function call etc), so there's no ambiguity.
+
+
 ## Prior Art
 
 The immediate inspriration of `unit-syntax` is a language called [Fortress](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.6323&rep=rep1&type=pdf
 ) from Sun Microsystems.  Fortress was intended as a modern Fortran, and had first-class support for units in both the syntax and type system.
 
 F# (an OCaml derivative from Microsoft) also [has first class support for units](https://en.wikibooks.org/wiki/F_Sharp_Programming/Units_of_Measure).
 
 The Julia package [Unitful.jl](http://painterqubits.github.io/Unitful.jl/stable/)
 
-
 ## Open questions and future work
 
  * Fortress uses an `in` operator to apply units to a non-literal value, e.g `x in meters`.  This has the advantage of being unambiguous regardless of parenthesization.  In python this would conflcit with `value in [a, b, c]`, but `as` is
 
-  
+ * Move to tree-sitter, which will be simpler and has a chance of providing syntax highlighting
  * Test against various ipython and python versions
  * Support standalone scripts through sys.meta_path
  * Check units at parse time
  * Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable).  More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
  * Pint does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
  * Demo colab notebook: https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV
-
+ * Describe parsing ambuguity like `1 meters * sin(45 degrees)`
+ * Figure out story around parenthesization
 
 ## Development
 
 To regenerate the parser:
 
-`python -m pegen grammar.txt -o unit_literals/parser.py`
+`python -m pegen grammar.txt -o unit_syntax/parser.py`
 
 Running tests:
 
 ```
  $ poetry install --with dev
  $ poetry run pytest
+```
 
 ## Future work and open questions
 
+ * Parenthisized units expressions
+ * Demo colab notebook
  * Move to tree-sitter so there's a chance of getting syntax highlighting
  * Jupyter syntax checks
  * Typography of output
  * Test against various ipython and python versions
  * Support standalone scripts through sys.meta_path
  * Check units at parse time
  * Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable).  More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166) 
  * Does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
- * Parenthisized units expressions
- * Demo colab notebook: https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV
+
```

### Comparing `unit_syntax-0.1.0/pyproject.toml` & `unit_syntax-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "unit-syntax"
-version = "0.1.0"
-description = ""
+version = "0.1.1"
 authors = ["Adam Hupp <adam@hupp.org>"]
 packages = [{include = "unit_syntax"}]
 readme = "README.md"
 repository = "https://github.com/ahupp/unit-syntax"
+description = "Literal physical units for Jupyter and IPython"
 
 [tool.poetry.dependencies]
 python = ">=3.8, < 4"
 Pint = "^0.20"
 ipython = ">=7"
 pegen = "^0.2"
```

### Comparing `unit_syntax-0.1.0/unit_syntax/__init__.py` & `unit_syntax-0.1.1/unit_syntax/__init__.py`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.1.0/unit_syntax/parser.py` & `unit_syntax-0.1.1/unit_syntax/parser.py`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.1.0/unit_syntax/transform.py` & `unit_syntax-0.1.1/unit_syntax/transform.py`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.1.0/PKG-INFO` & `unit_syntax-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: unit-syntax
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Literal physical units for Jupyter and IPython
 Home-page: https://github.com/ahupp/unit-syntax
 Author: Adam Hupp
 Author-email: adam@hupp.org
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -26,125 +26,124 @@
 10 meter
 ```
 
 Behind the scenes this is translated into standard Python that uses the excellent [Pint](https://pint.readthedocs.io/) units library.
 
 ## Getting Started
 
-Install the package with `pip install unit_syntax`.  Tip: In Google Colab, you can run this directly in a cell by prefixing the command with `!`.
+Install the package:
+
+```shell
+$ pip install unit-syntax
+```
 
 To enable unit-syntax in a Jupyter/IPython session run:
 
 ```python
 import unit_syntax
 unit_syntax.enable_ipython()
 ```
 
-Note that in Jupyter this must be run in its own cell before any units expressions are evaluated.
+Note: in Jupyter this must be run in its own cell before any units expressions are evaluated.
+
+## Usage
 
-## Syntax
+[An interactive notebook to play around with units](https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV)
 
-Units apply to the preceding value (literal, variable, function call or indexing), and have higher precedence than other operators:
+Units apply to the preceding value (a literal, variable, function call or indexing), and have higher precedence than other operators:
 
 ```python
 x * 1.21 gigawatts
 ```
 
 This is equivalent to `x * (1.21 gigawatts)`, and desugars to something like `x * Quantity(1.21, "gigawatts")`.  The high precedence means units apply to the literal not the whole expression.
 
 Values can be converted to another measurement system:
 
 ```python
 (88 miles / hour) furlongs / fortnight
 ```
 
-Pint transparently supports numpy when available:
+Pint transparently [supports numpy](https://pint.readthedocs.io/en/stable/user/numpy.html) when available:
 
 ```python
 velocity = [5, 7] meters/second**2
 location = velocity * 2 seconds
 distance_traveled = numpy.linalg.norm(location)
 ```
 
-Units must start with an identifier
-
-```python
-10 cm * sin(45 degrees)
-```
-
-This is a syntax error because `sin` is parsed as part of the units; to resolve add parentheses: `(10 cm) * sin(45 degrees)`
-
-
 The units term follows this grammar:
 
 ```
 units:
-    | '(' units ')'
     | NAME '/' units
     | NAME '*' units
     | NAME units
     | NAME '**' NUMBER
     | NAME
 ```
 
-The syntax takes advantage of the fact that that in python its illegal for a NAME to follow a "primary" (literal, function call etc), so there's no ambiguity.  
-
 ## Why?  How?
 
 I like using Python+[Jupyter Notebook](https://jupyter.org/) as a calculator for physical problems and often wish it had the clarity and type checking of explicit units. [Pint](https://pint.readthedocs.io/) is great, but (IMO) its necessary verbosity makes it hard to see the underlying calculation that's going.
 
 `unit-syntax` is an IPython/Jupyter [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) that rewrites expressions with units into calls to `pint.Quantity`.
 
 This is possible without ambiguity in the python grammar because it's otherwise invalid for a "primary" (literal, function call etc) to be immediately followed by 
 
 `unit-syntax` cannot (currently) be used for standalone python scripts outside of IPython/Jupyter, but that's in principle possible through [meta_path import hooks](https://docs.python.org/3/reference/import.html#the-meta-path).
 
+The syntax takes advantage of the fact that that in python its illegal for a NAME to follow a "primary" (literal, function call etc), so there's no ambiguity.
+
+
 ## Prior Art
 
 The immediate inspriration of `unit-syntax` is a language called [Fortress](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.6323&rep=rep1&type=pdf
 ) from Sun Microsystems.  Fortress was intended as a modern Fortran, and had first-class support for units in both the syntax and type system.
 
 F# (an OCaml derivative from Microsoft) also [has first class support for units](https://en.wikibooks.org/wiki/F_Sharp_Programming/Units_of_Measure).
 
 The Julia package [Unitful.jl](http://painterqubits.github.io/Unitful.jl/stable/)
 
-
 ## Open questions and future work
 
  * Fortress uses an `in` operator to apply units to a non-literal value, e.g `x in meters`.  This has the advantage of being unambiguous regardless of parenthesization.  In python this would conflcit with `value in [a, b, c]`, but `as` is
 
-  
+ * Move to tree-sitter, which will be simpler and has a chance of providing syntax highlighting
  * Test against various ipython and python versions
  * Support standalone scripts through sys.meta_path
  * Check units at parse time
  * Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable).  More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
  * Pint does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
  * Demo colab notebook: https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV
-
+ * Describe parsing ambuguity like `1 meters * sin(45 degrees)`
+ * Figure out story around parenthesization
 
 ## Development
 
 To regenerate the parser:
 
-`python -m pegen grammar.txt -o unit_literals/parser.py`
+`python -m pegen grammar.txt -o unit_syntax/parser.py`
 
 Running tests:
 
 ```
  $ poetry install --with dev
  $ poetry run pytest
+```
 
 ## Future work and open questions
 
+ * Parenthisized units expressions
+ * Demo colab notebook
  * Move to tree-sitter so there's a chance of getting syntax highlighting
  * Jupyter syntax checks
  * Typography of output
  * Test against various ipython and python versions
  * Support standalone scripts through sys.meta_path
  * Check units at parse time
  * Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable).  More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166) 
  * Does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
- * Parenthisized units expressions
- * Demo colab notebook: https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV
+
```

