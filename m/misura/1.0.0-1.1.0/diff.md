# Comparing `tmp/misura-1.0.0.tar.gz` & `tmp/misura-1.1.0.tar.gz`

## Comparing `misura-1.0.0.tar` & `misura-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.0.0/.gitattributes
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 misura-1.0.0/Makefile
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 misura-1.0.0/__main__.py
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 misura-1.0.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 misura-1.0.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 misura-1.0.0/.github/SECURITY.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 misura-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 misura-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 misura-1.0.0/docs/docs.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 misura-1.0.0/src/misura/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 misura-1.0.0/src/misura/globals.py
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 misura-1.0.0/src/misura/units.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.0.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.0.0/LICENSE
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 misura-1.0.0/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 misura-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.1.0/.gitattributes
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 misura-1.1.0/Makefile
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 misura-1.1.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 misura-1.1.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 misura-1.1.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 misura-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 misura-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     6623 2020-02-02 00:00:00.000000 misura-1.1.0/docs/docs.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 misura-1.1.0/src/misura/__init__.py
+-rw-r--r--   0        0        0    11410 2020-02-02 00:00:00.000000 misura-1.1.0/src/misura/conversion.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 misura-1.1.0/src/misura/globals.py
+-rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 misura-1.1.0/src/misura/units.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 misura-1.1.0/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 misura-1.1.0/PKG-INFO
```

### Comparing `misura-1.0.0/.github/CODE_OF_CONDUCT.md` & `misura-1.1.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `misura-1.0.0/.github/CONTRIBUTING.md` & `misura-1.1.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `misura-1.0.0/.github/SECURITY.md` & `misura-1.1.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `misura-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `misura-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `misura-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `misura-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `misura-1.0.0/.github/workflows/python-publish.yml` & `misura-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `misura-1.0.0/src/misura/units.py` & `misura-1.1.0/src/misura/units.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,27 @@
-# Unit class.
-
 from colorama import Style
 from re import findall
 
+from .conversion import *
+
+# Unit class.
+
 class unit:
     def __init__(self, value: any, symbol: str) -> None:
         try:
             assert type(symbol) == str
             assert symbol != ""
 
         except(AssertionError):
             raise UnitError(symbol)
 
         self.value = value
         
         # From symbol: str to self.symbols: dict.
-        self.symbols = dict()
-        symbols = symbol.split(" ")
-        
-        for sym in symbols:
-            candidate = findall(r"-?\d+\.?\d*", sym)
-
-            if len(candidate) == 1:
-                power = candidate[0]
-            
-            elif len(candidate) > 1:
-                raise UnitError(symbol)
-            
-            else:
-                power = "1"
-
-            self.symbols[sym.replace(power, "")] = float(power)
+        self.symbols = dictFromSymbol(symbol)
 
     # Returns a readable symbol.
     def symbol(self, print: bool = False) -> str:
         from .globals import style # Unit highlighting.
 
         # Fancy version.
         if print:
@@ -50,15 +37,15 @@
             
             return "[" + numerator + denominator + "]" if numerator else ""
         
         # {"m": 1, "s": -1} -> "m s-1".
         return symbolFromDict(self.symbols)
 
 
-    # STRINGS
+    # STRINGS.
 
 
     def __str__(self) -> str:
         return "{} {}".format(self.value, self.symbol(print=True)) if self.symbol() else str(self.value)
     
     def __repr__(self) -> str:
         return str(self)
@@ -83,15 +70,15 @@
         return complex(self.value)
 
     # Bool.
     def __bool__(self) -> bool:
         return bool(self.value)
 
 
-    # MATH
+    # MATH.
 
 
     # Abs.
     def __abs__(self) -> "unit":
         return unit(abs(self.value), self.symbol())
     
     # Positive.
@@ -124,37 +111,38 @@
     def __trunc__(self) -> "unit":
         from math import trunc
         return unit(trunc(self.value), self.symbol())
     
     # Addition.
     def __add__(self, other: "unit") -> "unit":
         if self.symbol() != other.symbol():
-            raise SymbolError(self, other, "+")
+            other = convert(other, self.symbol())
         
         return unit(self.value + other.value, self.symbol())
     
     def __radd__(self, other: "unit") -> "unit":
         return self.__add__(other)
     
     # Subtraction.
     def __sub__(self, other: "unit") -> "unit":
         if self.symbol() != other.symbol():
-            raise SymbolError(self, other, "-")
+            other = convert(other, self.symbol())
         
         return unit(self.value - other.value, self.symbol())
     
     def __rsub__(self, other: "unit") -> "unit":
         return self.__sub__(other)
 
     # Multiplication.
     def __mul__(self, other: any) -> any:
         if type(other) != unit:
             return unit(self.value * other, self.symbol())
         
         newSymbols = self.symbols.copy()
+        other = convert(other, self.symbol(), partial=True)
 
         for sym in newSymbols:
             if sym in other.symbols:
                 newSymbols[sym] += other.symbols[sym]
         
         for sym in other.symbols:
             if sym not in newSymbols:
@@ -167,14 +155,15 @@
     
     # Division.
     def __truediv__(self, other: any) -> any:
         if type(other) != unit:
             return unit(self.value / other, self.symbol())
         
         newSymbols = self.symbols.copy()
+        other = convert(other, self.symbol(), partial=True)
 
         for sym in newSymbols:
             if sym in other.symbols:
                 newSymbols[sym] -= other.symbols[sym]
         
         for sym in other.symbols:
             if sym not in newSymbols:
@@ -201,15 +190,15 @@
         return unit(self.value ** other, symbolFromDict(newSymbols))
     
     # Modulo.
     def __mod__(self, other: any) -> "unit":
         return unit(self.value % other, self.symbol())
     
 
-    # COMPARISONS
+    # COMPARISONS.
 
 
     # Less than.
     def __lt__(self, other: any) -> "unit":
         if type(other) != unit:
             return self.value < other
         
@@ -258,16 +247,83 @@
     # Not equal.
     def __ne__(self, other: any) -> "unit":
         if type(other) != unit:
             return self.value != other
         
         return self.value != other.value or self.symbol() != other.symbol()
 
+# Conversion function.
+def convert(first: "unit", target: "str", partial: bool = False) -> unit:
+    factor = 1.0
+    symbols = first.symbols.copy()
+    targetSymbols = dictFromSymbol(target)
+
+    partialTargets = []
+
+    table = SI_TABLE.copy()
+    table.update(SI_DERIVED_TABLE)
+
+    for sym in symbols.keys():
+        for unitFamily in table:
+            if sym in table[unitFamily]:
+                family = unitFamily
+                break
+
+        familyCounter = 0
+
+        for targetSym in targetSymbols:
+            if targetSym in table[family]:
+                targetSymbol = targetSym
+                familyCounter += 1
+
+        if familyCounter == 0:
+            if not partial:
+                raise ConversionError(first, target)
+            
+            partialTargets.append(sym + str(symbols[sym]))
+            continue
+
+        elif familyCounter > 1:
+            raise ConversionError(first, target)
+        
+        elif sym != targetSymbol:
+            if symbols[sym] != targetSymbols[targetSymbol]:
+                raise ConversionError(first, target)
+            
+            factor *= (table[family][sym] / table[family][targetSymbol]) ** symbols[sym]
+            partialTargets.append(targetSymbol + str(targetSymbols[targetSymbol]))
+            continue
+
+    return unit(first.value * factor, target) if not partial else unit(first.value * factor, " ".join(partialTargets))
+
 # Utilities.
 
+def dictFromSymbol(symbol: str) -> dict:
+    symbols = dict()
+        
+    for sym in symbol.split(" "):
+        candidate = findall(r"-?\d+\.?\d*", sym)
+
+        if len(candidate) == 1:
+            power = candidate[0]
+        
+        elif len(candidate) > 1:
+            raise UnitError(symbol)
+        
+        else:
+            power = "1"
+
+        try:
+            symbols[sym.replace(power, "")] = int(power)
+
+        except(ValueError):
+            symbols[sym.replace(power, "")] = float(power)
+
+    return symbols
+
 def symbolFromDict(symbols: dict) -> str:
     return " ".join(sorted([sym + ("{}".format(symbols[sym]) if symbols[sym] != 1 else "") for sym in symbols if symbols[sym] != 0]))
 
 # Exceptions.
 
 class UnitError(TypeError):
     def __init__(self, symbol: str) -> None:
```

### Comparing `misura-1.0.0/LICENSE` & `misura-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `misura-1.0.0/README.md` & `misura-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 ![PyPI](https://img.shields.io/pypi/v/misura)
 ![GitHub last commit](https://img.shields.io/github/last-commit/diantonioandrea/misura)
 ![GitHub Release Date](https://img.shields.io/github/release-date/diantonioandrea/misura)
 
 # misura
 
-Python library for easy unit handling and conversion[^1] for scientific & engineering applications.  
+Python library for easy unit handling and conversion for scientific & engineering applications.  
 
 **misura** is a Python library designed to simplify the *handling of units of measure* for scientific and engineering applications. It provides a unified interface for *dealing with different units and their conversions*, allowing for quick and accurate calculations without the need for complex manual conversions.  
 
-Make sure to take a look at the [documentation](https://github.com/diantonioandrea/misura/blob/main/docs/docs.md#introduction), at the [contributing guidelines](https://github.com/diantonioandrea/misura/blob/main/.github/CONTRIBUTING.md) and at the [examples](#examples).
+Make sure to take a look at the [documentation](https://github.com/diantonioandrea/misura/blob/main/docs/docs.md), at the [contributing guidelines](https://github.com/diantonioandrea/misura/blob/main/.github/CONTRIBUTING.md) and at the [examples](#examples).
 
-[^1]: To be implemented.
+### Features
+
+* Mathematical and logic perations between units: [Example](#mathematical-operations), [example](#comparisons).
+* Manual conversions: [Example](#manual-and-automatic-conversion).
+* Automatic conversions on operations: [Example](#manual-and-automatic-conversion).
+* Large compatibility with other libraries: [Example](#working-with-other-libraries).
+* Custom exceptions: [Example](#comparisons).
 
 ## Installation
 
 ### Installing misura
 
 **misura** can be installed from [PyPI](https://pypi.org) by:
 
@@ -59,17 +65,63 @@
 print(num1 / num3)
 print(num3 ** 2)
 ```
 
 The output is:
 
 	6 m / s
-	8 m(2.0) / s(2.0)
-	1.0 m / s(2.0)
-	4 s(2.0)
+	8 m(2) / s(2)
+	1.0 m / s(2)
+	4 s(2)
+
+### Working with other libraries
+
+``` python
+from misura import unit, convert
+from decimal import Decimal, getcontext
+import numpy
+
+getcontext().prec = 40
+
+arr1 = numpy.array([unit(2, "m"), unit(50, "m s-1"), unit(2, "kg")])
+arr2 = unit(numpy.array([1, 2, 3]), "J")
+num2 = unit(numpy.sqrt(Decimal(5)), "kg")
+
+print(arr1 * 3)
+print(arr2 ** 2)
+print(num2)
+```
+
+The output is:
+
+	[6 m 150 m / s 6 kg]
+	[1 4 9] J(2)
+	2.236067977499789696409173668731276235441 kg
+
+Unit highlighting helps distinguish between different numbers.
+
+### Manual and automatic conversion
+
+``` python
+from misura import unit, convert
+
+num1 = unit(2, "m2")
+num2 = unit(4, "kg")
+num3 = unit(400, "m s-1")
+
+print(convert(num1, "cm2"))
+print(num2 + unit(5, "g"))
+print(convert(num3, "km", partial=True))
+```
+
+The output is:
+
+	20000.0 cm(2)
+	4.005 kg
+	0.4 km / s
 
 ### Comparisons
 
 ``` python
 from misura import unit
 
 num1 = unit(2, "m s-1")
@@ -79,19 +131,17 @@
 print(num1 > num2)
 print(num2 < 6)
 print(num1 > num3)
 ```
 
 The output is:
 
-``` python
-False
-True
-"misura.units.SymbolError: unsupported operand symbol(s) for >: 'm s-1.0' and 's'"
-```
+	False
+	True
+	misura.units.SymbolError: unsupported operand symbol(s) for >: 'm s-1.0' and 's'
 
 ### Unary operators and functions
 
 ``` python
 from misura import unit
 from misura import style
 from math import trunc
```

### Comparing `misura-1.0.0/pyproject.toml` & `misura-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "misura"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "Python library for easy unit handling and conversion for scientific & engineering applications."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["setuptools", "colorama"]
```

### Comparing `misura-1.0.0/PKG-INFO` & `misura-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misura
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python library for easy unit handling and conversion for scientific & engineering applications.
 Project-URL: Homepage, https://github.com/diantonioandrea/misura
 Project-URL: Documentation, https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/misura/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -17,21 +17,27 @@
 
 ![PyPI](https://img.shields.io/pypi/v/misura)
 ![GitHub last commit](https://img.shields.io/github/last-commit/diantonioandrea/misura)
 ![GitHub Release Date](https://img.shields.io/github/release-date/diantonioandrea/misura)
 
 # misura
 
-Python library for easy unit handling and conversion[^1] for scientific & engineering applications.  
+Python library for easy unit handling and conversion for scientific & engineering applications.  
 
 **misura** is a Python library designed to simplify the *handling of units of measure* for scientific and engineering applications. It provides a unified interface for *dealing with different units and their conversions*, allowing for quick and accurate calculations without the need for complex manual conversions.  
 
-Make sure to take a look at the [documentation](https://github.com/diantonioandrea/misura/blob/main/docs/docs.md#introduction), at the [contributing guidelines](https://github.com/diantonioandrea/misura/blob/main/.github/CONTRIBUTING.md) and at the [examples](#examples).
+Make sure to take a look at the [documentation](https://github.com/diantonioandrea/misura/blob/main/docs/docs.md), at the [contributing guidelines](https://github.com/diantonioandrea/misura/blob/main/.github/CONTRIBUTING.md) and at the [examples](#examples).
 
-[^1]: To be implemented.
+### Features
+
+* Mathematical and logic perations between units: [Example](#mathematical-operations), [example](#comparisons).
+* Manual conversions: [Example](#manual-and-automatic-conversion).
+* Automatic conversions on operations: [Example](#manual-and-automatic-conversion).
+* Large compatibility with other libraries: [Example](#working-with-other-libraries).
+* Custom exceptions: [Example](#comparisons).
 
 ## Installation
 
 ### Installing misura
 
 **misura** can be installed from [PyPI](https://pypi.org) by:
 
@@ -76,17 +82,63 @@
 print(num1 / num3)
 print(num3 ** 2)
 ```
 
 The output is:
 
 	6 m / s
-	8 m(2.0) / s(2.0)
-	1.0 m / s(2.0)
-	4 s(2.0)
+	8 m(2) / s(2)
+	1.0 m / s(2)
+	4 s(2)
+
+### Working with other libraries
+
+``` python
+from misura import unit, convert
+from decimal import Decimal, getcontext
+import numpy
+
+getcontext().prec = 40
+
+arr1 = numpy.array([unit(2, "m"), unit(50, "m s-1"), unit(2, "kg")])
+arr2 = unit(numpy.array([1, 2, 3]), "J")
+num2 = unit(numpy.sqrt(Decimal(5)), "kg")
+
+print(arr1 * 3)
+print(arr2 ** 2)
+print(num2)
+```
+
+The output is:
+
+	[6 m 150 m / s 6 kg]
+	[1 4 9] J(2)
+	2.236067977499789696409173668731276235441 kg
+
+Unit highlighting helps distinguish between different numbers.
+
+### Manual and automatic conversion
+
+``` python
+from misura import unit, convert
+
+num1 = unit(2, "m2")
+num2 = unit(4, "kg")
+num3 = unit(400, "m s-1")
+
+print(convert(num1, "cm2"))
+print(num2 + unit(5, "g"))
+print(convert(num3, "km", partial=True))
+```
+
+The output is:
+
+	20000.0 cm(2)
+	4.005 kg
+	0.4 km / s
 
 ### Comparisons
 
 ``` python
 from misura import unit
 
 num1 = unit(2, "m s-1")
@@ -96,19 +148,17 @@
 print(num1 > num2)
 print(num2 < 6)
 print(num1 > num3)
 ```
 
 The output is:
 
-``` python
-False
-True
-"misura.units.SymbolError: unsupported operand symbol(s) for >: 'm s-1.0' and 's'"
-```
+	False
+	True
+	misura.units.SymbolError: unsupported operand symbol(s) for >: 'm s-1.0' and 's'
 
 ### Unary operators and functions
 
 ``` python
 from misura import unit
 from misura import style
 from math import trunc
```

